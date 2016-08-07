---
layout: post
title: "Lean Happy Hour - August"
categories: events
event:
  facebook-id: 
  eventbrite-id: lean-happy-hour-august-2016-tickets-26990211449 
  date: 2016-08-09
  time: 4:00 PM to 6:00 PM

  presenter:
    name: 
    title: 
    bio: 

  location:
    name: Eater A
    address: 2932 Ingersoll Ave
    citystatezip: Des Moines, IA 50312 
    instructions: 

  description: | 
    By popular demand of non-morning people everywhere...  We introduce Lean Happy Hour!
    
    Some of us aren't morning people or don't have the flexibility to make it to Lean Coffee so to cater to those who prefer after work events and perhaps something a little stronger than coffee... Here you go!  Join us for a beverage or two (maybe more) and talk with others about whatever topics come to mind.  This is a chance to network with others in our professions and pick their brains or just hang out and socialize.
    
    Hope to see you there! 
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
{{page.event.description | markdownify}}

<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank">Register on EventBrite</a>
