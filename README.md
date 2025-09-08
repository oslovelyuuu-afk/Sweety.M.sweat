<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="Your name — Portfolio & Shop with services, products and contact." />
  <title>Your Name — Portfolio & Shop</title>

  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7dd3fc; --glass: rgba(255,255,255,0.03);
      --radius:12px; --maxw:1100px; font-family: Inter, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0; background:linear-gradient(180deg,#071023 0%, #07132a 100%);
      color:#e6eef6; line-height:1.5; padding:32px 16px;
      display:flex; justify-content:center;
    }
    .wrap{max-width:var(--maxw); width:100%}
    header{display:flex; justify-content:space-between; align-items:center; margin-bottom:28px}
    .brand{display:flex; gap:12px; align-items:center; text-decoration:none; color:inherit}
    .logo{width:44px; height:44px; background:linear-gradient(135deg,var(--accent),#60a5fa); color:#012; font-weight:700; display:flex; align-items:center; justify-content:center; border-radius:10px}
    nav{display:flex; gap:16px}
    nav a{color:var(--muted); text-decoration:none; font-weight:600}
    nav a:hover{color:var(--accent)}

    /* Hero */
    .hero{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);
      padding:32px; border-radius:var(--radius); margin-bottom:28px; display:flex; gap:24px; align-items:center}
    .hero-left{flex:1}
    .eyebrow{color:var(--accent); font-weight:700; margin-bottom:8px}
    h1{margin:0 0 12px 0; font-size:clamp(24px,4.6vw,40px)}
    p.lead{color:var(--muted); margin:0 0 18px; max-width:55ch}
    .cta-row{display:flex; gap:12px; flex-wrap:wrap}
    .btn{background:linear-gradient(90deg,var(--accent),#60a5fa); color:#022; padding:10px 16px; border-radius:10px; font-weight:700; text-decoration:none; display:inline-block}
    .btn-ghost{background:transparent; color:var(--muted); border:1px solid rgba(255,255,255,0.1)}

    .hero-right{width:300px; max-width:40%}
    .card{background:var(--card); padding:18px; border-radius:12px}
    .profile{display:flex; gap:12px; align-items:center}
    .avatar{width:56px; height:56px; border-radius:10px; background:linear-gradient(180deg,#1f2937,#111827); display:flex; align-items:center; justify-content:center; font-weight:700}
    .meta small{color:var(--muted)}

    /* Sections */
    section{margin-bottom:20px}
    .grid{display:grid; gap:16px}
    .services{grid-template-columns:repeat(auto-fit,minmax(220px,1fr))}
    .service{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent); padding:18px; border-radius:12px}
    .service h3{margin:6px 0}

    .portfolio{grid-template-columns:repeat(auto-fit,minmax(180px,1fr))}
    .work{height:140px; border-radius:10px; overflow:hidden; display:flex; align-items:flex-end; padding:12px; background-size:cover; background-position:center; color:#021029; font-weight:700}

    /* Shop */
    .products{display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:20px; margin-top:20px}
    .product{background:var(--card); padding:15px; border-radius:10px; text-align:center; box-shadow:0 2px 8px rgba(0,0,0,0.3)}
    .product img{max-width:100%; border-radius:8px; margin-bottom:10px}
    .product h3{margin:6px 0}
    .product p{margin:6px 0; color:var(--muted)}

    /* Contact */
    form label{display:block; margin-bottom:6px; font-weight:600}
    input, textarea{width:100%; padding:10px; border-radius:8px; border:1px solid rgba(255,255,255,0.1); background:rgba(255,255,255,0.02); color:#fff}
    textarea{min-height:100px}
    footer{text-align:center; padding:20px; color:var(--muted)}

    /* Animation */
    .fade-up{transform:translateY(10px); opacity:0; transition:all 600ms}
    .inview{transform:none; opacity:1}
    @media(max-width:900px){.hero{flex-direction:column} .hero-right{width:100%}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <a class="brand" href="#"><div class="logo">YN</div><div><b>Your Name</b><br><small class="muted">Portfolio & Shop</small></div></a>
      <nav>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#shop">Shop</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <!-- Hero -->
      <section class="hero">
        <div class="hero-left">
          <div class="eyebrow">I build clean products</div>
          <h1>Hi — I'm Your Name. I design, develop, and sell online.</h1>
          <p class="lead">Portfolio + online shop combined. Explore my services, past work, and browse products available for purchase.</p>
          <div class="cta-row">
            <a href="#shop" class="btn">Shop Now</a>
            <a href="#contact" class="btn btn-ghost">Hire Me</a>
          </div>
        </div>
        <aside class="hero-right card">
          <div class="profile">
            <div class="avatar">YN</div>
            <div class="meta"><b>Your Name</b><br><small>Developer & Seller</small></div>
          </div>
        </aside>
      </section>

      <!-- About -->
      <section id="about" class="card fade-up">
        <h2>About</h2>
        <p class="muted">I’m a web designer, developer, and e-commerce enthusiast. I help brands build websites and also sell my own digital and physical products online.</p>
      </section>

      <!-- Services -->
      <section id="services" class="grid services">
        <article class="service card fade-up">
          <h3>Web Design</h3>
          <p class="muted small">Modern, responsive, user-friendly interfaces.</p>
        </article>
        <article class="service card fade-up">
          <h3>Development</h3>
          <p class="muted small">Clean code, fast websites, optimized performance.</p>
        </article>
        <article class="service card fade-up">
          <h3>E-commerce</h3>
          <p class="muted small">Shops, product catalogs, and payment integration.</p>
        </article>
      </section>

      <!-- Portfolio -->
      <section id="portfolio" class="grid portfolio" aria-labelledby="work-title">
        <h2 id="work-title">Portfolio</h2>
        <div class="work" style="background-image:url('https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=600');">Landing Page</div>
        <div class="work" style="background-image:url('https://images.unsplash.com/photo-1508385082359-f7599006a7e1?auto=format&fit=crop&w=600');">Dashboard UI</div>
      </section>

      <!-- Shop -->
      <section id="shop" class="card fade-up">
        <h2>Shop</h2>
        <p class="muted">Browse my products below:</p>
        <div class="products">
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

      <!-- Contact -->
      <section id="contact" class="card fade-up">
        <h2>Contact</h2>
        <form id="contactForm">
          <label for="name">Name</label>
          <input id="name" name="name" type="text" required>
          <label for="email">Email</label>
          <input id="email" name="email" type="email" required>
          <label for="message">Message</label>
          <textarea id="message" name="message" required></textarea>
          <button type="submit" class="btn">Send</button>
        </form>
        <p class="muted">Or email me directly: <a href="mailto:hello@example.com">hello@example.com</a></p>
      </section>
    </main>

    <footer>
      © <span id="year"></span> Your Name — Portfolio & Shop
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    // Reveal animation
    const observer = new IntersectionObserver((entries)=>{
      entries.forEach(ent=>{ if(ent.isIntersecting) ent.target.classList.add('inview'); });
    }, {threshold:0.1});
    document.querySelectorAll('.fade-up').forEach(el=>observer.observe(el));

    // Simple form handler (mailto fallback)
    document.getElementById('contactForm').addEventListener('submit', function(e){
      e.preventDefault();
      const name = encodeURIComponent(this.name.value);
      const email = encodeURIComponent(this.email.value);
      const message = encodeURIComponent(this.message.value);
      window.location.href = `mailto:hello@example.com?subject=Contact from ${name}&body=Email: ${email}%0D%0A${message}`;
    });
  </script>
</body>
</html>
