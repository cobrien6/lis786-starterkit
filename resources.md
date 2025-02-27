---
title: Resources
layout: page
permalink: /resources
---
{% for location in site.locations %}
    <h2>{{ location.title }}</h2>
    {{ location.description | markdownify }}
{% endfor %}
