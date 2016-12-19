require "rubygems"
require "tmpdir"

require "bundler/setup"
require "jekyll"

# Change your GitHub reponame eg. "kippt/jekyll-incorporated"
GITHUB_REPONAME = "agileiowa/jekyll-web"

task :default => [:watch]

desc "Watch the site and regenerate when it changes"
task :watch do
  puts "Starting to watch source with Jekyll..."
  #system "sass --update _sass:css -f -l -r ./_sass/bourbon/lib/bourbon.rb"
  jekyllPid = Process.spawn("jekyll serve --watch --future")
  #sassPid = Process.spawn("sass --watch _sass:css -l -r ./_sass/bourbon/lib/bourbon.rb")

  trap("INT") {
    [jekyllPid].each { |pid| Process.kill(9, pid) rescue Errno::ESRCH }
    exit 0
  }

  [jekyllPid].each { |pid| Process.wait(pid) }
end # task :watch

namespace :generate do
  desc "Generate new Lean Coffee event: lean_coffee['2017-01-01']"
  task :lean_coffee, :date do | t, args |  
    datestamp = Time.now.strftime('%F')
    # publish 20 days before the event
    event_date = Date.parse(args[:date])
    publish_date = event_date - 20
    puts "Publish Date: #{publish_date}"

    event_month_name = event_date.strftime("%B")
    puts "Event Month: #{event_month_name}"
    post_filename = "_drafts/#{publish_date}-lean-coffee-#{event_month_name}.md"

    template = File.read('_templates/lean-coffee-template.md')
    post = template.gsub(/\{\{month\}\}/, event_month_name)
    .gsub(/\{\{date\}\}/, args[:date])
    File.open(post_filename, "w") { | f | f.puts post }
    
    puts "Created Draft at #{post_filename}"
  end

  desc "Generate new post"
  task :post, :post_title, :date, :time do | t, args |
    datestamp = Time.now.strftime('%F')
    post_filename = build_target_filename(datestamp, args[:post_title])

    post_template = File.read('_templates/post-template.md')
    post = post_template.gsub(/\{\{date\}\}/, args[:date])
                        .gsub(/\{\{time\}\}/, args[:time])
                        .gsub(/\{\{title\}\}/, args[:post_title])
    File.open(post_filename, "w") { | f | f.puts post }

    open_for_editing(post_filename)
  end

  def build_target_filename(datestamp, title)
    file_title = title.downcase.strip.gsub(' ', '-').gsub(/[^\w-]/, '')
    "_posts/#{datestamp}-#{file_title}.md"
  end

  def open_for_editing(post_filename)
    system "open #{post_filename}" if (/darwin/ =~ RUBY_PLATFORM)
    system "start #{post_filename}" if (/cygwin|mswin|mingw|bccwin|wince|emx/ =~ RUBY_PLATFORM)
  end
end
namespace :site do
  desc "Generate blog files"
  task :generate do
    Jekyll::Site.new(Jekyll.configuration({
      "source"      => ".",
      "destination" => "_site"
    })).process
  end

  task :check do
      if (has_unpushed_commits())
          puts "\e[31mYou have un-pushed changes. NO PUBLISH FOR YOU!!\e[0m"
          exit 0
      end
  end

  def has_unpushed_commits()
    system "git fetch origin master -q"
    status = `git status -sb`
    (status =~ /\[ahead \d{1,}\]/)
  end

  desc "Generate and publish blog to gh-pages"
  task :publish => [:check, :generate] do
    Dir.mktmpdir do |tmp|
      cp_r "_site/.", tmp
      Dir.chdir tmp
      system "git init"
      system "git add ."
      message = "Site updated at #{Time.now.utc}"
      system "git commit -m #{message.inspect}"
      system "git remote add origin https://github.com/#{GITHUB_REPONAME}.git"
      system "git push origin master:refs/heads/gh-pages --force"
    end
  end
end
