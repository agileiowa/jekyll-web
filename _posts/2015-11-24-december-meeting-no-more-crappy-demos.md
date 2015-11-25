---
layout: post
title: December Meeting - No More Crappy Demos
category: events
event:
  eventbrite-id: december-meeting-no-more-crappy-demos-tickets-19530485207
  date: 2015-12-02
  time: 11:30 AM - 1:30 PM
#  slides:

  presenter:
    name: Josh Carson
    title: Product Owner/Scrum Master/Innovation Lead, Product Development at John Deere
#    bio:

  location:
    name: The Principal
    address: 750 Park Street
    citystatezip: Des Moines, IA 50309
    instructions: Room 1A16

  description: Demos are a crucial part of the feedback loop that Agile development relies on.  However, all too often demos fail to hit the mark and distract from the work being done.  This talk is to help you give demos that don't suck so that you can get the feedback you need to create amazing products for your customers.
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
