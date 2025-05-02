<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Optim Vente</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #fff;
      color: #333;
    }
    header {
      background-color: #b30000;
      color: white;
      padding: 1rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }
    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }
    nav a {
      margin: 0 1rem;
      color: white;
      text-decoration: none;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .lang-switcher {
      margin-left: auto;
    }
    section {
      padding: 2rem;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
    }
    .gallery div {
      background-color: #eee;
      height: 150px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #999;
    }
    footer {
      background-color: #f0f0f0;
      text-align: center;
      padding: 1rem;
    }
    @media (max-width: 600px) {
      nav {
        width: 100%;
        margin-top: 1rem;
        text-align: center;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">Optim Vente</div>
    <nav>
      <a href="#home" data-fr="Accueil" data-en="Home">Accueil</a>
      <a href="#services" data-fr="Services" data-en="Services">Services</a>
      <a href="#gallery" data-fr="Galerie" data-en="Gallery">Galerie</a>
    </nav>
    <div class="lang-switcher">
      <button onclick="setLang('fr')">FR</button>
      <button onclick="setLang('en')">EN</button>
    </div>
  </header>

  <section id="home">
    <h2 data-fr="Bienvenue chez Optim Vente" data-en="Welcome to Optim Vente">Bienvenue chez Optim Vente</h2>
    <p data-fr="Votre partenaire en optimisation commerciale." data-en="Your partner in sales optimization.">Votre partenaire en optimisation commerciale.</p>
  </section>

  <section id="services">
    <h2 data-fr="Nos Services" data-en="Our Services">Nos Services</h2>
    <p data-fr="Nous offrons des solutions adaptées pour booster vos ventes." data-en="We offer tailored solutions to boost your sales.">Nous offrons des solutions adaptées pour booster vos ventes.</p>
  </section>

  <section id="gallery">
    <h2 data-fr="Galerie" data-en="Gallery">Galerie</h2>
    <div class="gallery">
      <div>Image 1</div>
      <div>Image 2</div>
      <div>Image 3</div>
    </div>
  </section>

  <footer>
    &copy; 2025 Optim Vente
  </footer>

  <script>
    function setLang(lang) {
      document.querySelectorAll('[data-fr]').forEach(el => {
        el.textContent = el.getAttribute('data-' + lang);
      });
    }
  </script>
</body>
</html>
