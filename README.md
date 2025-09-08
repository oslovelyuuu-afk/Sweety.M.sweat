<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="Your name / company — short tagline" />
  <title>Your Name — Services & Portfolio</title>

  <!-- Basic SEO/OpenGraph -->
  <meta property="og:title" content="Your Name — Services & Portfolio" />
  <meta property="og:description" content="Professional services, portfolio and contact" />
  <meta property="og:type" content="website" />

  <!-- Simple, self-contained styles -->
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7dd3fc; --glass: rgba(255,255,255,0.03);
      --radius:12px; --maxw:1100px; font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background: linear-gradient(180deg,#071023 0%, #07132a 100%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:32px 16px;
      display:flex;
      justify-content:center;
      font-size:16px;
    }
    .wrap{max-width:var(--maxw); width:100%;}

    header{
      display:flex; align-items:center; justify-content:space-between;
      margin-bottom:28px;
    }
    .brand{display:flex; gap:12px; align-items:center; text-decoration:none; color:inherit}
    .logo{
      width:44px; height:44px; display:flex; align-items:center; justify-content:center;
      background:linear-gradient(135deg,var(--accent),#60a5fa);
      color:#012; font-weight:700; border-radius:10px; box-shadow: 0 6px 18px rgba(0,0,0,0.5);
    }
    nav{display:flex; gap:16px; align-items:center}
    nav a{color:var(--muted); text-decoration:none; font-weight:600}
    nav a:hover{color:var(--accent)}

    /* Hero */
    .hero{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
      padding:32px; border-radius:var(--radius); margin-bottom:28px; display:flex; gap:24px; align-items:center;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      backdrop-filter: blur(6px);
    }
    .hero-left{flex:1; min-width:260px}
    .eyebrow{color:var(--accent); font-weight:700; letter-spacing:0.6px; margin-bottom:8px}
    h1{margin:0 0 12px 0; font-size:clamp(24px,4.6vw,40px)}
    p.lead{color:var(--muted); margin:0 0 18px; max-width:55ch}

    .cta-row{display:flex; gap:12px; flex-wrap:wrap}
    .btn{
      background:linear-gradient(90deg,var(--accent),#60a5fa);
      color:#022; padding:10px 16px; border-radius:10px; border:0; cursor:pointer; font-weight:700;
      text-decoration:none; display:inline-flex; gap:8px; align-items:center;
      box-shadow: 0 6px 18px rgba(96,165,250,0.12);
    }
    .btn-ghost{background:transparent; color:var(--muted); border:1px solid rgba(255,255,255,0.04)}

    .hero-right{width:340px; max-width:40%; min-width:220px}
    .card{
      background:var(--card); padding:18px; border-radius:12px; box-shadow: 0 6px 30px rgba(2,6,23,0.6);
    }
    .profile{display:flex; gap:12px; align-items:center}
    .avatar{width:56px; height:56px; border-radius:10px; flex-shrink:0; background:linear-gradient(180deg,#1f2937,#111827); display:flex; align-items:center; justify-content:center; font-weight:700}
    .meta small{color:var(--muted); display:block}
    .stats{display:flex; gap:12px; margin-top:12px}
    .stat{background:var(--glass); padding:10px; border-radius:10px; text-align:center; flex:1}

    /* Sections */
    section{margin-bottom:20px}
    .grid{display:grid; gap:16px}
    .services{grid-template-columns:repeat(auto-fit,minmax(220px,1fr))}
    .service{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); padding:18px; border-radius:12px}
    .service h3{margin:6px 0 8px}
    .portfolio{grid-template-columns:repeat(auto-fit,minmax(180px,1fr))}
    .work{height:140px; border-radius:10px; overflow:hidden; display:flex; align-items:flex-end; padding:12px; background-size:cover; background-position:center; color:#021029; font-weight:700}

    /* Contact */
    .contact-row{display:grid; grid-template-columns:1fr 360px; gap:20px}
    @media (max-width:920px){ .contact-row{grid-template-columns:1fr} .hero{flex-direction:column} .hero-right{max-width:none; width:100%} }
    form label{display:block; font-weight:600; margin-bottom:6px}
    input, textarea{
      width:100%; padding:10px 12px; border-radius:8px; border:1px solid rgba(255,255,255,0.06); background:rgba(255,255,255,0.02); color:inherit;
    }
    textarea{min-height:120px; resize:vertical}
    .muted{color:var(--muted); font-size:0.95rem}
    footer{color:var(--muted); text-align:center; padding:24px 0}
    .small{font-size:0.92rem}

    /* subtle animation */
    .fade-up{transform:translateY(10px); opacity:0; transition:all 600ms cubic-bezier(.2,.9,.2,1)}
    .inview{transform:none; opacity:1}
  </style>
</head>
<body>
  <div class="wrap" id="page">
    <header>
      <a class="brand" href="#">
        <div class="logo" aria-hidden="true">YN</div>
        <div>
          <div style="font-weight:800">Your Name</div>
          <div class="muted small">Designer • Developer • Creator</div>
        </div>
      </a>

      <nav aria-label="Main navigation">
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero" aria-labelledby="hero-title">
        <div class="hero-left">
          <div class="eyebrow">I build clean products</div>
          <h1 id="hero-title">Hi — I'm Your Name. I design & build delightful web experiences.</h1>
          <p class="lead">I help businesses and creators ship usable, accessible, and modern websites — fast. Available for freelance and long-term projects.</p>

          <div class="cta-row">
            <a class="btn" href="#contact" id="hireBtn">Hire me</a>
            <a class="btn btn-ghost" href="#portfolio">See work</a>
          </div>
        </div>

        <aside class="hero-right card" aria-label="Profile card">
          <div class="profile">
            <div class="avatar" aria-hidden="true">YN</div>
            <div class="meta">
              <div style="font-weight:700">Your Name</div>
              <small class="muted">Frontend & UI Designer</small>
            </div>
          </div>

          <div class="stats" aria-hidden="true">
            <div class="stat">
              <div style="font-size:18px;font-weight:800">5+</div>
              <div class="muted small">Years experience</div>
            </div>
            <div class="stat">
              <div style="font-size:18px;font-weight:800">120+</div>
              <div class="muted small">Projects</div>
            </div>
          </div>

        </aside>
      </section>

      <section id="about" class="card fade-up" aria-labelledby="about-title">
        <h2 id="about-title">About</h2>
        <p class="muted">I’m a product-minded designer and developer who focuses on front-end performance, accessibility, and clean design. I turn ideas into production-ready sites and prototypes.</p>
      </section>

      <section id="services" class="grid services" aria-label="Services">
        <article class="service card fade-up">
          <h3>Web Design</h3>
          <p class="muted small">UI/UX, prototypes, visual systems, design tokens.</p>
        </article>
        <article class="service card fade-up">
          <h3>Frontend Development</h3>
          <p class="muted small">Responsive sites, components, JS interactions, performance.</p>
        </article>
        <article class="service card fade-up">
          <h3>Performance & Accessibility</h3>
          <p class="muted small">Lighthouse optimization, semantic HTML, keyboard + screen reader testing.</p>
        </article>
      </section>

      <section id="portfolio" class="grid portfolio" aria-labelledby="work-title">
        <h2 id="work-title">Portfolio</h2>

        <div class="work" style="background-image:linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02)), url('https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=1200&q=60');">
          Landing page redesign
        </div>
        <div class="work" style="background-image:linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02)), url('https://images.unsplash.com/photo-1522202195469-6b5a1c9c1e1b?auto=format&fit=crop&w=1200&q=60');">
          Startup marketing site
        </div>
        <div class="work" style="background-image:linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02)), url('https://images.unsplash.com/photo-1508385082359-f7599006a7e1?auto=format&fit=crop&w=1200&q=60');">
          E-Commerce UI
        </div>
        <div class="work" style="background-image:linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02)), url('https://images.unsplash.com/photo-1517694712202-14dd9538aa97?auto=format&fit=crop&w=1200&q=60');">
          Dashboard & analytics
        </div>
      </section>

      <section id="contact" class="card fade-up" aria-labelledby="contact-title">
        <h2 id="contact-title">Contact</h2>

        <div class="contact-row">
          <div>
            <p class="muted">Prefer email? <strong><a id="mailtoLink" href="mailto:hello@example.com?subject=Inquiry%20from%20website">hello@example.com</a></strong></p>

            <form id="contactForm" aria-label="Contact form">
              <div style="margin-bottom:12px">
                <label for="name">Name</label>
                <input id="name" name="name" type="text" required placeholder="Your full name" />
              </div>

              <div style="margin-bottom:12px">
                <label for="email">Email</label>
                <input id="email" name="email" type="email" required placeholder="you@domain.com" />
              </div>

              <div style="margin-bottom:12px">
                <label for="message">Message</label>
                <textarea id="message" name="message" required placeholder="Tell me about your project..."></textarea>
              </div>

              <div style="display:flex; gap:8px; align-items:center">
                <button class="btn" type="submit">Send message</button>
                <button class="btn btn-ghost" type="button" id="clearBtn">Clear</button>
                <div id="formMsg" class="muted small" style="margin-left:auto"></div>
              </div>
            </form>
          </div>

          <aside class="card" aria-label="Contact info">
            <h3>Quick info</h3>
            <p class="muted">I usually reply within 24–48 hours. Available for freelance & remote work.</p>
            <p class="muted small"><strong>Location:</strong> Remote / Your City</p>
            <p class="muted small"><strong>Availability:</strong> Open to new projects</p>
          </aside>
        </div>
      </section>

    </main>

    <footer>
      <div class="small">© <span id="year"></span> Your Name — Built with care.</div>
    </footer>
  </div>

  <script>
    // Small interactions & form behavior (no server required)
    document.getElementById('year').textContent = new Date().getFullYear();

    // Smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const target = document.querySelector(a.getAttribute('href'));
        if(target){
          e.preventDefault();
          target.scrollIntoView({behavior:'smooth', block:'start'});
        }
      });
    });

    // Form: client-side mailto fallback
    const form = document.getElementById('contactForm');
    const formMsg = document.getElementById('formMsg');
    form.addEventListener('submit', (e)=>{
      e.preventDefault();
      const name = encodeURIComponent(form.name.value.trim());
      const email = encodeURIComponent(form.email.value.trim());
      const message = encodeURIComponent(form.message.value.trim());
      if(!name || !email || !message){
        formMsg.textContent = 'Please fill all fields.';
        return;
      }

      // Try to open user's default mail client using mailto:
      const subject = encodeURIComponent('Website inquiry from ' + name);
      const body = encodeURIComponent(`Name: ${decodeURIComponent(name)}\nEmail: ${decodeURIComponent(email)}\n\nMessage:\n${decodeURIComponent(message)}`);
      const mailto = `mailto:hello@example.com?subject=${subject}&body=${body}`;
      window.location.href = mailto;

      // show immediate confirmation (doesn't guarantee send)
      formMsg.textContent = 'Opening your mail app…';
      setTimeout(()=>{ formMsg.textContent = ''; }, 4000);
    });

    document.getElementById('clearBtn').addEventListener('click', ()=>{
      form.reset();
      document.getElementById('formMsg').textContent = '';
    });

    // Reveal animations when in view
    const observer = new IntersectionObserver((entries)=>{
      entries.forEach(ent=>{
        if(ent.isIntersecting) ent.target.classList.add('inview');
      });
    }, {threshold:0.12});
    document.querySelectorAll('.fade-up').forEach(el => observer.observe(el));
  </script>
</body>
</html><!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>My Shop</title>
  <style>
    body{font-family:Arial, sans-serif; margin:0; padding:0; background:#f7f7f7}
    header{background:#222; color:#fff; padding:15px; display:flex; justify-content:space-between}
    header h1{margin:0}
    nav a{color:#fff; margin-left:15px; text-decoration:none}
    .products{display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:20px; padding:20px}
    .product{background:#fff; padding:15px; border-radius:8px; box-shadow:0 2px 6px rgba(0,0,0,0.1)}
    .product img{max-width:100%; border-radius:8px}
    .product h3{margin:10px 0 5px}
    .btn{background:#0077ff; color:#fff; padding:8px 12px; border:none; border-radius:5px; cursor:pointer}
    footer{text-align:center; padding:20px; background:#222; color:#fff; margin-top:20px}
  </style>
</head>
<body>
  <header>
    <h1>My Shop</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">Products</a>
      <a href="#">Cart</a>
    </nav>
  </header>

  <section class="products">
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 1">
      <h3>Product 1</h3>
      <p>$10.00</p>
      <button class="btn">Add to Cart</button>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 2">
      <h3>Product 2</h3>
      <p>$15.00</p>
      <button class="btn">Add to Cart</button>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 3">
      <h3>Product 3</h3>
      <p>$20.00</p>
      <button class="btn">Add to Cart</button>
    </div>
  </section>

  <footer>
    © 2025 My Shop — All rights reserved
  </footer>
</body>
</html><section id="shop" class="card fade-up" aria-labelledby="shop-title">
  <h2 id="shop-title">Shop</h2>
  <p class="muted">Browse some of my products below:</p>

  <div class="grid products">
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 1">
      <h3>Product 1</h3>
      <p>$10.00</p>
      <button class="btn">Add to Cart</button>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 2">
      <h3>Product 2</h3>
      <p>$15.00</p>
      <button class="btn">Add to Cart</button>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 3">
      <h3>Product 3</h3>
      <p>$20.00</p>
      <button class="btn">Add to Cart</button>
    </div>
  </div>
</section>
