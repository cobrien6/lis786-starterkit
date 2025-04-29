---
title: Resources
layout: page
permalink: /resources
---
<div>
{% for location in site.locations %}
    {{ location.title }}
    {{ location.description }}
{% endfor %}
</div>
