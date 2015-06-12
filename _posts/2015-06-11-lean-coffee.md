---
layout: post
title: "Lean Coffee - June"
categories: events leancoffee
event:
  eventbrite-id: lean-coffee-june-2015-tickets-17362482653 
  date: 2015-06-18
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

<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank">Register on EventBrite</a>

**Description**  
 The format of this meeting is simple:

  - Show up
  - Order breakfast (optional)
  - Suggest topics
  - Vote on topics
  - Discuss topics with the most votes

Last month we discussed two topics:
  1. Preventing the improvement backslide - Signals and strategies to reverse agile adoptions that have stalled or regressed. 
  1. Identify and minimize non-value add activities - Do the thing that creates value. Stop doing (or minimize) the things that don't (large analysis efforts, detailed estimation and detailed planning)  
  
We ended the meeting with a 2 minute retro to determine how we could improve. Based on the feedback this meeting will not include a fee. Will the price impact attendance and no-shows? Will new people participate? Stop by and find out the answers to these exciting questions!!!

I hope to see you there!

{{page.event.description | markdownify}}

<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank">Register on EventBrite</a>
