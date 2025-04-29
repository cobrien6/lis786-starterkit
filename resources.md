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
label {
  font-weight: bold;
  margin-right: 10px;
}
select {
  padding: 5px;
  font-size: 16px;
}
</style>

</head>
<body>

<div class="dropdown">
  <label for="geneva">Geneva:</label>
  <select id="geneva">
    <option value="">Select an option</option>
    <option value="park">Park</option>
    <option value="library">Library</option>
    <option value="museum">Museum</option>
  </select>
</div>

<div class="dropdown">
  <label for="batavia">Batavia:</label>
  <select id="batavia">
    <option value="">Select an option</option>
    <option value="riverwalk">Riverwalk</option>
    <option value="museum">Museum</option>
    <option value="highschool">High School</option>
  </select>
</div>

<div class="dropdown">
  <label for="stcharles">St. Charles:</label>
  <select id="stcharles">
    <option value="">Select an option</option>
    <option value="zoo">Zoo</option>
    <option value="theater">Theater</option>
    <option value="library">Library</option>
  </select>
</div>

</body>
</html>

