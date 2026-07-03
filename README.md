<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Priyanka Asthana — Constrained AI Systems / NLP Research</title>
<meta name="description" content="Priyanka Asthana — patented conversational medical AI, constrained LLM systems, RAG reliability research.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --void: #0a0e14;
  --panel: #10151e;
  --panel-2: #151c28;
  --line: #212a3a;
  --text: #e7edf5;
  --text-dim: #8b96a8;
  --teal: #5eead4;
  --violet: #a78bfa;
  --amber: #f0b429;
  --danger: #fb7185;
  --radius: 3px;
}

*{margin:0;padding:0;box-sizing:border-box;}

html{scroll-behavior:smooth;}

@media (prefers-reduced-motion: reduce){
  html{scroll-behavior:auto;}
  *{animation-duration:0.001ms !important; animation-iteration-count:1 !important; transition-duration:0.001ms !important;}
}

body{
  background:var(--void);
  color:var(--text);
  font-family:'Inter', sans-serif;
  line-height:1.6;
  overflow-x:hidden;
  background-image:
    linear-gradient(var(--line) 1px, transparent 1px),
    linear-gradient(90deg, var(--line) 1px, transparent 1px);
  background-size: 64px 64px;
  background-position: -1px -1px;
}

::selection{background:var(--violet); color:var(--void);}

a{color:inherit; text-decoration:none;}

.mono{font-family:'IBM Plex Mono', monospace;}
.display{font-family:'Space Grotesk', sans-serif;}

/* ---------- layout shell ---------- */
.wrap{
  max-width:1100px;
  margin:0 auto;
  padding:0 32px;
}

/* ---------- nav ---------- */
.nav{
  position:fixed;
  top:0; left:0; right:0;
  z-index:100;
  background:rgba(10,14,20,0.82);
  backdrop-filter:blur(10px);
  border-bottom:1px solid var(--line);
}
.nav-inner{
  max-width:1100px;
  margin:0 auto;
  padding:0 32px;
  height:56px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}
.nav-id{
  display:flex;
  align-items:center;
  gap:10px;
  font-size:13px;
  letter-spacing:0.02em;
}
.status-dot{
  width:7px; height:7px;
  border-radius:50%;
  background:var(--teal);
  box-shadow:0 0 8px var(--teal);
  animation:pulse-dot 2.4s ease-in-out infinite;
}
@keyframes pulse-dot{
  0%,100%{opacity:1;}
  50%{opacity:0.35;}
}
.nav-links{
  display:flex;
  gap:28px;
  font-size:12px;
  letter-spacing:0.06em;
  color:var(--text-dim);
}
.nav-links a{transition:color 0.2s;}
.nav-links a:hover{color:var(--teal);}
.nav-links span{color:var(--violet); margin-right:4px;}
@media (max-width:720px){ .nav-links{display:none;} }

/* ---------- hero ---------- */
.hero{
  position:relative;
  min-height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  padding-top:56px;
  overflow:hidden;
}
#node-canvas{
  position:absolute;
  inset:0;
  width:100%; height:100%;
  opacity:0.9;
}
.hero-fade{
  position:absolute;
  inset:0;
  background:linear-gradient(180deg, rgba(10,14,20,0.15) 0%, rgba(10,14,20,0.55) 55%, var(--void) 100%);
  pointer-events:none;
}
.hero-content{
  position:relative;
  z-index:2;
}
.eyebrow{
  font-size:12px;
  letter-spacing:0.14em;
  color:var(--teal);
  text-transform:uppercase;
  display:flex;
  align-items:center;
  gap:10px;
  margin-bottom:22px;
}
.eyebrow::before{
  content:'';
  width:22px; height:1px;
  background:var(--teal);
}
h1.name{
  font-size:clamp(42px, 8vw, 88px);
  font-weight:700;
  line-height:0.98;
  letter-spacing:-0.02em;
  margin-bottom:18px;
}
h1.name .last{color:var(--text-dim); font-weight:500;}
.typewrap{
  font-size:clamp(16px, 2.4vw, 22px);
  color:var(--violet);
  min-height:34px;
  margin-bottom:26px;
  display:flex;
  align-items:center;
}
.typewrap .cursor{
  display:inline-block;
  width:9px; height:1.1em;
  background:var(--violet);
  margin-left:4px;
  animation:blink 1s step-end infinite;
}
@keyframes blink{ 50%{opacity:0;} }
.hero-desc{
  max-width:560px;
  color:var(--text-dim);
  font-size:16px;
  margin-bottom:38px;
}
.hero-desc strong{color:var(--text); font-weight:500;}
.hero-ctas{
  display:flex;
  gap:14px;
  flex-wrap:wrap;
  margin-bottom:64px;
}
.btn{
  font-family:'IBM Plex Mono', monospace;
  font-size:13px;
  padding:12px 20px;
  border-radius:var(--radius);
  border:1px solid var(--line);
  transition:all 0.2s ease;
  display:inline-flex;
  align-items:center;
  gap:8px;
}
.btn-primary{
  background:var(--teal);
  color:var(--void);
  border-color:var(--teal);
  font-weight:600;
}
.btn-primary:hover{background:#7ff2e0; transform:translateY(-1px);}
.btn-ghost{color:var(--text); }
.btn-ghost:hover{border-color:var(--violet); color:var(--violet); transform:translateY(-1px);}

.annotation{
  font-size:12px;
  color:var(--text-dim);
  max-width:340px;
  border-left:2px solid var(--amber);
  padding-left:14px;
}
.annotation .tag{
  color:var(--amber);
  font-weight:600;
}
.annotation .tag2{
  color:var(--teal);
  font-weight:600;
}

.scroll-cue{
  position:absolute;
  bottom:28px;
  left:32px;
  font-size:11px;
  letter-spacing:0.08em;
  color:var(--text-dim);
  display:flex;
  align-items:center;
  gap:8px;
  z-index:2;
}
.scroll-cue .bar{
  width:1px; height:28px;
  background:linear-gradient(var(--text-dim), transparent);
  animation:scrolldown 1.8s ease-in-out infinite;
}
@keyframes scrolldown{
  0%{transform:scaleY(0); transform-origin:top;}
  50%{transform:scaleY(1); transform-origin:top;}
  51%{transform-origin:bottom;}
  100%{transform:scaleY(0); transform-origin:bottom;}
}

/* ---------- sections general ---------- */
section{
  position:relative;
  padding:120px 0;
  border-top:1px solid var(--line);
}
.sec-head{
  display:flex;
  align-items:baseline;
  gap:16px;
  margin-bottom:56px;
}
.sec-num{
  font-family:'IBM Plex Mono', monospace;
  font-size:13px;
  color:var(--violet);
}
.sec-title{
  font-family:'Space Grotesk', sans-serif;
  font-size:clamp(26px, 4vw, 38px);
  font-weight:600;
}
.sec-sub{
  color:var(--text-dim);
  max-width:600px;
  margin-top:-32px;
  margin-bottom:48px;
  font-size:15px;
}

.reveal{
  opacity:0;
  transform:translateY(28px);
  transition:opacity 0.7s ease, transform 0.7s ease;
}
.reveal.is-visible{
  opacity:1;
  transform:translateY(0);
}

/* ---------- incident report ---------- */
.log-panel{
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:var(--radius);
  padding:36px;
  position:relative;
}
.log-panel::before{
  content:'case_history.log';
  position:absolute;
  top:-11px; left:20px;
  background:var(--void);
  padding:0 8px;
  font-family:'IBM Plex Mono', monospace;
  font-size:11px;
  color:var(--text-dim);
}
.log-line{
  font-family:'IBM Plex Mono', monospace;
  font-size:13.5px;
  color:var(--text-dim);
  margin-bottom:14px;
  padding-left:20px;
  position:relative;
}
.log-line::before{
  content:'>';
  position:absolute;
  left:0;
  color:var(--violet);
}
.log-line.flag{color:var(--danger);}
.log-line.flag::before{content:'!'; color:var(--danger);}
.log-line.fix{color:var(--teal);}
.log-line.fix::before{content:'✓'; color:var(--teal);}
.log-body{
  margin-top:20px;
  padding-top:20px;
  border-top:1px solid var(--line);
  color:var(--text);
  font-size:16px;
  max-width:680px;
}
.log-body strong{color:var(--teal);}

/* ---------- case files (projects) ---------- */
.case{
  border:1px solid var(--line);
  border-radius:var(--radius);
  background:var(--panel);
  margin-bottom:24px;
  overflow:hidden;
  transition:border-color 0.3s ease, transform 0.3s ease;
}
.case:hover{border-color:var(--violet); transform:translateY(-2px);}
.case-head{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:22px 28px;
  border-bottom:1px solid var(--line);
  cursor:default;
  flex-wrap:wrap;
  gap:10px;
}
.case-id{
  font-family:'IBM Plex Mono', monospace;
  font-size:12px;
  color:var(--violet);
  letter-spacing:0.05em;
}
.case-title{
  font-family:'Space Grotesk', sans-serif;
  font-size:22px;
  font-weight:600;
  margin-top:4px;
}
.case-links{
  display:flex;
  gap:16px;
  font-family:'IBM Plex Mono', monospace;
  font-size:12px;
  color:var(--text-dim);
}
.case-links a:hover{color:var(--teal);}
.case-body{
  padding:28px;
  display:grid;
  grid-template-columns:1.3fr 1fr;
  gap:36px;
}
@media (max-width:760px){ .case-body{grid-template-columns:1fr;} }

.case-field{margin-bottom:18px;}
.case-field:last-child{margin-bottom:0;}
.case-field .fl{
  font-family:'IBM Plex Mono', monospace;
  font-size:10.5px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  color:var(--text-dim);
  margin-bottom:6px;
}
.case-field p{font-size:14.5px; color:var(--text);}

.vitals{display:flex; flex-direction:column; gap:16px;}
.vital{}
.vital-top{
  display:flex;
  justify-content:space-between;
  font-family:'IBM Plex Mono', monospace;
  font-size:12px;
  margin-bottom:6px;
}
.vital-top .num{color:var(--teal); font-weight:600;}
.vital-track{
  height:5px;
  background:var(--panel-2);
  border-radius:4px;
  overflow:hidden;
  border:1px solid var(--line);
}
.vital-fill{
  height:100%;
  width:0%;
  background:linear-gradient(90deg, var(--violet), var(--teal));
  border-radius:4px;
  transition:width 1.4s cubic-bezier(.16,1,.3,1);
}
.case.is-visible .vital-fill{ }

.stack{
  display:flex;
  flex-wrap:wrap;
  gap:8px;
  margin-top:16px;
}
.chip{
  font-family:'IBM Plex Mono', monospace;
  font-size:11px;
  padding:5px 10px;
  border:1px solid var(--line);
  border-radius:20px;
  color:var(--text-dim);
}

/* ---------- research/IP ---------- */
.ip-grid{
  display:grid;
  grid-template-columns:repeat(3, 1fr);
  gap:20px;
}
@media (max-width:820px){ .ip-grid{grid-template-columns:1fr;} }
.ip-card{
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:var(--radius);
  padding:26px;
  transition:border-color 0.3s, transform 0.3s;
}
.ip-card:hover{border-color:var(--amber); transform:translateY(-3px);}
.ip-kind{
  font-family:'IBM Plex Mono', monospace;
  font-size:10.5px;
  letter-spacing:0.1em;
  color:var(--amber);
  text-transform:uppercase;
  margin-bottom:14px;
}
.ip-card h3{
  font-family:'Space Grotesk', sans-serif;
  font-size:17px;
  font-weight:600;
  margin-bottom:10px;
  line-height:1.3;
}
.ip-card p{font-size:13px; color:var(--text-dim); margin-bottom:14px;}
.ip-card .ref{
  font-family:'IBM Plex Mono', monospace;
  font-size:11.5px;
  color:var(--teal);
}

/* ---------- experience timeline ---------- */
.timeline{position:relative; padding-left:32px;}
.timeline::before{
  content:'';
  position:absolute;
  left:5px; top:6px; bottom:6px;
  width:1px;
  background:var(--line);
}
.tl-item{position:relative; margin-bottom:44px;}
.tl-item:last-child{margin-bottom:0;}
.tl-item::before{
  content:'';
  position:absolute;
  left:-32px; top:5px;
  width:11px; height:11px;
  border-radius:50%;
  background:var(--void);
  border:2px solid var(--violet);
}
.tl-when{
  font-family:'IBM Plex Mono', monospace;
  font-size:11.5px;
  color:var(--text-dim);
  margin-bottom:6px;
}
.tl-role{
  font-family:'Space Grotesk', sans-serif;
  font-size:19px;
  font-weight:600;
  margin-bottom:4px;
}
.tl-where{color:var(--teal); font-size:13.5px; margin-bottom:12px;}
.tl-item ul{padding-left:18px; color:var(--text-dim); font-size:14px;}
.tl-item li{margin-bottom:6px;}

/* ---------- skills ---------- */
.skill-grid{
  display:grid;
  grid-template-columns:repeat(3, 1fr);
  gap:1px;
  background:var(--line);
  border:1px solid var(--line);
  border-radius:var(--radius);
  overflow:hidden;
}
@media (max-width:820px){ .skill-grid{grid-template-columns:1fr;} }
.skill-col{
  background:var(--panel);
  padding:26px;
}
.skill-col h4{
  font-family:'IBM Plex Mono', monospace;
  font-size:11px;
  letter-spacing:0.08em;
  text-transform:uppercase;
  color:var(--violet);
  margin-bottom:16px;
}
.skill-col ul{list-style:none;}
.skill-col li{
  font-size:13.5px;
  color:var(--text-dim);
  padding:6px 0;
  border-bottom:1px dashed var(--line);
}
.skill-col li:last-child{border-bottom:none;}

/* ---------- awards ---------- */
.award-row{
  display:flex;
  justify-content:space-between;
  align-items:flex-start;
  padding:22px 0;
  border-bottom:1px solid var(--line);
  gap:20px;
  flex-wrap:wrap;
}
.award-row:first-child{padding-top:0;}
.award-row:last-child{border-bottom:none;}
.award-name{
  font-family:'Space Grotesk', sans-serif;
  font-size:18px;
  font-weight:600;
}
.award-org{color:var(--text-dim); font-size:13.5px; margin-top:4px;}
.award-when{
  font-family:'IBM Plex Mono', monospace;
  font-size:12px;
  color:var(--amber);
  white-space:nowrap;
}

/* ---------- footer / contact ---------- */
.contact{
  text-align:center;
  padding:140px 0 80px;
}
.contact .sec-num{display:block; margin-bottom:18px;}
.contact h2{
  font-family:'Space Grotesk', sans-serif;
  font-size:clamp(30px, 6vw, 54px);
  font-weight:700;
  margin-bottom:20px;
}
.contact p{color:var(--text-dim); max-width:480px; margin:0 auto 40px;}
.contact-links{
  display:flex;
  justify-content:center;
  gap:16px;
  flex-wrap:wrap;
}
footer{
  text-align:center;
  padding:30px 0 60px;
  font-family:'IBM Plex Mono', monospace;
  font-size:11.5px;
  color:var(--text-dim);
}
</style>
</head>
<body>

<nav class="nav">
  <div class="nav-inner">
    <div class="nav-id mono">
      <span class="status-dot"></span> PRIYANKA_ASTHANA.SYS
    </div>
    <div class="nav-links mono">
      <a href="#incident"><span>01</span>Origin</a>
      <a href="#cases"><span>02</span>Case Files</a>
      <a href="#research"><span>03</span>Research &amp; IP</a>
      <a href="#experience"><span>04</span>Experience</a>
      <a href="#skills"><span>05</span>Stack</a>
      <a href="#contact"><span>06</span>Contact</a>
    </div>
  </div>
</nav>

<header class="hero">
  <canvas id="node-canvas"></canvas>
  <div class="hero-fade"></div>
  <div class="wrap hero-content">
    <div class="eyebrow mono">case_history.log — status: open</div>
    <h1 class="name display">Priyanka <span class="last">Asthana</span></h1>
    <div class="typewrap mono"><span id="typed"></span><span class="cursor"></span></div>
    <p class="hero-desc">
      I build systems that route symptoms, retrieve culture, and allocate blood under scarcity —
      then I spend most of my time trying to make them <strong>fail safely</strong> instead of confidently.
      Patent holder. Two papers under review at Springer Nature. Cambridge ERA:AI Fellowship finalist.
    </p>
    <div class="hero-ctas">
      <a class="btn btn-primary" href="#cases">View case files ↓</a>
      <a class="btn btn-ghost mono" href="mailto:asthanapriyanka829@gmail.com">Email</a>
      <a class="btn btn-ghost mono" href="https://www.linkedin.com/in/priyanka-asthana-1b9a74250" target="_blank" rel="noopener">LinkedIn</a>
      <a class="btn btn-ghost mono" href="https://github.com/PriyankaAsthana" target="_blank" rel="noopener">GitHub</a>
    </div>
    <div class="annotation mono">
      <span class="tag">flagged:</span> ungrounded token drifting from the answer cluster —
      <span class="tag2">constraint layer</span> pulls it back before generation completes.
      This is what DiagnoseAI does to every clinical response.
    </div>
  </div>
  <div class="scroll-cue mono"><div class="bar"></div>SCROLL</div>
</header>

<section id="incident">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">01</span>
      <h2 class="sec-title">The failure that redirected everything</h2>
    </div>
    <div class="log-panel reveal">
      <div class="log-line">14:32:01 — DiagnoseAI v0 returned symptom triage for simulated patient #217</div>
      <div class="log-line flag">14:32:01 — output: structurally valid, clinically dangerous</div>
      <div class="log-line">14:32:04 — root cause search initiated</div>
      <div class="log-line">14:41:52 — cause: model was confident and wrong, in a domain where that's the worst combination</div>
      <div class="log-line fix">14:52:10 — question changed from "does it work" to "why does it fail, and what does it take to actually fix that"</div>
      <div class="log-body">
        That single response is the reason every project since has a <strong>constraint layer</strong> in it somewhere —
        a routing step, a retrieval check, a token reservation, a benchmark against RAGAS metrics. I'm not chasing
        bigger models. I'm chasing the smaller, harder problem of knowing when a model shouldn't be trusted, and building
        the scaffolding that catches it before a person downstream does.
      </div>
    </div>
  </div>
</section>

<section id="cases">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">02</span>
      <h2 class="sec-title">Case files</h2>
    </div>
    <p class="sec-sub reveal">Three systems, three failure modes, three ways of catching them before they reach someone who needed the right answer.</p>

    <div class="case reveal">
      <div class="case-head">
        <div>
          <div class="case-id mono">CASE-001 · PATENTED, MAR 2026</div>
          <div class="case-title">DiagnoseAI</div>
        </div>
        <div class="case-links mono">
          <a href="https://diagnoseai-ai-medical-system.onrender.com/" target="_blank" rel="noopener">live ↗</a>
          <a href="https://github.com/PriyankaAsthana/DiagnoseAI---AI-MEDICAL-DIAGNOSIS-SYSTEM-" target="_blank" rel="noopener">code ↗</a>
        </div>
      </div>
      <div class="case-body">
        <div>
          <div class="case-field">
            <div class="fl">symptom</div>
            <p>Free-form patient speech needs to reach the right specialist agent without a wrong turn costing someone their diagnosis.</p>
          </div>
          <div class="case-field">
            <div class="fl">diagnosis</div>
            <p>Voice → semantic parsing → intent classification routes input to specialist agents (cardiology, dermatology, etc.) via LangChain orchestration, each constrained to its own clinical scope.</p>
          </div>
          <div class="case-field">
            <div class="fl">treatment</div>
            <p>A constraint layer sits between the LLM and the final report — the actual contribution isn't the model, it's what stops the model from improvising.</p>
          </div>
          <div class="stack">
            <span class="chip">Speech-to-Text</span><span class="chip">LangChain</span><span class="chip">Multi-Agent</span><span class="chip">Constrained LLM</span><span class="chip">Python</span>
          </div>
        </div>
        <div class="vitals">
          <div class="vital">
            <div class="vital-top"><span>disease detection accuracy</span><span class="num">92%</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="92"></div></div>
          </div>
          <div class="vital">
            <div class="vital-top"><span>simulated patient scenarios</span><span class="num">500+</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="88"></div></div>
          </div>
          <div class="vital">
            <div class="vital-top"><span>IP status</span><span class="num">Patent 202611012869</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="100"></div></div>
          </div>
        </div>
      </div>
    </div>

    <div class="case reveal">
      <div class="case-head">
        <div>
          <div class="case-id mono">CASE-002 · SPRINGER NATURE, UNDER REVIEW</div>
          <div class="case-title">RAKT</div>
        </div>
        <div class="case-links mono">
          <a href="https://github.com/PriyankaAsthana/RAKT_Blood_Bank_Management" target="_blank" rel="noopener">code ↗</a>
          <a href="https://doi.org/10.5281/zenodo.18149564" target="_blank" rel="noopener">preprint ↗</a>
        </div>
      </div>
      <div class="case-body">
        <div>
          <div class="case-field">
            <div class="fl">symptom</div>
            <p>Emergency blood units in transit could be concurrently reallocated by existing systems — a race condition with life-or-death stakes.</p>
          </div>
          <div class="case-field">
            <div class="fl">diagnosis</div>
            <p>K-means clustering on GPS coordinates with haversine distance, run against real inventory from e-Raktkosh, India's national blood transfusion portal.</p>
          </div>
          <div class="case-field">
            <div class="fl">treatment</div>
            <p>A time-bound token reservation mechanism — the same "don't let the system lie to itself" instinct as DiagnoseAI, applied to logistics instead of language.</p>
          </div>
          <div class="stack">
            <span class="chip">GeoAI</span><span class="chip">K-Means</span><span class="chip">Token Reservation</span><span class="chip">Python</span>
          </div>
        </div>
        <div class="vitals">
          <div class="vital">
            <div class="vital-top"><span>high-priority allocation</span><span class="num">100%</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="100"></div></div>
          </div>
          <div class="vital">
            <div class="vital-top"><span>distance reduction under scarcity</span><span class="num">6.6%</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="30"></div></div>
          </div>
        </div>
      </div>
    </div>

    <div class="case reveal">
      <div class="case-head">
        <div>
          <div class="case-id mono">CASE-003 · 1ST PLACE, ABHYUDAY'26</div>
          <div class="case-title">KashiVani</div>
        </div>
        <div class="case-links mono">
          <a href="https://kashivani.onrender.com/" target="_blank" rel="noopener">live ↗</a>
          <a href="https://doi.org/10.5281/zenodo.20399130" target="_blank" rel="noopener">preprint ↗</a>
        </div>
      </div>
      <div class="case-body">
        <div>
          <div class="case-field">
            <div class="fl">symptom</div>
            <p>A standard RAG pipeline over Varanasi's cultural heritage corpus kept confidently generating answers that weren't in the source material.</p>
          </div>
          <div class="case-field">
            <div class="fl">diagnosis</div>
            <p>Systematic benchmark of three embedding models (MiniLM, MPNet, multilingual MiniLM) against RAGAS metrics — faithfulness, answer relevancy, factual correctness — to find where retrieval was actually breaking.</p>
          </div>
          <div class="case-field">
            <div class="fl">treatment</div>
            <p>Model selection driven by measured semantic failure points, not defaults — FAISS retrieval tuned to what the RAGAS scores actually showed.</p>
          </div>
          <div class="stack">
            <span class="chip">RAG</span><span class="chip">FAISS</span><span class="chip">RAGAS</span><span class="chip">LangChain</span>
          </div>
        </div>
        <div class="vitals">
          <div class="vital">
            <div class="vital-top"><span>hallucination reduction vs. baseline</span><span class="num">40%</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="40"></div></div>
          </div>
          <div class="vital">
            <div class="vital-top"><span>result</span><span class="num">1st Place</span></div>
            <div class="vital-track"><div class="vital-fill" data-fill="100"></div></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="research">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">03</span>
      <h2 class="sec-title">Research &amp; IP</h2>
    </div>
    <div class="ip-grid reveal">
      <div class="ip-card">
        <div class="ip-kind">Patent — Published Mar 2026</div>
        <h3>AI-Driven Conversational Medical Voice Assistant</h3>
        <p>Multi-agent system routing patient symptom input to specialist agents via NLP intent classification. Stress-tested across 500 simulated scenarios at 92% detection accuracy.</p>
        <div class="ref">Indian Patent App. No. 202611012869</div>
      </div>
      <div class="ip-card">
        <div class="ip-kind">Paper — SN Computer Science</div>
        <h3>Embedding Model Selection for Domain-Specific RAG</h3>
        <p>Benchmark evaluation of three embedding models on an Indian cultural heritage corpus, scored on faithfulness, relevancy, and factual correctness.</p>
        <div class="ref">doi.org/10.5281/zenodo.20399130</div>
      </div>
      <div class="ip-card">
        <div class="ip-kind">Paper — J. Computational Social Science</div>
        <h3>Priority-Weighted Spatial Framework for Emergency Blood Allocation</h3>
        <p>GeoAI framework combining spatial clustering with time-bound token reservation for real-world resource allocation under scarcity.</p>
        <div class="ref">doi.org/10.5281/zenodo.18149564</div>
      </div>
    </div>
  </div>
</section>

<section id="experience">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">04</span>
      <h2 class="sec-title">Experience</h2>
    </div>
    <div class="timeline reveal">
      <div class="tl-item">
        <div class="tl-when mono">FEB 2026 — JUL 2026</div>
        <div class="tl-role">NLP Engineer Intern</div>
        <div class="tl-where">IIT BHU</div>
        <ul>
          <li>Built an NLP test automation pipeline for heritage-text systems, processing 1,000+ inputs for semantic accuracy validation.</li>
          <li>Diagnosed and resolved 20+ live parsing failures, improving pipeline reliability by 25% and documenting root-cause fixes for the senior engineering team.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-when mono">DEC 2025 — FEB 2026</div>
        <div class="tl-role">AI Research Intern</div>
        <div class="tl-where">Bharat Space Education Research Centre</div>
        <ul>
          <li>Applied ML to real-time sensor fusion across 5 experimental UAS modules in simulated space-mission environments.</li>
          <li>Contributed to a 20% reduction in trajectory-prediction / subsystem latency.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-when mono">JUL 2025 — SEP 2025</div>
        <div class="tl-role">Business Analyst Intern</div>
        <div class="tl-where">Hindalco Industries, Aditya Birla Group</div>
        <ul>
          <li>Built SQL queries against Oracle ERP to extract, validate, and transform data; ran gap analysis into Tableau dashboards for senior leadership.</li>
          <li>Reduced manual processing time by 25% and improved API query performance by 10%.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">05</span>
      <h2 class="sec-title">Stack</h2>
    </div>
    <div class="skill-grid reveal">
      <div class="skill-col">
        <h4>AI / GenAI / RAG</h4>
        <ul>
          <li>RAG pipeline design</li>
          <li>Constrained LLM reasoning</li>
          <li>Multi-agent architectures</li>
          <li>LangChain · Agentic workflows</li>
          <li>RAGAS · FAISS</li>
          <li>Prompt engineering</li>
        </ul>
      </div>
      <div class="skill-col">
        <h4>ML &amp; Data</h4>
        <ul>
          <li>PyTorch · TensorFlow</li>
          <li>Scikit-learn · HuggingFace</li>
          <li>Sentence Transformers</li>
          <li>Pandas · NumPy</li>
          <li>Tableau · SQL</li>
          <li>Spatial analysis (K-means, haversine)</li>
        </ul>
      </div>
      <div class="skill-col">
        <h4>Languages &amp; Platforms</h4>
        <ul>
          <li>Python (primary)</li>
          <li>JavaScript · React · Tailwind</li>
          <li>Azure AI-900 / AI-102 certified</li>
          <li>Oracle AI Vector Search certified</li>
          <li>Oracle Cloud — Gen AI Professional</li>
          <li>Git</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="awards">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-num mono">06</span>
      <h2 class="sec-title">Awards &amp; leadership</h2>
    </div>
    <div class="reveal">
      <div class="award-row">
        <div>
          <div class="award-name">ERA:AI Fellowship Finalist, Technical Track</div>
          <div class="award-org">Cambridge University, UK — selected from a global applicant pool for a fully funded AI safety research fellowship</div>
        </div>
        <div class="award-when mono">APR 2026</div>
      </div>
      <div class="award-row">
        <div>
          <div class="award-name">NPTEL STAR Award</div>
          <div class="award-org">IIT Kanpur — recognizing top national performance across NPTEL coursework</div>
        </div>
        <div class="award-when mono">AUG 2025</div>
      </div>
      <div class="award-row">
        <div>
          <div class="award-name">Gold Medalist, I-DIV with Distinction</div>
          <div class="award-org">AKTU — BTech (Hons.) CSE, CGPA 8.63/10</div>
        </div>
        <div class="award-when mono">2022 — 2026</div>
      </div>
      <div class="award-row">
        <div>
          <div class="award-name">Student Council President</div>
          <div class="award-org">Ashoka Institute of Technology and Management — representing 500+ students</div>
        </div>
        <div class="award-when mono">MAY 2025 — MAY 2026</div>
      </div>
      <div class="award-row">
        <div>
          <div class="award-name">Patriotic Youth Ambassador</div>
          <div class="award-org">Veterans India</div>
        </div>
        <div class="award-when mono">AUG — SEP 2025</div>
      </div>
    </div>
  </div>
</section>

<section id="contact" style="border-bottom:none;">
  <div class="wrap contact reveal">
    <span class="sec-num mono">07 / END OF LOG</span>
    <h2 class="display">Open to the next hard failure to fix.</h2>
    <p>PhD-bound in trustworthy AI — currently deciding between an offer letter and a job offer. Reach out about either.</p>
    <div class="contact-links">
      <a class="btn btn-primary" href="mailto:asthanapriyanka829@gmail.com">asthanapriyanka829@gmail.com</a>
      <a class="btn btn-ghost mono" href="https://www.linkedin.com/in/priyanka-asthana-1b9a74250" target="_blank" rel="noopener">LinkedIn ↗</a>
      <a class="btn btn-ghost mono" href="https://github.com/PriyankaAsthana" target="_blank" rel="noopener">GitHub ↗</a>
    </div>
  </div>
</section>

<footer class="mono">system uptime: since 2022 · last diagnostic: 2026 · built without a template</footer>

<script>
// ---------- typewriter ----------
const lines = [
  "constrained LLM systems",
  "RAG that doesn't hallucinate its way to harm",
  "GeoAI for emergency resource allocation",
  "PhD-bound — trustworthy AI"
];
const typedEl = document.getElementById('typed');
const reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;

if (reduceMotion) {
  typedEl.textContent = lines[0];
} else {
  let li = 0, ci = 0, deleting = false;
  function tick(){
    const full = lines[li];
    if(!deleting){
      ci++;
      typedEl.textContent = full.slice(0, ci);
      if(ci === full.length){ deleting = true; setTimeout(tick, 1600); return; }
    } else {
      ci--;
      typedEl.textContent = full.slice(0, ci);
      if(ci === 0){ deleting = false; li = (li+1) % lines.length; }
    }
    setTimeout(tick, deleting ? 28 : 55);
  }
  tick();
}

// ---------- scroll reveal ----------
const revealEls = document.querySelectorAll('.reveal, .case');
const io = new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      e.target.classList.add('is-visible');
      if(e.target.classList.contains('case')){
        e.target.querySelectorAll('.vital-fill').forEach(f=>{
          f.style.width = f.dataset.fill + '%';
        });
      }
    }
  });
}, {threshold:0.15});
revealEls.forEach(el=>io.observe(el));

// ---------- hero canvas: embedding space with a caught hallucination ----------
const canvas = document.getElementById('node-canvas');
const ctx = canvas.getContext('2d');
let W, H, nodes = [];
const NODE_COUNT = 46;
const COLORS = { violet:'#a78bfa', teal:'#5eead4', amber:'#f0b429', danger:'#fb7185', line:'#212a3a' };

function resize(){
  W = canvas.width = canvas.offsetWidth * devicePixelRatio;
  H = canvas.height = canvas.offsetHeight * devicePixelRatio;
}
window.addEventListener('resize', resize);

function initNodes(){
  nodes = [];
  for(let i=0;i<NODE_COUNT;i++){
    nodes.push({
      x: Math.random()*W,
      y: Math.random()*H,
      vx: (Math.random()-0.5)*0.15*devicePixelRatio,
      vy: (Math.random()-0.5)*0.15*devicePixelRatio,
      r: (Math.random()*1.6+1.2)*devicePixelRatio,
      flagged: false,
      flagTimer: Math.random()*600 + 300
    });
  }
}

let frame = 0;
function draw(){
  frame++;
  ctx.clearRect(0,0,W,H);

  // occasionally flag a node (simulated hallucination), then resolve it
  nodes.forEach(n=>{
    n.flagTimer--;
    if(n.flagTimer <= 0 && !n.flagged){
      n.flagged = true;
      n.flagLife = 140;
    }
    if(n.flagged){
      n.flagLife--;
      if(n.flagLife <= 0){ n.flagged = false; n.flagTimer = Math.random()*700+400; }
    }
    n.x += n.vx; n.y += n.vy;
    if(n.x < 0 || n.x > W) n.vx *= -1;
    if(n.y < 0 || n.y > H) n.vy *= -1;
  });

  // connections
  for(let i=0;i<nodes.length;i++){
    for(let j=i+1;j<nodes.length;j++){
      const a = nodes[i], b = nodes[j];
      const dx = a.x-b.x, dy = a.y-b.y;
      const dist = Math.sqrt(dx*dx+dy*dy);
      const maxDist = 130*devicePixelRatio;
      if(dist < maxDist){
        const alpha = (1-dist/maxDist) * 0.35;
        let strokeColor = `rgba(33,42,58,${alpha})`;
        if(a.flagged || b.flagged){
          strokeColor = `rgba(240,180,41,${alpha*1.8})`;
        }
        ctx.strokeStyle = strokeColor;
        ctx.lineWidth = 1;
        ctx.beginPath();
        ctx.moveTo(a.x,a.y); ctx.lineTo(b.x,b.y);
        ctx.stroke();
      }
    }
  }

  // nodes
  nodes.forEach(n=>{
    let color = COLORS.violet;
    let radius = n.r;
    if(n.flagged){
      color = n.flagLife > 60 ? COLORS.danger : COLORS.teal;
      radius = n.r * 1.8;
    }
    ctx.beginPath();
    ctx.fillStyle = color;
    ctx.globalAlpha = n.flagged ? 0.95 : 0.55;
    ctx.arc(n.x, n.y, radius, 0, Math.PI*2);
    ctx.fill();
    ctx.globalAlpha = 1;
  });

  if(!reduceMotion){
    requestAnimationFrame(draw);
  }
}

resize();
initNodes();
draw();

document.addEventListener('visibilitychange', ()=>{
  if(!document.hidden && !reduceMotion) requestAnimationFrame(draw);
});
</script>

</body>
</html>
