---
layout: post
title: "Move Over Continuous Integration, We've Got Continuous Compliance"
categories: events
event:
  facebook-id: 
  eventbrite-id: move-over-continuous-integration-weve-got-continuous-compliance-tickets-35569088100
  date: 2017-07-12
  time: 12:00 PM to 1:00 PM

  presenter:
    name:  Brandon Carlson
    title: IT Nerd
    bio: Brandon is an Agile guy that lives in the Des Moines metro area. He likes Pina coladas and getting caught in the rain.

  location:
    name: John Deere Financial 
    address: 6400 NW 86th St.
    citystatezip: Johnston, IA 50131
    instructions: 

  description: Continuous Delivery (CD) and regulatory compliance are two critically important ingredients in today’s connected organizations. CD enables you to move quickly and respond to change in an era where change is increasing at an exponential rate with no sign of slowing down. Regulatory compliance ensures that your organization takes the appropriate steps to follow applicable laws and appear to require adding burdensome processes and controls to your software development lifecycle. While they appear to be at odds with one another at first, they actually complement each other well. While maintaining, analyzing, confirming, and reporting on the status of required information security, compliance, and privacy controls can be difficult, integrating these tasks within your CD pipeline is easier than you think. Using examples from real-world projects in organizations just like yours, Brandon explains how to integrate compliance and reporting into your CD pipeline using tools you already know such as pair programming, Jenkins, Chef, Metasploit, and others, leading you to the regulatory promised land known as “Continuous Compliance”.
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

{% if page.event.eventbrite-id %}
<a class="btn" title="EventBrite Registration"  href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank" data-eventdate="{{page.event.date | date: '%D'}}">Register on EventBrite</a>
{% endif %}

**Description**  
{{page.event.description | markdownify}}

{% if page.event.eventbrite-id %}
<a class="btn" title="EventBrite Registration" href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank">Register on EventBrite</a>
{% endif %}
