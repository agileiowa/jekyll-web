---
layout: post
title: "June Meeting - Evolution of Agile/Lean at Nationwide"
category: events
event:
  eventbrite-id: evolution-of-agilelean-at-nationwide-tickets-17136571948
  date: 2015-06-09
  time: 11:30 PM to 1:00 PM

  presenter:
    name: Larry Brandmeyer
    title: Associate Vice President, Application Development Center
    bio: Larry is an experienced executive and former business owner having led multiple information systems operations and leadership teams through all phases of execution. A proven track record that demonstrates an effective understanding of the business needs of an organization and the ability to apply technology solutions and policy to promote the current and future growth of that company. Expansive thinker with an outstanding record of achievement implementing new business concepts and delivering innovative business solutions.

  location:
    name: Nationwide Insurance
    address: 1200 Locust Street
    citystatezip: Des Moines, IA  50391
    instructions: Check in at the 2nd floor security desk which is accessible from the building front entrance or skywalk.

  description: Join us for a discussion on Nationwide's journey to Agile and Lean development including where it all started, how we got to where we are today, and what lies ahead.  With over 100 Agile teams in 3 locations, Nationwide has fully embraced a future in Agile development.   
  slides: brandmeyer-agileIowa-presentation-2015-06-09.pdf
---
**{{page.event.date | date: "%A, %B %-d, %Y" }} from
 {{page.event.time}}**
{% if page.event.slides %}
  **Download the slides:**
  [{{page.event.slides}}](p/{{page.event.slides}})
{% endif %}

**Description**  
{{page.event.description}}

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
