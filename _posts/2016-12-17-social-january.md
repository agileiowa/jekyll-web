---
layout: post
title: "Agile Iowa Social - January"
categories: events
event:
  facebook-id: 
  eventbrite-id: agile-iowa-social-january-2017-tickets-30448066988
  date: 2017-01-24
  time: 4:30 PM to 8:00 PM

  presenter:
    name: 
    title: 
    bio: 

  location:
    name: Draught House 1908 Downtown Des Moines 
    address: 409 Court Ave
    citystatezip: Des Moines, IA 50309
    instructions: 

  description: | 
    By popular demand of non-morning people everywhere...  We introduce Agile Iowa Social!
    
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
