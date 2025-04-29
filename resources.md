---
title: Resources
layout: page
permalink: /resources
---

{% for location in site.locations %}
  <h1>{{ location.title }}</h1>
  <p>{{ location.description }}</p>

  {% if location.video_link %}
    <div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
      <iframe src="{{ location.video_link }}" 
              style="position:absolute;top:0;left:0;width:100%;height:100%;" 
              frameborder="0" 
              allowfullscreen>
      </iframe>
    </div>
  {% endif %}
{% endfor %}
