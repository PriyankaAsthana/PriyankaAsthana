<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    ASTHANA.OS // HERO                          -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<svg width="100%" viewBox="0 0 1200 520" xmlns="http://www.w3.org/2000/svg">

  <defs>

    <!-- Background -->
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#03050A"/>
      <stop offset="50%" stop-color="#07101C"/>
      <stop offset="100%" stop-color="#12051C"/>
    </linearGradient>

    <!-- Cyan glow -->
    <filter id="cyanGlow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Violet glow -->
    <filter id="violetGlow">
      <feGaussianBlur stdDeviation="7" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Grid -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M40 0H0V40" fill="none" stroke="#00E5FF" stroke-opacity=".07"/>
    </pattern>

    <!-- Radial light -->
    <radialGradient id="core">
      <stop offset="0%" stop-color="#00E5FF" stop-opacity=".20"/>
      <stop offset="50%" stop-color="#7B2CFF" stop-opacity=".08"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
    </radialGradient>

  </defs>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- BACKGROUND -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <rect width="1200" height="520" rx="24" fill="url(#bg)"/>

  <rect width="1200" height="520" rx="24" fill="url(#grid)"/>

  <ellipse cx="900" cy="260" rx="390" ry="300" fill="url(#core)"/>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- TOP SYSTEM BAR -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <line
    x1="45"
    y1="42"
    x2="1155"
    y2="42"
    stroke="#00E5FF"
    stroke-opacity=".35"
  />

  <text
    x="55"
    y="30"
    fill="#00E5FF"
    font-family="monospace"
    font-size="13"
    letter-spacing="3"
  >
    ASTHANA.OS
  </text>

  <text
    x="1145"
    y="30"
    fill="#7CFFB2"
    font-family="monospace"
    font-size="12"
    text-anchor="end"
  >
    ● SYSTEM ONLINE
  </text>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- LEFT IDENTITY PANEL -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <text
    x="70"
    y="125"
    fill="#667080"
    font-family="monospace"
    font-size="13"
    letter-spacing="3"
  >
    AI SYSTEMS / RESEARCH / ROBOTICS
  </text>

  <text
    x="65"
    y="190"
    fill="#FFFFFF"
    font-family="sans-serif"
    font-size="58"
    font-weight="700"
    letter-spacing="-2"
  >
    PRIYANKA
  </text>

  <text
    x="65"
    y="250"
    fill="#00E5FF"
    font-family="sans-serif"
    font-size="58"
    font-weight="700"
    letter-spacing="-2"
    filter="url(#cyanGlow)"
  >
    ASTHANA
  </text>

  <text
    x="68"
    y="285"
    fill="#AAB4C4"
    font-family="monospace"
    font-size="15"
    letter-spacing="2"
  >
    BTECH (HONS.) CSE  //  MINOR: ROBOTICS
  </text>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- TERMINAL -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <rect
    x="65"
    y="325"
    width="500"
    height="105"
    rx="10"
    fill="#03060B"
    stroke="#00E5FF"
    stroke-opacity=".30"
  />

  <circle cx="87" cy="346" r="5" fill="#FF5F56"/>
  <circle cx="104" cy="346" r="5" fill="#FFBD2E"/>
  <circle cx="121" cy="346" r="5" fill="#27C93F"/>

  <text
    x="88"
    y="377"
    fill="#667080"
    font-family="monospace"
    font-size="13"
  >
    ~/priyanka
  </text>

  <text
    x="88"
    y="402"
    fill="#00E5FF"
    font-family="monospace"
    font-size="14"
  >
    &gt; building intelligent systems from raw data
  </text>

  <text
    x="88"
    y="420"
    fill="#7CFFB2"
    font-family="monospace"
    font-size="14"
  >
    &gt; research_mode = TRUE
  </text>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- RIGHT: 3D / ORBITAL AI CORE -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <g transform="translate(885 245)">

    <!-- outer orbital rings -->

    <ellipse
      cx="0"
      cy="0"
      rx="235"
      ry="82"
      fill="none"
      stroke="#7B2CFF"
      stroke-opacity=".25"
      stroke-width="2"
      transform="rotate(-20)"
    />

    <ellipse
      cx="0"
      cy="0"
      rx="200"
      ry="68"
      fill="none"
      stroke="#00E5FF"
      stroke-opacity=".30"
      stroke-width="2"
      transform="rotate(55)"
    />

    <ellipse
      cx="0"
      cy="0"
      rx="155"
      ry="55"
      fill="none"
      stroke="#FFFFFF"
      stroke-opacity=".12"
      transform="rotate(105)"
    />

    <!-- central sphere -->

    <circle
      cx="0"
      cy="0"
      r="92"
      fill="#07131D"
      stroke="#00E5FF"
      stroke-width="2"
      filter="url(#cyanGlow)"
    />

    <circle
      cx="0"
      cy="0"
      r="70"
      fill="none"
      stroke="#7B2CFF"
      stroke-opacity=".55"
      stroke-width="2"
    />

    <!-- neural nodes -->

    <circle cx="-38" cy="-25" r="7" fill="#00E5FF"/>
    <circle cx="35" cy="-38" r="6" fill="#7B2CFF"/>
    <circle cx="48" cy="25" r="7" fill="#00E5FF"/>
    <circle cx="-30" cy="38" r="6" fill="#7B2CFF"/>
    <circle cx="5" cy="5" r="9" fill="#FFFFFF"/>

    <!-- neural connections -->

    <line x1="-38" y1="-25" x2="5" y2="5"
          stroke="#00E5FF" stroke-opacity=".7"/>

    <line x1="35" y1="-38" x2="5" y2="5"
          stroke="#7B2CFF" stroke-opacity=".7"/>

    <line x1="48" y1="25" x2="5" y2="5"
          stroke="#00E5FF" stroke-opacity=".7"/>

    <line x1="-30" y1="38" x2="5" y2="5"
          stroke="#7B2CFF" stroke-opacity=".7"/>

    <!-- orbiting nodes -->

    <circle cx="150" cy="-50" r="8"
            fill="#00E5FF"
            filter="url(#cyanGlow)"/>

    <circle cx="-145" cy="60" r="7"
            fill="#7B2CFF"
            filter="url(#violetGlow)"/>

    <circle cx="65" cy="100" r="6"
            fill="#7CFFB2"/>

  </g>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- TELEMETRY -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <text
    x="690"
    y="405"
    fill="#667080"
    font-family="monospace"
    font-size="11"
    letter-spacing="2"
  >
    ACTIVE SYSTEMS
  </text>

  <text
    x="690"
    y="425"
    fill="#FFFFFF"
    font-family="monospace"
    font-size="12"
  >
    AI/ML
  </text>

  <text
    x="770"
    y="425"
    fill="#7CFFB2"
    font-family="monospace"
    font-size="12"
  >
    ● ONLINE
  </text>

  <text
    x="690"
    y="447"
    fill="#FFFFFF"
    font-family="monospace"
    font-size="12"
  >
    RESEARCH
  </text>

  <text
    x="770"
    y="447"
    fill="#7CFFB2"
    font-family="monospace"
    font-size="12"
  >
    ● ACTIVE
  </text>

  <text
    x="690"
    y="469"
    fill="#FFFFFF"
    font-family="monospace"
    font-size="12"
  >
    ROBOTICS
  </text>

  <text
    x="770"
    y="469"
    fill="#00E5FF"
    font-family="monospace"
    font-size="12"
  >
    ● BUILDING
  </text>


  <!-- ═══════════════════════════════════════════════════════════ -->
  <!-- BOTTOM STATUS -->
  <!-- ═══════════════════════════════════════════════════════════ -->

  <line
    x1="45"
    y1="485"
    x2="1155"
    y2="485"
    stroke="#00E5FF"
    stroke-opacity=".20"
  />

  <text
    x="55"
    y="507"
    fill="#566170"
    font-family="monospace"
    font-size="10"
    letter-spacing="2"
  >
    BUILD • RESEARCH • ITERATE
  </text>

  <text
    x="1145"
    y="507"
    fill="#566170"
    font-family="monospace"
    font-size="10"
    text-anchor="end"
  >
    NODE://AI-RESEARCH
  </text>

</svg>

<br>

<a href="https://github.com/PriyankaAsthana">
<img src="https://img.shields.io/badge/EXPLORE_GITHUB-05070D?style=for-the-badge&logo=github&logoColor=00E5FF&labelColor=05070D" />
</a>

&nbsp;

<a href="YOUR_LINKEDIN_URL">
<img src="https://img.shields.io/badge/LINKEDIN-05070D?style=for-the-badge&logo=linkedin&logoColor=7B2CFF&labelColor=05070D" />
</a>

&nbsp;

<a href="YOUR_PORTFOLIO_URL">
<img src="https://img.shields.io/badge/PORTFOLIO-05070D?style=for-the-badge&logo=googlechrome&logoColor=7CFFB2&labelColor=05070D" />
</a>

</div>
<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                 02 // ACTIVE RESEARCH                          -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<br>

<img
src="https://capsule-render.vercel.app/api?type=rect&height=2&color=00E5FF"
width="90%"
/>

<br><br>

<h2>☀️ SOLARDROUGHT // ACTIVE RESEARCH</h2>

<p>
<b>AI-DRIVEN SOLAR RESOURCE INTELLIGENCE</b>
</p>

<code>DAVOS, SWITZERLAND</code>
&nbsp;&nbsp;
<code>HOURLY RESOLUTION</code>
&nbsp;&nbsp;
<code>RESEARCH MODE: ACTIVE</code>

<br><br>

</div>


<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                      RESEARCH HUD                              -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<table width="100%">
<tr>

<td width="62%" valign="top">

<div align="center">

<h3>◉ SOLAR RESOURCE MONITOR</h3>

</div>

<br>

<!-- Put your REAL SolarDrought primary visualization here -->
<img
src="./assets/solardrought/ghi-analysis.png"
width="100%"
alt="SolarDrought GHI analysis"
/>

<br>

<div align="center">

<sub>
PRIMARY SIGNAL // GLOBAL HORIZONTAL IRRADIANCE
</sub>

</div>

</td>


<td width="38%" valign="top">

<div align="center">

<h3>RESEARCH TELEMETRY</h3>

</div>

<br>

<table width="100%">

<tr>
<td><b>LOCATION</b></td>
<td>Davos, Switzerland</td>
</tr>

<tr>
<td><b>RESOLUTION</b></td>
<td>Hourly</td>
</tr>

<tr>
<td><b>PRIMARY</b></td>
<td>GHI</td>
</tr>

<tr>
<td><b>REFERENCE</b></td>
<td>Clear-Sky</td>
</tr>

<tr>
<td><b>ATMOSPHERE</b></td>
<td>Clouds + AOD</td>
</tr>

<tr>
<td><b>DETECTION</b></td>
<td>Anomaly + Threshold</td>
</tr>

<tr>
<td><b>PERSISTENCE</b></td>
<td>Event-aware</td>
</tr>

<tr>
<td><b>VALIDATION</b></td>
<td>Time-aware</td>
</tr>

</table>

<br>

<div align="center">

<code>● DATA PIPELINE ACTIVE</code>

<br><br>

<code>● ANOMALY ENGINE ACTIVE</code>

<br><br>

<code>● EVENT ENGINE ACTIVE</code>

<br><br>

<code>○ PREDICTION NEXT PHASE</code>

</div>

</td>

</tr>
</table>


<br><br>


<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    RESEARCH PIPELINE                           -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<h3>⚡ RESEARCH PIPELINE</h3>

<br>

<table width="100%">
<tr>

<td align="center">
<b>01</b><br>
RAW SOLAR DATA
</td>

<td align="center">
<b>→</b>
</td>

<td align="center">
<b>02</b><br>
DATA QUALITY
</td>

<td align="center">
<b>→</b>
</td>

<td align="center">
<b>03</b><br>
CLEAR-SKY
</td>

<td align="center">
<b>→</b>
</td>

<td align="center">
<b>04</b><br>
ANOMALY
</td>

<td align="center">
<b>→</b>
</td>

<td align="center">
<b>05</b><br>
PERSISTENCE
</td>

<td align="center">
<b>→</b>
</td>

<td align="center">
<b>06</b><br>
EVENTS
</td>

</tr>
</table>

<br>

<code>
INTENSITY
</code>

&nbsp;&nbsp;→&nbsp;&nbsp;

<code>
DURATION
</code>

&nbsp;&nbsp;→&nbsp;&nbsp;

<code>
SEVERITY
</code>

&nbsp;&nbsp;→&nbsp;&nbsp;

<code>
TIME-AWARE VALIDATION
</code>

</div>


<br><br>


<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    ANALYTICS GRID                              -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<table width="100%">
<tr>

<td width="50%" valign="top">

<div align="center">

<h3>📈 ANOMALY ENGINE</h3>

</div>

<img
src="./assets/solardrought/anomaly-analysis.png"
width="100%"
alt="SolarDrought anomaly analysis"
/>

<div align="center">

<sub>
ANOMALY / THRESHOLD / PERSISTENCE ANALYSIS
</sub>

</div>

</td>


<td width="50%" valign="top">

<div align="center">

<h3>⚠️ EVENT CHARACTERIZATION</h3>

</div>

<img
src="./assets/solardrought/event-analysis.png"
width="100%"
alt="SolarDrought event characterization"
/>

<div align="center">

<sub>
INTENSITY / DURATION / SEVERITY
</sub>

</div>

</td>

</tr>
</table>


<br><br>


<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                     SYSTEM ARCHITECTURE                        -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<h3>🛰️ SYSTEM ARCHITECTURE</h3>

<br>

<table width="100%">
<tr>

<td align="center">
☀️<br>
<b>SOLAR RADIATION</b><br>
<sub>CAMS Solar Radiation</sub>
</td>

<td align="center">→</td>

<td align="center">
🌤️<br>
<b>ATMOSPHERE</b><br>
<sub>Clouds / AOD / Meteorology</sub>
</td>

<td align="center">→</td>

<td align="center">
🧠<br>
<b>INTELLIGENCE</b><br>
<sub>Anomaly Detection</sub>
</td>

<td align="center">→</td>

<td align="center">
⚠️<br>
<b>EVENT ENGINE</b><br>
<sub>Persistence + Severity</sub>
</td>

</tr>
</table>

<br>

<table width="100%">
<tr>

<td align="center">
<b>PRIMARY</b><br>
GHI
</td>

<td align="center">
<b>NORMALIZATION</b><br>
Clear-Sky
</td>

<td align="center">
<b>DETECTION</b><br>
Threshold
</td>

<td align="center">
<b>VALIDATION</b><br>
Time-Aware
</td>

<td align="center">
<b>FUTURE</b><br>
Prediction
</td>

</tr>
</table>

</div>


<br><br>


<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                        RESEARCH CARD                           -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<table width="92%">
<tr>

<td align="center">

<h3>☀️ THE RESEARCH QUESTION</h3>

<br>

<p>
How can unusually reduced solar-resource availability
be detected, characterized and validated from
high-resolution solar and atmospheric data?
</p>

<br>

<code>
GHI → CLEAR-SKY NORMALIZATION → ANOMALY
→ PERSISTENCE → EVENT → SEVERITY
</code>

<br><br>

<a href="YOUR_SOLARDROUGHT_REPO_URL">
<img
src="https://img.shields.io/badge/VIEW_SOLARDROUGHT_REPOSITORY-00E5FF?style=for-the-badge&logo=github&logoColor=000000"
/>
</a>

</td>

</tr>
</table>

</div>


<br>

<div align="center">

<code>
SOLARDROUGHT // RESEARCH SYSTEM // ACTIVE
</code>

</div>

<br>
