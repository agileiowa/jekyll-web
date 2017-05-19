---
layout: post
title: "Mob Programming with Woody Zuill"
category: events
event:
  eventbrite-id: mob-programming-with-woody-zuill-tickets-34738941108
  date: 2017-05-20
  time: 11:00 AM - 3:00 PM
  slides: 

  agenda: 

  presenter:
    name: Woody Zuill
    photo: 
    title: Mob Programming with Woody Zuill
    bio: | 
        Woody Zuill has been programming computers for 35+ years, and is an independent Developer, Agile Coach and Trainer. He and his previous team at Hunter Industries are the originators of the Mob Programming approach to teamwork in software development, and Woody is considered one of the founders of the "#NoEstimates" discussion on Twitter.

        Over the last 15+ years he has worked as an Agile Coach, Application Development Manager, Trainer, and Extreme Programmer. He believes that code must be simple, clean, and maintainable so that we can realize the Agile promise of Responding to Change, and that we must constantly "Inspect and Adapt". He has a passion tackling code that is hard to maintain and cleaning, refactoring, and bringing it back into a manageable state.

        Learn more:
        @WoodyZuill
        
        http://zuill.us/WoodyZuill/

  location:
    name: Gravitate
    address: 206 6th Avenue, 3rd Floor
    citystatezip: Des Moines, IA 50309
    instructions: 
   
  description: | 
    Woody Zuill has graciously offered to make a quick 
    trip to Des Moines, IA this Saturday, May 20th. (Yes you are reading that right, it's this Saturday!)

    He is speaking at Nebraska Code this week and decided to make the quick drive up to Iowa for the day to spend some time with fellow Agile enthusiasts and practice mob programming.

---
**{{page.event.date | date: "%A, %B %-d, %Y" }} from
 {{page.event.time}}**
{% if page.event.slides %}
  **Download the slides:**
  [{{page.event.slides}}](/p/{{page.event.slides}})
{% endif %}

{{ page.event.agenda }}

**Description**  
{{page.event.description}}

<a class="btn" title="EventBrite Registration"  href="http://www.eventbrite.com/e/{{page.event.eventbrite-id}}" target="_blank" data-eventdate="{{page.event.date | date: '%D'}}">Register on EventBrite</a>

**Speaker**  

<div class="speaker">
{% if page.event.presenter.photo %}
    <div><img alt="speaker" src="/images/speakers/{{page.event.presenter.photo}}"/></div>
{% endif %}
<h2>{{page.event.presenter.name}}</h2>
{% if page.event.presenter.title%}
<h4>{{page.event.presenter.title}}</h4>
{% endif %}
</div>
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
