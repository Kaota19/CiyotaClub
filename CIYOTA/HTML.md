<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>CIYOTA CLUB</title>
  <link rel="stylesheet" href="ciyota.css">
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <div class="logo">CIYOTA <span class="club">CLUB</span></div>
      <nav class="nav">
        <a href="#about">À propos</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container">
        <h1>Bienvenue au <strong>CIYOTA CLUB</strong></h1>
        <p>Nous connectons les talents, formons les communautés et développons des projets blockchain locaux.</p>
        <p class="cta-row">
          <a class="btn" href="#services">Nos services</a>
          <a class="btn ghost" href="#contact">Nous contacter</a>
        </p>
      </div>
    </section>

    <section id="about" class="container card">
      <h2>À propos</h2>
      <p>CIYOTA CLUB est une entreprise dédiée à l'éducation, l'accompagnement et l'innovation dans l'écosystème Web3. Nous proposons des formations, des ateliers et des services de conseil adaptés aux besoins locaux.</p>
    </section>

    <section id="services" class="container grid">
      <h2>Services</h2>
      <div class="cards">
        <article class="service">
          <h3>Formations</h3>
          <p>Ateliers pratiques et cours sur blockchain, développement et sécurité.</p>
        </article>
        <article class="service">
          <h3>Consulting</h3>
          <p>Accompagnement de projets, audits et stratégie technique.</p>
        </article>
        <article class="service">
          <h3>Communauté</h3>
          <p>Organisation d'événements, meetups et hackathons.</p>
        </article>
      </div>
    </section>

    <section id="contact" class="container card">
      <h2>Contact</h2>
      <p>Envie d'échanger ? Écrivez-nous :</p>
      <form class="contact-form" action="#" method="post" onsubmit="alert('Formulaire de démo — remplacez action pour l\'envoyer')">
        <label>
          Nom
          <input type="text" name="name" placeholder="Votre nom" required>
        </label>
        <label>
          Email
          <input type="email" name="email" placeholder="vous@exemple.com" required>
        </label>
        <label>
          Message
          <textarea name="message" rows="4" placeholder="Votre message..." required></textarea>
        </label>
        <div class="form-row">
          <button class="btn" type="submit">Envoyer</button>
        </div>
      </form>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <small>© <span id="year"></span> CIYOTA CLUB — Tous droits réservés</small>
      <div class="social">
        <a href="#" aria-label="Twitter">Twitter</a>
        <a href="#" aria-label="LinkedIn">LinkedIn</a>
      </div>
    </div>
  </footer>

  <script>
    // année courante
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
