---
title: Contact Us
layout: page
permalink: /contact
owner_name: Colin O'Brien
secretary_name: John Smith
---

<style>
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

button {
  background-color: #4FC3F7; /* Light blue */
  border: none;
  color: white;
  padding: 12px 24px;
  margin: 8px 4px;
  font-size: 16px;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #039BE5; /* Darker blue on hover */
}

button:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(79, 195, 247, 0.5);
}
</style>

<body>
<div id="contact-text" class="contact-container">
  <div class="contact-section">
    <h3>{{ page.owner_name }}</h3>
    <p><span>Phone:</span> 630-303-3222</p>
    <p><span>Email:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
    <p>For inquiries concerning partnerships and collaborations with our organization, please directly contact Colin O'Brien via the contact information provided above.</p>
  </div>

  <div class="contact-section">
    <h3>{{ page.secretary_name }}</h3>
    <p><span>Phone:</span> 708-524-6296</p>
    <p><span>Email:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
    <p>For general inquiries and finding a resource for you, please contact John Smith, secretary and community coordinator.</p>
  </div>
</div>

<button onclick="setLanguage('en')">English</button>
<button onclick="setLanguage('es')">Español</button>
<button onclick="setLanguage('pl')">Polski</button>
<button onclick="setLanguage('pt')">Português</button>

<script>
const translations = {
  en: `
    <div class="contact-section">
      <h3>{{ page.owner_name }}</h3>
      <p><span>Phone:</span> 630-303-3222</p>
      <p><span>Email:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
      <p>For inquiries concerning partnerships and collaborations with our organization, please directly contact Colin O'Brien via the contact information provided above.</p>
    </div>
    <div class="contact-section">
      <h3>{{ page.secretary_name }}</h3>
      <p><span>Phone:</span> 708-524-6296</p>
      <p><span>Email:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
      <p>For general inquiries and finding a resource for you, please contact John Smith, secretary and community coordinator.</p>
    </div>
  `,
  es: `
    <div class="contact-section">
      <h3>{{ page.owner_name }}</h3>
      <p><span>Teléfono:</span> 630-303-3222</p>
      <p><span>Correo electrónico:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
      <p>Para consultas sobre asociaciones y colaboraciones, comuníquese directamente con Colin O'Brien utilizando la información proporcionada arriba.</p>
    </div>
    <div class="contact-section">
      <h3>{{ page.secretary_name }}</h3>
      <p><span>Teléfono:</span> 708-524-6296</p>
      <p><span>Correo electrónico:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
      <p>Para consultas generales y para encontrar recursos, comuníquese con John Smith, secretario y coordinador comunitario.</p>
    </div>
  `,
  pl: `
    <div class="contact-section">
      <h3>{{ page.owner_name }}</h3>
      <p><span>Telefon:</span> 630-303-3222</p>
      <p><span>Email:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
      <p>W sprawach dotyczących partnerstw i współpracy prosimy o bezpośredni kontakt z Colinem O'Brienem pod podanym powyżej adresem.</p>
    </div>
    <div class="contact-section">
      <h3>{{ page.secretary_name }}</h3>
      <p><span>Telefon:</span> 708-524-6296</p>
      <p><span>Email:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
      <p>W sprawach ogólnych i pomocy w znalezieniu zasobów prosimy o kontakt z Johnem Smithem, sekretarzem i koordynatorem społeczności.</p>
    </div>
  `,
  pt: `
    <div class="contact-section">
      <h3>{{ page.owner_name }}</h3>
      <p><span>Telefone:</span> 630-303-3222</p>
      <p><span>Email:</span> <a href="mailto:cobrien@my.dom.edu">cobrien@my.dom.edu</a></p>
      <p>Para parcerias e colaborações, entre em contato diretamente com Colin O'Brien usando as informações acima.</p>
    </div>
    <div class="contact-section">
      <h3>{{ page.secretary_name }}</h3>
      <p><span>Telefone:</span> 708-524-6296</p>
      <p><span>Email:</span> <a href="mailto:dom@dom.edu">dom@dom.edu</a></p>
      <p>Para dúvidas gerais e ajuda para encontrar recursos, entre em contato com John Smith, secretário e coordenador comunitário.</p>
    </div>
  `
};

function setLanguage(lang) {
  document.getElementById('contact-text').innerHTML = translations[lang];
}
</script>
</body>
