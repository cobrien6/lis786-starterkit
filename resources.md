---
title: Resources
layout: page
permalink: /resources
---

{% for location in site.locations %}
  <h1>{{ location.title }}</h1>
  <p>{{ location.description }}</p>
{% endfor %}

<div class="video-container"><iframe src="https://www.youtube.com/embed/xaPv7zjSXD8" frameborder="0" allowfullscreen></iframe></div><style>.video-container {position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;}.video-container iframe {position: absolute; top: 0; left: 0; width: 100%; height: 100%;}</style>


