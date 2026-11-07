* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  min-height: 100vh;
  margin: 0;
  display: flex;
  flex-direction: column;
  font-family: Arial, sans-serif;
  color: #203b32;
  background: #f8fbf7;
}

.site-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
  padding: 20px 7%;
  border-bottom: 1px solid #e0e9df;
  background: #fff;
}

.logo {
  color: #245b45;
  font-size: 1.8rem;
  font-weight: 800;
  text-decoration: none;
}

.logo span {
  color: #e58b55;
}

.navigation {
  display: flex;
  align-items: center;
  gap: 28px;
}

.navigation a {
  color: #496257;
  text-decoration: none;
}

.navigation a:hover {
  color: #24714e;
}

.header-cta,
.hero-button {
  display: inline-block;
  padding: 12px 18px;
  border-radius: 8px;
  background: #286c4d;
  color: white;
  font-weight: bold;
  text-decoration: none;
}

.hero {
  width: min(1120px, 100%);
  margin: auto;
  padding: 72px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 56px;
}

.hero-copy {
  flex: 1 1 48%;
}

.eyebrow {
  margin: 0 0 12px;
  color: #d17442;
  font-size: 0.8rem;
  font-weight: bold;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}

.hero h1 {
  max-width: 560px;
  margin: 0;
  font-size: clamp(2.5rem, 5vw, 4.4rem);
  line-height: 1.08;
  letter-spacing: -0.04em;
}

.hero-description {
  max-width: 500px;
  margin: 20px 0 26px;
  color: #5c7066;
  font-size: 1.08rem;
  line-height: 1.7;
}

.hero-art {
  position: relative;
  flex: 1 1 45%;
  max-width: 500px;
}

.hero-art img {
  display: block;
  width: 100%;
  height: 390px;
  object-fit: cover;
  border-radius: 24px;
}

.art-caption {
  position: absolute;
  right: 16px;
  bottom: 16px;
  padding: 10px 14px;
  border-radius: 8px;
  background: #fff;
  color: #245b45;
  font-weight: bold;
  box-shadow: 0 4px 14px #193b2a24;
}

.features {
  padding: 38px 20px;
  background: #eaf3e9;
  text-align: center;
}

.features h2 {
  margin: 0 0 8px;
}

.features p {
  margin: 0;
  color: #5c7066;
}

footer {
  margin-top: auto;
  padding: 18px;
  background: #203b32;
  color: white;
  text-align: center;
}

footer p {
  margin: 0;
}

@media (max-width: 720px) {
  .site-header {
    flex-wrap: wrap;
    justify-content: center;
    padding: 16px 20px;
  }

  .navigation {
    order: 3;
    width: 100%;
    justify-content: center;
    gap: 18px;
  }

  .hero {
    flex-direction: column;
    padding: 48px 22px;
    gap: 32px;
  }

  .hero-art {
    width: 100%;
    max-width: 560px;
  }

  .hero-art img {
    height: 300px;
  }
}

@media (max-width: 420px) {
  .header-cta {
    padding: 10px 12px;
  }

  .navigation {
    gap: 12px;
    font-size: 0.92rem;
  }

  .hero-art img {
    height: 240px;
  }
}