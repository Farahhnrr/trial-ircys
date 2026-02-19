<template>
  <div class="page">
    <SiteNav />

    <main class="canvas">
      <section class="hero">
        <p class="section-kicker">About us</p>
        <h1 class="page-title">ABOUT US - WHAT IS IRCYS</h1>
        <p class="lead">
          The International Research Competition for Young Scientists (IRCYS) is a premier global
          event dedicated to fostering scientific research among youth. Unlike typical invention
          fairs, IRCYS places a strong emphasis on the research process, methodology, and
          scientific analysis.
        </p>
        <p class="lead">
          Moving to its 7th Edition in 2026, IRCYS transforms into a mid-year grand summit,
          inviting young brilliant minds to gather in the Island of Gods, Bali, to present their
          discoveries.
        </p>
      </section>
    </main>

    <footer class="footer">
      <div class="footer-brand">
        <img src="/img/logo.png" alt="International Research Competition logo" />
        <p>International Research Competition &amp; Olympiad</p>
      </div>
      <div class="footer-links">
        <div>
          <h4>Programs</h4>
          <a href="#">Categories</a>
          <a href="#">Mentors</a>
          <a href="#">Awards</a>
        </div>
        <div>
          <h4>Resources</h4>
          <a href="#">Guidebook</a>
          <a href="#">FAQ</a>
          <a href="#">Press</a>
        </div>
        <div>
          <h4>Contact</h4>
          <a href="#">info@olympiad.org</a>
          <a href="#">+62 21 555 4421</a>
          <a href="#">Jakarta, Indonesia</a>
        </div>
      </div>
      <p class="footer-note">(c) 2026 Olympiad Network. All rights reserved.</p>
    </footer>
  </div>
</template>

<style scoped>
.page {
  min-height: 100vh;
  padding: 0.8rem 3rem 2rem;
  background-color: #f3f2ed;
}

.canvas {
  padding: 3rem 0 4rem;
  display: flex;
  flex-direction: column;
}

.hero {
  max-width: 720px;
  background: rgba(255, 255, 255, 0.86);
  padding: 2.5rem 3rem;
  border-radius: 28px;
  box-shadow: 0 20px 40px rgba(60, 47, 32, 0.12);
  margin-bottom: 1.6rem;
}

.section-kicker {
  margin: 0 0 0.6rem;
  font-size: 0.75rem;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  color: #7b5a36;
}

.page-title {
  margin: 0 0 1rem;
  font-size: clamp(2rem, 4vw, 2.6rem);
  font-family: "Erode", "Times New Roman", serif;
  color: #241c14;
}

.lead {
  margin: 0;
  font-size: 1.1rem;
  line-height: 1.7;
  color: #4b3f32;
}

.lead + .lead {
  margin-top: 1rem;
}

.footer {
  margin-top: 2rem;
  padding: 2.5rem 3rem 2rem;
  background: rgba(33, 26, 18, 0.92);
  color: #f7f1e7;
  border-radius: 32px;
}

.footer-brand {
  display: flex;
  align-items: center;
  gap: 1.2rem;
  margin-bottom: 2rem;
}

.footer-brand img {
  width: 80px;
  height: 80px;
  object-fit: contain;
}

.footer-links {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.footer-links h4 {
  margin: 0 0 0.8rem;
  font-size: 0.95rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

.footer-links a {
  display: block;
  color: rgba(247, 241, 231, 0.8);
  text-decoration: none;
  margin-bottom: 0.5rem;
  font-size: 0.9rem;
}

.footer-links a:hover,
.footer-links a:focus {
  color: #ffffff;
}

@media (max-width: 900px) {
  .page {
    padding: 2rem 1.5rem 2rem;
  }

  .canvas {
    padding: 2.4rem 0 3rem;
  }

  .hero,
  .footer {
    padding: 2rem;
  }
}
</style>

