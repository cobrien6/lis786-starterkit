---
title: Contact Us
layout: page
permalink: /contact
owner_name: Colin O'Brien
secretary_name: John Smith
---
<style>
body {
  font-family: Arial, sans-serif;
  background-color: #f4f7fa;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.contact-container {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  width: 80%;
  max-width: 800px;
  padding: 30px;
  margin: 20px;
}

.contact-section {
  margin-bottom: 20px;
  padding-bottom: 20px;
  border-bottom: 1px solid #ddd;
}

.contact-section h3 {
  color: #0056b3;
  font-size: 1.5em;
  margin-bottom: 10px;
}

.contact-section p {
  font-size: 1.1em;
  line-height: 1.6;
  color: #555;
  margin: 5px 0;
}

.contact-section p span {
  font-weight: bold;
  color: #333;
}

.contact-section p a {
  color: #0056b3;
  text-decoration: none;
  font-weight: bold;
}

.contact-section p a:hover {
  text-decoration: underline;
}

</style>

<body>
<div class="contact-container">
  <div class="contact-section">
    <h3>{{ page.owner_name }}</h3>
    <p><span>Phone:</span> 630-303-3222</p>
    <p><span>Email:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
    <p>For inquiries concerning partnerships and collaborations with our organization, please directly contact Colin O'Brien via the contact information provided above.</p>
  </div>

  <div class="contact-section">
    <h3>{{ page.secretary.name }}</h3>
    <p><span>Phone:</span> 708-524-6296</p>
    <p><span>Email:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
    <p>For general inquiries and finding a resource for you, please contact John Smith, secretary and community coordinator.</p>
  </div>
</div>
</body>

