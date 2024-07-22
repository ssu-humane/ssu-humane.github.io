---
title: "HUMANE Lab - Team"
layout: gridlay
excerpt: "HUMANE Lab: Team members"
sitemap: false
permalink: /team/
---

# Team members

## Current members
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-portrait" width="35%" height="200px" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br><{{ member.email }}></i>
    
  <ul style="overflow: hidden">
    
  {% if member.number_interest == 1 %}
  <li> {{ member.interest1 }} </li>
  {% endif %}

  {% if member.number_interest == 2 %}
  <li> {{ member.interest1 }} </li>
  <li> {{ member.interest2 }} </li>
  {% endif %}
    
   </ul>
  
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni

- 송 선영 (Seonyeong Song), MS, 2024.8
- 박 채원 (Chaewon Park), BS, 2024.2

