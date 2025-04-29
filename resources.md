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


<style>
body {
  font-family: Arial, sans-serif;
  padding: 20px;
}
.dropdown {
  margin-bottom: 20px;
}
button {
  background-color: #4FC3F7;
  border: none;
  color: white;
  padding: 12px 24px;
  font-size: 16px;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  margin-bottom: 10px;
}
button:hover {
  background-color: #039BE5;
}
.content {
  display: none;
  margin-top: 10px;
  padding: 10px;
  border-left: 3px solid #4FC3F7;
}
</style>

<div class="dropdown">
  <button onclick="toggleContent('geneva')">Geneva</button>
  <div id="geneva" class="content">
    <p>Geneva offers a range of educational resources, including a vibrant public library, excellent schools, and community learning centers.</p>
  </div>
</div>

<div class="dropdown">
  <button onclick="toggleContent('batavia')">Batavia</button>
  <div id="batavia" class="content">
    <p>Batavia is home to great public schools, a popular park district, and local programs supporting literacy and lifelong learning.</p>
  </div>
</div>

<div class="dropdown">
  <button onclick="toggleContent('stcharles')">St. Charles</button>
  <div id="stcharles" class="content">
    <p>St. Charles features a highly rated school district, an active library system, and plenty of events focused on family education and community engagement.</p>
  </div>
</div>

<script>
function toggleContent(id) {
  const content = document.getElementById(id);
  content.style.display = content.style.display === "block" ? "none" : "block";
}
</script>

