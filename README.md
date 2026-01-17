<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Top Fuel Heating & Cooling | Clarksville & Woodlawn HVAC</title>
  <meta name="description" content="Top Fuel Heating & Cooling in Clarksville, Woodlawn & surrounding areas. Call or text (931) 801-2394 for HVAC repair, maintenance, and installs." />

  <style>
    :root{
      --bg:#070b12;
      --text:#eaf0ff;
      --muted:#a9b4cf;
      --accent:#ff2d55;
      --accent2:#ffb703;
      --border: rgba(255,255,255,.12);
      --shadow: 0 16px 40px rgba(0,0,0,.35);
      --radius: 18px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      background:
        radial-gradient(1200px 700px at 15% 10%, rgba(255,45,85,.18), transparent 60%),
        radial-gradient(1000px 600px at 85% 15%, rgba(255,183,3,.14), transparent 55%),
        radial-gradient(800px 500px at 50% 90%, rgba(106,140,255,.10), transparent 60%),
        var(--bg);
      color:var(--text);
      line-height:1.55;
      padding-bottom: 78px; /* space for sticky mobile bar */
    }
    a{color:inherit; text-decoration:none}
    .wrap{max-width:1100px; margin:0 auto; padding:22px 18px 72px}

    /* Top bar */
    .topbar{
      display:flex; align-items:center; justify-content:space-between; gap:14px;
      padding:12px 14px;
      border:1px solid var(--border);
      border-radius: 999px;
      background: rgba(15,22,36,.62);
      backdrop-filter: blur(10px);
      position: sticky; top: 12px; z-index: 50;
      box-shadow: var(--shadow);
    }
    .brand{
      display:flex; align-items:center; gap:10px;
      font-weight:900; letter-spacing:.2px;
      white-space:nowrap;
      min-width: 220px;
    }
    .logo{
      width:34px; height:34px; border-radius:10px;
      object-fit:contain;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(7,11,18,.30);
      padding:4px;
    }
    .nav{
      display:flex; gap:10px; flex-wrap:wrap; justify-content:flex-end;
    }
    .chip{
      padding:8px 12px;
      border:1px solid var(--border);
      border-radius: 999px;
      color: var(--muted);
      font-size: 14px;
      background: rgba(7,11,18,.18);
    }
    .chip:hover{border-color:rgba(255,255,255,.22); color:var(--text)}
    .chip.primary{
      border:none;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      color:#070b12;
      font-weight:900;
    }

    /* Hero with flyer image */
    .hero{
      padding: 18px 6px 18px;
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 16px;
      align-items: stretch;
    }
    @media (max-width: 900px){
      .hero{grid-template-columns: 1fr}
      .topbar{position:static; border-radius: 18px}
    }

    .heroBanner{
      border:1px solid var(--border);
      border-radius: var(--radius);
      overflow:hidden;
      box-shadow: var(--shadow);
      position:relative;
      min-height: 220px;
      background:
        linear-gradient(180deg, rgba(7,11,18,.35), rgba(7,11,18,.85)),
        url("flyer.webp"); /* <-- CHANGE to flyer.png if needed */
      background-size: cover;
      background-position: center;
    }
    .heroBanner .inner{
      padding: 18px;
      position:absolute; inset:0;
      display:flex; flex-direction:column; justify-content:flex-end;
      gap: 10px;
    }
    .badge{
      display:inline-flex; align-items:center; gap:10px;
      padding:7px 12px;
      border:1px solid var(--border);
      border-radius:999px;
      color:var(--muted);
      font-size:13px;
      background: rgba(7,11,18,.45);
      width: fit-content;
    }
    .heroTitle{
      margin:0;
      font-size: clamp(30px, 4.2vw, 52px);
      line-height:1.05;
    }
    .sub{
      margin:0;
      color:var(--muted);
      font-size: clamp(15px, 2vw, 18px);
      max-width: 60ch;
    }
    .cta{
      display:flex; flex-wrap:wrap; gap:10px;
      margin-top: 8px;
    }
    .btn{
      display:inline-flex; align-items:center; justify-content:center; gap:10px;
      padding:12px 14px;
      border-radius: 14px;
      border:1px solid var(--border);
      background: rgba(7,11,18,.30);
      font-weight:900;
      letter-spacing:.1px;
      cursor:pointer;
      transition: transform .12s ease;
    }
    .btn:hover{transform: translateY(-1px)}
    .btn.primary{
      border:none;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      color:#070b12;
    }

    /* Right card */
    .side{
      border:1px solid var(--border);
      border-radius: var(--radius);
      background: rgba(15,22,36,.55);
      backdrop-filter: blur(10px);
      box-shadow: var(--shadow);
      padding: 18px;
    }
    .side h3{margin:0 0 10px}
    .callout{
      display:grid; gap:10px;
      padding:12px;
      border:1px solid var(--border);
      border-radius: 14px;
      background: rgba(7,11,18,.28);
    }
    .callout .row{
      display:flex; justify-content:space-between; gap:12px;
      color:var(--muted);
      font-size: 14px;
    }
    .callout .row b{color:var(--text)}
    .mini{margin-top:10px; color:var(--muted); font-size: 13px}

    /* Sections */
    section{margin-top: 22px}
    .sectionCard{
      border:1px solid var(--border);
      border-radius: var(--radius);
      background: rgba(15,22,36,.52);
      backdrop-filter: blur(10px);
      box-shadow: var(--shadow);
      padding: 18px;
    }
    h2{margin:0 0 10px; font-size: 26px}
    .grid{
      display:grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 12px;
    }
    .item{
      grid-column: span 4;
      padding:16px;
      border:1px solid var(--border);
      border-radius: 16px;
      background: rgba(7,11,18,.26);
      min-height: 118px;
    }
    .item strong{display:block; margin-bottom:6px}
    .item p{margin:0; color:var(--muted); font-size: 14px}
    @media (max-width: 900px){ .item{grid-column: span 12} }

    /* Reviews */
    .reviews{
      display:grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 12px;
      margin-top: 10px;
    }
    .review{
      grid-column: span 6;
      padding:16px;
      border:1px solid var(--border);
      border-radius: 16px;
      background: rgba(7,11,18,.26);
    }
    .review .top{
      display:flex; align-items:center; justify-content:space-between; gap:12px;
      margin-bottom: 8px;
    }
    .stars{letter-spacing:1px}
    .review p{margin:0; color:var(--muted); font-size:14px}
    .review b{font-size:14px}
    @media (max-width: 900px){ .review{grid-column: span 12} }

    /* Contact form */
    form{display:grid; gap:10px; max-width: 760px}
    input, textarea{
      width:100%;
      padding:12px 12px;
      border-radius: 14px;
      border:1px solid var(--border);
      background: rgba(7,11,18,.35);
      color: var(--text);
      outline:none;
    }
    textarea{min-height:120px; resize:vertical}
    .tiny{color:var(--muted); font-size: 12px}
    .footer{
      margin-top: 24px;
      padding-top: 16px;
      border-top: 1px solid var(--border);
      color: var(--muted);
      font-size: 14px;
      display:flex; justify-content:space-between; gap:12px; flex-wrap:wrap;
    }

    /* Sticky mobile bar */
    .stickyBar{
      position: fixed;
      left: 12px; right: 12px; bottom: 12px;
      display:flex; gap:10px;
      padding:10px;
      border-radius: 18px;
      border:1px solid var(--border);
      background: rgba(15,22,36,.75);
      backdrop-filter: blur(12px);
      box-shadow: var(--shadow);
      z-index: 99;
    }
    .stickyBar a{flex:1}
    .stickyBar .btn{width:100%}
    @media (min-width: 901px){
      .stickyBar{display:none}
      body{padding-bottom:0}
    }
  </style>
</head>

<body>
  <div class="wrap">

    <header class="topbar">
      <div class="brand">
        <!-- Put your logo file in the repo as logo.png -->
        <img class="logo" src="logo.png" alt="Top Fuel Heating & Cooling logo" />
        <span>Top Fuel Heating &amp; Cooling</span>
      </div>
      <nav class="nav">
        <a class="chip" href="#services">Services</a>
        <a class="chip" href="#service-area">Service Area</a>
        <a class="chip" href="#reviews">Reviews</a>
        <a class="chip" href="#contact">Contact</a>
        <a class="chip primary" href="tel:19318012394">Call Now</a>
      </nav>
    </header>

    <main class="hero" id="top">
      <div class="heroBanner" aria-label="Top Fuel flyer banner">
        <div class="inner">
          <div class="badge">🏁 Performance you can feel • Comfort you can trust</div>
          <h1 class="heroTitle">Fast HVAC service — done right.</h1>
          <p class="sub">
            Serving <b>Clarksville, Woodlawn</b> &amp; surrounding areas. Repairs, maintenance, and installs.
          </p>

          <div class="cta">
            <a class="btn primary" href="tel:19318012394">📞 Call (931) 801-2394</a>
            <a class="btn" href="sms:19318012394">💬 Text Now</a>
            <a class="btn" href="#contact">🧾 Get a Quote</a>
          </div>
        </div>
      </div>

      <aside class="side">
        <h3>Quick Info</h3>
        <div class="callout">
          <div class="row"><span>Call / Text</span><b>(931) 801-2394</b></div>
          <div class="row"><span>Email</span><b>topfuelhvac@gmail.com</b></div>
          <div class="row"><span>Service Area</span><b>Clarksville • Woodlawn + nearby</b></div>
        </div>

        <div class="cta" style="margin-top:12px">
          <a class="btn primary" href="tel:19318012394">Call Now</a>
          <a class="btn" href="sms:19318012394">Text Now</a>
          <a class="btn" href="https://g.page/r/CZp9-lTwZh0aEBM/review" target="_blank" rel="noreferrer">⭐ Leave a Review</a>
        </div>

        <div class="mini">
          Want your Facebook page button here too? I’ll add it.
        </div>
      </aside>
    </main>

    <section id="services" class="sectionCard">
      <h2>Services</h2>
      <div class="grid">
        <div class="item"><strong>AC Repair</strong><p>No cool air? We diagnose fast and get you back comfortable.</p></div>
        <div class="item"><strong>Heat Repair</strong><p>Furnace/heat pump issues — safe, reliable fixes.</p></div>
        <div class="item"><strong>System Install</strong><p>New installs and replacements (right-sized &amp; clean).</p></div>
        <div class="item"><strong>Maintenance</strong><p>Tune-ups to keep performance high and breakdowns low.</p></div>
        <div class="item"><strong>Airflow &amp; Comfort</strong><p>Hot/cold rooms, weak air — we track the cause and correct it.</p></div>
        <div class="item"><strong>Thermostats</strong><p>Upgrades, installs, setup help (including smart thermostats).</p></div>
      </div>
    </section>

    <section id="service-area" class="sectionCard">
      <h2>Service Area</h2>
      <p class="sub" style="margin-top:0">
        We proudly serve <b>Clarksville, Woodlawn</b> and surrounding areas.
        If you’re nearby, call/text and we’ll confirm availability.
      </p>
      <div class="grid">
        <div class="item"><strong>Main Areas</strong><p>Clarksville • Woodlawn</p></div>
        <div class="item"><strong>Surrounding Areas</strong><p>Nearby towns &amp; rural areas (ask us!)</p></div>
        <div class="item"><strong>Fast Contact</strong><p><a href="tel:19318012394">Call</a> or <a href="sms:19318012394">Text</a> for quickest response.</p></div>
      </div>
    </section>

    <section id="reviews" class="sectionCard">
      <h2>Reviews</h2>
      <p class="sub" style="margin-top:0">
        If we’ve helped you out, leaving a review helps people find us.
      </p>

      <div class="cta" style="margin: 8px 0 14px;">
        <a class="btn primary" href="https://g.page/r/CZp9-lTwZh0aEBM/review" target="_blank" rel="noreferrer">⭐ Leave a Google Review</a>
        <a class="btn" href="tel:19318012394">📞 Call Now</a>
        <a class="btn" href="sms:19318012394">💬 Text Now</a>
      </div>

      <div class="reviews">
        <div class="review">
          <div class="top"><b>“Fast and honest.”</b><span class="stars">★★★★★</span></div>
          <p>Showed up quick, explained everything clearly, and got our AC blowing cold again.</p>
          <p class="tiny" style="margin-top:8px">— Customer, Clarksville</p>
        </div>
        <div class="review">
          <div class="top"><b>“Clean work, fair price.”</b><span class="stars">★★★★★</span></div>
          <p>Great communication, quality work, and left everything clean. Highly recommend.</p>
          <p class="tiny" style="margin-top:8px">— Customer, Woodlawn</p>
        </div>
      </div>

      <p class="tiny" style="margin-top:12px">
        Replace those sample reviews with your real ones anytime.
      </p>
    </section>

    <section id="contact" class="sectionCard">
      <h2>Contact / Request Service</h2>
      <p class="sub" style="margin-top:0">
        Call or text now for fastest service — or send a message below.
      </p>

      <div class="cta" style="margin: 6px 0 14px;">
        <a class="btn primary" href="tel:19318012394">📞 Call Now</a>
        <a class="btn" href="sms:19318012394">💬 Text Now</a>
        <a class="btn" href="mailto:topfuelhvac@gmail.com">✉️ Email</a>
      </div>

      <!-- OPTIONAL FORM:
           If you want this form to email you, create a free Formspree form and replace YOUR_FORM_ID.
           https://formspree.io
      -->
      <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
        <input name="name" placeholder="Your name" required />
        <input name="phone" placeholder="Phone number" />
        <input name="email" type="email" placeholder="Email" required />
        <input name="city" placeholder="City/Area (Clarksville, Woodlawn, etc.)" />
        <textarea name="message" placeholder="What do you need help with? (AC not cooling, heat issue, install quote, etc.)" required></textarea>
        <button class="btn primary" type="submit">Send Request</button>
        <div class="tiny">
          Replace <b>YOUR_FORM_ID</b> with your Formspree ID to make this form work.
        </div>
      </form>
    </section>

    <footer class="footer">
      <div>© <span id="year"></span> Top Fuel Heating &amp; Cooling</div>
      <div><a href="#top">Back to top ↑</a></div>
    </footer>

  </div>

  <!-- Sticky mobile Call/Text bar -->
  <div class="stickyBar" aria-label="Quick contact bar">
    <a href="tel:19318012394"><span class="btn primary">📞 Call Now</span></a>
    <a href="sms:19318012394"><span class="btn">💬 Text Now</span></a>
  </div>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
