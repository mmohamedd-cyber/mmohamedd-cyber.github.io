

<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<title>Homework – Bearings (with Hover Answers)</title>

<style>
:root{
  --blue:#0b2d5c;
  --blue2:#123a73;
  --gold:#d8b24c;
}
*{box-sizing:border-box}
body{
  margin:0;
  background:#111;
  font-family:"Segoe UI",Arial,sans-serif;
  display:flex;
  justify-content:center;
  padding:24px;
}
.page{
  width:1200px;
  background:#fff;
  border-radius:18px;
  box-shadow:0 14px 50px rgba(0,0,0,.35);
  overflow:hidden;
}
.topbar{
  height:14px;
  background:linear-gradient(90deg,var(--blue),var(--blue2),var(--gold));
}
header{
  padding:18px 26px;
  border-bottom:2px solid rgba(11,45,92,.15);
}
h1{
  margin:0;
  color:var(--blue);
  font-size:32px;
}
main{padding:22px}
.grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:16px;
}

/* QUESTION CARD */
.qcard{
  position:relative;
  border:2px solid rgba(11,45,92,.18);
  border-radius:16px;
  overflow:hidden;
}
.qhead{
  background:linear-gradient(90deg,var(--blue),var(--blue2));
  color:#fff;
  font-weight:900;
  padding:12px 14px;
  border-bottom:4px solid var(--gold);
}
.qbody{
  padding:14px;
}
.prompt{
  font-size:16px;
  margin-bottom:8px;
}

/* SVG */
svg{
  width:100%;
  height:220px;
  border:2px solid rgba(11,45,92,.12);
  border-radius:12px;
  background:#fff;
}
.s-axis{stroke:rgba(11,45,92,.2);stroke-width:2}
.s-ray{stroke:var(--blue);stroke-width:3;fill:none}
.s-arc{stroke:var(--gold);stroke-width:3;fill:none}
.s-dot{fill:var(--blue)}
.s-text{fill:var(--blue);font-weight:800;font-size:16px}
.s-angle{fill:var(--blue);font-weight:900;font-size:14px}

/* ANSWER OVERLAY */
.answer-reveal{
  position:absolute;
  inset:0;
  background:rgba(11,45,92,.92);
  color:#fff;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  font-size:26px;
  font-weight:900;
  letter-spacing:.5px;
  opacity:0;
  transition:opacity .25s ease;
  pointer-events:none;
}
.qcard:hover .answer-reveal{
  opacity:1;
}

/* Print safety */
@media print{
  .answer-reveal{display:none !important;}
  body{background:#fff;}
}
</style>
</head>

<body>
<div class="page">
<div class="topbar"></div>

<header>
<h1>Homework: Bearings</h1>
</header>

<main>
<div class="grid">

<!-- Q1 -->
<div class="qcard">
<div class="qhead">Q1</div>
<div class="qbody">
<div class="prompt"><b>Find the bearing of B from A.</b></div>
<svg viewBox="0 0 520 260">
  <defs>
    <marker id="m1" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto">
      <path d="M0,0 L10,3 L0,6 Z" fill="#0b2d5c"/>
    </marker>
  </defs>
  <line x1="260" y1="30" x2="260" y2="230" class="s-axis"/>
  <line x1="120" y1="130" x2="400" y2="130" class="s-axis"/>
  <text x="252" y="24" class="s-text">N</text>
  <circle cx="260" cy="130" r="5" class="s-dot"/>
  <text x="272" y="150" class="s-text">A</text>
  <line x1="260" y1="130" x2="350" y2="80" class="s-ray" marker-end="url(#m1)"/>
  <circle cx="350" cy="80" r="5" class="s-dot"/>
  <text x="362" y="85" class="s-text">B</text>
  <path d="M260 100 A30 30 0 0 1 282 112" class="s-arc"/>
  <text x="285" y="95" class="s-angle">40°</text>
</svg>
</div>
<div class="answer-reveal">Answer: <br>040°</div>
</div>

<!-- Q2 -->
<div class="qcard">
<div class="qhead">Q2</div>
<div class="qbody">
<div class="prompt"><b>Find the bearing of D from C.</b></div>
<svg viewBox="0 0 520 260">
  <defs>
    <marker id="m2" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto">
      <path d="M0,0 L10,3 L0,6 Z" fill="#0b2d5c"/>
    </marker>
  </defs>
  <line x1="260" y1="30" x2="260" y2="230" class="s-axis"/>
  <line x1="120" y1="130" x2="400" y2="130" class="s-axis"/>
  <text x="252" y="24" class="s-text">N</text>
  <circle cx="260" cy="130" r="5" class="s-dot"/>
  <text x="272" y="150" class="s-text">C</text>
  <line x1="260" y1="130" x2="340" y2="210" class="s-ray" marker-end="url(#m2)"/>
  <circle cx="340" cy="210" r="5" class="s-dot"/>
  <text x="352" y="215" class="s-text">D</text>
  <path d="M260 100 A34 34 0 0 1 292 162" class="s-arc"/>
  <text x="300" y="150" class="s-angle">135°</text>
</svg>
</div>
<div class="answer-reveal">Answer: <br>135°</div>
</div>

<!-- Q3 -->
<div class="qcard">
<div class="qhead">Q3</div>
<div class="qbody">
<div class="prompt"><b>The bearing of F from E is 070°. Find the bearing of E from F.</b></div>
</div>
<div class="answer-reveal">Answer: <br>250°</div>
</div>

<!-- Q4 -->
<div class="qcard">
<div class="qhead">Q4</div>
<div class="qbody">
<div class="prompt"><b>The bearing of H from G is 210°. Find the bearing of G from H.</b></div>
</div>
<div class="answer-reveal">Answer: <br>030°</div>
</div>

<!-- Q5 -->
<div class="qcard">
<div class="qhead">Q5</div>
<div class="qbody">
<div class="prompt"><b>From Q, find the bearing of R.</b></div>
</div>
<div class="answer-reveal">Answer: <br>150°</div>
</div>

<!-- Q6 -->
<div class="qcard">
<div class="qhead">Q6</div>
<div class="qbody">
<div class="prompt"><b>Find the bearing of C from A.</b></div>
</div>
<div class="answer-reveal">Answer: <br>070°</div>
</div>

</div>
</main>
</div>
</body>
</html>
