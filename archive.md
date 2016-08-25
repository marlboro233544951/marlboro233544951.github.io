---
layout: page
title: "Archive"
description: "努力，奋斗"
header-img: "img/orange.jpg"
---


<ul class="listing" >
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator" style="color:#e58172;font-size:1.5em">{{ y }}</li>
  {% endif %}
  <li class="listing-item" >
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}" title="{{ post.title }}" style="color:#6b92dd">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>