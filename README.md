<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="Fast roadside assistance: spare tire change, air filling, battery jump start, lockout service, and remote programming. Mobile help to your location." />
  <title>YOUR_BUSINESS_NAME | Roadside Assistance</title>

  <!-- Basic SEO -->
  <meta property="og:title" content="YOUR_BUSINESS_NAME | Roadside Assistance" />
  <meta property="og:description" content="Fast roadside help: tire change, jump start, lockout, air fill, and remote programming." />
  <meta property="og:type" content="website" />

  <style>
    :root{
      --bg:#0b1220;
      --card:#111a2e;
      --muted:#a7b0c0;
      --text:#eef2ff;
      --brand:#5eead4;
      --brand2:#60a5fa;
      --danger:#fb7185;
      --shadow: 0 20px 50px rgba(0,0,0,.45);
      --radius: 18px;
      --max: 1100px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
      background: radial-gradient(1200px 700px at 20% -10%, rgba(96,165,250,.25), transparent 60%),
                  radial-gradient(900px 600px at 80% 10%, rgba(94,234,212,.18), transparent 60%),
                  var(--bg);
      color:var(--text);
      line-height:1.45;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max); margin:0 auto; padding:24px;}
    .topbar{
      position: sticky; top:0; z-index:999;
      backdrop-filter: blur(10px);
      background: rgba(11,18,32,.65);
      border-bottom: 1px solid rgba(255,255,255,.08);
    }
    .topbar .wrap{display:flex; align-items:center; justify-content:space-between; gap:12px;}
    .brand{
      display:flex; align-items:center; gap:10px; font-weight:800; letter-spacing:.2px;
    }
    .logo{
      width:38px; height:38px; border-radius:12px;
      background: linear-gradient(135deg, rgba(94,234,212,.95), rgba(96,165,250,.95));
      box-shadow: var(--shadow);
      display:grid; place-items:center; color:#071120; font-weight:900;
    }
    .nav{display:flex; gap:16px; align-items:center; flex-wrap:wrap}
    .nav a{color:var(--muted); font-weight:600}
    .nav a:hover{color:var(--text)}
    .ctaRow{display:flex; gap:10px; flex-wrap:wrap; justify-content:flex-end}
    .btn{
      padding:11px 14px; border-radius:14px;
      border:1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.06);
      color:var(--text);
      font-weight:800;
      display:inline-flex; align-items:center; gap:10px;
      transition:.15s transform ease, .15s background ease, .15s border-color ease;
    }
    .btn:hover{transform: translateY(-1px); background: rgba(255,255,255,.1); border-color: rgba(255,255,255,.2);}
    .btn.primary{
      border:none;
      background: linear-gradient(135deg, rgba(94,234,212,.95), rgba(96,165,250,.95));
      color:#06121d;
    }
    .btn.danger{
      border:none;
      background: linear-gradient(135deg, rgba(251,113,133,.95), rgba(244,63,94,.95));
      color:#1a0610;
    }
    .hero{
      padding:54px 0 24px;
      display:grid; grid-template-columns: 1.25fr .85fr; gap:20px;
      align-items:stretch;
    }
    @media (max-width: 920px){
      .hero{grid-template-columns: 1fr; padding-top:34px;}
      .ctaRow{justify-content:flex-start}
    }
    .hCard{
      background: linear-gradient(180deg, rgba(255,255,255,.08), rgba(255,255,255,.03));
      border:1px solid rgba(255,255,255,.10);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding:26px;
      position:relative;
      overflow:hidden;
    }
    .hCard:before{
      content:"";
      position:absolute; inset:-2px;
      background: radial-gradient(600px 240px at 20% 20%, rgba(94,234,212,.14), transparent 60%),
                  radial-gradient(600px 240px at 90% 10%, rgba(96,165,250,.14), transparent 60%);
      pointer-events:none;
    }
    h1{
      margin:0 0 10px;
      font-size: clamp(28px, 4vw, 46px);
      line-height:1.05;
      letter-spacing:-.8px;
    }
    .sub{
      color:var(--muted);
      font-size: 16px;
      max-width: 60ch;
      margin:0 0 18px;
    }
    .chips{display:flex; gap:10px; flex-wrap:wrap; margin:18px 0 0}
    .chip{
      padding:8px 10px; border-radius:999px;
      border:1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.06);
      color: var(--text);
      font-weight:700;
      font-size: 13px;
    }
    .grid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:14px;
      margin: 18px 0;
    }
    @media (max-width: 920px){ .grid{grid-template-columns: 1fr;} }
    .card{
      background: rgba(17,26,46,.65);
      border:1px solid rgba(255,255,255,.10);
      border-radius: var(--radius);
      padding:18px;
      box-shadow: 0 12px 30px rgba(0,0,0,.35);
    }
    .card h3{margin:0 0 6px; font-size: 16px}
    .card p{margin:0; color:var(--muted); font-size: 14px}
    section{padding:22px 0}
    .sectionTitle{
      font-size: 22px; margin: 0 0 8px; letter-spacing:-.3px
    }
    .sectionDesc{color:var(--muted); margin:0 0 14px}
    .twoCol{
      display:grid; grid-template-columns: 1fr 1fr; gap:14px;
    }
    @media (max-width: 920px){ .twoCol{grid-template-columns:1fr} }
    .list{margin:0; padding-left:18px; color:var(--muted)}
    .list li{margin:8px 0}
    .badge{
      display:inline-flex; align-items:center; gap:8px;
      padding:8px 10px; border-radius:999px;
      background: rgba(94,234,212,.12);
      border:1px solid rgba(94,234,212,.25);
      color: var(--text);
      font-weight:800;
      font-size: 13px;
    }
    .form{
      display:grid; gap:10px;
    }
    input, textarea, select{
      width:100%;
      padding:12px 12px;
      border-radius:14px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.06);
      color: var(--text);
      outline:none;
    }
    textarea{min-height:110px; resize:vertical}
    label{font-weight:800; font-size: 13px; color: var(--muted)}
    .fineprint{color:var(--muted); font-size: 12px; margin:10px 0 0}
    footer{
      border-top: 1px solid rgba(255,255,255,.08);
      margin-top: 30px;
      padding: 22px 0 40px;
      color: var(--muted);
      font-size: 13px;
    }
  </style>
</head>
<body>

  <div class="topbar">
    <div class="wrap">
      <div class="brand">
        <div class="logo">RA</div>
        <div>
          <div style="font-size:14px;">YOUR_BUSINESS_NAME</div>
          <div style="font-size:12px;color:var(--muted);font-weight:700;">Roadside Assistance • Mobile Service</div>
        </div>
      </div>

      <div class="nav">
        <a href="#services">Services</a>
        <a href="#how">How it works</a>
        <a href="#area">Service area</a>
        <a href="#contact">Request help</a>
      </div>

      <div class="ctaRow">
        <a class="btn danger" href="tel:YOUR_PHONE">📞 Call</a>
        <a class="btn primary" href="sms:YOUR_PHONE?&body=Hi!%20I%20need%20roadside%20assistance.%20My%20location%20is%20____.%20Service%20needed:%20____.">💬 Text</a>
      </div>
    </div>
  </div>

  <main class="wrap">
    <div class="hero">
      <div class="hCard">
        <div class="badge">⚡ Fast response • Upfront pricing • Mobile service</div>
        <h1>Roadside Help When You Need It — Tire, Jump, Lockout & Remote Programming</h1>
        <p class="sub">
          Stuck at home, work, or on the road? We come to your location for
          <strong>spare tire changes</strong>, <strong>air filling</strong>, <strong>battery jump starts</strong>,
          <strong>lockouts</strong>, and <strong>remote programming</strong>.
        </p>

        <div class="ctaRow" style="justify-content:flex-start; margin-top:8px;">
          <a class="btn danger" href="tel:YOUR_PHONE">📞 Call for Help</a>
          <a class="btn primary" href="#contact">📝 Request Help</a>
        </div>

        <div class="chips">
          <div class="chip">✅ Tire Change</div>
          <div class="chip">✅ Jump Start</div>
          <div class="chip">✅ Lockout</div>
          <div class="chip">✅ Air Fill</div>
          <div class="chip">✅ Remote Programming</div>
        </div>
      </div>

      <div class="hCard">
        <h2 style="margin:0 0 10px; font-size:22px; letter-spacing:-.2px;">Quick Estimate</h2>
        <p class="sectionDesc">Select a service to see typical ranges (edit these anytime).</p>

        <div class="form">
          <label for="svc">Service needed</label>
          <select id="svc">
            <option value="Tire Change">Spare Tire Change</option>
            <option value="Air Fill">Air Filling</option>
            <option value="Jump Start">Battery Jump Start</option>
            <option value="Lockout">Lockout Service</option>
            <option value="Remote Programming">Remote Programming</option>
          </select>

          <label for="loc">Your location (landmark / address)</label>
          <input id="loc" placeholder="Example: Broadlands, Ashburn VA" />

          <div class="card" id="estimateCard">
            <h3 style="margin:0 0 6px;">Estimated range</h3>
            <p id="estimateText" style="margin:0; color:var(--muted);">Select a service to view estimate.</p>
          </div>

          <a class="btn primary" id="textBtn" href="#">💬 Text for exact quote</a>
          <div class="fineprint">
            Final price depends on distance, vehicle type, and complexity. We’ll confirm before dispatch.
          </div>
        </div>
      </div>
    </div>

    <section id="services">
      <h2 class="sectionTitle">Services</h2>
      <p class="sectionDesc">Fast, professional roadside help — we come to you.</p>

      <div class="grid">
        <div class="card">
          <h3>🛞 Spare Tire Change</h3>
          <p>Safe jack-up, remove flat, install spare, torque check. (Spare required.)</p>
        </div>
        <div class="card">
          <h3>💨 Air Filling</h3>
          <p>Top up tires and check pressure. Great for slow leaks until you reach a shop.</p>
        </div>
        <div class="card">
          <h3>🔋 Battery Jump Start</h3>
          <p>Quick jump start and basic charging check to get you moving again.</p>
        </div>
        <div class="card">
          <h3>🔑 Lockout Service</h3>
          <p>Non-damaging entry methods whenever possible. Fast help when keys are inside.</p>
        </div>
        <div class="card">
          <h3>📡 Remote Programming</h3>
          <p>Remote/key programming support (availability varies by vehicle and system).</p>
        </div>
        <div class="card">
          <h3>⏱️ Quick Dispatch</h3>
          <p>Call or text with your location + issue. We’ll confirm ETA and price upfront.</p>
        </div>
      </div>
    </section>

    <section id="how">
      <h2 class="sectionTitle">How it works</h2>
      <div class="twoCol">
        <div class="card">
          <h3>1) Call or text</h3>
          <p>Tell us your location, vehicle, and the issue (tire, jump, lockout, etc.).</p>
        </div>
        <div class="card">
          <h3>2) Get an ETA + upfront price</h3>
          <p>We confirm service details and a price range before dispatch.</p>
        </div>
        <div class="card">
          <h3>3) We arrive and help</h3>
          <p>Fast, professional service — we’ll get you back on the road ASAP.</p>
        </div>
        <div class="card">
          <h3>4) Pay & go</h3>
          <p>Pay after service. Request a receipt if needed for reimbursement.</p>
        </div>
      </div>
    </section>

    <section id="area">
      <h2 class="sectionTitle">Service Area</h2>
      <p class="sectionDesc">
        Mobile roadside assistance in <strong>Loudoun County</strong> and nearby areas.
        (Update this list to match exactly where you operate.)
      </p>
      <div class="card">
        <ul class="list">
          <li>Ashburn • Broadlands • Brambleton</li>
          <li>Sterling • Herndon • Reston</li>
          <li>Leesburg • South Riding • Chantilly</li>
        </ul>
      </div>
    </section>

    <section id="contact">
      <h2 class="sectionTitle">Request Help</h2>
      <p class="sectionDesc">Fill this out and we’ll respond ASAP. For emergencies, call/text for fastest response.</p>

      <div class="twoCol">
        <div class="card">
          <form class="form" onsubmit="return buildEmail(event)">
            <label for="name">Name</label>
            <input id="name" placeholder="Your name" required />

            <label for="phone">Phone</label>
            <input id="phone" placeholder="(###) ###-####" required />

            <label for="service">Service</label>
            <select id="service">
              <option>Spare Tire Change</option>
              <option>Air Filling</option>
              <option>Battery Jump Start</option>
              <option>Lockout Service</option>
              <option>Remote Programming</option>
            </select>

            <label for="address">Current location</label>
            <input id="address" placeholder="Address or nearby landmark" required />

            <label for="details">Details</label>
            <textarea id="details" placeholder="Vehicle year/make/model, what happened, any special notes."></textarea>

            <button class="btn primary" type="submit">📩 Send Request</button>
            <div class="fineprint">
              This form opens your email app to send the request. If you prefer, text us instead for faster dispatch.
            </div>
          </form>
        </div>

        <div class="card">
          <h3 style="margin-top:0;">Contact</h3>
          <p style="color:var(--muted);margin-top:0;">
            Phone: <a href="tel:YOUR_PHONE" style="color:var(--text);font-weight:900;">YOUR_PHONE</a><br/>
            Text: <a href="sms:YOUR_PHONE" style="color:var(--text);font-weight:900;">SMS YOUR_PHONE</a><br/>
            Hours: 24/7 (or set your real hours)<br/>
            Payment: Cash, Card, Zelle, Cash App (edit)
          </p>

          <div style="margin-top:14px;">
            <a class="btn danger" href="tel:YOUR_PHONE">📞 Call Now</a>
            <a class="btn primary" href="sms:YOUR_PHONE?&body=Hi!%20I%20need%20roadside%20assistance.%20My%20location%20is%20____.%20Service%20needed:%20____.">💬 Text Now</a>
          </div>

          <div class="fineprint" style="margin-top:14px;">
            Tip: Add your Google reviews link here once you have it, to build instant trust.
          </div>
        </div>
      </div>
    </section>

    <footer>
      © <span id="yr"></span> YOUR_BUSINESS_NAME. All rights reserved.
      <div style="margin-top:8px;">Emergency? If you’re in a dangerous location, move to safety and call 911 first.</div>
    </footer>
  </main>

  <script>
    const PHONE = "YOUR_PHONE"; // e.g. "+17035551234" (include country code if you want)
    const estimates = {
      "Tire Change": "$75–$150 (depends on wheel type, location, and roadside conditions)",
      "Air Fill": "$40–$75 (basic fill + pressure check)",
      "Jump Start": "$60–$130 (depends on access and battery condition)",
      "Lockout": "$75–$180 (vehicle type + complexity)",
      "Remote Programming": "Quoted after details (varies widely by vehicle/system)"
    };

    const svcEl = document.getElementById("svc");
    const locEl = document.getElementById("loc");
    const estText = document.getElementById("estimateText");
    const textBtn = document.getElementById("textBtn");

    function updateEstimate(){
      const svc = svcEl.value;
      estText.textContent = estimates[svc] || "Select a service to view estimate.";
      const loc = encodeURIComponent(locEl.value || "my location");
      const body = encodeURIComponent(`Hi! I need ${svc}. My location is ${locEl.value || "____"}. Can you send ETA and exact quote?`);
      textBtn.href = `sms:${PHONE}?&body=${body}`;
    }

    svcEl.addEventListener("change", updateEstimate);
    locEl.addEventListener("input", updateEstimate);
    updateEstimate();

    document.getElementById("yr").textContent = new Date().getFullYear();

    function buildEmail(e){
      e.preventDefault();
      const name = document.getElementById("name").value.trim();
      const phone = document.getElementById("phone").value.trim();
      const service = document.getElementById("service").value.trim();
      const address = document.getElementById("address").value.trim();
      const details = document.getElementById("details").value.trim();

      const subject = encodeURIComponent(`Roadside Request: ${service} — ${name}`);
      const body = encodeURIComponent(
        `Name: ${name}\nPhone: ${phone}\nService: ${service}\nLocation: ${address}\nDetails: ${details}\n\nPlease reply with ETA + total price before dispatch.`
      );

      // Replace with your business email if you want mailto to go to you:
      const yourEmail = "youremail@example.com";
      window.location.href = `mailto:${yourEmail}?subject=${subject}&body=${body}`;
      return false;
    }
    window.buildEmail = buildEmail;
  </script>

</body>
</html>
