---
layout: default
title:  Events 
---
{% for post in site.categories.events %}
<div class="event">
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
