<template>
  <div class="page">
    <header class="top">
      <div class="brand">
        <img class="brand-logo" src="/img/logo.png" alt="International Research Competition logo" />
      </div>

      <nav class="top-nav">
        <NuxtLink to="/" class="nav-link">Home</NuxtLink>
        <NuxtLink to="/about" class="nav-link">About us</NuxtLink>
        <NuxtLink to="/competition" class="nav-link">Competition</NuxtLink>
        <a href="#" class="nav-link">Categories</a>
        <NuxtLink to="/medal-and-award" class="nav-link is-active">Medal and Award</NuxtLink>
        <a href="#" class="nav-link">Get Involved</a>
        <a href="#" class="nav-link">FAQ</a>
        <a href="#" class="nav-link">Contact</a>
      </nav>

      <button class="nav-cta">Register</button>
    </header>

    <main class="canvas">
      <section class="award-shell" aria-label="Awards overview">
        <aside class="award-rail">
          <p class="section-kicker">Medal & Award</p>
          <h1 class="hero-title">Celebrate excellence with globally recognized honors.</h1>
          <p class="hero-copy">
            Winners receive medals, scholarships, and international recognition. Each award is
            guided by a transparent rubric and validated by our academic partners.
          </p>
          <div class="hero-actions">
            <button class="primary-btn">Download Awards Guide</button>
            <button class="ghost-btn">View Past Winners</button>
          </div>
          <div class="rail-medals">
            <p class="card-kicker">Award tiers</p>
            <div class="medal-item">
              <span class="medal-dot gold"></span>
              <div>
                <strong>Gold Medal</strong>
                <span>Top 5% overall score</span>
              </div>
            </div>
            <div class="medal-item">
              <span class="medal-dot silver"></span>
              <div>
                <strong>Silver Medal</strong>
                <span>Top 10% overall score</span>
              </div>
            </div>
            <div class="medal-item">
              <span class="medal-dot bronze"></span>
              <div>
                <strong>Bronze Medal</strong>
                <span>Top 20% overall score</span>
              </div>
            </div>
          </div>
        </aside>

        <div class="award-main">
          <section class="award-banner">
            <div>
              <p class="card-kicker">Recognition package</p>
              <h2>What winners receive</h2>
              <p>Scholarships, research grants, media coverage, and mentor placements.</p>
            </div>
            <div class="banner-metrics">
              <div class="banner-item">
                <svg class="banner-icon" viewBox="0 0 24 24" aria-hidden="true">
                  <path
                    d="M6 4h12a2 2 0 0 1 2 2v11a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                  />
                  <path
                    d="M8 8h8M8 12h5"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                    stroke-linecap="round"
                  />
                </svg>
                <div>
                  <strong>48</strong>
                  <span>Scholarships</span>
                </div>
              </div>
              <div class="banner-item">
                <svg class="banner-icon" viewBox="0 0 24 24" aria-hidden="true">
                  <path
                    d="M6 7h12v12H6z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                  />
                  <path
                    d="M9 5h6M12 5v2"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                    stroke-linecap="round"
                  />
                </svg>
                <div>
                  <strong>12</strong>
                  <span>Research grants</span>
                </div>
              </div>
              <div class="banner-item">
                <svg class="banner-icon" viewBox="0 0 24 24" aria-hidden="true">
                  <path
                    d="M8 11a3 3 0 1 1 6 0 3 3 0 0 1-6 0Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                  />
                  <path
                    d="M4 20a8 8 0 0 1 16 0"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.6"
                    stroke-linecap="round"
                  />
                </svg>
                <div>
                  <strong>25</strong>
                  <span>Mentor partners</span>
                </div>
              </div>
            </div>
          </section>

          <section class="award-highlights" aria-label="Award highlights">
            <article class="award-card">
              <h2>Grand Champion</h2>
              <p>Highest composite score across all categories and presentations.</p>
              <ul>
                <li>Full scholarship package</li>
                <li>International press feature</li>
                <li>Mentor placement</li>
              </ul>
            </article>
            <article class="award-card">
              <h2>Category Excellence</h2>
              <p>Top-scoring teams within each research category.</p>
              <ul>
                <li>Category medal & certificate</li>
                <li>Research grant support</li>
                <li>Panel feedback report</li>
              </ul>
            </article>
            <article class="award-card">
              <h2>Innovation Impact</h2>
              <p>Projects with strong real-world adoption potential.</p>
              <ul>
                <li>Innovation badge</li>
                <li>Partner incubation access</li>
                <li>Pitch showcase slot</li>
              </ul>
            </article>
          </section>

          <section class="award-criteria" aria-label="Judging criteria">
            <div class="criteria-card">
              <h2>Judging criteria</h2>
              <p>
                Each medal is determined by weighted scoring across originality, impact, and
                presentation quality.
              </p>
              <div class="criteria-bars">
                <div>
                  <span>Originality & research depth</span>
                  <div class="bar"><span style="width: 40%"></span></div>
                </div>
                <div>
                  <span>Impact potential</span>
                  <div class="bar"><span style="width: 35%"></span></div>
                </div>
                <div>
                  <span>Presentation & execution</span>
                  <div class="bar"><span style="width: 25%"></span></div>
                </div>
              </div>
            </div>
            <div class="criteria-panel">
              <h3>Feedback timeline</h3>
              <p>All finalists receive scorecards and mentor feedback within two weeks.</p>
              <button class="secondary-btn">Request full rubric</button>
            </div>
          </section>

          <section class="award-showcase" aria-label="Award showcase">
            <div class="showcase-card">
              <h2>Hall of recognition</h2>
              <p>Celebrate the most inspiring teams from the last season.</p>
              <div class="showcase-grid">
                <div>
                  <strong>2025</strong>
                  <span>AI for Climate Risk</span>
                </div>
                <div>
                  <strong>2024</strong>
                  <span>Bio-based Packaging</span>
                </div>
                <div>
                  <strong>2023</strong>
                  <span>Clean Water Sensors</span>
                </div>
              </div>
            </div>
            <div class="showcase-cta">
              <h3>Ready to earn a medal?</h3>
              <p>Get the awards guide and prepare your submission early.</p>
              <button class="primary-btn">Start your journey</button>
            </div>
          </section>
        </div>
      </section>
    </main>

    <footer class="footer">
      <div class="footer-brand">
        <img src="/img/logo.png" alt="International Research Competition logo" />
        <p>International Research Competition & Olympiad</p>
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

<script setup>
</script>

<style scoped>
.page {
  min-height: 100vh;
  padding: 0.8rem 3rem 2rem;
  background-color: #f3f2ed;
  background-image: url("/img/bg2.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  position: relative;
  overflow: hidden;
}

.page::before {
  content: "";
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  background-image: none;
  background-repeat: no-repeat;
  background-position: center 70%;
  background-size: min(1100px, 90vw) auto;
  opacity: 0.18;
  transform: scaleX(-1) rotate(45deg);
  transform-origin: center;
}

.top {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  position: relative;
  z-index: 1;
  gap: 2rem;
  flex-wrap: wrap;
}

.brand {
  display: flex;
  align-items: center;
  min-width: 140px;
}

.brand-logo {
  width: 140px;
  height: 140px;
  object-fit: contain;
}

.canvas {
  flex: 1;
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  gap: 4rem;
  padding: 3rem 0 4rem;
}

.award-shell {
  display: grid;
  grid-template-columns: minmax(260px, 0.45fr) minmax(0, 1fr);
  gap: 2.5rem;
  align-items: start;
}

.award-rail {
  position: sticky;
  top: 2rem;
  align-self: start;
  background: rgba(255, 255, 255, 0.9);
  padding: 2.4rem 2.2rem;
  border-radius: 28px;
  box-shadow: 0 20px 36px rgba(60, 47, 32, 0.12);
  backdrop-filter: blur(8px);
}

.rail-medals {
  margin-top: 2rem;
  padding-top: 1.6rem;
  border-top: 1px solid rgba(77, 63, 50, 0.18);
  display: grid;
  gap: 1.2rem;
}

.medal-item {
  display: flex;
  gap: 0.8rem;
  align-items: flex-start;
}

.medal-item strong {
  display: block;
  font-size: 1.05rem;
}

.medal-item span {
  color: #4b3f32;
  font-size: 0.9rem;
}

.medal-dot {
  width: 12px;
  height: 12px;
  border-radius: 999px;
  margin-top: 0.35rem;
}

.medal-dot.gold {
  background: #c79a46;
}

.medal-dot.silver {
  background: #b8bfc8;
}

.medal-dot.bronze {
  background: #b37b4b;
}

.award-main {
  display: flex;
  flex-direction: column;
  gap: 2.4rem;
}

.award-banner {
  background: rgba(34, 27, 19, 0.88);
  color: #f7f1e7;
  padding: 2.4rem;
  border-radius: 28px;
  box-shadow: 0 22px 40px rgba(40, 28, 17, 0.25);
  display: grid;
  gap: 1.8rem;
}

.award-banner h2 {
  margin: 0.4rem 0 0.6rem;
}

.banner-metrics {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.2rem;
}

.banner-item {
  display: flex;
  align-items: center;
  gap: 0.8rem;
}

.banner-icon {
  width: 40px;
  height: 40px;
  color: #f7f1e7;
  flex: 0 0 auto;
}

.banner-metrics strong {
  display: block;
  font-size: 1.4rem;
  color: #f7f1e7;
}

.banner-metrics span {
  color: rgba(247, 241, 231, 0.8);
  font-size: 0.85rem;
}

.award-highlights {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1.6rem;
}

.award-card {
  background: rgba(255, 255, 255, 0.88);
  padding: 2.2rem;
  border-radius: 26px;
  box-shadow: 0 18px 30px rgba(60, 47, 32, 0.12);
}

.award-card h2 {
  margin-top: 0;
  font-family: "Erode", "Times New Roman", serif;
}

.award-card ul {
  margin: 1.2rem 0 0;
  padding-left: 1.1rem;
  color: #4b3f32;
  line-height: 1.6;
}

.award-card p {
  color: #4b3f32;
  line-height: 1.6;
}

.award-criteria {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 0.7fr);
  gap: 2.5rem;
  align-items: center;
}

.criteria-card {
  background: rgba(255, 255, 255, 0.88);
  padding: 2.5rem;
  border-radius: 28px;
  box-shadow: 0 22px 40px rgba(60, 47, 32, 0.12);
}

.criteria-card h2 {
  margin-top: 0;
  font-family: "Erode", "Times New Roman", serif;
}

.criteria-card p {
  color: #4b3f32;
  line-height: 1.6;
}

.criteria-bars {
  display: grid;
  gap: 1rem;
  margin-top: 1.4rem;
}

.criteria-bars span {
  display: block;
  font-size: 0.9rem;
  color: #4b3f32;
  margin-bottom: 0.4rem;
}

.bar {
  height: 8px;
  border-radius: 999px;
  background: rgba(163, 123, 75, 0.2);
  overflow: hidden;
}

.bar span {
  display: block;
  height: 100%;
  background: #a37b4b;
}

.criteria-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.2rem;
  text-align: center;
  margin-top: 1.4rem;
}

.criteria-grid strong {
  display: block;
  font-size: 1.4rem;
  color: #a37b4b;
}

.criteria-grid span {
  font-size: 0.85rem;
  color: #5d4a35;
}

.criteria-panel {
  background: rgba(34, 27, 19, 0.86);
  color: #f7f1e7;
  padding: 2.2rem;
  border-radius: 26px;
}

.criteria-panel p {
  color: rgba(247, 241, 231, 0.82);
  line-height: 1.6;
}

.award-showcase {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 0.7fr);
  gap: 2.5rem;
  align-items: center;
}

.showcase-card {
  background: rgba(255, 255, 255, 0.88);
  padding: 2.5rem;
  border-radius: 28px;
  box-shadow: 0 22px 40px rgba(60, 47, 32, 0.12);
}

.showcase-card h2 {
  margin-top: 0;
  font-family: "Erode", "Times New Roman", serif;
}

.showcase-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1rem;
  margin-top: 1.4rem;
}

.showcase-grid strong {
  display: block;
  font-size: 1.1rem;
  color: #a37b4b;
}

.showcase-grid span {
  font-size: 0.85rem;
  color: #5d4a35;
}

.showcase-cta {
  background: rgba(34, 27, 19, 0.86);
  color: #f7f1e7;
  padding: 2.2rem;
  border-radius: 26px;
}

.showcase-cta p {
  color: rgba(247, 241, 231, 0.82);
  line-height: 1.6;
}

.section-kicker {
  margin: 0 0 0.4rem;
  font-size: 0.75rem;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  color: #7b5a36;
}

.hero-title {
  font-family: "Erode", "Times New Roman", serif;
  font-size: clamp(2rem, 4.5vw, 3rem);
  margin: 0 0 1rem;
  color: #241c14;
}

.hero-copy {
  margin: 0 0 1.6rem;
  max-width: 36rem;
  font-size: 1.05rem;
  line-height: 1.65;
  color: #4b3f32;
}

.hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.card-kicker {
  font-size: 0.7rem;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  margin: 0 0 1.2rem;
  color: rgba(247, 241, 231, 0.75);
}

.top-nav {
  display: flex;
  flex-wrap: wrap;
  gap: 4rem;
  justify-content: center;
  flex: 1 1 520px;
  max-width: 100%;
}

.nav-link {
  color: #1f1b15;
  text-decoration: none;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  border-bottom: 1px solid transparent;
  padding-bottom: 0.2rem;
}

.nav-link.is-active {
  border-bottom-color: #1f1b15;
}

.nav-link:hover,
.nav-link:focus {
  border-bottom-color: #1f1b15;
}

.nav-cta {
  border: 1px solid #a37b4b;
  background: #ffffff;
  color: #a37b4b;
  padding: 0.6rem 1.6rem;
  border-radius: 999px;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: background-color 160ms ease, transform 160ms ease;
}

.nav-cta:hover,
.nav-cta:focus {
  background: #f1ede6;
  transform: translateY(-1px);
}

.primary-btn,
.ghost-btn {
  border-radius: 999px;
  padding: 0.65rem 1.7rem;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  border: 1px solid transparent;
  transition: transform 160ms ease, box-shadow 160ms ease;
}

.secondary-btn {
  border-radius: 999px;
  padding: 0.6rem 1.6rem;
  border: 1px solid rgba(247, 241, 231, 0.6);
  background: transparent;
  color: #f7f1e7;
  text-transform: uppercase;
  font-size: 0.75rem;
  letter-spacing: 0.08em;
  cursor: pointer;
}

.primary-btn {
  background: #a37b4b;
  color: #ffffff;
  box-shadow: 0 12px 20px rgba(163, 123, 75, 0.3);
}

.ghost-btn {
  background: transparent;
  color: #a37b4b;
  border-color: rgba(163, 123, 75, 0.6);
}

.primary-btn:hover,
.primary-btn:focus,
.ghost-btn:hover,
.ghost-btn:focus {
  transform: translateY(-1px);
}

.footer {
  position: relative;
  z-index: 1;
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

.footer-note {
  margin: 0;
  font-size: 0.8rem;
  color: rgba(247, 241, 231, 0.7);
}

@media (max-width: 900px) {
  .page {
    padding: 2rem 1.5rem 2rem;
  }

  .top {
    flex-direction: column;
    align-items: flex-start;
  }

  .top-nav {
    justify-content: flex-start;
    gap: 1.5rem 2rem;
  }

  .nav-cta {
    align-self: flex-start;
  }

  .canvas {
    padding: 2.5rem 0 3rem;
    gap: 3rem;
  }

  .award-shell,
  .award-criteria,
  .award-showcase {
    grid-template-columns: 1fr;
  }

  .award-rail,
  .criteria-card,
  .showcase-card {
    padding: 2.2rem 2rem;
  }

  .award-rail {
    position: static;
  }

  .criteria-grid,
  .showcase-grid,
  .banner-metrics {
    grid-template-columns: 1fr;
    text-align: left;
  }

  .footer {
    padding: 2.2rem 2rem 1.8rem;
  }
}
</style>
