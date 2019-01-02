---
layout: post
title: "Lean Coffee - December"
categories: events leancoffee
event:
  eventbrite-id: agileiowa-lean-coffee-december-2019-tickets-54276399171
  date: 2019-12-19
  time: 7:00 AM to 8:30 AM

  presenter:
    name: 
    title: 
    bio:

  location:
    name: Machine Shed Restaurant 
    address: 11151 Hickman Road
    citystatezip: Urbandale, IA 50322
    instructions: 

  description: 
  slides: 

---
**{{page.event.date | date: "%A, %B %-d, %Y" }} from
 {{page.event.time}}**
{% if page.event.slides %}
  **Download the slides:**
  [{{page.event.slides}}](p/{{page.event.slides}})
{% endif %}

**Location**  
{{page.event.location.name}}  
{{page.event.location.address}}  
{{page.event.location.citystatezip}}  

{% if page.event.location.instructions %}
  *Additional instructions*: 
  {{page.event.location.instructions}}
{% endif %}

<a class="btn" title="EventBrite Registration"  href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank" data-eventdate="{{page.event.date | date: '%D'}}">Register on EventBrite</a>

**Description**  
 The format of this meeting is simple:

  - Show up
  - Order breakfast (optional)
  - Suggest topics
  - Vote on topics
  - Discuss topics with the most votes

I hope to see you there!

{{page.event.description | markdownify}}

<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank">Register on EventBrite</a>

