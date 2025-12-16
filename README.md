<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="FatSlim (HY7601 + KY1032) – Expo & advertising landing page." />
  <meta name="robots" content="index,follow" />
  <title>FatSlim | HY7601 + KY1032</title>

  <!-- Open Graph (optional) -->
  <meta property="og:title" content="FatSlim | HY7601 + KY1032" />
  <meta property="og:description" content="A probiotic solution designed to fit into a daily body-fat management routine." />
  <meta property="og:type" content="website" />
  <!-- <meta property="og:image" content="https://YOUR-DOMAIN/og-image.png" /> -->

  <style>
    :root{
      --bg:#0b0f17;
      --panel:#101826;
      --panel2:#0f1522;
      --text:#eaf0ff;
      --muted:#a9b4d0;
      --line:rgba(255,255,255,.10);
      --accent:#7c5cff;
      --accent2:#26d3ff;
      --ok:#33e6a6;
      --warn:#ffd166;
      --shadow: 0 20px 60px rgba(0,0,0,.45);
      --radius: 18px;
      --radius2: 26px;
      --max: 1100px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Noto Sans", sans-serif;
      color:var(--text);
      background:
        radial-gradient(1200px 700px at 20% 0%, rgba(124,92,255,.25), transparent 60%),
        radial-gradient(900px 600px at 90% 10%, rgba(38,211,255,.18), transparent 55%),
        radial-gradient(800px 600px at 50% 120%, rgba(51,230,166,.12), transparent 60%),
        var(--bg);
      line-height:1.55;
    }
    a{color:inherit}
    .wrap{max-width:var(--max); margin:0 auto; padding:28px 18px 70px}
    header{
      display:flex; align-items:center; justify-content:space-between;
      gap:14px; padding:8px 2px 18px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; text-decoration:none;
    }
    .logo{
      width:36px; height:36px; border-radius:12px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 10px 30px rgba(124,92,255,.25);
    }
    .brand b{letter-spacing:.2px}
    nav{display:flex; gap:10px; flex-wrap:wrap; justify-content:flex-end}
    .pill{
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      padding:9px 12px; border-radius:999px;
      text-decoration:none; color:var(--muted);
      font-size:13px;
      transition:transform .15s ease, background .15s ease;
    }
    .pill:hover{transform:translateY(-1px); background:rgba(255,255,255,.07); color:var(--text)}
    .hero{
      margin-top:10px;
      background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02));
      border:1px solid var(--line);
      border-radius: var(--radius2);
      padding: 34px 22px;
      box-shadow: var(--shadow);
      position:relative;
      overflow:hidden;
    }
    .hero:before{
      content:"";
      position:absolute; inset:-200px -200px auto auto;
      width:420px; height:420px;
      background: radial-gradient(circle at 30% 30%, rgba(124,92,255,.35), transparent 60%);
      filter: blur(6px);
    }
    .grid-hero{
      display:grid;
      grid-template-columns: 1.25fr .9fr;
      gap:22px;
      align-items:center;
    }
    @media (max-width: 900px){
      .grid-hero{grid-template-columns:1fr}
    }
    .badgeRow{display:flex; gap:10px; flex-wrap:wrap; margin-bottom:14px}
    .badge{
      font-size:12px;
      color:var(--muted);
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      padding:7px 10px;
      border-radius:999px;
    }
    h1{
      margin:0 0 10px;
      font-size: clamp(30px, 4.2vw, 54px);
      letter-spacing:-.6px;
      line-height:1.08;
    }
    .sub{
      margin:0 0 16px;
      color:var(--muted);
      font-size: 16px;
      max-width: 65ch;
    }
    .ctaRow{display:flex; gap:12px; flex-wrap:wrap; align-items:center; margin-top:16px}
    .btn{
      display:inline-flex; align-items:center; justify-content:center; gap:10px;
      padding: 12px 14px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.06);
      text-decoration:none;
      color:var(--text);
      font-weight:650;
      box-shadow: 0 14px 40px rgba(0,0,0,.35);
      transition: transform .16s ease, background .16s ease;
      cursor:pointer;
    }
    .btn:hover{transform: translateY(-1px); background: rgba(255,255,255,.09)}
    .btn.primary{
      border: 0;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      color:#07101b;
    }
    .btn.primary:hover{filter:brightness(1.03)}
    .hint{font-size:12px; color:var(--muted)}
    .panel{
      margin-top:18px;
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
    }
    @media (max-width: 900px){ .panel{grid-template-columns:1fr} }
    .card{
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      border-radius: var(--radius);
      padding: 16px;
    }
    .kpi{
      display:flex; align-items:flex-start; justify-content:space-between; gap:10px;
    }
    .kpi b{font-size:26px}
    .kpi span{color:var(--muted); font-size:13px}
    .tag{
      font-size:12px;
      color:#07101b;
      background: rgba(51,230,166,.92);
      padding: 6px 10px;
      border-radius: 999px;
      font-weight:700;
      white-space:nowrap;
    }
    .tag.warn{background: rgba(255,209,102,.92)}
    .section{margin-top:26px}
    .section h2{
      margin:0 0 10px;
      font-size: 22px;
      letter-spacing:-.3px;
    }
    .section p{margin:0 0 12px; color:var(--muted)}
    .two{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:12px;
    }
    @media (max-width: 900px){ .two{grid-template-columns:1fr} }
    .list{
      margin:0; padding-left:18px; color:var(--muted);
    }
    .list li{margin:8px 0}
    .quoteGrid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
      margin-top:12px;
    }
    @media (max-width: 900px){ .quoteGrid{grid-template-columns:1fr} }
    .quote{
      border:1px solid var(--line);
      background: linear-gradient(180deg, rgba(255,255,255,.05), rgba(255,255,255,.02));
      border-radius: var(--radius);
      padding: 16px;
    }
    .quote .meta{margin-top:10px; font-size:12px; color:var(--muted)}
    .hr{height:1px; background:var(--line); margin:16px 0}
    details{
      border:1px solid var(--line);
      border-radius: var(--radius);
      padding: 12px 14px;
      background: rgba(255,255,255,.03);
    }
    details + details{margin-top:10px}
    summary{cursor:pointer; font-weight:650}
    summary::marker{color:var(--muted)}
    .foot{
      margin-top:26px;
      color:var(--muted);
      font-size:12px;
    }
    .qrBox{
      display:flex; gap:14px; align-items:center; flex-wrap:wrap;
    }
    .qr{
      width:120px; height:120px; border-radius: 18px;
      border:1px dashed rgba(255,255,255,.25);
      display:flex; align-items:center; justify-content:center;
      color:rgba(255,255,255,.6);
      background: rgba(255,255,255,.02);
    }
    .mini{
      font-size:12px; color:var(--muted)
    }
    .accentLine{
      height:2px; width:92px; border-radius: 99px;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      margin:10px 0 14px;
    }
    .fineprint{
      font-size:11px;
      color:rgba(233,241,255,.62);
      border:1px solid rgba(255,255,255,.10);
      background: rgba(0,0,0,.16);
      padding: 12px 14px;
      border-radius: 16px;
    }
    .mutedLink{color:var(--muted); text-decoration:underline dotted; text-underline-offset:3px}
    .smallCaps{letter-spacing:.12em; text-transform:uppercase; font-size:11px; color:rgba(233,241,255,.70)}
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <a class="brand" href="#top" aria-label="FatSlim Home">
        <span class="logo" aria-hidden="true"></span>
        <div>
          <b>FatSlim</b><div class="hint">HY7601 + KY1032</div>
        </div>
      </a>

      <nav aria-label="Page">
        <a class="pill" href="#why">Key Benefits</a>
        <a class="pill" href="#formula">Strains & Formula</a>
        <a class="pill" href="#reviews">Reviews</a>
        <a class="pill" href="#expo">Expo & Contact</a>
        <a class="pill" href="#faq">FAQ</a>
      </nav>
    </header>

    <main id="top" class="hero">
      <div class="grid-hero">
        <div>
          <div class="badgeRow">
            <span class="badge">Body-fat management concept</span>
            <span class="badge">Expo & advertising landing</span>
            <span class="badge">Single-page (fast)</span>
          </div>

          <h1>A Probiotic Solution<br/>for a Lighter Daily Routine</h1>

          <p class="sub">
            <b>FatSlim</b> is built around the <b>HY7601 + KY1032</b> strain combination,
            designed to fit seamlessly into a daily routine oriented toward body-fat management.
          </p>

          <div class="ctaRow">
            <a class="btn primary" href="#expo">Request a Booth Consultation / Sample</a>
            <a class="btn" href="#catalog">View Brochure</a>
            <span class="hint">Note: Replace copy and claims based on your internal evidence and local ad regulations.</span>
          </div>

          <div class="panel" style="margin-top:18px">
            <div class="card">
              <div class="kpi">
                <div>
                  <b>2-Strain</b><br/>
                  <span>HY7601 + KY1032</span>
                </div>
                <span class="tag">COMBO</span>
              </div>
              <div class="hr"></div>
              <div class="hint">Core message: “combination-based design.”</div>
            </div>

            <div class="card">
              <div class="kpi">
                <div>
                  <b>Daily</b><br/>
                  <span>routine-friendly concept</span>
                </div>
                <span class="tag warn">DAILY</span>
              </div>
              <div class="hr"></div>
              <div class="hint">Optimized for expo and ad comprehension.</div>
            </div>

            <div class="card">
              <div class="kpi">
                <div>
                  <b>Clear</b><br/>
                  <span>simple information design</span>
                </div>
                <span class="tag" style="background:rgba(38,211,255,.92)">CLEAR</span>
              </div>
              <div class="hr"></div>
              <div class="hint">One page. Key points only.</div>
            </div>
          </div>
        </div>

        <div class="card" style="background:rgba(255,255,255,.02)">
          <h2 style="margin:0 0 10px; font-size:18px">Product Image</h2>
          <div class="hint" style="margin-bottom:10px">
            Add a front-facing PNG/JPG for best expo visuals.
          </div>

          <div style="border:1px dashed rgba(255,255,255,.22); border-radius:18px; padding:14px; text-align:center">
            <img
              src="assets/fatslim-product.png"
              alt="FatSlim product image"
              style="max-width:100%; height:auto; border-radius:14px; display:block; margin:0 auto"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='block';"
            />
            <div style="display:none; color:rgba(255,255,255,.6); padding:42px 10px">
              Add file: <b>assets/fatslim-product.png</b><br/>and it will appear here.
            </div>
          </div>

          <div class="hr"></div>
          <div class="mini">
            Tip: For expo use, a transparent-background PNG + a square thumbnail works well.
          </div>
        </div>
      </div>
    </main>

    <section id="why" class="section">
      <h2>Why FatSlim</h2>
      <div class="accentLine"></div>
      <p>
        Expo and ad landings perform best when visitors can understand the value in 5–10 seconds.
        Keep messaging concise and consistent across booth materials, QR, and ads.
      </p>

      <div class="two">
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">1) Routine-first positioning</h3>
          <ul class="list">
            <li>Designed to fit naturally into a daily consumption routine.</li>
            <li>Short, high-clarity copy works well for booth conversations and ad creatives.</li>
          </ul>
        </div>

        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">2) 2-strain combination concept</h3>
          <ul class="list">
            <li>Keep “HY7601 + KY1032” as the core differentiator.</li>
            <li>Move detailed evidence (study design, charts) to a separate brochure/PDF.</li>
          </ul>
        </div>
      </div>

      <div class="quoteGrid" aria-label="Testimonials">
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“Easy to understand at the booth.”</div>
          <div class="meta">Example placeholder • Replace with verified feedback</div>
          <div class="hint" style="margin-top:10px">Use only verified testimonials you have rights to publish.</div>
        </div>
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“Clear structure—helps recall.”</div>
          <div class="meta">Example placeholder • Ad landing format</div>
          <div class="hint" style="margin-top:10px">Avoid medical/disease claims unless compliant.</div>
        </div>
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“QR → brochure makes follow-up easy.”</div>
          <div class="meta">Example placeholder • Sales/partner flow</div>
          <div class="hint" style="margin-top:10px">Link to your PDF and contact form for conversions.</div>
        </div>
      </div>
    </section>

    <section id="formula" class="section">
      <h2>Strains & Formula (At a Glance)</h2>
      <div class="accentLine"></div>
      <p>
        This section is designed to communicate professionalism without overstating claims.
        Final copy should be reviewed against your evidence package and local advertising regulations.
      </p>

      <div class="two">
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">Core composition</h3>
          <ul class="list">
            <li><b>HY7601</b> — origin/characteristics (replace with your approved description)</li>
            <li><b>KY1032</b> — origin/characteristics (replace with your approved description)</li>
            <li>Suggested usage: once daily (replace with your label directions)</li>
          </ul>
        </div>

        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">Expo-friendly talking points</h3>
          <ul class="list">
            <li>Fix one sentence: “2-strain combination for routine-based body-fat management.”</li>
            <li>Move detailed data to a QR-linked brochure (PDF).</li>
            <li>Repeat CTA: sample request / partner inquiry / brochure download.</li>
          </ul>
        </div>
      </div>

      <div class="fineprint" style="margin-top:12px">
        <b>Disclaimer (example)</b><br/>
        This page is for informational purposes only. Individual results may vary.
        This product is not intended to diagnose, treat, cure, or prevent any disease.
      </div>
    </section>

    <section id="catalog" class="section">
      <h2>Brochure & Supporting Materials</h2>
      <div class="accentLine"></div>
      <p>
        A high-conversion expo flow is: <b>1) explain → 2) QR scan → 3) brochure → 4) contact</b>.
        Replace the buttons below with your PDF / reference links.
      </p>

      <div class="ctaRow">
        <!-- Replace href with your actual PDF path or URL -->
        <a class="btn" href="assets/fatslim-brochure.pdf" target="_blank" rel="noopener">
          Open Brochure (PDF)
        </a>
        <!-- Replace href with your evidence/reference page -->
        <a class="btn" href="#" onclick="alert('Replace this with your evidence/references link.'); return false;">
          View Supporting Materials
        </a>
      </div>

      <div class="hint" style="margin-top:10px">
        Tip: You can host PDFs directly in the same GitHub Pages repository (static file hosting).
      </div>
    </section>

    <section id="reviews" class="section">
      <h2>Reviews & Mentions</h2>
      <div class="accentLine"></div>
      <p>
        Public “reviews” mentioning specific probiotic strains can be limited. For expo use, provide:
        (1) search links for transparency and (2) embedded highlights for curated, verifiable sources.
      </p>

      <div class="ctaRow">
        <a class="btn primary" target="_blank" rel="noopener"
           href="https://www.google.com/search?q=HY7601+KY1032+review">
          Search HY7601 + KY1032 on Google
        </a>
        <a class="btn" target="_blank" rel="noopener"
           href="https://www.google.com/search?q=FatSlim+HY7601+KY1032+review">
          Search “FatSlim” on Google
        </a>
        <a class="btn" target="_blank" rel="noopener"
           href="https://www.reddit.com/search/?q=HY7601%20KY1032">
          Search on Reddit
        </a>
      </div>

      <div class="hr"></div>

      <div class="card">
        <div class="smallCaps">Embedded Highlights (Reddit)</div>
        <h3 style="margin:6px 0 8px; font-size:16px">Preview cards for specific posts</h3>
        <div class="hint" style="margin-bottom:10px">
          Replace the example URLs with real Reddit post URLs you want to showcase.
          If you don’t have URLs yet, you can remove this card or keep it hidden.
        </div>

        <!-- EXAMPLE EMBED: Replace with a real Reddit post link -->
        <blockquote class="reddit-embed-bq" data-embed-height="240">
          <a href="https://www.reddit.com/r/Supplements/comments/POST_ID/example_title/">
            View discussion
          </a>
        </blockquote>

        <div class="hint" style="margin-top:10px">
          If the embed doesn’t show, the post may not allow embedding or the URL may be incorrect.
        </div>
      </div>

      <!-- Reddit embed script (only once per page) -->
      <script async src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script>
    </section>

    <section id="expo" class="section">
      <h2>Expo & Contact</h2>
      <div class="accentLine"></div>
      <p>
        This block is optimized for booth tablets and for the final CTA in ad landings.
        For lead capture, link to an external form (Google Forms / Typeform / etc.).
      </p>

      <div class="card">
        <div class="qrBox">
          <div class="qr" aria-label="QR placeholder">QR</div>

          <div>
            <div style="font-weight:750; font-size:16px">Scan to request a consultation / sample</div>
            <div class="mini">Add your QR image as <b>assets/qr.png</b> and it will appear below.</div>

            <div class="hr"></div>

            <img
              src="assets/qr.png"
              alt="QR code for inquiry"
              style="max-width:160px; height:auto; border-radius:14px; display:block"
              onerror="this.style.display='none';"
            />

            <div class="ctaRow" style="margin-top:12px">
              <!-- Replace with your actual email/phone/form link -->
              <a class="btn primary" href="mailto:hello@example.com?subject=FatSlim%20Expo%20Inquiry">
                Email inquiry
              </a>
              <a class="btn" href="tel:+82-10-0000-0000">Call</a>
              <a class="btn" href="#" onclick="alert('Replace this with your contact form link (Google Forms/Typeform).'); return false;">
                Open inquiry form
              </a>
            </div>

            <div class="hint" style="margin-top:10px">
              Recommended lead fields: Name / Company / Contact / Interest (Sample · Distributor · OEM).
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="faq" class="section">
      <h2>FAQ</h2>
      <div class="accentLine"></div>

      <details>
        <summary>Q. How should we position HY7601 + KY1032?</summary>
        <div class="hint" style="margin-top:10px">
          A. Use a single consistent definition (e.g., “a 2-strain combination designed for routine-based body-fat management”),
          and move detailed evidence to your brochure/references page.
        </div>
      </details>

      <details>
        <summary>Q. What CTAs work best for expo landings?</summary>
        <div class="hint" style="margin-top:10px">
          A. Typically: (1) sample request, (2) partner/distributor inquiry, (3) brochure download—repeated near the top and bottom.
        </div>
      </details>

      <details>
        <summary>Q. Can we state strong weight-loss claims?</summary>
        <div class="hint" style="margin-top:10px">
          A. Final claim language must match your evidence package and comply with local advertising rules and platform policies.
          This template intentionally avoids medical/disease claims and absolute promises.
        </div>
      </details>
    </section>

    <footer class="foot">
      <div class="fineprint">
        <b>Disclaimer</b><br/>
        This page is an initial draft for expo/advertising use. Before publication or ad spend,
        review all copy for regulatory compliance and alignment with your internal supporting materials.
      </div>

      <div style="margin-top:10px">
        © <span id="y"></span> FatSlim. All rights reserved.
      </div>
    </footer>
  </div>

  <script>
    document.getElementById("y").textContent = new Date().getFullYear();
  </script>
</body>
</html>

