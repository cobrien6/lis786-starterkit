---
title: Resources
layout: page
permalink: /resources
---
{% for location in site.locations %}
    {{ location.title | markdownify }}
    {{ location.description | markdownify }}
{% endfor %}
