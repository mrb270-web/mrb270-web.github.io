
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Harry G. Anderson Heating & Plumbing — Trusted Residential Plumbing</title>
<meta name="description" content="Harry G. Anderson Heating & Plumbing — friendly, reliable residential plumbing and heating services. Call for a free quote today." />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Merriweather:wght@700;900&display=swap" rel="stylesheet">
<style>
  :root {
    --blue-900: #0b3a5b;
    --blue-700: #14517a;
    --blue-500: #2a7fb8;
    --blue-100: #e4f1fb;
    --accent: #f2a93b;
    --accent-dark: #d98f1f;
    --cream: #fff8ed;
    --ink: #1f2a33;
    --muted: #5a6a75;
    --card: #ffffff;
    --border: #e5e9ee;
    --shadow: 0 10px 30px rgba(11, 58, 91, 0.08);
    --radius: 14px;
  }

  * { box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body {
    margin: 0;
    font-family: 'Nunito', system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
    color: var(--ink);
    background: #fff;
    line-height: 1.6;
  }
  h1, h2, h3 { font-family: 'Merriweather', Georgia, serif; color: var(--blue-900); line-height: 1.2; margin: 0 0 .5em; }
  h1 { font-size: clamp(2.1rem, 4.4vw, 3.4rem); }
  h2 { font-size: clamp(1.7rem, 3vw, 2.3rem); }
  h3 { font-size: 1.25rem; }
  p { margin: 0 0 1em; color: var(--ink); }
  a { color: var(--blue-700); text-decoration: none; }
  a:hover { text-decoration: underline; }
  img { max-width: 100%; display: block; }

  .container { width: min(1140px, 92%); margin: 0 auto; }

  /* ---------- Top bar ---------- */
  .topbar {
    background: var(--blue-900);
    color: #fff;
    font-size: .9rem;
  }
  .topbar .container {
    display: flex; justify-content: space-between; align-items: center;
    padding: .5rem 0;
    flex-wrap: wrap; gap: .5rem;
  }
  .topbar a { color: #fff; font-weight: 600; }
  .topbar .pill {
    background: var(--accent); color: #1f2a33;
    padding: .2rem .7rem; border-radius: 999px; font-weight: 700;
  }

  /* ---------- Header / Nav ---------- */
  header.site {
    background: #fff;
    position: sticky; top: 0; z-index: 50;
    border-bottom: 1px solid var(--border);
  }
  header.site .container {
    display: flex; align-items: center; justify-content: space-between;
    padding: 1rem 0;
  }
  .logo {
    display: flex; align-items: center; gap: .7rem;
    font-family: 'Merriweather', serif;
    font-weight: 900;
    color: var(--blue-900);
    font-size: 1.15rem;
    line-height: 1.1;
  }
  .logo-mark {
    width: 44px; height: 44px; border-radius: 50%;
    background: linear-gradient(135deg, var(--blue-700), var(--blue-500));
    display: grid; place-items: center; color: #fff;
    box-shadow: var(--shadow);
  }
  .logo small { display: block; font-family: 'Nunito', sans-serif; font-weight: 600; font-size: .72rem; color: var(--muted); letter-spacing: .08em; text-transform: uppercase; }

  nav.primary { display: flex; align-items: center; gap: 1.4rem; }
  nav.primary a { color: var(--ink); font-weight: 600; }
  nav.primary a:hover { color: var(--blue-700); text-decoration: none; }

  .btn {
    display: inline-flex; align-items: center; gap: .5rem;
    background: var(--accent); color: #1f2a33;
    font-weight: 800;
    padding: .8rem 1.2rem; border-radius: 999px;
    border: none; cursor: pointer;
    transition: transform .15s ease, background .15s ease, box-shadow .15s ease;
    box-shadow: 0 6px 18px rgba(242, 169, 59, .35);
  }
  .btn:hover { background: var(--accent-dark); transform: translateY(-1px); text-decoration: none; }
  .btn.outline {
    background: transparent; color: #fff; border: 2px solid #fff;
    box-shadow: none;
  }
  .btn.outline:hover { background: rgba(255,255,255,.1); color: #fff; }
  .btn.blue { background: var(--blue-700); color: #fff; box-shadow: 0 6px 18px rgba(20, 81, 122, .3); }
  .btn.blue:hover { background: var(--blue-900); }

  .menu-toggle { display: none; background: none; border: 0; font-size: 1.6rem; color: var(--blue-900); cursor: pointer; }

  /* ---------- Hero ---------- */
  .hero {
    position: relative;
    background:
      linear-gradient(180deg, rgba(11,58,91,.78), rgba(11,58,91,.62)),
      url('https://images.unsplash.com/photo-1607472586893-edb57bdc0e39?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
    color: #fff;
    padding: clamp(4rem, 9vw, 7rem) 0 clamp(4rem, 8vw, 6rem);
  }
  .hero h1 { color: #fff; }
  .hero p.lead { font-size: 1.15rem; max-width: 640px; color: #f3f7fb; }
  .hero .cta-row {
    display: flex; flex-wrap: wrap; gap: .9rem; margin-top: 1.7rem;
  }
  .trust-strip {
    margin-top: 2.5rem;
    display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem;
    max-width: 720px;
  }
  .trust-strip div {
    background: rgba(255,255,255,.1);
    backdrop-filter: blur(6px);
    border: 1px solid rgba(255,255,255,.18);
    border-radius: 12px;
    padding: .8rem .7rem;
    text-align: center;
    font-weight: 700;
    font-size: .85rem;
  }
  .trust-strip strong { display:block; font-size: 1.25rem; font-family: 'Merriweather', serif; color: var(--accent); }

  /* ---------- Sections ---------- */
  section { padding: clamp(3.5rem, 7vw, 5.5rem) 0; }
  .section-head { text-align: center; margin-bottom: 2.5rem; }
  .eyebrow {
    color: var(--blue-500); text-transform: uppercase; letter-spacing: .15em;
    font-weight: 800; font-size: .78rem; margin-bottom: .6rem;
  }
  .section-head p { color: var(--muted); max-width: 620px; margin: 0 auto; }

  /* About */
  .about { background: var(--cream); }
  .about-grid {
    display: grid; grid-template-columns: 1.1fr 1fr; gap: 3rem; align-items: center;
  }
  .about-image {
    border-radius: var(--radius);
    overflow: hidden;
    box-shadow: var(--shadow);
    aspect-ratio: 4/3;
    background: url('plumber.jpg') center/cover no-repeat;
  }
  .feature-list {
    list-style: none; padding: 0; margin: 1.5rem 0 0;
    display: grid; grid-template-columns: 1fr 1fr; gap: 1rem 1.5rem;
  }
  .feature-list li {
    display: flex; align-items: flex-start; gap: .6rem;
    font-weight: 600;
  }
  .check {
    flex: none;
    width: 26px; height: 26px; border-radius: 50%;
    background: var(--accent); color: #1f2a33;
    display: grid; place-items: center; font-weight: 900;
    margin-top: 2px;
  }

  /* Services */
  .services-grid {
    display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem;
  }
  .service-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.7rem 1.5rem;
    box-shadow: var(--shadow);
    transition: transform .2s ease, box-shadow .2s ease;
  }
  .service-card:hover { transform: translateY(-4px); box-shadow: 0 18px 40px rgba(11,58,91,.12); }
  .service-icon {
    width: 56px; height: 56px; border-radius: 14px;
    background: var(--blue-100); color: var(--blue-700);
    display: grid; place-items: center; font-size: 1.6rem;
    margin-bottom: 1rem;
  }
  .service-card h3 { margin-bottom: .3rem; }
  .service-card p { color: var(--muted); margin-bottom: 0; font-size: .97rem; }

  /* Why choose us strip */
  .why {
    background: var(--blue-900);
    color: #fff;
  }
  .why h2 { color: #fff; }
  .why .section-head p { color: #c9dbe8; }
  .why-grid {
    display: grid; grid-template-columns: repeat(4, 1fr); gap: 1.5rem;
  }
  .why-card {
    text-align: center;
    padding: 1.5rem 1rem;
  }
  .why-num {
    font-family: 'Merriweather', serif; color: var(--accent);
    font-size: 2.4rem; font-weight: 900; line-height: 1;
    margin-bottom: .6rem;
  }
  .why-card h3 { color: #fff; font-size: 1.05rem; margin-bottom: .3rem; }
  .why-card p { color: #c9dbe8; font-size: .93rem; margin: 0; }

  /* Gallery */
  .gallery {
    display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem;
  }
  .gallery figure {
    margin: 0; border-radius: var(--radius); overflow: hidden;
    box-shadow: var(--shadow); position: relative;
    aspect-ratio: 4/3;
  }
  .gallery img {
    width: 100%; height: 100%; object-fit: cover;
    transition: transform .4s ease;
  }
  .gallery figure:hover img { transform: scale(1.05); }
  .gallery figcaption {
    position: absolute; left: 0; right: 0; bottom: 0;
    background: linear-gradient(180deg, transparent, rgba(11,58,91,.85));
    color: #fff; padding: 1.2rem 1rem .8rem; font-weight: 700;
  }

  /* Testimonials */
  .testimonials { background: var(--cream); }
  .testi-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }
  .testi-card {
    background: #fff;
    border-radius: var(--radius);
    padding: 1.7rem;
    box-shadow: var(--shadow);
    border: 1px solid var(--border);
    display: flex; flex-direction: column;
  }
  .stars { color: var(--accent); margin-bottom: .7rem; font-size: 1.1rem; letter-spacing: 2px; }
  .testi-card blockquote {
    margin: 0 0 1.2rem; font-style: italic; color: var(--ink);
    flex: 1;
  }
  .testi-author {
    display: flex; align-items: center; gap: .8rem;
    border-top: 1px solid var(--border); padding-top: 1rem;
  }
  .avatar {
    width: 44px; height: 44px; border-radius: 50%;
    background: var(--blue-100); color: var(--blue-700);
    display: grid; place-items: center; font-weight: 800;
  }
  .testi-author strong { display: block; }
  .testi-author span { color: var(--muted); font-size: .88rem; }

  /* CTA band */
  .cta-band {
    background: linear-gradient(135deg, var(--blue-700), var(--blue-900));
    color: #fff; text-align: center;
  }
  .cta-band h2 { color: #fff; }
  .cta-band p { color: #d6e5f1; max-width: 620px; margin: 0 auto 1.5rem; }
  .cta-band .big-phone {
    display: inline-block; margin-top: 1rem;
    font-family: 'Merriweather', serif; font-weight: 900;
    font-size: clamp(1.8rem, 4vw, 2.6rem); color: var(--accent);
  }

  /* Contact */
  .contact-grid {
    display: grid; grid-template-columns: 1fr 1fr; gap: 3rem; align-items: start;
  }
  .contact-info ul {
    list-style: none; padding: 0; margin: 1.5rem 0 0;
  }
  .contact-info li {
    display: flex; gap: 1rem; align-items: flex-start;
    padding: .8rem 0; border-bottom: 1px solid var(--border);
  }
  .contact-info li:last-child { border-bottom: 0; }
  .contact-icon {
    width: 42px; height: 42px; border-radius: 10px;
    background: var(--blue-100); color: var(--blue-700);
    display: grid; place-items: center; flex: none; font-size: 1.1rem;
  }
  .contact-info strong { display: block; color: var(--blue-900); }
  .contact-info span { color: var(--muted); }

  form.quote {
    background: #fff;
    border: 1px solid var(--border);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    padding: 1.8rem;
  }
  form.quote label { display: block; font-weight: 700; margin-bottom: .3rem; font-size: .92rem; }
  form.quote input, form.quote select, form.quote textarea {
    width: 100%;
    padding: .75rem .9rem;
    border: 1px solid var(--border);
    border-radius: 10px;
    font-family: inherit; font-size: 1rem;
    margin-bottom: 1rem;
    background: #fafcfe;
    transition: border .15s ease, box-shadow .15s ease;
  }
  form.quote input:focus, form.quote select:focus, form.quote textarea:focus {
    outline: none;
    border-color: var(--blue-500);
    box-shadow: 0 0 0 3px rgba(42, 127, 184, .15);
  }
  form.quote .row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }
  form.quote .note { font-size: .82rem; color: var(--muted); margin-top: -.5rem; }

  /* Footer */
  footer {
    background: #0a2a43;
    color: #c9dbe8;
    padding: 3rem 0 1.5rem;
    font-size: .93rem;
  }
  .footer-grid {
    display: grid; grid-template-columns: 2fr 1fr 1fr 1fr; gap: 2rem;
  }
  footer h4 { color: #fff; font-family: 'Merriweather', serif; margin: 0 0 .8rem; font-size: 1rem; }
  footer a { color: #c9dbe8; }
  footer a:hover { color: var(--accent); text-decoration: none; }
  footer ul { list-style: none; padding: 0; margin: 0; }
  footer ul li { padding: .25rem 0; }
  .copyright {
    border-top: 1px solid rgba(255,255,255,.1);
    margin-top: 2.5rem; padding-top: 1.2rem; text-align: center;
    color: #8ea7b9;
  }

  /* Responsive */
  @media (max-width: 900px) {
    nav.primary { display: none; position: absolute; top: 100%; left: 0; right: 0; background: #fff; flex-direction: column; gap: 0; padding: 1rem 0; border-bottom: 1px solid var(--border); box-shadow: var(--shadow); }
    nav.primary.open { display: flex; }
    nav.primary a { padding: .7rem 1.5rem; width: 100%; border-bottom: 1px solid var(--border); }
    nav.primary .btn { margin: .7rem 1.5rem; }
    .menu-toggle { display: block; }
    .about-grid, .contact-grid { grid-template-columns: 1fr; gap: 2rem; }
    .services-grid, .gallery, .testi-grid, .why-grid { grid-template-columns: 1fr 1fr; }
    .feature-list { grid-template-columns: 1fr; }
    .trust-strip { grid-template-columns: 1fr 1fr; }
    .footer-grid { grid-template-columns: 1fr 1fr; }
    form.quote .row { grid-template-columns: 1fr; }
  }
  @media (max-width: 560px) {
    .services-grid, .gallery, .testi-grid, .why-grid { grid-template-columns: 1fr; }
    .footer-grid { grid-template-columns: 1fr; }
    .topbar .container { justify-content: center; text-align: center; }
  }
</style>
</head>
<body>

<!-- Top bar -->
<div class="topbar">
  <div class="container">
    <span>🕒 Mon–Sat, 7am–7pm &nbsp;|&nbsp; 📍 [Your Service Area]</span>
    <span><span class="pill">Free Quotes</span> &nbsp; Call us: <a href="tel:+10000000000">(000) 000-0000</a></span>
  </div>
</div>

<!-- Header -->
<header class="site">
  <div class="container">
    <a href="#" class="logo" aria-label="Harry G. Anderson Heating & Plumbing home">
      <span class="logo-mark" aria-hidden="true">
        <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14.7 6.3a4 4 0 0 0-5.4 5.4l-6 6a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l6-6a4 4 0 0 0 5.4-5.4l-2.5 2.5-2-2 2.5-2.5z"/></svg>
      </span>
      <span>
        Harry G. Anderson
        <small>Heating &amp; Plumbing</small>
      </span>
    </a>
    <button class="menu-toggle" aria-label="Toggle menu" onclick="document.querySelector('nav.primary').classList.toggle('open')">☰</button>
    <nav class="primary">
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#why">Why Us</a>
      <a href="#gallery">Our Work</a>
      <a href="#testimonials">Reviews</a>
      <a href="#contact" class="btn">📞 Free Quote</a>
    </nav>
  </div>
</header>

<!-- Hero -->
<section class="hero">
  <div class="container">
    <span class="eyebrow" style="color: var(--accent);">Trusted Residential Plumbing</span>
    <h1>Plumbing you can count on — from a family you can trust.</h1>
    <p class="lead">From leaky faucets to full home repipes, Harry G. Anderson Heating &amp; Plumbing has been helping neighbors keep water flowing and homes comfortable for over 25 years. Honest work. Fair prices. Done right the first time.</p>
    <div class="cta-row">
      <a href="tel:+10000000000" class="btn">📞 Call for a Free Quote</a>
      <a href="#services" class="btn outline">See Our Services</a>
    </div>
    <div class="trust-strip" aria-label="Company highlights">
      <div><strong>25+</strong>Years Serving Homes</div>
      <div><strong>5,000+</strong>Happy Customers</div>
      <div><strong>100%</strong>Satisfaction Guaranteed</div>
      <div><strong>A+</strong>BBB Rating</div>
    </div>
  </div>
</section>

<!-- About -->
<section id="about" class="about">
  <div class="container">
    <div class="about-grid">
      <div>
        <span class="eyebrow">About Us</span>
        <h2>A family-run company that treats your home like our own.</h2>
        <p>We started Harry G. Anderson Heating &amp; Plumbing because we believe homeowners deserve better — a plumber who shows up on time, explains things clearly, and charges a fair price for great work. No surprises, no pressure, no shortcuts.</p>
        <p>Whether it's a small repair, a bathroom remodel, or a brand-new build, every job gets the same care and attention we'd want in our own home.</p>
        <ul class="feature-list">
          <li><span class="check" aria-hidden="true">✓</span> Licensed &amp; fully insured</li>
          <li><span class="check" aria-hidden="true">✓</span> Upfront, honest pricing</li>
          <li><span class="check" aria-hidden="true">✓</span> Respectful, clean crews</li>
          <li><span class="check" aria-hidden="true">✓</span> Workmanship guarantee</li>
          <li><span class="check" aria-hidden="true">✓</span> Local &amp; family-owned</li>
          <li><span class="check" aria-hidden="true">✓</span> Free, no-pressure quotes</li>
        </ul>
      </div>
      <div class="about-image" role="img" aria-label="Plumber working under a kitchen sink with a tool bag of supplies"></div>
    </div>
  </div>
</section>

<!-- Services -->
<section id="services">
  <div class="container">
    <div class="section-head">
      <span class="eyebrow">What We Do</span>
      <h2>Residential plumbing services, done right.</h2>
      <p>From minor fixes to full construction plumbing, we handle every job with care, quality materials, and craftsmanship you can rely on for years to come.</p>
    </div>
    <div class="services-grid">
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">🚿</div>
        <h3>Bathroom &amp; Kitchen Plumbing</h3>
        <p>Remodels, fixture upgrades, sink &amp; faucet installs, tub and shower replacements — beautifully finished, built to last.</p>
      </article>
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">🔧</div>
        <h3>Leak &amp; Pipe Repair</h3>
        <p>Fast, thorough diagnosis of leaks, low water pressure, and pipe issues. We fix the root cause — not just the symptom.</p>
      </article>
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">🏠</div>
        <h3>New Home Plumbing</h3>
        <p>Full rough-in and finish plumbing for new builds and major renovations, coordinated closely with your builder or GC.</p>
      </article>
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">💧</div>
        <h3>Water Heater Install &amp; Repair</h3>
        <p>Tank and tankless water heaters — expert installation, replacement, and repair for reliable hot water on demand.</p>
      </article>
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">🌡️</div>
        <h3>Heating Systems</h3>
        <p>Boilers, radiant heat, and hydronic heating — installed, serviced, and tuned up for efficient comfort all winter long.</p>
      </article>
      <article class="service-card">
        <div class="service-icon" aria-hidden="true">🚰</div>
        <h3>Drain Cleaning &amp; Sewer</h3>
        <p>Clogged drains, slow sinks, main line issues — cleared quickly with modern equipment and clean, respectful service.</p>
      </article>
    </div>
  </div>
</section>

<!-- Why Choose Us -->
<section id="why" class="why">
  <div class="container">
    <div class="section-head">
      <span class="eyebrow" style="color: var(--accent);">Why Hire Us</span>
      <h2>Four reasons homeowners keep calling us back.</h2>
      <p>We're not the biggest plumbing company in town — and we don't want to be. We'd rather do fewer jobs, better, and earn your trust for life.</p>
    </div>
    <div class="why-grid">
      <div class="why-card">
        <div class="why-num">01</div>
        <h3>Honest, Upfront Pricing</h3>
        <p>You'll know the price before we start. No surprise fees, no pressure to upsell — ever.</p>
      </div>
      <div class="why-card">
        <div class="why-num">02</div>
        <h3>Craftsmanship That Lasts</h3>
        <p>Quality materials, tidy installs, and work we're proud to put our name on.</p>
      </div>
      <div class="why-card">
        <div class="why-num">03</div>
        <h3>On Time, Every Time</h3>
        <p>We respect your schedule. If we say we'll be there at 9, we'll be there at 9.</p>
      </div>
      <div class="why-card">
        <div class="why-num">04</div>
        <h3>Real People, Real Answers</h3>
        <p>Call us and talk to a human who knows your home — not a call center.</p>
      </div>
    </div>
  </div>
</section>

<!-- Gallery -->
<section id="gallery">
  <div class="container">
    <div class="section-head">
      <span class="eyebrow">Our Work</span>
      <h2>Recent projects we're proud of.</h2>
      <p>A glimpse of the homes and families we've helped. Your project could be next.</p>
    </div>
    <div class="gallery">
      <figure>
        <img src="https://images.unsplash.com/photo-1620626011761-996317b8d101?auto=format&fit=crop&w=800&q=80" alt="Modern bathroom remodel with tile shower" />
        <figcaption>Bathroom Remodel — Riverside</figcaption>
      </figure>
      <figure>
        <img src="https://images.unsplash.com/photo-1556909114-f6e7ad7d3136?auto=format&fit=crop&w=800&q=80" alt="Custom kitchen with farmhouse sink" />
        <figcaption>Kitchen Renovation — Oak Hill</figcaption>
      </figure>
      <figure>
        <img src="new-construction.jpg" alt="New construction plumbing rough-in" />
        <figcaption>New Home Rough-In — Cedar Ridge</figcaption>
      </figure>
      <figure>
        <img src="water-heater.jpg" alt="Water heater installation" />
        <figcaption>Water Heater Install</figcaption>
      </figure>
      <figure>
        <img src="radiant-heat.webp" alt="Radiant floor heating installation" />
        <figcaption>Radiant Heat Install — Maple St.</figcaption>
      </figure>
      <figure>
        <img src="copper.jpg" alt="Whole-home copper repipe project" />
        <figcaption>Whole-Home Repipe — Elmwood</figcaption>
      </figure>
    </div>
  </div>
</section>

<!-- Testimonials -->
<section id="testimonials" class="testimonials">
  <div class="container">
    <div class="section-head">
      <span class="eyebrow">What Customers Say</span>
      <h2>Neighbors who've trusted us with their homes.</h2>
    </div>
    <div class="testi-grid">
      <article class="testi-card">
        <div class="stars" aria-label="5 out of 5 stars">★★★★★</div>
        <blockquote>“Harry and his team were on time, respectful, and left the place cleaner than they found it. They explained everything in plain English and the price was exactly what they quoted. Couldn't ask for more.”</blockquote>
        <div class="testi-author">
          <div class="avatar">SM</div>
          <div><strong>Sarah M.</strong><span>Bathroom Remodel</span></div>
        </div>
      </article>
      <article class="testi-card">
        <div class="stars" aria-label="5 out of 5 stars">★★★★★</div>
        <blockquote>“We had a mystery leak that two other plumbers couldn't find. Harry figured it out in 20 minutes and had it fixed the same day. Honest, skilled, and a really nice guy.”</blockquote>
        <div class="testi-author">
          <div class="avatar">DR</div>
          <div><strong>David R.</strong><span>Leak Repair</span></div>
        </div>
      </article>
      <article class="testi-card">
        <div class="stars" aria-label="5 out of 5 stars">★★★★★</div>
        <blockquote>“We used Anderson for the full plumbing on our new build. The quality of their work is beautiful and their crew was a pleasure to have on site. We'd hire them again in a heartbeat.”</blockquote>
        <div class="testi-author">
          <div class="avatar">JT</div>
          <div><strong>Jen &amp; Tom K.</strong><span>New Construction</span></div>
        </div>
      </article>
    </div>
  </div>
</section>

<!-- CTA Band -->
<section class="cta-band">
  <div class="container">
    <span class="eyebrow" style="color: var(--accent);">Ready to Get Started?</span>
    <h2>Get your free, no-pressure quote today.</h2>
    <p>Give us a call — we'll listen, take a look, and give you a straight answer about what your project needs and what it'll cost.</p>
    <a href="tel:+10000000000" class="btn">📞 Call Now for a Free Quote</a>
    <div class="big-phone"><a href="tel:+10000000000" style="color:inherit;">(000) 000-0000</a></div>
  </div>
</section>

<!-- Contact -->
<section id="contact">
  <div class="container">
    <div class="section-head">
      <span class="eyebrow">Get in Touch</span>
      <h2>We'd love to hear from you.</h2>
      <p>Call us for the fastest response, or send us a message and we'll get back to you within one business day.</p>
    </div>
    <div class="contact-grid">
      <div class="contact-info">
        <h3>Contact Information</h3>
        <p>Prefer to talk to a real person? Give us a call — we answer the phone ourselves during business hours.</p>
        <ul>
          <li>
            <div class="contact-icon">📞</div>
            <div><strong>Phone</strong><span><a href="tel:+10000000000">(000) 000-0000</a></span></div>
          </li>
          <li>
            <div class="contact-icon">✉️</div>
            <div><strong>Email</strong><span><a href="mailto:hello@andersonplumbing.com">hello@andersonplumbing.com</a></span></div>
          </li>
          <li>
            <div class="contact-icon">📍</div>
            <div><strong>Service Area</strong><span>[Your City] and surrounding communities</span></div>
          </li>
          <li>
            <div class="contact-icon">🕒</div>
            <div><strong>Hours</strong><span>Mon–Sat: 7:00 AM – 7:00 PM<br>Sunday: Emergency calls only</span></div>
          </li>
        </ul>
      </div>
      <form class="quote" onsubmit="event.preventDefault(); alert('Thanks! Connect this form to your email service to receive submissions.');">
        <h3>Request a Free Quote</h3>
        <div class="row">
          <div>
            <label for="name">Your Name</label>
            <input id="name" type="text" placeholder="Jane Smith" required />
          </div>
          <div>
            <label for="phone">Phone</label>
            <input id="phone" type="tel" placeholder="(555) 555-5555" required />
          </div>
        </div>
        <label for="email">Email</label>
        <input id="email" type="email" placeholder="you@example.com" required />
        <label for="service">What do you need help with?</label>
        <select id="service" required>
          <option value="">Please select…</option>
          <option>Bathroom or kitchen plumbing</option>
          <option>Leak or pipe repair</option>
          <option>New home construction</option>
          <option>Water heater</option>
          <option>Heating system</option>
          <option>Drain or sewer</option>
          <option>Something else</option>
        </select>
        <label for="message">Tell us a little about your project</label>
        <textarea id="message" rows="4" placeholder="A few sentences about what's going on is plenty..."></textarea>
        <button type="submit" class="btn blue" style="width: 100%; justify-content: center;">Send My Request</button>
        <p class="note">We'll reply within one business day. For faster help, please call us directly.</p>
      </form>
    </div>
  </div>
</section>

<!-- Footer -->
<footer>
  <div class="container">
    <div class="footer-grid">
      <div>
        <h4>Harry G. Anderson Heating &amp; Plumbing</h4>
        <p>Family-owned residential plumbing and heating serving [Your City] and surrounding communities. Honest work, fair prices, done right.</p>
      </div>
      <div>
        <h4>Services</h4>
        <ul>
          <li><a href="#services">Bathroom &amp; Kitchen</a></li>
          <li><a href="#services">Leak &amp; Pipe Repair</a></li>
          <li><a href="#services">New Construction</a></li>
          <li><a href="#services">Water Heaters</a></li>
          <li><a href="#services">Heating Systems</a></li>
        </ul>
      </div>
      <div>
        <h4>Company</h4>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#why">Why Choose Us</a></li>
          <li><a href="#gallery">Our Work</a></li>
          <li><a href="#testimonials">Reviews</a></li>
        </ul>
      </div>
      <div>
        <h4>Contact</h4>
        <ul>
          <li><a href="tel:+10000000000">(000) 000-0000</a></li>
          <li><a href="mailto:hello@andersonplumbing.com">hello@andersonplumbing.com</a></li>
          <li>Mon–Sat, 7am–7pm</li>
          <li>Licensed &amp; Insured</li>
        </ul>
      </div>
    </div>
    <div class="copyright">
      © <span id="year"></span> Harry G. Anderson Heating &amp; Plumbing. All rights reserved. &nbsp;|&nbsp; Licensed &amp; Insured.
    </div>
  </div>
</footer>

<script>
  document.getElementById('year').textContent = new Date().getFullYear();
</script>

</body>
</html>
