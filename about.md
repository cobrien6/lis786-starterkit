---
title: About Us
layout: page
permalink: /about
---
<style>
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

<p>Select Language / Seleccionar idioma / Wybierz język / Selecionar idioma</p>

<button onclick="setLanguage('en')">English</button>
<button onclick="setLanguage('es')">Español</button>
<button onclick="setLanguage('pl')">Polski</button>
<button onclick="setLanguage('pt')">Português</button>

<div id="about-text">
<p>Welcome to Tri-City Education Connections!</p>
<p>We are dedicated to helping individuals and families in Geneva, Batavia, and St. Charles find the educational resources they need — especially those who are new to English or seeking further learning opportunities.</p>
<p>Our website brings together trusted local information from libraries, schools, government offices, and private organizations. Whether you're looking for English language classes, bilingual materials, or support for your children's education, we make it easy to connect with the right resources in your community.</p>
<p>At Tri-City Education Connections, we believe that language should never be a barrier to opportunity. Our goal is to empower everyone with clear pathways to education, growth, and success.</p>
</div>

<script>
const translations = {
  en: `
    <p>Welcome to Tri-City Education Connections!</p>
    <p>We are dedicated to helping individuals and families in Geneva, Batavia, and St. Charles find the educational resources they need — especially those who are new to English or seeking further learning opportunities.</p>
    <p>Our website brings together trusted local information from libraries, schools, government offices, and private organizations. Whether you're looking for English language classes, bilingual materials, or support for your children's education, we make it easy to connect with the right resources in your community.</p>
    <p>At Tri-City Education Connections, we believe that language should never be a barrier to opportunity. Our goal is to empower everyone with clear pathways to education, growth, and success.</p>
  `,
  es: `
    <p>¡Bienvenidos a Conexiones Educativas de Tri-City!</p>
    <p>Estamos dedicados a ayudar a individuos y familias en Geneva, Batavia y St. Charles a encontrar los recursos educativos que necesitan, especialmente a quienes están aprendiendo inglés o buscan oportunidades educativas adicionales.</p>
    <p>Nuestro sitio web reúne información confiable de bibliotecas, escuelas, oficinas gubernamentales y organizaciones privadas. Ya sea que busque clases de inglés, materiales bilingües o apoyo para la educación de sus hijos, le ayudamos a conectarse con los recursos adecuados en su comunidad.</p>
    <p>En Conexiones Educativas de Tri-City, creemos que el idioma nunca debe ser una barrera para el progreso. Nuestro objetivo es empoderar a todos con caminos claros hacia la educación, el crecimiento y el éxito.</p>
  `,
  pl: `
    <p>Witamy w Tri-City Education Connections!</p>
    <p>Pomagamy osobom i rodzinom w Geneva, Batavii i St. Charles znaleźć potrzebne zasoby edukacyjne — zwłaszcza tym, którzy nie mówią po angielsku lub szukają możliwości dalszej nauki.</p>
    <p>Nasza strona internetowa łączy zaufane lokalne informacje z bibliotek, szkół, urzędów i organizacji prywatnych. Niezależnie od tego, czy szukasz kursów języka angielskiego, materiałów dwujęzycznych czy wsparcia edukacyjnego dla dzieci, pomożemy Ci znaleźć odpowiednie zasoby w Twojej społeczności.</p>
    <p>W Tri-City Education Connections wierzymy, że język nie powinien być przeszkodą w osiąganiu celów. Naszym celem jest umożliwienie każdemu dostępu do edukacji, rozwoju i sukcesu.</p>
  `,
  pt: `
    <p>Bem-vindo ao Tri-City Education Connections!</p>
    <p>Estamos comprometidos em ajudar indivíduos e famílias em Geneva, Batavia e St. Charles a encontrar os recursos educacionais de que precisam — especialmente aqueles que não falam inglês ou buscam oportunidades de aprendizado.</p>
    <p>Nosso site reúne informações confiáveis de bibliotecas, escolas, órgãos governamentais e entidades privadas. Se você procura aulas de inglês, materiais bilíngues ou apoio educacional para seus filhos, ajudamos a conectar você com os recursos certos em sua comunidade.</p>
    <p>No Tri-City Education Connections, acreditamos que o idioma nunca deve ser uma barreira para o sucesso. Nosso objetivo é capacitar todos com caminhos claros para a educação, o crescimento e o sucesso.</p>
  `
};

function setLanguage(lang) {
  document.getElementById('about-text').innerHTML = translations[lang];
}
</script>

</body>

