<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Telephone Society — Partner Overview</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }

:root {
–cyan: #2a9d9d;
–cyan-light: #4FC3C3;
–black: #080c10;
–white: #f0f4f8;
–gray: #6b7a87;
–rule: #1a2535;
–bg: #070d14;
–subtle: #0d1520;
}

body {
background: var(–bg);
color: var(–white);
font-family: ‘DM Sans’, sans-serif;
font-weight: 300;
max-width: 680px;
margin: 0 auto;
padding: 0 24px 80px;
}

/* HEADER */
.header {
display: flex;
justify-content: space-between;
align-items: center;
padding: 32px 0 20px;
border-bottom: 1px solid #1a2535;
margin-bottom: 48px;
}

.brand {
display: flex;
align-items: center;
gap: 8px;
}

.brand-dot {
width: 6px;
height: 6px;
border-radius: 50%;
background: var(–cyan);
}

.brand-name {
font-size: 10px;
font-weight: 500;
letter-spacing: 0.22em;
text-transform: uppercase;
color: var(–white);
}

.doc-tag {
font-size: 9px;
letter-spacing: 0.2em;
text-transform: uppercase;
color: var(–gray);
}

/* OPENING */
.opening {
margin-bottom: 48px;
}

.opening h1 {
font-family: ‘Cormorant Garamond’, serif;
font-weight: 300;
font-size: clamp(32px, 6vw, 48px);
line-height: 1.1;
letter-spacing: -0.02em;
color: var(–white);
margin-bottom: 20px;
}

.opening h1 em {
font-style: italic;
color: var(–cyan);
display: block;
}

.opening p {
font-size: 15px;
line-height: 1.8;
color: var(–gray);
max-width: 520px;
}

/* DIVIDER */
.divider {
width: 36px;
height: 2px;
background: var(–cyan);
margin: 48px 0;
}

/* SECTION LABEL */
.label {
font-size: 9px;
letter-spacing: 0.3em;
text-transform: uppercase;
color: var(–cyan);
margin-bottom: 24px;
font-weight: 400;
}

/* TRUTHS */
.truths {
margin-bottom: 48px;
}

.truth-grid {
display: grid;
grid-template-columns: 1fr 1fr 1fr;
gap: 2px;
background: var(–rule);
}

.truth-item {
background: var(–subtle);
padding: 24px 20px;
}

.truth-num {
font-family: ‘Cormorant Garamond’, serif;
font-size: 28px;
font-weight: 300;
color: var(–cyan);
line-height: 1;
margin-bottom: 8px;
display: block;
}

.truth-title {
font-size: 11px;
font-weight: 500;
letter-spacing: 0.1em;
text-transform: uppercase;
color: var(–white);
margin-bottom: 8px;
}

.truth-body {
font-size: 12px;
line-height: 1.65;
color: var(–gray);
}

/* HOW IT WORKS */
.how {
margin-bottom: 48px;
}

.steps {
border-top: 1px solid var(–rule);
}

.step {
display: flex;
gap: 20px;
align-items: flex-start;
padding: 20px 0;
border-bottom: 1px solid var(–rule);
}

.step-num {
font-family: ‘Cormorant Garamond’, serif;
font-size: 13px;
color: var(–cyan);
letter-spacing: 0.1em;
min-width: 20px;
padding-top: 1px;
flex-shrink: 0;
}

.step-title {
font-size: 13px;
font-weight: 500;
color: var(–white);
margin-bottom: 4px;
}

.step-desc {
font-size: 12px;
color: var(–gray);
line-height: 1.6;
}

/* SKETCH */
.sketch {
margin-bottom: 48px;
}

.sketch-placeholder {
background: var(–subtle);
border: 1px solid var(–rule);
border-radius: 4px;
padding: 48px 24px;
text-align: center;
}

.sketch-placeholder p {
font-size: 12px;
color: var(–gray);
font-style: italic;
}

/* COST */
.cost {
margin-bottom: 48px;
}

.cost-headline {
font-family: ‘Cormorant Garamond’, serif;
font-size: 36px;
font-weight: 300;
line-height: 1.15;
color: var(–white);
margin-bottom: 14px;
}

.cost-body {
font-size: 13px;
line-height: 1.8;
color: var(–gray);
max-width: 480px;
}

/* PROMISE */
.promise {
border-left: 3px solid var(–cyan);
padding: 24px 28px;
margin-bottom: 48px;
background: var(–subtle);
}

.promise-text {
font-family: ‘Cormorant Garamond’, serif;
font-size: 20px;
font-weight: 300;
font-style: italic;
line-height: 1.55;
color: var(–white);
margin-bottom: 12px;
}

.promise-attr {
font-size: 9px;
letter-spacing: 0.2em;
text-transform: uppercase;
color: var(–cyan);
}

/* ASK */
.ask {
margin-bottom: 48px;
}

.ask h2 {
font-family: ‘Cormorant Garamond’, serif;
font-size: 32px;
font-weight: 300;
color: var(–white);
margin-bottom: 12px;
line-height: 1.2;
}

.ask p {
font-size: 13px;
line-height: 1.8;
color: var(–gray);
max-width: 440px;
}

/* FOOTER */
.footer {
border-top: 1px solid #f0f4f8;
padding-top: 28px;
display: flex;
justify-content: space-between;
align-items: flex-end;
flex-wrap: wrap;
gap: 20px;
}

.footer-brand {
font-family: ‘Cormorant Garamond’, serif;
font-size: 14px;
font-weight: 500;
letter-spacing: 0.12em;
text-transform: uppercase;
color: var(–cyan);
margin-bottom: 4px;
}

.footer-tagline {
font-size: 10px;
color: var(–gray);
letter-spacing: 0.06em;
}

.footer-contact {
text-align: right;
}

.footer-name {
font-size: 12px;
font-weight: 500;
color: var(–white);
margin-bottom: 2px;
}

.footer-title {
font-size: 9px;
letter-spacing: 0.12em;
text-transform: uppercase;
color: var(–cyan);
margin-bottom: 6px;
}

.footer-info {
font-size: 11px;
color: var(–gray);
line-height: 1.8;
}

.footer-info a {
color: #7a8694;
text-decoration: none;
}

/* RESPONSIVE */
@media (max-width: 520px) {
.truth-grid { grid-template-columns: 1fr; }
.footer { flex-direction: column; }
.footer-contact { text-align: left; }
}
</style>

</head>
<body>

  <header class="header">
    <div class="brand">
      <div class="brand-dot"></div>
      <div class="brand-name">The Telephone Society</div>
    </div>
    <div class="doc-tag">Partner Overview</div>
  </header>

  <section class="opening">
    <h1>
      Your guests chose to be here.
      <em>That choice has value.</em>
    </h1>
    <p>Every person who walks through your door made a choice. They chose your venue over every other option available to them. We believe that choice deserves to be honored — and that honoring it creates something most loyalty programs never do: guests who feel genuinely seen, not just rewarded.</p>
  </section>

  <div class="divider"></div>

  <section class="truths">
    <div class="label">What this does for you</div>
    <div class="truth-grid">
      <div class="truth-item">
        <span class="truth-num">01</span>
        <div class="truth-title">Repeat Visits</div>
        <div class="truth-body">People come back to places that made them feel something. Not because of points — because someone noticed they were there.</div>
      </div>
      <div class="truth-item">
        <span class="truth-num">02</span>
        <div class="truth-title">Higher Spend</div>
        <div class="truth-body">A gesture creates goodwill. Goodwill creates additional purchases. When people feel valued they stay longer and spend more.</div>
      </div>
      <div class="truth-item">
        <span class="truth-num">03</span>
        <div class="truth-title">Guest Retention</div>
        <div class="truth-body">The guests most likely to walk out — the ones waiting, the ones on the fence — stay. Because their time is being recognized not ignored.</div>
      </div>
    </div>
  </section>

  <section class="how">
    <div class="label">How it works</div>
    <div class="steps">
      <div class="step">
        <div class="step-num">I</div>
        <div>
          <div class="step-title">A sign is placed at your point of entry</div>
          <div class="step-desc">Printed. Premium. One sentence. No explanation required.</div>
        </div>
      </div>
      <div class="step">
        <div class="step-num">II</div>
        <div>
          <div class="step-title">Your guest scans once</div>
          <div class="step-desc">Their phone receives a simple message. Their time here is recognized. Nothing collected. Nothing tracked. Just a moment honored.</div>
        </div>
      </div>
      <div class="step">
        <div class="step-num">III</div>
        <div>
          <div class="step-title">They speak with your team</div>
          <div class="step-desc">One gesture — entirely at your discretion. Per visit, not per transaction.</div>
        </div>
      </div>
      <div class="step">
        <div class="step-num">IV</div>
        <div>
          <div class="step-title">They stay. They spend more. They return.</div>
          <div class="step-desc">The network grows. Your business grows with it.</div>
        </div>
      </div>
    </div>
  </section>

  <section class="sketch">
    <div class="label">The experience visualized</div>
    <div class="sketch-placeholder">
      <p>[ Insert guest experience sketch diagram here ]</p>
    </div>
  </section>

  <section class="cost">
    <div class="label">What it costs you</div>
    <div class="cost-headline">One gesture.<br>Your choice.<br>Your terms.</div>
    <p class="cost-body">The house decides what. The house decides when. The house decides how often. We simply provide the moment that makes it worth remembering.</p>
  </section>

  <div class="promise">
    <div class="promise-text">"They chose to be here. We make sure they know it mattered. Nothing else does that."</div>
    <div class="promise-attr">— The Telephone Society</div>
  </div>

  <section class="ask">
    <div class="label">What we ask of you</div>
    <h2>Post the sign.<br>That's it.</h2>
    <p>No commitment beyond this conversation. Place the sign at your point of entry and let your guests tell you what it means to feel recognized.</p>
  </section>

  <footer class="footer">
    <div>
      <div class="footer-brand">The Telephone Society</div>
      <div class="footer-tagline">Your time creates value. We return it.</div>
    </div>
    <div class="footer-contact">
      <div class="footer-name">Nicholas Godinez</div>
      <div class="footer-title">Founder & CEO</div>
      <div class="footer-info">
        <a href="mailto:thetelephonesociety@gmail.com">thetelephonesociety@gmail.com</a><br>
        720.380.6352
      </div>
    </div>
  </footer>

</body>
</html>
