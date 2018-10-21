# AgileIowa.org Website

[![Build Status](https://travis-ci.org/agileiowa/jekyll-web.svg?branch=master)](https://travis-ci.org/agileiowa/jekyll-web)

Jekyll version of the agileiowa.org website

## Local Dev
Install `rbenv` to to use the version of ruby defined in `.ruby-version`.

Run: `rake` will start the jekyll server in *watch* mode.

## Update Library

Run `bundle update` to update all the gems to the latest version.

## How to publish
Run `rake site:publish`
This will generate the site locally and overwrite the gh-pages branch. 

We use a `git submodule` for the `_site` folder. If you build it and experience problems, run `git submodule update --init` to reset the `_site/` folder.
