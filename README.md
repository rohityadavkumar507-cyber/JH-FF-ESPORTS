<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>JH FF Esports — Registration</title>
<style>
  :root{
    --bg:#0f0f10;
    --card:#161616;
    --muted:#a9a9a9;
    --accent:#f6c523; /* yellow */
    --accent-dark:#d2a41a;
    --input:#1f1f1f;
    --radius:14px;
    font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  }
  html,body{height:100%;}
  body{
    margin:0;
    background:linear-gradient(180deg,#0b0b0b 0%, #0f0f0f 100%);
    color:#eee;
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing:grayscale;
    padding:18px;
    display:flex;
    justify-content:center;
    align-items:flex-start;
    font-size:15px;
  }

  .container{
    width:100%;
    max-width:420px;
  }

  header{
    text-align:center;
    margin-bottom:14px;
  }
  .brand{
    font-weight:800;
    color:var(--accent);
    letter-spacing:0.8px;
    font-size:28px;
    margin-bottom:4px;
  }
  .subtitle{ color:var(--muted); font-weight:600; font-size:14px; }

  .card{
    background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border-radius:var(--radius);
    padding:20px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.6);
    margin-bottom:18px;
  }

  .section-title{
    color:var(--accent);
    font-weight:800;
    font-size:22px;
    margin-bottom:12px;
    text-align:center;
  }

  .info-grid{ display:grid; gap:10px; }

  .info-row{
    display:flex; gap:12px; align-items:flex-start;
  }
  .info-icon{
    width:36px; height:36px; border-radius:9px; display:flex; align-items:center; justify-content:center;
    background:rgba(255,255,255,0.02); color:var(--accent);
    flex-shrink:0; font-weight:700;
  }
  .info-body{ flex:1; }
  .info-label{ font-weight:700; color:#fff; margin-bottom:4px; }
  .info-text{ color:var(--muted); font-size:14px; }

  .prizes-list{ margin:8px 0 0 18px; color:var(--muted); }
  .prizes-list li{ margin:6px 0; }

  /* slots box */
  .slots{
    margin-top:12px;
    background:linear-gradient(180deg, rgba(246,197,35,0.08), rgba(246,197,35,0.04));
    padding:12px;
    border-radius:12px;
    display:flex;
    justify-content:space-between;
    gap:10px;
  }
  .slot-card{ flex:1; text-align:center; padding:10px 6px; border-radius:10px; }
  .slot-title{ font-weight:800; color:#111; background:transparent; }
  .slot-count{ color:#111; font-weight:700; margin-top:6px; opacity:0.85; }

  /* registration form */
  form{ margin-top:10px; }
  .form-card{ background:var(--card); border-radius:12px; padding:18px; }
  label{ display:block; font-weight:600; margin-bottom:6px; color:#fff; font-size:14px; }
  input[type="text"], input[type="tel"], input[type="file"]{
    width:100%; display:block; padding:12px 14px; border-radius:12px; border: none;
    background:var(--input); color:#fff; outline: none; box-sizing:border-box;
    margin-bottom:14px; font-size:14px;
  }
  input[type="file"]{ padding:10px; }
  .muted{ color:var(--muted); font-size:13px; margin-top:-10px; margin-bottom:12px; }

  .radios{ display:flex; flex-direction:column; gap:8px; margin-bottom:14px; }
  .radio-row{ display:flex; gap:10px; align-items:center; }
  .radio-circle{
    width:18px; height:18px; border-radius:50%; border:2px solid var(--accent);
    display:inline-block; position:relative; box-sizing:border-box;
  }
  .radio-circle.checked{ background:var(--accent); border-color:var(--accent-dark); }

  .payment-box{
    background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.01));
    padding:14px; border-radius:12px; text-align:center; margin-bottom:12px;
  }
  .qr-placeholder{
    width:100%; height:180px; border-radius:10px; display:flex; align-items:center; justify-content:center;
    background:linear-gradient(180deg,#0b0b0b,#151515); color:var(--muted); border:1px dashed rgba(255,255,255,0.03);
    margin-bottom:10px; font-size:14px;
  }
  .upi{ font-weight:700; color:#fff; margin-top:6px; }

  .submit-row{ text-align:center; margin-top:6px; }
  button.submit{
    background:linear-gradient(180deg,var(--accent),var(--accent-dark));
    border:none; color:#111; font-weight:800; padding:14px 18px; width:100%;
    border-radius:12px; font-size:16px; cursor:pointer; box-shadow:0 6px 20px rgba(210,164,26,0.12);
  }
  button.submit:active{ transform:translateY(1px); }

  .small-note{ color:var(--muted); font-size:13px; text-align:center; margin-top:8px; }

  /* responsive tweaks */
  @media (max-width:420px){
    body{ padding:12px; }
    .brand{ font-size:24px; }
    .section-title{ font-size:20px; }
  }
</style>
</head>
<body>
  <div class="container" role="main">
    <header>
      <div class="brand">JH FF ESPORTS</div>
      <div class="subtitle">Free Fire Tournament</div>
    </header>

    <section class="card" aria-labelledby="tournament-info">
      <h2 id="tournament-info" class="section-title">Tournament Information</h2>

      <div class="info-grid">
        <div class="info-row">
          <div class="info-icon">📅</div>
          <div class="info-body">
            <div class="info-label">Date:</div>
            <div class="info-text">September 28, 2025</div>
          </div>
        </div>

        <div class="info-row">
          <div class="info-icon">⏰</div>
          <div class="info-body">
            <div class="info-label">Time:</div>
            <div class="info-text">1st Match: 12 PM<br>2nd Match: 6 PM</div>
          </div>
        </div>

        <div class="info-row">
          <div class="info-icon">👥</div>
          <div class="info-body">
            <div class="info-label">Total Players:</div>
            <div class="info-text">48 (12 Squads × 4 Players)</div>
          </div>
        </div>

        <div class="info-row">
          <div class="info-icon">₹</div>
          <div class="info-body">
            <div class="info-label">Entry Fee:</div>
            <div class="info-text">₹120 per Squad</div>
          </div>
        </div>

        <div class="info-row">
          <div class="info-icon">🚫</div>
          <div class="info-body">
            <div class="info-label">Rule:</div>
            <div class="info-text">No hackers allowed</div>
          </div>
        </div>

        <div class="info-row">
          <div class="info-icon">🗺️</div>
          <div class="info-body">
            <div class="info-label">Map:</div>
            <div class="info-text">Bermuda</div>
          </div>
        </div>

        <div>
          <div class="info-label" style="margin-left:4px; margin-top:8px;">🏆 Prizes:</div>
          <ul class="prizes-list">
            <li>1st Prize: ₹700</li>
            <li>2nd Prize: ₹500</li>
            <li>3rd Prize: ₹300</li>
          </ul>
        </div>

        <div class="slots" aria-hidden="false">
          <div class="slot-card">
            <div class="slot-title">12:00 PM<br><small style="font-weight:600; color:#111; opacity:0.9">Slots</small></div>
            <div id="slot12" class="slot-count">0 / 12</div>
          </div>
          <div class="slot-card">
            <div class="slot-title">06:00 PM<br><small style="font-weight:600; color:#111; opacity:0.9">Slots</small></div>
            <div id="slot18" class="slot-count">0 / 12</div>
          </div>
        </div>

        <div class="small-note">Custom ID and password will be sent via WhatsApp 10 minutes before the tournament.</div>
      </div>
    </section>

    <form id="registrationForm" class="form-card" onsubmit="return onSubmit(event)" novalidate>
      <h3 class="section-title" style="font-size:20px; margin-top:0; margin-bottom:8px;">Registration Form</h3>

      <label for="squad">Squad Name</label>
      <input id="squad" name="squad" type="text" placeholder="Enter squad name" required>

      <label for="p1">Player 1 FF UID</label>
      <input id="p1" name="player1" type="text" placeholder="Player 1 UID" required>

      <label for="p2">Player 2 FF UID</label>
      <input id="p2" name="player2" type="text" placeholder="Player 2 UID" required>

      <label for="p3">Player 3 FF UID</label>
      <input id="p3" name="player3" type="text" placeholder="Player 3 UID" required>

      <label for="p4">Player 4 FF UID</label>
      <input id="p4" name="player4" type="text" placeholder="Player 4 UID" required>

      <label for="sub">Substitute Player FF UID (Optional)</label>
      <input id="sub" name="substitute" type="text" placeholder="Sub UID (optional)">

      <label for="whatsapp">WhatsApp Number</label>
      <input id="whatsapp" name="whatsapp" type="tel" placeholder="+91 9xxxxxxxxx" required>
      <div class="muted">We'll send match details to this number.</div>

      <div style="margin-bottom:6px; font-weight:700; color:#fff;">Select Match Time</div>
      <div class="radios" role="radiogroup" aria-label="Select Match Time">
        <label class="radio-row" style="cursor:pointer" onclick="selectTime('12')">
          <span id="r12" class="radio-circle" aria-hidden="true"></span>
          <input id="time12" name="matchTime" type="radio" value="12" style="display:none" required>
          <span style="color:var(--muted); margin-left:6px;">12:00 PM</span>
        </label>
        <label class="radio-row" style="cursor:pointer" onclick="selectTime('18')">
          <span id="r18" class="radio-circle" aria-hidden="true"></span>
          <input id="time18" name="matchTime" type="radio" value="18" style="display:none">
          <span style="color:var(--muted); margin-left:6px;">06:00 PM</span>
        </label>
      </div>

      <div style="font-weight:700; color:#fff; margin-bottom:8px;">Payment</div>
      <div class="payment-box">
        <div class="qr-placeholder" aria-hidden="true">
          Payment QR Code (placeholder)
        </div>
        <div class="muted">Scan the QR code to pay the entry fee.</div>
        <div class="upi">UPI ID: <span style="font-weight:800">8340139152@fam</span></div>
      </div>

      <label for="screenshot">Payment Screenshot</label>
      <input id="screenshot" name="screenshot" type="file" accept="image/*" required>

      <div class="submit-row">
        <button type="submit" class="submit">Submit Registration</button>
      </div>
      <div class="small-note">By submitting you agree to the tournament rules. We will confirm by WhatsApp after payment verification.</div>
    </form>
  </div>

<script>
  // Simple slot counters and radio visual toggling
  // Initially both 0/12. In a real app these would come from server.
  const maxSlots = 12;
  let slotCounts = { '12': 0, '18': 0 };

  const el12 = document.getElementById('slot12');
  const el18 = document.getElementById('slot18');
  const r12 = document.getElementById('r12');
  const r18 = document.getElementById('r18');

  function updateSlots() {
    el12.textContent = slotCounts['12'] + ' / ' + maxSlots;
    el18.textContent = slotCounts['18'] + ' / ' + maxSlots;
  }
  updateSlots();

  function selectTime(t) {
    // update hidden radio inputs
    document.getElementById('time12').checked = (t === '12');
    document.getElementById('time18').checked = (t === '18');

    // visual toggle
    r12.classList.toggle('checked', t === '12');
    r18.classList.toggle('checked', t === '18');
  }

  // on submit: basic client-side checks, increment slot if available
  function onSubmit(e) {
    e.preventDefault();
    const form = document.getElementById('registrationForm');
    // use HTML5 validity
    if (!form.checkValidity()) {
      form.reportValidity();
      return false;
    }
    const chosen = document.querySelector('input[name="matchTime"]:checked');
    if (!chosen) {
      alert('Please select a match time.');
      return false;
    }
    const t = chosen.value;
    if (slotCounts[t] >= maxSlots) {
      alert('Sorry, the selected slot is full. Please choose another time.');
      return false;
    }

    // Here you'd normally send the form to your server and verify payment.
    // We'll simulate a successful registration & increment slot count.
    slotCounts[t] += 1;
    updateSlots();

    // Simple success feedback
    alert('Registration submitted! We will verify payment and confirm via WhatsApp.');
    form.reset();
    r12.classList.remove('checked');
    r18.classList.remove('checked');
    return false;
  }
</script>
</body>
</html>
