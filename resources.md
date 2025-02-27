---
title: Resources
layout: page
permalink: /resources
---
{% for location in site.locations %}
    <h2>
    {{ location.title | markdownify }}
    </h2>
    <p>
    {{ location.description | markdownify }}
    </p>
{% endfor %}
