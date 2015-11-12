---
layout: post
title: {{title}}
category: events
event:
  eventbrite-id:
  date: {{date}}
  time: {{time}}
  slides:

  presenter:
    name:
    title:
    bio:

  location:
    name:
    address:
    citystatezip:
    instructions:

  description:
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
