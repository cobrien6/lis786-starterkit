---
title: Resources
layout: page
permalink: /resources
---
{% for location in site.locations %}
    {{ location.title }}
    {{ location.description }}
{% endfor %}
