# melandjoy
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mel & Joy Beauty | Advanced Skincare & Aesthetic Treatments Auckland</title>
  <meta name="description" content="Certified advanced skincare, bespoke facials, microneedling, and holistic massage therapy in Birkdale, North Shore Auckland by Ana Garcia." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
  
  <style>
    :root {
      --blush-light: #FDF7F5;
      --blush-surface: #F9EFEB;
      --blush-accent: #E8CAC1;
      --rose-taupe: #C99E94;
      --deep-wine: #5C2430;
      --charcoal: #2A2426;
      --cream: #FAF6F0;
      --gold-accent: #C5A059;
      --whatsapp-green: #25D366;
      --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      background-color: var(--cream);
      color: var(--charcoal);
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 16px;
      line-height: 1.7;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }

    h1, h2, h3, h4, .serif-font {
      font-family: 'Cormorant Garamond', Georgia, serif;
      letter-spacing: 0.02em;
    }

    /* TOP BAR - Restored to classic Blush/Rose Taupe */
    .top-bar {
      background-color: var(--blush-surface);
      color: var(--deep-wine);
      padding: 9px 24px;
      font-size: 0.85rem;
      border-bottom: 1px solid var(--blush-accent);
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .top-bar a {
      color: var(--deep-wine);
      text-decoration: none;
      font-weight: 500;
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }

    .top-bar-left, .top-bar-right {
      display: flex;
      align-items: center;
      gap: 18px;
    }

    /* NAVBAR */
    header {
      background: rgba(253, 247, 245, 0.96);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(232, 202, 193, 0.5);
      position: sticky;
      top: 38px;
      z-index: 99;
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 14px 24px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .brand-logo-wrap {
      display: flex;
      align-items: center;
      gap: 12px;
      text-decoration: none;
      color: var(--deep-wine);
    }

    .brand-badge {
      width: 44px;
      height: 44px;
      border-radius: 50%;
      border: 1.5px solid var(--rose-taupe);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Cormorant Garamond', serif;
      font-weight: 600;
      font-size: 1.25rem;
      color: var(--deep-wine);
      background: var(--blush-light);
    }

    .brand-title {
      font-size: 1.45rem;
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
      align-items: center;
    }

    nav a {
      text-decoration: none;
      color: var(--charcoal);
      font-size: 0.95rem;
      font-weight: 500;
      transition: var(--transition);
    }

    nav a:hover {
      color: var(--rose-taupe);
    }

    .btn-wa-nav {
      background-color: var(--deep-wine);
      color: #fff !important;
      padding: 9px 20px;
      border-radius: 40px;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
      font-size: 0.88rem;
    }

    .btn-wa-nav:hover {
      background-color: #7A3241;
      transform: translateY(-1px);
    }

    /* HERO SECTION */
    .hero {
      position: relative;
      height: 82vh;
      min-height: 580px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: #fff;
      overflow: hidden;
    }

    .hero-video-bg {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: 1;
      filter: brightness(0.62);
    }

    .hero-overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(180deg, rgba(42,36,38,0.4) 0%, rgba(92,36,48,0.3) 100%);
      z-index: 2;
    }

    .hero-content {
      position: relative;
      z-index: 3;
      max-width: 820px;
      padding: 0 20px;
    }

    .hero-badge {
      display: inline-block;
      padding: 6px 16px;
      border: 1px solid rgba(255,255,255,0.4);
      border-radius: 30px;
      font-size: 0.85rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      margin-bottom: 20px;
      background: rgba(0,0,0,0.25);
      backdrop-filter: blur(4px);
    }

    .hero h1 {
      font-size: clamp(2.4rem, 5.5vw, 4.4rem);
      font-weight: 300;
      line-height: 1.15;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: clamp(1rem, 2vw, 1.25rem);
      max-width: 640px;
      margin: 0 auto 32px;
      font-weight: 300;
      color: rgba(255,255,255,0.92);
    }

    .hero-actions {
      display: flex;
      gap: 16px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn {
      padding: 13px 30px;
      border-radius: 30px;
      font-size: 0.95rem;
      text-decoration: none;
      font-weight: 500;
      display: inline-flex;
      align-items: center;
      gap: 9px;
      transition: var(--transition);
      cursor: pointer;
    }

    .btn-primary {
      background-color: var(--whatsapp-green);
      color: #fff;
    }

    .btn-primary:hover {
      background-color: #1EBE5D;
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(37, 211, 102, 0.35);
    }

    .btn-secondary {
      background-color: rgba(255,255,255,0.15);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(255,255,255,0.6);
      color: #fff;
    }

    .btn-secondary:hover {
      background-color: rgba(255,255,255,0.3);
      transform: translateY(-2px);
    }

    /* ABOUT THE THERAPIST SECTION */
    .therapist-section {
      padding: 100px 24px;
      max-width: 1140px;
      margin: 0 auto;
    }

    .therapist-grid {
      display: grid;
      grid-template-columns: 1fr 1.35fr;
      gap: 60px;
      align-items: center;
    }

    .therapist-image-card {
      position: relative;
    }

    .therapist-frame {
      position: relative;
      border-radius: 24px;
      overflow: hidden;
      box-shadow: 0 20px 40px rgba(92, 36, 48, 0.12);
      border: 8px solid #fff;
    }

    .therapist-frame img {
      width: 100%;
      height: 520px;
      object-fit: cover;
      object-position: center top;
      display: block;
    }

    .therapist-tag {
      position: absolute;
      bottom: -18px;
      right: 20px;
      background: var(--blush-surface);
      border: 1px solid var(--rose-taupe);
      padding: 12px 22px;
      border-radius: 30px;
      color: var(--deep-wine);
      box-shadow: 0 8px 24px rgba(0,0,0,0.06);
    }

    .therapist-tag span {
      display: block;
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: #777;
    }

    .therapist-tag strong {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.3rem;
    }

    .therapist-info h2 {
      font-size: 2.8rem;
      line-height: 1.15;
      color: var(--deep-wine);
      margin-bottom: 12px;
    }

    .therapist-subtitle {
      font-size: 1.1rem;
      color: var(--rose-taupe);
      font-weight: 500;
      margin-bottom: 24px;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .therapist-info p {
      font-size: 1.05rem;
      color: #555;
      margin-bottom: 20px;
    }

    .therapist-quote {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: 1.35rem;
      font-style: italic;
      color: var(--deep-wine);
      border-left: 3px solid var(--rose-taupe);
      padding-left: 20px;
      margin: 28px 0;
    }

    /* SERVICES / MENU */
    .services-section {
      background-color: var(--blush-light);
      padding: 100px 24px;
      border-top: 1px solid var(--blush-accent);
      border-bottom: 1px solid var(--blush-accent);
    }

    .section-head {
      text-align: center;
      max-width: 680px;
      margin: 0 auto 60px;
    }

    .section-subtitle {
      font-size: 0.85rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--rose-taupe);
      display: block;
      margin-bottom: 8px;
    }

    .section-head h2 {
      font-size: clamp(2rem, 3.5vw, 3rem);
      color: var(--deep-wine);
      margin-bottom: 16px;
    }

    .category-title {
      font-size: 1.6rem;
      color: var(--deep-wine);
      margin: 40px 0 24px;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .category-title::after {
      content: "";
      flex: 1;
      height: 1px;
      background: var(--blush-accent);
    }

    .services-grid {
      max-width: 1140px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
      gap: 28px;
    }

    .service-card {
      background: #fff;
      border: 1px solid rgba(232, 202, 193, 0.7);
      border-radius: 16px;
      padding: 32px;
      transition: var(--transition);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .service-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 30px rgba(92, 36, 48, 0.08);
      border-color: var(--rose-taupe);
    }

    .service-tag {
      font-size: 0.75rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      padding: 4px 10px;
      border-radius: 20px;
      display: inline-block;
      margin-bottom: 14px;
      background: var(--blush-surface);
      color: var(--deep-wine);
    }

    .service-card h3 {
      font-size: 1.6rem;
      color: var(--deep-wine);
      margin-bottom: 12px;
    }

    .service-card p {
      font-size: 0.95rem;
      color: #666;
      margin-bottom: 24px;
      flex-grow: 1;
    }

    .btn-card-wa {
      color: var(--deep-wine);
      text-decoration: none;
      font-size: 0.88rem;
      font-weight: 600;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      border-top: 1px dashed var(--blush-accent);
      padding-top: 16px;
    }

    .btn-card-wa:hover {
      color: var(--whatsapp-green);
    }

    /* WHATSAPP CTA BANNER */
    .wa-cta-banner {
      max-width: 1140px;
      margin: 60px auto 0;
      background: linear-gradient(135deg, var(--deep-wine) 0%, #3d141d 100%);
      border-radius: 20px;
      padding: 48px;
      color: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 30px;
      flex-wrap: wrap;
    }

    .wa-cta-text h3 {
      font-size: 2.2rem;
      margin-bottom: 10px;
    }

    .wa-cta-text p {
      color: rgba(255,255,255,0.85);
      font-size: 1.05rem;
    }

    /* INFO & HOURS SECTION */
    .details-section {
      padding: 90px 24px;
      max-width: 1140px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
    }

    .info-card {
      background: #fff;
      border: 1px solid var(--blush-accent);
      border-radius: 20px;
      padding: 40px;
    }

    .info-card h3 {
      font-size: 2rem;
      color: var(--deep-wine);
      margin-bottom: 24px;
    }

    .hours-table {
      width: 100%;
      border-collapse: collapse;
    }

    .hours-table tr {
      border-bottom: 1px solid #f2e9e6;
    }

    .hours-table td {
      padding: 11px 0;
      font-size: 0.95rem;
    }

    .hours-table td:last-child {
      text-align: right;
      font-weight: 500;
    }

    .status-badge {
      display: inline-block;
      padding: 4px 10px;
      border-radius: 20px;
      font-size: 0.8rem;
      font-weight: 600;
      margin-bottom: 18px;
      background: #e8f5e9;
      color: #2e7d32;
    }

    /* FOOTER */
    footer {
      background: var(--charcoal);
      color: #fff;
      padding: 60px 24px 30px;
      font-size: 0.9rem;
    }

    .footer-container {
      max-width: 1140px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 40px;
      margin-bottom: 40px;
    }

    .footer-col h4 {
      font-size: 1.3rem;
      color: var(--blush-accent);
      margin-bottom: 18px;
    }

    .footer-col p, .footer-col a {
      color: rgba(255,255,255,0.7);
      text-decoration: none;
      line-height: 1.8;
      display: block;
    }

    .footer-col a:hover {
      color: #fff;
    }

    .footer-bottom {
      border-top: 1px solid rgba(255,255,255,0.1);
      padding-top: 24px;
      text-align: center;
      color: rgba(255,255,255,0.5);
      font-size: 0.85rem;
    }

    @media (max-width: 900px) {
      .therapist-grid, .details-section {
        grid-template-columns: 1fr;
        gap: 40px;
      }
      .therapist-frame img {
        height: 400px;
      }
      .top-bar-right {
        display: none;
      }
    }
  </style>
</head>
<body>

  <!-- RESTORED TOP BAR -->
  <div class="top-bar">
    <div class="top-bar-left">
      <span>📍 73 Salisbury Rd, Birkdale, Auckland</span>
      <span>•</span>
      <a href="tel:0211089950">📞 021 108 9950</a>
    </div>
    <div class="top-bar-right">
      <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20enquire%20about%20a%20treatment%20at%20Mel%20%26%20Joy%20Beauty" target="_blank" rel="noopener">
        💬 Direct WhatsApp: 021 108 9950
      </a>
    </div>
  </div>

  <!-- HEADER NAVIGATION -->
  <header>
    <div class="nav-container">
      <a href="#" class="brand-logo-wrap">
        <div class="brand-badge">MJ</div>
        <div>
          <span class="brand-title">Mel & Joy</span>
          <div style="font-size: 0.68rem; letter-spacing: 0.18em; text-transform: uppercase; color: var(--rose-taupe);">Beauty • Auckland</div>
        </div>
      </a>

      <nav>
        <ul>
          <li><a href="#about">About Ana</a></li>
          <li><a href="#services">Treatments</a></li>
          <li><a href="#hours">Hours & Location</a></li>
          <li>
            <a href="https://wa.me/64211089950?text=Hello%20Ana,%20I%20would%20like%20to%20book%20a%20consultation%20with%20you%20at%20Mel%20%26%20Joy%20Beauty." 
               class="btn-wa-nav" 
               target="_blank" 
               rel="noopener">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12.031 6.172c-3.181 0-5.767 2.586-5.768 5.766-.001 1.298.38 2.27 1.019 3.287l-.711 2.598 2.666-.699c.974.53 1.815.814 2.802.814l.003-.004c3.18 0 5.767-2.586 5.768-5.766 0-3.18-2.587-5.766-5.779-5.766zm9.969 5.766c0 5.514-4.486 10-10 10-1.745 0-3.385-.453-4.821-1.246l-7.179 1.882 1.916-6.994c-.886-1.488-1.396-3.228-1.396-5.086 0-5.514 4.486-10 10-10s10 4.486 10 10z"/></svg>
              WhatsApp Booking
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- HERO SECTION -->
  <section class="hero">
    <video class="hero-video-bg" autoplay muted loop playsinline poster="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?auto=format&fit=crop&w=1600&q=80">
      <source src="https://assets.mixkit.co/videos/preview/mixkit-skin-care-treatment-at-a-spa-center-40742-large.mp4" type="video/mp4">
    </video>
    <div class="hero-overlay"></div>
    <div class="hero-content">
      <span class="hero-badge">Birkdale • North Shore Aesthetics</span>
      <h1>Beauty with Comfort & Care</h1>
      <p>Natural, beautiful results delivered by certified aesthetician Ana Garcia. Modern equipment, targeted clinical treatments, and therapeutic massage tailored to your skin.</p>
      <div class="hero-actions">
        <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20a%20complimentary%20skin%20consultation." 
           class="btn btn-primary" 
           target="_blank" 
           rel="noopener">
           <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12.031 6.172c-3.181 0-5.767 2.586-5.768 5.766-.001 1.298.38 2.27 1.019 3.287l-.711 2.598 2.666-.699c.974.53 1.815.814 2.802.814l.003-.004c3.18 0 5.767-2.586 5.768-5.766 0-3.18-2.587-5.766-5.779-5.766zm9.969 5.766c0 5.514-4.486 10-10 10-1.745 0-3.385-.453-4.821-1.246l-7.179 1.882 1.916-6.994c-.886-1.488-1.396-3.228-1.396-5.086 0-5.514 4.486-10 10-10s10 4.486 10 10z"/></svg>
           Book Consultation on WhatsApp
        </a>
        <a href="#services" class="btn btn-secondary">Explore Treatments</a>
      </div>
    </div>
  </section>

  <!-- ABOUT THE THERAPIST SECTION -->
  <section id="about" class="therapist-section">
    <div class="therapist-grid">
      <div class="therapist-image-card">
        <div class="therapist-frame">
          <!-- Portrait of Ana Garcia -->
          <img src="image_4.png" alt="Ana Garcia - Mel and Joy Beauty Therapist">
        </div>
        <div class="therapist-tag">
          <span>Owner & Beauty Specialist</span>
          <strong>Ana Garcia</strong>
        </div>
      </div>

      <div class="therapist-info">
        <span class="section-subtitle">Meet Your Skin Specialist</span>
        <h2>Personalised Skin Health in Caring Hands</h2>
        <div class="therapist-subtitle">Founder & Certified Aesthetician</div>
        
        <p>Welcome to Mel & Joy Beauty. As the founder and practitioner, Ana Garcia believes that healthy, radiant skin begins with understanding what makes your skin unique.</p>
        
        <div class="therapist-quote">
          “Self-care should feel like something you want to do, not something you have to fit in. At Mel & Joy, every detail matters.”
        </div>

        <p>Combining modern clinical technologies with comforting, personalized care, Ana works closely with you to design treatments that deliver visible results without compromising skin barrier health. Whether you are addressing acne, rejuvenating texture, or seeking restorative bodywork, you receive honest advice and undivided attention.</p>
        
        <div style="margin-top: 30px;">
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20discuss%20my%20skin%20goals%20with%20you!" 
             class="btn btn-primary" 
             target="_blank" 
             rel="noopener">
            Message Ana on WhatsApp
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES & TREATMENT MENU -->
  <section id="services" class="services-section">
    <div class="section-head">
      <span class="section-subtitle">Tailored Care & Bodywork</span>
      <h2>Our Treatment Menu</h2>
      <p>All sessions begin with a consultation to tailor formulas and modalities to your individual skin goals.</p>
    </div>

    <div style="max-width: 1140px; margin: 0 auto;">
      
      <!-- Massage & Rituals Category -->
      <h3 class="category-title">Restorative Bodywork & Rituals</h3>
      <div class="services-grid">
        
        <!-- Lymphatic Drainage -->
        <div class="service-card">
          <div>
            <span class="service-tag">Detox & Circulation</span>
            <h3>Lymphatic Drainage Massage</h3>
            <p>A gentle, specialized technique using rhythmic, light strokes designed to stimulate the flow of lymph fluid. Assists the body's natural detoxification process, eases fluid retention, soothes inflammation, and leaves you feeling refreshed and decongested.</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20a%20Lymphatic%20Drainage%20Massage" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

        <!-- Tropical Ritual (Seasonal) -->
        <div class="service-card">
          <div>
            <span class="service-tag" style="background:#FFF3E0; color:#E65100;">Seasonal Special</span>
            <h3>Tropical Ritual</h3>
            <p>An invigorating Mango & Mandarin full-body scrub that gently exfoliates dull surface skin, followed by a deeply hydrating collagen-infused massage. Nourishes the skin with rich botanicals while melting away stress.</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20the%20Seasonal%20Tropical%20Ritual" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

        <!-- Relaxing Massage -->
        <div class="service-card">
          <div>
            <span class="service-tag">Wellness & Calm</span>
            <h3>Relaxing Massage</h3>
            <p>A tranquil full-body massage utilizing soothing pressure, sweeping strokes, and therapeutic aromatics. Designed to alleviate accumulated muscular tension, promote calm, and rebalance your well-being.</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20a%20Relaxing%20Massage" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

      </div>

      <!-- Advanced Facial Treatments Category -->
      <h3 class="category-title">Advanced Skincare & Facials</h3>
      <div class="services-grid">
        
        <!-- Combined: Electroporation & Collagen Infusion -->
        <div class="service-card">
          <div>
            <span class="service-tag">Needle-Free Infusion</span>
            <h3>Electroporation & Collagen Infusion</h3>
            <p>Gentle needle-free mesotherapy that utilizes gentle micro-pulses to open cellular pathways, delivering concentrated collagen and active nutrients directly into deeper skin layers for instantaneous plumping and luminous hydration.</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20an%20Electroporation%20%26%20Collagen%20Infusion" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

        <!-- Combined: Deep Clean & Hydrojelly Treatment -->
        <div class="service-card">
          <div>
            <span class="service-tag">Pore Clarifying</span>
            <h3>Deep Clean & Hydrojelly Treatment</h3>
            <p>A thorough skin purification ritual featuring clinical pore cleansing and gentle clarification, finished with an electrolyte-rich Hydrojelly mask tailored to soothe, lock in moisture, and restore a calm glow.</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20book%20a%20Deep%20Clean%20%26%20Hydrojelly%20Treatment" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

        <!-- Salmon PDRN -->
        <div class="service-card">
          <div>
            <span class="service-tag">K-Beauty Aesthetics</span>
            <h3>Salmon PDRN Rejuvenation</h3>
            <p>An innovative Korean skin restorative therapy harnessing salmon DNA-derived polynucleotides to encourage cellular skin repair, enhance elasticity, and promote radiant "glass skin."</p>
          </div>
          <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I'd%20like%20to%20enquire%20about%20Salmon%20PDRN%20Skin%20Rejuvenation" class="btn-card-wa" target="_blank" rel="noopener">
            Book via WhatsApp →
          </a>
        </div>

      </div>

      <!-- DIRECT WHATSAPP BANNER -->
      <div class="wa-cta-banner">
        <div class="wa-cta-text">
          <h3>Ready for Your Appointment?</h3>
          <p>Ana handles all consultations directly on WhatsApp for prompt scheduling and personal guidance.</p>
        </div>
        <a href="https://wa.me/64211089950?text=Hi%20Ana,%20I%20would%20like%20to%20book%20an%20appointment%20at%20Mel%20%26%20Joy%20Beauty." 
           class="btn btn-primary" 
           target="_blank" 
           rel="noopener"
           style="font-size: 1.05rem; padding: 15px 34px;">
           Message on WhatsApp (021 108 9950)
        </a>
      </div>

    </div>
  </section>

  <!-- HOURS & LOCATION -->
  <section id="hours" class="details-section">
    
    <!-- Hours Table -->
    <div class="info-card">
      <div class="status-badge" id="openStatus">Open for Appointments</div>
      <h3>Studio Hours</h3>
      <table class="hours-table">
        <tr><td>Monday</td><td>9:00 am – 7:30 pm</td></tr>
        <tr><td>Tuesday</td><td style="color:#888;">Closed</td></tr>
        <tr><td>Wednesday</td><td>9:00 am – 7:30 pm</td></tr>
        <tr><td>Thursday</td><td>9:00 am – 6:30 pm</td></tr>
        <tr><td>Friday</td><td>9:00 am – 6:30 pm</td></tr>
        <tr><td>Saturday</td><td>7:00 am – 4:00 pm</td></tr>
        <tr><td>Sunday</td><td style="color:#888;">Closed</td></tr>
      </table>
      <p style="font-size: 0.85rem; color: #888; margin-top: 18px;">*Bookings are by appointment only. Early morning & evening slots available upon request.</p>
    </div>

    <!-- Location & Directions -->
    <div class="info-card">
      <span class="section-subtitle">Visit The Studio</span>
      <h3>Location & Parking</h3>
      <p style="margin-bottom: 16px;"><strong>Mel & Joy Beauty</strong><br>73 Salisbury Road, Birkdale, Auckland 0626</p>
      <p style="color: #666; margin-bottom: 24px;">Located in a tranquil Birkdale setting with private client access and convenient on-street parking.</p>
      
      <div style="display: flex; gap: 14px; flex-wrap: wrap;">
        <a href="https://maps.google.com/?q=73+Salisbury+Road,+Birkdale,+Auckland+0626" 
           target="_blank" 
           rel="noopener" 
           class="btn btn-secondary" 
           style="background: var(--blush-surface); color: var(--deep-wine); border-color: var(--rose-taupe);">
          📍 Get Directions on Google Maps
        </a>
        <a href="tel:0211089950" class="btn btn-secondary" style="background: var(--blush-surface); color: var(--deep-wine); border-color: var(--rose-taupe);">
          📞 Call 021 108 9950
        </a>
      </div>
    </div>

  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-container">
      <div class="footer-col">
        <h4 style="font-family: 'Cormorant Garamond', serif; font-size: 1.6rem; color: #fff;">Mel & Joy Beauty</h4>
        <p>Auckland certified aesthetician specializing in clinical skin health, needle-free infusions, and restorative massage therapy.</p>
      </div>

      <div class="footer-col">
        <h4>Direct Contact</h4>
        <a href="https://wa.me/64211089950" target="_blank" rel="noopener">WhatsApp: 021 108 9950</a>
        <a href="tel:0211089950">Phone: 021 108 9950</a>
        <p>73 Salisbury Rd, Birkdale, Auckland</p>
      </div>

      <div class="footer-col">
        <h4>Social Media</h4>
        <a href="https://instagram.com/mel.joybeauty" target="_blank" rel="noopener">Instagram: @mel.joybeauty</a>
        <a href="https://facebook.com/MelJoyBeauty" target="_blank" rel="noopener">Facebook: Mel & Joy Beauty</a>
      </div>
    </div>

    <div class="footer-bottom">
      &copy; 2026 Mel & Joy Beauty. All rights reserved. Created with care for Ana Garcia.
    </div>
  </footer>

  <script>
    // Live business status detection for Auckland (NZST/NZDT)
    function checkHours() {
      const now = new Date();
      const nzTime = new Date(now.toLocaleString("en-US", { timeZone: "Pacific/Auckland" }));
      const day = nzTime.getDay(); // 0 is Sun, 1 is Mon, etc.
      const hour = nzTime.getHours() + nzTime.getMinutes() / 60;
      
      const badge = document.getElementById("openStatus");
      let isOpen = false;

      if (day === 1 && hour >= 9 && hour < 19.5) isOpen = true; // Mon
      else if (day === 3 && hour >= 9 && hour < 19.5) isOpen = true; // Wed
      else if (day === 4 && hour >= 9 && hour < 18.5) isOpen = true; // Thu
      else if (day === 5 && hour >= 9 && hour < 18.5) isOpen = true; // Fri
      else if (day === 6 && hour >= 7 && hour < 16) isOpen = true; // Sat

      if (isOpen) {
        badge.textContent = "● Studio Open Today";
        badge.style.background = "#E8F5E9";
        badge.style.color = "#2E7D32";
      } else {
        badge.textContent = "○ Currently Closed • Booking on WhatsApp";
        badge.style.background = "#FBE9E7";
        badge.style.color = "#D84315";
      }
    }
    checkHours();
  </script>
</body>
</html>
