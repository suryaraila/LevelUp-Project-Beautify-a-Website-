# LevelUp-Project-Beautify-a-Website-
/* Base Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  color: #3e3a33;
  background:
    radial-gradient(
      circle at top left,
      rgba(186, 64, 79, 0.12),
      transparent 220px
    ),
    radial-gradient(
      circle at bottom right,
      rgba(74, 103, 65, 0.14),
      transparent 260px
    ),
    #fdf7f2;
  font-family:
    "Quicksand",
    system-ui,
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    sans-serif;
  line-height: 1.7;
}

body::before {
  content: "";
  position: fixed;
  inset: 0;
  background-image: radial-gradient(
    circle,
    rgba(255, 255, 255, 0.45) 1px,
    transparent 1px
  );
  background-size: 42px 42px;
  opacity: 0.35;
  pointer-events: none;
}

img {
  max-width: 100%;
  display: block;
}

/* Typography */
html {
  font-size: 16px;
}

h1,
h2,
h3 {
  font-family: "Playfair", serif;
  font-weight: 800;
  line-height: 1.2;
}

h1 {
  font-size: clamp(2.75rem, 4vw, 4.5rem);
  margin-bottom: 0.5rem;
}

h2 {
  font-size: clamp(2rem, 3vw, 3rem);
  margin-bottom: 1.75rem;
  text-align: center;
}

h3 {
  font-size: 1.5rem;
  margin: 1rem 0 0.75rem;
}

p {
  margin-bottom: 1rem;
  color: #57504b;
}

/* Links & Accents */
a {
  color: #4a6741;
  text-decoration: underline;
  text-decoration-color: rgba(74, 103, 65, 0.35);
}

a:hover,
a:focus {
  text-decoration-color: #4a6741;
}

.accent {
  color: #ba404f;
}

/* Layout */
.header-content,
.footer-content,
main {
  max-width: 1200px;
  margin: 0 auto;
}

header,
footer {
  text-align: center;
  padding: 3rem 1.5rem;
}

header {
  position: relative;
  overflow: hidden;
}

header::after {
  content: "";
  position: absolute;
  inset: 0;
  background:
    radial-gradient(
      circle at 20% 20%,
      rgba(186, 64, 79, 0.12),
      transparent 18%
    ),
    radial-gradient(circle at 80% 25%, rgba(74, 103, 65, 0.14), transparent 20%);
  pointer-events: none;
}

.header-content {
  position: relative;
  z-index: 1;
}

.tagline {
  color: #5a5a5a;
  letter-spacing: 0.08em;
  margin-top: 0.75rem;
}

#hero-container {
  max-width: 1150px;
  margin: 0 auto;
  padding: 0 1rem;
}

.hero-img {
  width: 100%;
  height: min(620px, 70vh);
  object-fit: cover;
  border: 1px solid #e8ded8;
  border-radius: 24px;
  box-shadow: 0 24px 60px rgba(82, 57, 53, 0.12);
}

main {
  padding: 0 1.5rem 3rem;
}

section {
  margin: 0 auto;
  padding: 4rem 0;
  max-width: 900px;
}

section:not(:last-of-type) {
  border-bottom: 1px solid #f2e6e0;
}

.about-us {
  padding-top: 2rem;
}

.about-us p:last-child {
  margin-bottom: 0;
}

.specials {
  max-width: 1150px;
  padding: 4rem 0;
}

.specials-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 2rem;
  align-items: stretch;
}

.special-offer {
  background: rgba(255, 255, 255, 0.92);
  border: 1px solid #efe2db;
  border-radius: 24px;
  padding: 2rem;
  text-align: center;
  box-shadow: 0 16px 32px rgba(78, 55, 49, 0.08);
  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease;
}

.special-offer:hover {
  transform: translateY(-6px);
  box-shadow: 0 26px 48px rgba(78, 55, 49, 0.14);
}

.special-offer img {
  height: 220px;
  width: auto;
  border: 1px solid #e8ded8;
  border-radius: 18px;
  padding: 0.75rem;
  margin-bottom: 1.25rem;
  background: #fff;
}

.price-now {
  color: #ba404f;
  font-size: 1.35rem;
  font-weight: 700;
  margin: 0.5rem 0;
}

.price-was {
  color: #7a6f6a;
  font-size: 0.95rem;
  text-decoration: line-through;
}

.visit-us {
  padding-bottom: 4rem;
}

.contact-info {
  display: grid;
  gap: 1rem;
  justify-items: center;
}

.address-block,
.phone-block {
  background: #fff;
  border: 1px solid #eadbd5;
  border-radius: 18px;
  padding: 1.2rem 1.4rem;
  width: min(520px, 100%);
}

address {
  font-style: normal;
  color: #514840;
}

iframe {
  width: 100%;
  min-height: 360px;
  border: none;
  border-radius: 24px;
  margin-top: 1.75rem;
  box-shadow: 0 18px 36px rgba(78, 55, 49, 0.08);
}

footer {
  margin-top: 2rem;
  padding-bottom: 3rem;
}

.footer-content {
  position: relative;
  z-index: 1;
}

footer p {
  color: #6b5b52;
  margin: 0.5rem 0;
}

@media (max-width: 720px) {
  header,
  footer,
  section {
    padding-left: 1rem;
    padding-right: 1rem;
  }

  .special-offer {
    padding: 1.75rem;
  }
}
