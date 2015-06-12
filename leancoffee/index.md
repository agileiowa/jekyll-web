---
layout: default
title:  Lean Coffee 
---
{% for post in site.categories.leancoffee%}
<div class="event" data-event-date="{{post.event.date | date: "%Y-%m-%d"}}">
  <div class="cal">
    <div class="month">
      {{ post.event.date | date: "%b" }}
    </div>
    <div class="day">
      {{ post.event.date | date: "%d" }}
    </div>
  </div>
  <div class="title">
    <a href="{{post.url}}">{{ post.title }}</a>
  </div>
</div>

{% endfor %}
