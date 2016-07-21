---
layout: post
title: August Lunch Meeting - Building Better Idiots
category: events
event:
  eventbrite-id: august-meeting-building-better-idiots-tickets-26649537484
  date: 2016-08-09
  time: 11:30 AM - 1:00 PM
  slides: 

  presenter:
    name: Tony Bibbs 
    title: CEO at The GForge Group
    bio: | 
        Tony Bibbs is the lead geek and CEO at The GForge Group, Inc based out of West Des Moines, Iowa. Over his 19 year career he's practiced just about every software development methodology ranging from an organic "anti-process" he used to lead a large, open source project to waterfall in the late '90s to today's more agile approaches.  His experiences in aerospace, ag, government and tech start-ups has proven that the struggle for building better software is industry-wide. Furthermore his experience programming in Jovial, C++, Java, PHP and JavaScript has proven the struggle is real regardless of the technology stack.  At The GForge Group Tony is applying what he has learned by leading a small, multi-national team that helps some of the world's largest companies work smarter, collaborate better and get their ideas to market faster.

  location:
    name: The Principal
    address: 750 Park Street
    citystatezip: Des Moines, IA 50309
    instructions: Room 1A16

  description: | 
    The glass half-empty view of software development is that we are engaged in a back-and-forth tug of war by building better software only to find out the world has produced a better idiot. Besides the end-users it should be noted that the "idiots" in question often include us. Join me while I share a refreshingly candid series of missteps and lapses in judgements all of which lead me toward IT-enlightenment.  
    
    Over the lunch hour I'll briefly share the history of GForge and many of the common dilemmas we all face. Is it truly faster to rewrite that legacy system? How will we decide what features make it into the next release? Is TDD really worth it? How do you go from little-to-no automation to continuous integration and deployment?  How can a small company provide support and collect customer feedback without impacting overall velocity?

    Join me this Friday where we'll discuss all this including the age-old question, "WTF is Agile?"
  
---
**{{page.event.date | date: "%A, %B %-d, %Y" }} from
 {{page.event.time}}**
{% if page.event.slides %}
  **Download the slides:**
  [{{page.event.slides}}](/p/{{page.event.slides}})
{% endif %}

**Description**  
{{page.event.description}}

<a class="btn" title="EventBrite Registration"  href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank" data-eventdate="{{page.event.date | date: '%D'}}">Register on EventBrite</a>

**Speaker**  
{{page.event.presenter.name}}  
*{{page.event.presenter.title}}*  

{{page.event.presenter.bio}}

**Location**  
{{page.event.location.name}}  
{{page.event.location.address}}  
{{page.event.location.citystatezip}}  

{% if page.event.location.instructions %}
  *Additional instructions*:
  {{page.event.location.instructions}}
{% endif %}

<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank" data-eventdate="{{page.event.date | date: '%D'}}">Register on EventBrite</a>
