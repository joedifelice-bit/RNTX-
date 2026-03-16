[index (3).html](https://github.com/user-attachments/files/26037878/index.3.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>RNTX Travel Inc. — Corporate Accommodation Specialists · Toronto</title>
  <meta name="description" content="RNTX Travel Inc. are corporate accommodation specialists offering exclusive rates at furnished residences, boutique hotels, and luxury hotels across Ontario. Request a custom quote today."/>
  <meta property="og:title" content="RNTX Travel Inc. — Corporate Accommodation Specialists"/>
  <meta property="og:description" content="Exclusive rates at Ontario's finest furnished residences, boutique hotels, and luxury properties. Corporate-ready. Concierge-managed."/>
  <meta property="og:type" content="website"/>
  <link rel="preconnect" href="https://fonts.googleapis.com"/>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500&family=Jost:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --ivory:    #F7F3EC;
      --ivory2:   #EDE8DF;
      --ivory3:   #E2DAD0;
      --charcoal: #0F2040;
      --charcoal2:#162E55;
      --gold:     #A8822E;
      --gold-l:   #C9A84C;
      --gold-pale:#F0E6CE;
      --slate:    #6B7280;
      --white:    #FDFAF5;
      --ff-disp:  'Cormorant Garamond', Georgia, serif;
      --ff-sans:  'Jost', sans-serif;
      --ff-mono:  'DM Mono', monospace;
    }
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; -webkit-font-smoothing: antialiased; }
    body { font-family: var(--ff-sans); background: var(--ivory); color: var(--charcoal); overflow-x: hidden; }
    button, input, textarea, select { font-family: var(--ff-sans); }
    a { text-decoration: none; color: inherit; }

    /* ── NAV ── */
    .nav {
      position: sticky; top: 0; z-index: 200;
      background: var(--white); border-bottom: 1px solid var(--ivory3);
      display: flex; align-items: center; justify-content: space-between;
      padding: 0 60px; height: 68px;
    }
    .nav-brand {
      font-family: var(--ff-disp); font-size: 22px; font-weight: 500;
      letter-spacing: 2px; color: var(--charcoal); cursor: pointer;
    }
    .nav-brand span { color: var(--gold); }
    .nav-links { display: flex; gap: 36px; align-items: center; }
    .nav-link {
      font-size: 11px; font-weight: 500; letter-spacing: 2px; text-transform: uppercase;
      color: var(--slate); cursor: pointer; background: none; border: none;
      transition: color .2s; padding: 4px 0; position: relative;
    }
    .nav-link::after {
      content: ''; position: absolute; bottom: 0; left: 0; right: 0;
      height: 1px; background: var(--gold); transform: scaleX(0); transition: transform .2s;
    }
    .nav-link:hover, .nav-link.active { color: var(--charcoal); }
    .nav-link:hover::after, .nav-link.active::after { transform: scaleX(1); }
    .nav-cta {
      font-size: 11px; font-weight: 600; letter-spacing: 2px; text-transform: uppercase;
      background: var(--charcoal); color: var(--white); border: none;
      padding: 11px 28px; cursor: pointer; transition: background .2s;
    }
    .nav-cta:hover { background: var(--gold); }
    .nav-hamburger { display: none; background: none; border: none; cursor: pointer; padding: 4px; }

    /* ── HERO ── */
    .hero {
      background: var(--charcoal); min-height: 92vh;
      display: grid; grid-template-columns: 1fr 1fr;
      position: relative; overflow: hidden;
    }
    .hero-left {
      padding: 100px 60px 80px;
      display: flex; flex-direction: column; justify-content: center;
      position: relative; z-index: 2;
    }
    .hero-overline {
      font-family: var(--ff-mono); font-size: 10px; letter-spacing: 3px;
      text-transform: uppercase; color: var(--gold);
      margin-bottom: 24px; display: flex; align-items: center; gap: 12px;
    }
    .hero-overline::before { content: ''; display: block; width: 28px; height: 1px; background: var(--gold); }
    .hero-h1 {
      font-family: var(--ff-disp); font-size: clamp(46px, 5.5vw, 76px);
      font-weight: 300; line-height: 1.08; color: var(--white);
      letter-spacing: -.5px; margin-bottom: 22px;
    }
    .hero-h1 em { font-style: italic; color: var(--gold-l); }
    .hero-sub {
      font-size: 15px; color: rgba(255,255,255,.5); line-height: 1.8;
      max-width: 400px; margin-bottom: 48px; font-weight: 300;
    }
    .hero-pills { display: flex; gap: 10px; flex-wrap: wrap; }
    .pill {
      display: inline-flex; align-items: center; gap: 6px; padding: 6px 14px;
      border: 1px solid rgba(168,130,46,.3); color: rgba(255,255,255,.55);
      font-size: 10px; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase;
    }
    .pill-dot { width: 4px; height: 4px; border-radius: 50%; background: var(--gold); flex-shrink: 0; }

    /* ── QUOTE FORM ── */
    .hero-right {
      background: var(--white); padding: 52px 56px;
      display: flex; flex-direction: column; justify-content: center;
      overflow-y: auto;
    }
    .form-title {
      font-family: var(--ff-disp); font-size: 32px; font-weight: 500;
      color: var(--charcoal); margin-bottom: 6px;
    }
    .form-sub { font-size: 13px; color: var(--slate); margin-bottom: 22px; line-height: 1.6; }
    .form-section-lbl {
      font-family: var(--ff-mono); font-size: 9px; letter-spacing: 2.5px;
      text-transform: uppercase; color: var(--gold); margin-bottom: 14px;
      display: flex; align-items: center; gap: 10px;
    }
    .form-section-lbl::before { content: ''; display: block; width: 16px; height: 1px; background: var(--gold); }
    .form-divider { height: 1px; background: var(--ivory3); margin: 16px 0; }
    .field { margin-bottom: 13px; }
    .fl {
      display: block; font-family: var(--ff-mono); font-size: 9px; font-weight: 500;
      letter-spacing: 2.5px; text-transform: uppercase; color: var(--slate); margin-bottom: 7px;
    }
    .fi {
      width: 100%; padding: 11px 13px; background: var(--ivory);
      border: 1px solid var(--ivory3); font-size: 13px; color: var(--charcoal);
      outline: none; transition: border-color .2s; appearance: none;
    }
    .fi:focus { border-color: var(--gold); background: var(--white); }
    .fi::placeholder { color: #aaa; }
    select.fi {
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8' viewBox='0 0 12 8'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%236B7280' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: no-repeat; background-position: right 12px center;
      padding-right: 32px; cursor: pointer;
    }
    .field-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
    .form-btn {
      width: 100%; padding: 14px; background: var(--charcoal); color: var(--white);
      border: none; font-size: 11px; font-weight: 600; letter-spacing: 2px;
      text-transform: uppercase; cursor: pointer; transition: background .2s; margin-top: 6px;
    }
    .form-btn:hover { background: var(--gold); }
    .form-note { font-size: 11px; color: var(--slate); margin-top: 10px; text-align: center; line-height: 1.6; }
    .success-state { text-align: center; padding: 48px 32px; }
    .success-icon {
      width: 52px; height: 52px; border: 1px solid var(--gold); border-radius: 50%;
      margin: 0 auto 20px; display: flex; align-items: center; justify-content: center;
    }
    .success-h { font-family: var(--ff-disp); font-size: 26px; font-weight: 500; color: var(--charcoal); margin-bottom: 8px; }
    .success-p { font-size: 13px; color: var(--slate); line-height: 1.65; }

    /* ── SECTIONS ── */
    .sec { padding: 100px 60px; }
    .sec-lbl {
      font-family: var(--ff-mono); font-size: 10px; font-weight: 500;
      letter-spacing: 3px; text-transform: uppercase; color: var(--gold);
      margin-bottom: 16px; display: flex; align-items: center; gap: 12px;
    }
    .sec-lbl::before { content: ''; display: block; width: 24px; height: 1px; background: var(--gold); }
    .sec-h {
      font-family: var(--ff-disp); font-size: clamp(32px, 4vw, 52px);
      font-weight: 400; line-height: 1.1; letter-spacing: -.3px;
    }
    .sec-h.dark { color: var(--charcoal); }
    .sec-h.light { color: var(--white); }
    .sec-p { font-size: 15px; line-height: 1.8; color: var(--slate); font-weight: 300; max-width: 520px; margin-top: 16px; }

    /* ── SERVICES ── */
    .svc-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2px; margin-top: 52px; }
    .svc-card {
      background: var(--white); padding: 44px 36px;
      position: relative; overflow: hidden; transition: background .25s;
    }
    .svc-card:hover { background: var(--charcoal); }
    .svc-card:hover .svc-title, .svc-card:hover .svc-num { color: var(--white); }
    .svc-card:hover .svc-body { color: rgba(255,255,255,.55); }
    .svc-card:hover .svc-icon-wrap { border-color: rgba(168,130,46,.3); }
    .svc-card:hover .svc-tag { color: var(--gold-l); border-color: rgba(168,130,46,.3); }
    .svc-card::before {
      content: ''; position: absolute; bottom: 0; left: 0; right: 0;
      height: 2px; background: var(--gold); transform: scaleX(0);
      transform-origin: left; transition: transform .35s;
    }
    .svc-card:hover::before { transform: scaleX(1); }
    .svc-num { font-family: var(--ff-mono); font-size: 11px; color: var(--gold); letter-spacing: 2px; margin-bottom: 28px; transition: color .25s; }
    .svc-icon-wrap {
      width: 48px; height: 48px; border: 1px solid var(--ivory3);
      display: flex; align-items: center; justify-content: center;
      margin-bottom: 22px; transition: border-color .25s;
    }
    .svc-title { font-family: var(--ff-disp); font-size: 26px; font-weight: 500; color: var(--charcoal); margin-bottom: 14px; line-height: 1.2; transition: color .25s; }
    .svc-body { font-size: 13px; color: var(--slate); line-height: 1.75; transition: color .25s; }
    .svc-tag {
      display: inline-block; margin-top: 22px; font-family: var(--ff-mono); font-size: 9px;
      letter-spacing: 1.5px; text-transform: uppercase; color: var(--gold);
      border: 1px solid var(--gold-pale); padding: 5px 12px; transition: color .25s, border-color .25s;
    }

    /* ── WHY US ── */
    .why-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: center; }
    .why-item { display: flex; gap: 20px; padding: 20px 0; border-bottom: 1px solid rgba(255,255,255,.07); }
    .why-item-n { font-family: var(--ff-mono); font-size: 11px; color: rgba(168,130,46,.6); flex-shrink: 0; margin-top: 2px; }
    .why-item-title { font-family: var(--ff-disp); font-size: 18px; font-weight: 500; color: var(--white); margin-bottom: 6px; }
    .why-item-desc { font-size: 13px; color: rgba(255,255,255,.45); line-height: 1.7; font-weight: 300; }
    .why-visual { background: var(--ivory); padding: 48px; }
    .stat-block { text-align: center; padding: 28px 0; border-bottom: 1px solid var(--ivory3); }
    .stat-block:last-child { border-bottom: none; }
    .stat-num { font-family: var(--ff-disp); font-size: 52px; font-weight: 300; color: var(--charcoal); line-height: 1; }
    .stat-lbl { font-family: var(--ff-mono); font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(--slate); margin-top: 8px; }

    /* ── BRANDS ── */
    .brands-intro { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: end; margin-bottom: 52px; }
    .brands-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 2px; }
    .brand-card { background: var(--white); padding: 32px 28px; border-bottom: 2px solid transparent; transition: all .25s; }
    .brand-card:hover { border-bottom-color: var(--gold); background: var(--ivory); }
    .brand-cat { font-family: var(--ff-mono); font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(--gold); margin-bottom: 10px; }
    .brand-name { font-family: var(--ff-disp); font-size: 20px; font-weight: 500; color: var(--charcoal); line-height: 1.2; margin-bottom: 6px; }
    .brand-note { font-size: 11px; color: var(--slate); line-height: 1.55; }

    /* ── CTA BAND ── */
    .cta-band { background: var(--gold); padding: 72px 60px; display: flex; align-items: center; justify-content: space-between; gap: 40px; }
    .cta-band-h { font-family: var(--ff-disp); font-size: 40px; font-weight: 400; color: var(--charcoal); line-height: 1.15; max-width: 560px; }
    .cta-band-h em { font-style: italic; }
    .cta-band-btn {
      flex-shrink: 0; padding: 16px 44px; background: var(--charcoal); color: var(--white);
      border: none; font-size: 11px; font-weight: 600; letter-spacing: 2px;
      text-transform: uppercase; cursor: pointer; white-space: nowrap;
    }
    .cta-band-btn:hover { background: #000; }

    /* ── PARTNER PAGE ── */
    .partner-hero {
      background: var(--charcoal); padding: 100px 60px 80px;
      display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: start;
    }
    .partner-steps { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; margin-top: 36px; }
    .partner-step { padding: 24px 20px; background: rgba(255,255,255,.04); border: 1px solid rgba(255,255,255,.06); }
    .step-n { font-family: var(--ff-mono); font-size: 10px; color: var(--gold); margin-bottom: 8px; }
    .step-title { font-family: var(--ff-disp); font-size: 18px; font-weight: 500; color: var(--white); margin-bottom: 5px; }
    .step-desc { font-size: 12px; color: rgba(255,255,255,.4); line-height: 1.6; }
    .partner-form-wrap { background: var(--white); padding: 52px 48px; }

    /* ── ABOUT ── */
    .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: start; }
    .av-item { display: grid; grid-template-columns: 110px 1fr; gap: 20px; padding: 18px 0; border-bottom: 1px solid var(--ivory3); }
    .av-lbl { font-family: var(--ff-mono); font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(--slate); margin-top: 3px; }

    /* ── FOOTER ── */
    .footer { background: var(--charcoal2); padding: 56px 60px 32px; }
    .footer-top { display: grid; grid-template-columns: 2fr 1fr 1fr 1fr; gap: 48px; margin-bottom: 48px; }
    .footer-brand { font-family: var(--ff-disp); font-size: 22px; font-weight: 500; letter-spacing: 2px; color: var(--white); margin-bottom: 12px; }
    .footer-brand span { color: var(--gold); }
    .footer-desc { font-size: 12px; color: rgba(255,255,255,.35); line-height: 1.75; font-weight: 300; }
    .footer-col-title { font-family: var(--ff-mono); font-size: 9px; letter-spacing: 2.5px; text-transform: uppercase; color: var(--gold); margin-bottom: 16px; }
    .footer-lnk { font-size: 12px; color: rgba(255,255,255,.4); margin-bottom: 9px; cursor: pointer; transition: color .2s; display: block; }
    .footer-lnk:hover { color: var(--white); }
    .footer-bottom { border-top: 1px solid rgba(255,255,255,.06); padding-top: 22px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 12px; }
    .footer-copy { font-size: 11px; color: rgba(255,255,255,.2); }
    .footer-badges { display: flex; gap: 8px; }
    .fbadge { padding: 4px 12px; border: 1px solid rgba(255,255,255,.08); font-family: var(--ff-mono); font-size: 9px; color: rgba(255,255,255,.25); letter-spacing: 1px; }
    .back-btn { background: none; border: 1px solid rgba(255,255,255,.15); color: rgba(255,255,255,.5); font-size: 11px; letter-spacing: 2px; text-transform: uppercase; padding: 8px 20px; cursor: pointer; font-family: var(--ff-sans); }
    .back-btn:hover { border-color: var(--gold); color: var(--gold); }
    .city-card:hover { background: rgba(255,255,255,.08) !important; }

    /* ── UTILS ── */
    .ivory-bg { background: var(--ivory); }
    .white-bg  { background: var(--white); }
    .charcoal-bg { background: var(--charcoal); }

    /* ── MOBILE ── */
    @media (max-width: 900px) {
      .nav { padding: 0 24px; }
      .nav-links { display: none; }
      .nav-hamburger { display: block; }
      .nav-cta { display: none; }
      .hero { grid-template-columns: 1fr; min-height: auto; }
      .hero-left { padding: 80px 24px 56px; }
      .hero-right { padding: 48px 24px 64px; }
      .sec { padding: 72px 24px; }
      .svc-grid, .brands-grid { grid-template-columns: 1fr; }
      .why-grid, .brands-intro, .about-grid, .partner-hero { grid-template-columns: 1fr; gap: 40px; }
      .partner-steps { grid-template-columns: 1fr; }
      .partner-form-wrap { padding: 36px 24px; }
      .field-row { grid-template-columns: 1fr; }
      .cta-band { flex-direction: column; align-items: flex-start; padding: 56px 24px; }
      .footer-top { grid-template-columns: 1fr 1fr; }
      .footer { padding: 48px 24px 28px; }
      .why-visual { padding: 32px 24px; }
    }
    @media (max-width: 600px) {
      .footer-top { grid-template-columns: 1fr; }
      .brands-grid { grid-template-columns: 1fr 1fr; }
      .hero-h1 { font-size: 42px; }
    }
  </style>
</head>
<body>

<!-- NAV -->
<nav class="nav" id="main-nav">
  <div class="nav-brand" onclick="showPage('home')">RNTX<span>.</span></div>
  <div class="nav-links">
    <button class="nav-link active" onclick="showPage('home')" id="nav-home">Our Services</button>
    <button class="nav-link" onclick="showPage('partner')" id="nav-partner">Partnership</button>
    <button class="nav-link" onclick="showPage('about')" id="nav-about">About Us</button>
  </div>
  <button class="nav-cta" onclick="showPage('home'); setTimeout(()=>document.getElementById('quote-form').scrollIntoView({behavior:'smooth'}),100)">Get a Quote</button>
  <button class="nav-hamburger" onclick="toggleMobileMenu()" aria-label="Menu">
    <svg width="22" height="22" viewBox="0 0 22 22" fill="none" stroke="#0F2040" stroke-width="1.5" stroke-linecap="round">
      <line x1="3" y1="6" x2="19" y2="6"/><line x1="3" y1="11" x2="19" y2="11"/><line x1="3" y1="16" x2="19" y2="16"/>
    </svg>
  </button>
</nav>

<!-- MOBILE MENU -->
<div id="mobile-menu" style="display:none;position:fixed;top:68px;left:0;right:0;background:var(--white);border-bottom:1px solid var(--ivory3);z-index:199;padding:20px 24px 28px;display:none;flex-direction:column;gap:4px;">
  <button class="nav-link" style="text-align:left;padding:12px 0" onclick="showPage('home');closeMobileMenu()">Our Services</button>
  <button class="nav-link" style="text-align:left;padding:12px 0" onclick="showPage('partner');closeMobileMenu()">Partnership</button>
  <button class="nav-link" style="text-align:left;padding:12px 0" onclick="showPage('about');closeMobileMenu()">About Us</button>
  <button class="nav-cta" style="margin-top:12px;width:100%" onclick="showPage('home');closeMobileMenu()">Get a Quote</button>
</div>

<!-- ════════════════════════════════
     HOME PAGE
════════════════════════════════ -->
<div id="page-home">

  <!-- HERO -->
  <section class="hero">
    <div class="hero-left">
      <div class="hero-overline">Corporate Accommodation Specialists</div>
      <h1 class="hero-h1">Premium Stays for<br><em>Modern Business<br>Travel</em></h1>
      <p class="hero-sub">We source and secure exclusive rates at Toronto's finest furnished residences, boutique hotels, and luxury properties — so your team travels with confidence every time.</p>
      <div class="hero-pills">
        <div class="pill"><div class="pill-dot"></div>Exclusive Corporate Rates</div>
        <div class="pill"><div class="pill-dot"></div>Certified Partners Only</div>
        <div class="pill"><div class="pill-dot"></div>Consistent Quality Standards</div>
        <div class="pill"><div class="pill-dot"></div>Concierge Service</div>
      </div>
    </div>
    <div class="hero-right" id="quote-form">
      <div id="quote-content">
        <div class="form-title">Request a Custom Quote</div>
        <p class="form-sub">Tell us about your travel requirements and we'll arrange exclusive rates with our certified partners.</p>

        <div class="form-section-lbl">Contact Details</div>
        <div class="field-row">
          <div class="field"><label class="fl">First Name</label><input class="fi" type="text" placeholder="First name"/></div>
          <div class="field"><label class="fl">Last Name</label><input class="fi" type="text" placeholder="Last name"/></div>
        </div>
        <div class="field"><label class="fl">Company</label><input class="fi" type="text" placeholder="Your company name"/></div>
        <div class="field-row">
          <div class="field"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@company.com"/></div>
          <div class="field"><label class="fl">Phone</label><input class="fi" type="tel" placeholder="+1 (000) 000-0000"/></div>
        </div>

        <div class="form-divider"></div>
        <div class="form-section-lbl">Stay Details</div>

        <div class="field">
          <label class="fl">Accommodation Type</label>
          <select class="fi">
            <option value="">Select type...</option>
            <option>Furnished Residence</option>
            <option>Boutique Hotel</option>
            <option>Luxury Hotel</option>
            <option>Not sure — advise me</option>
          </select>
        </div>
        <div class="field-row">
          <div class="field"><label class="fl">Check-In Date</label><input class="fi" type="date"/></div>
          <div class="field"><label class="fl">Check-Out Date</label><input class="fi" type="date"/></div>
        </div>
        <div class="field-row">
          <div class="field">
            <label class="fl">Number of Guests</label>
            <select class="fi">
              <option value="">Select...</option>
              <option>1</option><option>2</option><option>3</option><option>4</option>
              <option>5</option><option>6</option><option>7</option><option>8</option>
              <option>9</option><option>10+</option>
            </select>
          </div>
          <div class="field">
            <label class="fl">Number of Bedrooms</label>
            <select class="fi">
              <option value="">Select...</option>
              <option>Studio</option>
              <option>1 Bedroom</option>
              <option>2 Bedrooms</option>
              <option>3 Bedrooms</option>
              <option>4+ Bedrooms</option>
              <option>Not applicable — hotel room</option>
            </select>
          </div>
        </div>
        <div class="field-row">
          <div class="field"><label class="fl">Destination City</label>
            <select class="fi">
              <option value="">Select city...</option>
              <option>Toronto</option>
              <option>Ottawa</option>
              <option>Kitchener-Waterloo</option>
              <option>Windsor</option>
              <option>Niagara Falls</option>
              <option>London</option>
              <option>Other — please specify in notes</option>
            </select>
          </div>
          <div class="field"><label class="fl">Preferred Neighbourhood</label><input class="fi" type="text" placeholder="e.g. Yorkville, King West"/></div>
        </div>

        <div class="form-divider"></div>
        <div class="form-section-lbl">Preferences &amp; Requirements</div>
        <div class="field">
          <label class="fl">Additional Requirements</label>
          <textarea class="fi" rows="4" style="resize:none" placeholder="Preferred hotels, amenities, pets, parking, budget range..."></textarea>
        </div>

        <button class="form-btn" onclick="submitQuote()">Submit Request</button>
        <p class="form-note">We respond within 4 business hours &nbsp;·&nbsp; No commitment required</p>
      </div>
    </div>
  </section>

  <!-- SERVICES -->
  <section class="sec ivory-bg">
    <div class="sec-lbl">What We Offer</div>
    <h2 class="sec-h dark">Three Categories.<br>One Standard of Excellence.</h2>
    <p class="sec-p">Every property we recommend is personally vetted against our quality criteria. We only work with certified partners who meet our operational, service, and compliance standards.</p>
    <div class="svc-grid">
      <div class="svc-card">
        <div class="svc-num">01</div>
        <div class="svc-icon-wrap">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"><path d="M6 2h12v20H6z"/><path d="M12 6v.01M12 10v.01M12 14v.01M9 6h.01M9 10h.01M9 14h.01M15 6h.01M15 10h.01M15 14h.01"/></svg>
        </div>
        <div class="svc-title">Furnished Residences</div>
        <div class="svc-body">Fully furnished, professionally managed residences with full kitchen access, in-suite laundry, dedicated workspace, and hotel-grade housekeeping. Designed for executives and consultants who need a real home base.</div>
        <div class="svc-tag">Extended Stay · 7–90+ Nights</div>
      </div>
      <div class="svc-card">
        <div class="svc-num">02</div>
        <div class="svc-icon-wrap">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"><path d="M3 22V7l9-5 9 5v15M5 22v-7h14v7M9 22v-4h6v4"/></svg>
        </div>
        <div class="svc-title">Boutique Hotels</div>
        <div class="svc-body">Independently operated luxury boutiques selected for exceptional service, distinctive design, and long-stay suitability. Every property is verified for consistency, corporate invoicing capability, and extended-stay amenities.</div>
        <div class="svc-tag">Premium Boutique · Curated Selection</div>
      </div>
      <div class="svc-card">
        <div class="svc-num">03</div>
        <div class="svc-icon-wrap">
          <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
        </div>
        <div class="svc-title">Luxury Hotels</div>
        <div class="svc-body">Access preferred corporate rates at Toronto's premier five-star properties — negotiated exclusively for our clients. Consistent standards, executive floor access, and direct billing arrangements for frictionless expense management.</div>
        <div class="svc-tag">5-Star Hotels · Exclusive Rates</div>
      </div>
    </div>
  </section>

  <!-- WHY US -->
  <section class="sec charcoal-bg">
    <div class="why-grid">
      <div>
        <div class="sec-lbl">Why Choose Us</div>
        <h2 class="sec-h light">Exclusive Rates.<br>Uncompromised Quality.</h2>
        <div style="margin-top:36px">
          <div class="why-item">
            <div class="why-item-n">01</div>
            <div><div class="why-item-title">Negotiated Exclusive Rates</div><div class="why-item-desc">We maintain direct commercial relationships with our certified partner properties, securing preferential corporate rates unavailable on public booking platforms.</div></div>
          </div>
          <div class="why-item">
            <div class="why-item-n">02</div>
            <div><div class="why-item-title">Certified Partner Network</div><div class="why-item-desc">Every property in our portfolio has passed our onboarding verification — covering management structure, service standards, amenity accuracy, and compliance capability.</div></div>
          </div>
          <div class="why-item">
            <div class="why-item-n">03</div>
            <div><div class="why-item-title">Single Point of Contact</div><div class="why-item-desc">One dedicated concierge manages your booking from inquiry to check-out. No call centres, no automated systems — a real person who knows your account.</div></div>
          </div>
          <div class="why-item">
            <div class="why-item-n">04</div>
            <div><div class="why-item-title">Corporate-Ready Documentation</div><div class="why-item-desc">GST/HST invoicing, consolidated billing, expense-ready receipts, and reporting for finance teams — built into every booking we manage.</div></div>
          </div>
        </div>
      </div>
      <div class="why-visual">
        <div class="stat-block"><div class="stat-num">100%</div><div class="stat-lbl">Professionally Managed Properties</div></div>
        <div class="stat-block"><div class="stat-num">24 hrs</div><div class="stat-lbl">Response SLA on All Requests</div></div>
        <div class="stat-block"><div class="stat-num">$0</div><div class="stat-lbl">Platform or Membership Fees</div></div>
        <div class="stat-block"><div class="stat-num">5+</div><div class="stat-lbl">Years Managing Corporate Stays</div></div>
      </div>
    </div>
  </section>

  <!-- BRANDS -->
  <section class="sec white-bg">
    <div class="brands-intro">
      <div>
        <div class="sec-lbl">Our Toronto Partners</div>
        <h2 class="sec-h dark">Where We Place<br>Our Clients</h2>
      </div>
      <p style="font-size:15px;color:var(--slate);line-height:1.8;font-weight:300;margin-top:8px">We have established preferred-rate relationships with Toronto's most respected properties across all three accommodation categories. Our clients receive access that is simply not available through standard OTAs or direct booking.</p>
    </div>
    <div class="brands-grid">
      <div class="brand-card"><div class="brand-cat">Luxury Hotel</div><div class="brand-name">Four Seasons Toronto</div><div class="brand-note">Yorkville · 5-Star · Executive Suites</div></div>
      <div class="brand-card"><div class="brand-cat">Luxury Hotel</div><div class="brand-name">Shangri-La Toronto</div><div class="brand-note">Bay St · 5-Star · Extended Stay Suites</div></div>
      <div class="brand-card"><div class="brand-cat">Luxury Hotel</div><div class="brand-name">The St. Regis Toronto</div><div class="brand-note">King West · 5-Star · Butler Service</div></div>
      <div class="brand-card"><div class="brand-cat">Luxury Hotel</div><div class="brand-name">Fairmont Royal York</div><div class="brand-note">Front St · Historic · Corporate Floors</div></div>
      <div class="brand-card"><div class="brand-cat">Luxury Hotel</div><div class="brand-name">Hyatt Regency Toronto</div><div class="brand-note">King West · 5-Star · Event &amp; Stay</div></div>
      <div class="brand-card"><div class="brand-cat">Boutique Hotel</div><div class="brand-name">The Hazelton Hotel</div><div class="brand-note">Yorkville · Boutique Luxury · Spa</div></div>
      <div class="brand-card"><div class="brand-cat">Boutique Hotel</div><div class="brand-name">Hôtel Le Germain</div><div class="brand-note">Mercer St · Boutique · Design Hotel</div></div>
      <div class="brand-card"><div class="brand-cat">Furnished Residence</div><div class="brand-name">StayRentX</div><div class="brand-note">King West · Full-Service · Extended Stay</div></div>
    </div>
  </section>

  <!-- CITIES -->
  <section class="sec charcoal-bg">
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:start">
      <div>
        <div class="sec-lbl">Where We Operate</div>
        <h2 class="sec-h light">Serving Business Travellers<br><em style="font-style:italic;color:var(--gold-l)">Across Ontario</em></h2>
        <p style="font-size:15px;color:rgba(255,255,255,.5);line-height:1.8;margin-top:18px;font-weight:300;max-width:420px">We place corporate clients in premium accommodations across Ontario's major business and government centres. Whether your team is based in Toronto or relocating to any of our serviced cities, we have certified partner properties ready.</p>
        <div style="margin-top:32px;display:inline-flex;align-items:center;gap:12px;padding:14px 22px;border:1px solid rgba(168,130,46,.25);background:rgba(168,130,46,.06)">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
          <span style="font-family:var(--ff-mono);font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Ontario-Wide Coverage</span>
        </div>
      </div>
      <div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:2px">
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Anchor Market</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">Toronto</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Finance · Consulting · Technology · Film Production</div>
          </div>
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Government Hub</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">Ottawa</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Federal Government · Contractors · Embassy Travel</div>
          </div>
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Tech Corridor</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">Kitchener–Waterloo</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Technology · Start-Ups · Google · Shopify Ecosystem</div>
          </div>
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">US Corridor</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">Windsor</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Automotive · Cross-Border Engineering · University</div>
          </div>
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Hospitality</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">Niagara Falls</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Tourism · Hospitality · Cross-Border Meetings</div>
          </div>
          <div class="city-card" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);padding:28px 26px;transition:background .2s;cursor:default">
            <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px">
              <div style="width:5px;height:5px;border-radius:50%;background:var(--gold);flex-shrink:0"></div>
              <span style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold)">Western Ontario</span>
            </div>
            <div style="font-family:var(--ff-disp);font-size:24px;font-weight:500;color:var(--white);margin-bottom:4px">London</div>
            <div style="font-size:11px;color:rgba(255,255,255,.35);line-height:1.55">Healthcare · Education · Legal · Insurance Sector</div>
          </div>
        </div>
        <div style="margin-top:2px;padding:16px 22px;background:rgba(168,130,46,.06);border:1px solid rgba(168,130,46,.14);display:flex;align-items:center;justify-content:space-between;gap:20px">
          <span style="font-size:13px;color:rgba(255,255,255,.45);font-weight:300">Need accommodation in a city not listed? We can often assist.</span>
          <button onclick="document.getElementById('quote-form').scrollIntoView({behavior:'smooth'})" style="flex-shrink:0;background:none;border:1px solid rgba(168,130,46,.35);color:var(--gold);font-family:var(--ff-sans);font-size:10px;font-weight:600;letter-spacing:2px;text-transform:uppercase;padding:9px 18px;cursor:pointer;white-space:nowrap;transition:all .2s" onmouseover="this.style.background='rgba(168,130,46,.12)'" onmouseout="this.style.background='none'">Ask Us →</button>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <div class="cta-band">
    <h2 class="cta-band-h">Ready to elevate your<br><em>corporate accommodation programme?</em></h2>
    <button class="cta-band-btn" onclick="document.getElementById('quote-form').scrollIntoView({behavior:'smooth'})">Request a Quote →</button>
  </div>

  <!-- FOOTER -->
  <footer class="footer">
    <div class="footer-top">
      <div>
        <div class="footer-brand">RNTX<span>.</span></div>
        <p class="footer-desc">Corporate accommodation specialists offering exclusive access to furnished residences, boutique hotels, and luxury hotels across Ontario. Toronto-based. Corporate-ready.</p>
      </div>
      <div>
        <div class="footer-col-title">Services</div>
        <span class="footer-lnk">Furnished Residences</span>
        <span class="footer-lnk">Boutique Hotels</span>
        <span class="footer-lnk">Luxury Hotels</span>
        <span class="footer-lnk">Group Travel</span>
        <span class="footer-lnk">Corporate Accounts</span>
      </div>
      <div>
        <div class="footer-col-title">Company</div>
        <span class="footer-lnk" onclick="showPage('about')">About Us</span>
        <span class="footer-lnk" onclick="showPage('partner')">Partnership</span>
        <span class="footer-lnk">Contact</span>
      </div>
      <div>
        <div class="footer-col-title">Legal</div>
        <span class="footer-lnk">Privacy Policy</span>
        <span class="footer-lnk">Terms of Service</span>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="footer-copy">© 2026 RNTX Travel Inc. All rights reserved. Toronto, ON, Canada.</div>
    </div>
  </footer>

</div><!-- /page-home -->


<!-- ════════════════════════════════
     PARTNER PAGE
════════════════════════════════ -->
<div id="page-partner" style="display:none">

  <div class="partner-hero">
    <div>
      <div class="sec-lbl">For Property Managers &amp; Hotels</div>
      <h1 class="sec-h light" style="font-size:clamp(38px,4.5vw,64px)">Become a<br>Certified Vendor</h1>
      <p style="font-size:15px;color:rgba(255,255,255,.5);line-height:1.8;margin-top:18px;font-weight:300;max-width:420px">Join our curated network of premium properties. We connect you directly with corporate travel managers and extended-stay clients seeking consistent, professional-grade accommodations.</p>
      <div class="partner-steps">
        <div class="partner-step"><div class="step-n">Step 1</div><div class="step-title">Submit Inquiry</div><div class="step-desc">Complete the inquiry form and describe your property portfolio.</div></div>
        <div class="partner-step"><div class="step-n">Step 2</div><div class="step-title">Qualification Review</div><div class="step-desc">Our team reviews your management structure and property standards.</div></div>
        <div class="partner-step"><div class="step-n">Step 3</div><div class="step-title">Standards Audit</div><div class="step-desc">Amenity verification, photo review, and policy confirmation.</div></div>
        <div class="partner-step"><div class="step-n">Step 4</div><div class="step-title">Onboarding &amp; Launch</div><div class="step-desc">Contract signing, rate setup, and go-live within 10 business days.</div></div>
      </div>
    </div>
    <div class="partner-form-wrap">
      <div id="partner-form-content">
        <div class="form-title" style="margin-bottom:6px">Partner Inquiry</div>
        <p class="form-sub">Tell us about your property portfolio. Our vendor team will review your inquiry and respond within 2 business days.</p>
        <div class="field"><label class="fl">Full Name</label><input class="fi" type="text" placeholder="Your full name"/></div>
        <div class="field"><label class="fl">Company / Property Name</label><input class="fi" type="text" placeholder="Company or property name"/></div>
        <div class="field-row">
          <div class="field"><label class="fl">Email</label><input class="fi" type="email" placeholder="you@company.com"/></div>
          <div class="field"><label class="fl">Phone</label><input class="fi" type="tel" placeholder="+1 (000) 000-0000"/></div>
        </div>
        <div class="field">
          <label class="fl">Property Type</label>
          <select class="fi">
            <option value="">Select type...</option>
            <option>Furnished Residences</option>
            <option>Boutique Hotel</option>
            <option>Luxury Hotel</option>
            <option>Mixed Portfolio</option>
          </select>
        </div>
        <div class="field-row">
          <div class="field"><label class="fl">Number of Units / Rooms</label><input class="fi" type="text" placeholder="e.g. 12 units"/></div>
          <div class="field"><label class="fl">City / Location</label><input class="fi" type="text" placeholder="e.g. Toronto, ON"/></div>
        </div>
        <div class="field"><label class="fl">Tell Us About Your Property</label><textarea class="fi" rows="4" style="resize:none" placeholder="Management structure, amenities offered, current channels, anything we should know..."></textarea></div>
        <button class="form-btn" onclick="submitPartner()">Submit Partner Inquiry</button>
        <p class="form-note">All inquiries are reviewed within 2 business days</p>
      </div>
    </div>
  </div>

  <section class="sec ivory-bg">
    <div class="sec-lbl">Why Partner With Us</div>
    <h2 class="sec-h dark">Access Corporate Demand<br>You Can't Reach Alone</h2>
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:2px;margin-top:48px" class="svc-grid-3">
      <div style="background:var(--white);padding:36px 28px;border-bottom:2px solid var(--gold)">
        <div style="font-family:var(--ff-disp);font-size:20px;font-weight:500;color:var(--charcoal);margin-bottom:12px;line-height:1.25">High-Value, Extended-Stay Clients</div>
        <div style="font-size:13px;color:var(--slate);line-height:1.75">Our clients are corporate travel managers, relocation coordinators, and executives booking 7–90+ night stays. These are the highest-value bookings in the accommodation category.</div>
      </div>
      <div style="background:var(--white);padding:36px 28px;border-bottom:2px solid var(--gold)">
        <div style="font-family:var(--ff-disp);font-size:20px;font-weight:500;color:var(--charcoal);margin-bottom:12px;line-height:1.25">No Marketplace Competition</div>
        <div style="font-size:13px;color:var(--slate);line-height:1.75">Unlike OTAs where you compete on price across thousands of listings, our curated roster is limited. Your property receives direct visibility to qualified buyers.</div>
      </div>
      <div style="background:var(--white);padding:36px 28px;border-bottom:2px solid var(--gold)">
        <div style="font-family:var(--ff-disp);font-size:20px;font-weight:500;color:var(--charcoal);margin-bottom:12px;line-height:1.25">Streamlined Operations</div>
        <div style="font-size:13px;color:var(--slate);line-height:1.75">We manage the client relationship, documentation, and invoicing. You focus on delivering a great stay. Booking confirmations, payments, and reporting are handled through our platform.</div>
      </div>
    </div>
  </section>

  <section class="sec charcoal-bg">
    <div style="max-width:600px">
      <div class="sec-lbl">Eligibility</div>
      <h2 class="sec-h light">Our Quality Standard</h2>
      <p style="font-size:15px;color:rgba(255,255,255,.5);line-height:1.8;margin-top:16px;font-weight:300">We maintain a curated network. Not every property qualifies — and that is precisely the point. Our standards protect the trust of our clients and the reputation of every partner in our portfolio.</p>
    </div>
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:3px;margin-top:40px">
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">Professional management entity — no individual hosts</span></div>
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">Minimum 5 active units or rooms</span></div>
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">7 AM–12 AM guest communications + after-hours emergency plan</span></div>
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">24-hour repair and maintenance response commitment</span></div>
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">Commercial insurance and articles of incorporation on file</span></div>
      <div style="display:flex;gap:14px;align-items:flex-start;padding:18px 20px;background:rgba(255,255,255,.03);border:1px solid rgba(255,255,255,.06)"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round"><path d="M20 6L9 17l-5-5"/></svg><span style="font-size:13px;color:rgba(255,255,255,.55);line-height:1.6">Ability to issue GST/HST invoices with itemised billing</span></div>
    </div>
  </section>

  <footer class="footer">
    <div class="footer-bottom" style="border-top:none;padding-top:0;justify-content:space-between">
      <div class="footer-copy">© 2026 RNTX Travel Inc. All rights reserved.</div>
      <button class="back-btn" onclick="showPage('home')">← Back to Home</button>
    </div>
  </footer>

</div><!-- /page-partner -->


<!-- ════════════════════════════════
     ABOUT PAGE
════════════════════════════════ -->
<div id="page-about" style="display:none">

  <div style="background:var(--charcoal);padding:100px 60px 80px">
    <div style="max-width:680px">
      <div class="sec-lbl">Our Story</div>
      <h1 class="sec-h light" style="font-size:clamp(42px,5vw,72px)">A Different Kind of<br>Travel Partner</h1>
      <p style="font-size:16px;color:rgba(255,255,255,.5);line-height:1.9;margin-top:22px;font-weight:300">We started as operators — managing furnished residences and placing corporate clients who demanded more than a standard OTA could deliver. We understood the gap firsthand: high-value travellers spending hours comparing platforms, only to land in properties that didn't live up to the listing.<br><br>RNTX Travel Inc. was built to solve that. Corporate accommodation specialists — with relationships, standards, and a genuine stake in the quality of every stay we arrange.</p>
    </div>
  </div>

  <section class="sec white-bg">
    <div class="about-grid">
      <div>
        <div class="sec-lbl">What We Stand For</div>
        <h2 class="sec-h dark">Values Built From<br>Operational Experience</h2>
        <div style="margin-top:32px">
          <div class="av-item"><div class="av-lbl">Quality Over Volume</div><div style="font-size:14px;color:var(--slate);line-height:1.7">We keep our certified partner roster intentionally limited. Every property we recommend has passed our review — and we only add properties we would book ourselves.</div></div>
          <div class="av-item"><div class="av-lbl">Transparency</div><div style="font-size:14px;color:var(--slate);line-height:1.7">No hidden fees. No ambiguous terms. Our clients know exactly what they're paying for and why the rate we've arranged represents real value.</div></div>
          <div class="av-item"><div class="av-lbl">Accountability</div><div style="font-size:14px;color:var(--slate);line-height:1.7">We don't disappear after a booking is confirmed. If something falls short, we own the resolution — because our reputation is tied to every stay.</div></div>
          <div class="av-item"><div class="av-lbl">Corporate-First</div><div style="font-size:14px;color:var(--slate);line-height:1.7">Everything about how we work — invoicing, documentation, reporting, approval workflows — is designed for finance teams and corporate travel managers.</div></div>
        </div>
      </div>
      <div style="background:var(--charcoal);padding:48px">
        <div class="sec-lbl">The Team</div>
        <div style="font-family:var(--ff-disp);font-size:22px;font-weight:500;color:var(--white);margin-bottom:8px">Joe DiFelice</div>
        <div style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:18px">Founder &amp; CEO</div>
        <p style="font-size:13px;color:rgba(255,255,255,.45);line-height:1.8;font-weight:300;margin-bottom:28px">Built RNTX after years managing premium furnished residences and placing corporate clients across Toronto. Understands the gap between what corporate travellers need and what the existing market delivers.</p>
        <div style="border-top:1px solid rgba(255,255,255,.08);padding-top:24px">
          <div style="font-family:var(--ff-mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:12px">Contact</div>
          <a href="/cdn-cgi/l/email-protection#fa90959fba889f948e829d88958f8ad4999597" style="font-size:13px;color:rgba(255,255,255,.55);display:block;margin-bottom:6px"><span class="__cf_email__" data-cfemail="056f6a604577606b717d62776a70752b666a68">[email&#160;protected]</span></a>
          <div style="font-size:13px;color:rgba(255,255,255,.35)">Toronto, ON, Canada</div>
        </div>
      </div>
    </div>
  </section>

  <div class="cta-band">
    <h2 class="cta-band-h">Let's arrange your next<br><em>corporate stay together.</em></h2>
    <button class="cta-band-btn" onclick="showPage('home')">Get a Quote →</button>
  </div>

  <footer class="footer">
    <div class="footer-bottom" style="border-top:none;padding-top:0">
      <div class="footer-copy">© 2026 RNTX Travel Inc. All rights reserved.</div>
      <button class="back-btn" onclick="showPage('home')">← Back to Home</button>
    </div>
  </footer>

</div><!-- /page-about -->


<script>
  window.showPage = function(name) {
    ['home','partner','about'].forEach(function(p) {
      document.getElementById('page-'+p).style.display = p===name ? 'block' : 'none';
    });
    ['nav-home','nav-partner','nav-about'].forEach(function(id) {
      document.getElementById(id).classList.remove('active');
    });
    var map = {home:'nav-home', partner:'nav-partner', about:'nav-about'};
    if (map[name]) document.getElementById(map[name]).classList.add('active');
    window.scrollTo({top:0, behavior:'smooth'});
  };

  window.toggleMobileMenu = function() {
    var m = document.getElementById('mobile-menu');
    m.style.display = (m.style.display === 'flex') ? 'none' : 'flex';
  };

  window.closeMobileMenu = function() {
    document.getElementById('mobile-menu').style.display = 'none';
  };

  window.submitQuote = function() {
    var form = document.getElementById('quote-form');
    var inputs = form.querySelectorAll('input, select, textarea');
    var labels = form.querySelectorAll('.fl');
    var lines = [];
    inputs.forEach(function(el, i) {
      var label = labels[i] ? labels[i].textContent.trim() : (el.placeholder || 'Field');
      var val = el.value.trim() || '(not provided)';
      lines.push(label + ': ' + val);
    });
    var subject = 'New RNTX Custom Quote Request';
    var body = lines.join('\n');
    window.location.href = 'mailto:hello@rntx.ca?subject=' + encodeURIComponent(subject) + '&body=' + encodeURIComponent(body);
    setTimeout(function() {
      document.getElementById('quote-content').innerHTML =
        '<div class="success-state">' +
          '<div class="success-icon">' +
            '<svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>' +
          '</div>' +
          '<div class="success-h">Request Received</div>' +
          '<p class="success-p">A member of our team will be in touch within 4 business hours with a tailored proposal.<br><br>' +
          'You can also reach us directly at <a href="mailto:hello@rntx.ca" style="color:var(--gold)">hello@rntx.ca</a></p>' +
        '</div>';
    }, 800);
  };

  window.submitPartner = function() {
    document.getElementById('partner-form-content').innerHTML =
      '<div class="success-state">' +
        '<div class="success-icon">' +
          '<svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A8822E" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>' +
        '</div>' +
        '<div class="success-h">Inquiry Submitted</div>' +
        '<p class="success-p">Thank you. Our team will review your portfolio and reach out within 2 business days to discuss next steps.</p>' +
      '</div>';
  };
</script>
</body>
</html>
