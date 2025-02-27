---
title: Resources
layout: page
permalink: /resources
---
{% for location in site.locations %}
    <h2>{{ location.title | raw}}</h2>
    {{ location.description | markdownify | raw}}
{% endfor %}
