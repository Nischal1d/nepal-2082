<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Nischal - Nepal Stock Market</title>
  <meta name="description" content="Your go-to source for the latest updates and insights on the Nepal stock market." />

  <style>
    /* Base / reset */
    * { box-sizing: border-box; }
    html,body{ height:100%; margin:0; font-family: Arial, Helvetica, sans-serif; color:#222; background:#f7f9f8; }

    /* Header */
    header.site-header{ background:#4CAF50; color:white; padding:28px 20px; display:flex; align-items:center; justify-content:space-between; gap:16px; }
    .brand{ display:flex; align-items:center; gap:12px; }
    .logo{ width:48px; height:48px; border-radius:8px; background:rgba(255,255,255,0.12); display:flex; align-items:center; justify-content:center; font-weight:700; font-size:18px; }
    .site-title{ font-size:20px; margin:0; }
    .site-tag{ font-size:13px; opacity:0.9; }

    /* Nav */
    nav.main-nav a{ color:white; text-decoration:none; margin-left:14px; font-weight:600; }

    /* Hero */
    .hero{ padding:36px 20px; display:flex; gap:24px; align-items:center; justify-content:space-between; flex-wrap:wrap; }
    .hero-left{ max-width:740px; }
    .hero h1{ margin:0 0 10px 0; font-size:34px; }
    .hero p{ margin:0 0 16px 0; font-size:16px; }
    .cta{ display:inline-block; padding:10px 16px; border-radius:8px; background:white; color:#4CAF50; font-weight:700; text-decoration:none; }

    /* Layout */
    main{ padding:20px; max-width:1100px; margin:0 auto; }
    .grid{ display:grid; grid-template-columns: repeat(12, 1fr); gap:18px; }
    .col-8{ grid-column: span 8; }
    .col-4{ grid-column: span 4; }

    /* Sections */
    section.card{ background:white; padding:18px; border-radius:10px; box-shadow: 0 2px 8px rgba(16,24,40,0.06); }
    section.card h2{ margin:0 0 8px 0; font-size:20px; }
    section.card p{ margin:0 0 12px 0; line-height:1.5; }

    /* Market table */
    .stock-table{ width:100%; border-collapse:collapse; margin-top:12px; }
    .stock-table th, .stock-table td{ padding:10px 8px; text-align:left; border-bottom:1px solid #eee; font-size:14px; }
    .stock-up{ color:#0a7a3b; font-weight:700; }
    .stock-down{ color:#b00020; font-weight:700; }

    /* Analysis cards */
    .analysis-list{ display:flex; gap:12px; flex-wrap:wrap; }
    .analysis-item{ flex:1 1 220px; min-width:200px; background:linear-gradient(180deg,#fff,#fbfffb); padding:12px; border-radius:8px; }
    .analysis-item h3{ margin:0 0 8px 0; font-size:16px; }
    .analysis-item p{ margin:0; font-size:13px; color:#444; }

    /* Contact */
    .contact-form{ display:flex; flex-direction:column; gap:8px; }
    .contact-form input, .contact-form textarea{ padding:10px; border-radius:6px; border:1px solid #ddd; font-size:14px; }
    .btn{ padding:10px 12px; border-radius:8px; border:none; cursor:pointer; font-weight:700; }
    .btn-primary{ background:#4CAF50; color:white; }

    /* Footer */
    footer.site-footer{ background:#333; color:#fff; padding:18px 20px; margin-top:28px; }
    footer .footer-inner{ max-width:1100px; margin:0 auto; display:flex; justify-content:space-between; gap:12px; align-items:center; flex-wrap:wrap; }

    /* Responsive */
    @media (max-width:900px){ .col-8{ grid-column: span 12; } .col-4{ grid-column: span 12; } .hero h1{ font-size:26px; } }
  </style>
</head>
<body>

  <header class="site-header">
    <div class="brand">
      <div class="logo">N</div>
      <div>
        <div class="site-title">Nischal</div>
        <div class="site-tag">Nepal Stock Market</div>
      </div>
    </div>

    <nav class="main-nav">
      <a href="#about">About</a>
      <a href="#news">Market News</a>
      <a href="#analysis">Stock Analysis</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <div class="hero" role="banner">
    <div class="hero-left">
      <h1>Welcome to Nischal</h1>
      <p>Your go-to source for the latest updates and insights on the Nepal stock market.</p>
      <a class="cta" href="#news">See latest market updates</a>
    </div>
    <div class="hero-right">
      <!-- Small summary card -->
      <div style="background:white;padding:14px;border-radius:10px;box-shadow:0 2px 12px rgba(16,24,40,0.06);min-width:220px;">
        <strong>Market Snapshot</strong>
        <div style="margin-top:8px;font-size:13px;color:#555;">NEPSE Index</div>
        <div id="nepse" style="font-size:20px;font-weight:800;margin-top:8px;">--</div>
        <small style="display:block;margin-top:8px;color:#777;">Updated locally (sample)</small>
      </div>
    </div>
  </div>

  <main>
    <div class="grid">

      <div class="col-8">
        <section id="about" class="card">
          <h2>About</h2>
          <p>Nischal is dedicated to providing accurate and timely information about the Nepal stock market, helping investors make informed decisions.</p>
        </section>

        <section id="news" class="card" style="margin-top:16px;">
          <h2>Market News</h2>
          <p>Stay updated with the latest stock market news and trends in Nepal.</p>

          <ul style="padding-left:18px;margin:12px 0 0 0;">
            <li><strong>Oct 20, 2023:</strong> Sample news headline about market activity in Nepal.</li>
            <li><strong>Sep 10, 2023:</strong> Sample update on investor sentiment and sector movement.</li>
            <li><strong>Jul 04, 2023:</strong> Sample item: regulatory or policy update affecting listed companies.</li>
          </ul>
        </section>

        <section id="analysis" class="card" style="margin-top:16px;">
          <h2>Stock Analysis</h2>
          <p>In-depth analysis of various stocks listed on the Nepal Stock Exchange.</p>

          <div class="analysis-list">
            <article class="analysis-item">
              <h3>Company A — Quick Take</h3>
              <p>Price momentum shows moderate growth. Watch quarterly earnings and promoter activity.</p>
            </article>
            <article class="analysis-item">
              <h3>Company B — Quick Take</h3>
              <p>Strong balance sheet but watch valuation. Dividend history is favourable.</p>
            </article>
            <article class="analysis-item">
              <h3>Company C — Quick Take</h3>
              <p>High volatility; suitable for short-term traders with tight risk controls.</p>
            </article>
          </div>

        </section>

      </div>

      <div class="col-4">
        <section class="card">
          <h2>Live Stocks (sample)</h2>
          <p>Example list of stocks — replace with real data via an API or server feed.</p>

          <table class="stock-table" aria-label="sample stock table">
            <thead>
              <tr><th>Symbol</th><th>Price</th><th>Change</th></tr>
            </thead>
            <tbody id="stock-rows">
              <tr><td>NEPSE</td><td>2,450.34</td><td class="stock-up">+12.50</td></tr>
              <tr><td>NLIC</td><td>1,250.00</td><td class="stock-down">-8.30</td></tr>
              <tr><td>HBL</td><td>1,012.45</td><td class="stock-up">+4.10</td></tr>
            </tbody>
          </table>
        </section>

        <section id="contact" class="card" style="margin-top:16px;">
          <h2>Contact</h2>
          <p>Get in touch with us for queries and collaborations.</p>

          <form class="contact-form" onsubmit="event.preventDefault(); alert('This is a demo form — wire up to your backend.');">
            <input type="text" placeholder="Your name" required />
            <input type="email" placeholder="Email" required />
            <textarea rows="4" placeholder="Message"></textarea>
            <button class="btn btn-primary" type="submit">Send</button>
          </form>
        </section>
      </div>

    </div>
  </main>

  <footer class="site-footer">
    <div class="footer-inner">
      <div>© 2023 Nischal. All rights reserved.</div>
      <div style="opacity:0.85;">Built with care in Nepal</div>
    </div>
  </footer>

  <script>
    // Small demo script that simulates updating the market snapshot and small price changes.
    (function(){
      const nepseEl = document.getElementById('nepse');
      const rows = document.querySelectorAll('#stock-rows tr');

      function randomBetween(min,max){ return (Math.random()*(max-min)+min).toFixed(2); }

      function updateSnapshot(){
        const value = (2400 + (Math.random()*120 - 60)).toFixed(2);
        nepseEl.textContent = value + ' pts';
      }

      function jitterPrices(){
        rows.forEach(r=>{
          const priceCell = r.cells[1];
          const changeCell = r.cells[2];
          const base = parseFloat(priceCell.textContent.replace(/,/g,'')) || 1000;
          const delta = (Math.random()*20-10).toFixed(2);
          const newPrice = (base + parseFloat(delta)).toFixed(2);
          priceCell.textContent = Number(newPrice).toLocaleString();
          changeCell.textContent = (delta>0?'+':'') + delta;
          changeCell.className = delta>0 ? 'stock-up' : 'stock-down';
        });
      }

      updateSnapshot();
      jitterPrices();
      setInterval(updateSnapshot, 8000);
      setInterval(jitterPrices, 6000);
    })();
  </script>

</body>
</html>
