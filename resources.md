---
title: Resources
layout: page
permalink: /resources
---
<div>
{% for location in site.locations %}
    <h1>{{ location.title }}</h1>
    <p>{{ location.description }}</p>
{% endfor %}
</div>
