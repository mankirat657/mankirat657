<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mankirat Singh · Profile</title>
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    }

    body {
      background: #0b1219;
      display: flex;
      justify-content: center;
      padding: 2rem 1rem;
    }

    .container {
      max-width: 1000px;
      width: 100%;
      background: #0f1a24;
      border-radius: 48px;
      padding: 2.5rem 2rem;
      box-shadow: 0 25px 50px -10px rgba(0, 255, 209, 0.15);
      border: 1px solid rgba(0, 255, 209, 0.08);
    }

    /* ===== header / capsule ===== */
    .capsule-header {
      margin-bottom: 1.5rem;
    }
    .capsule-header img {
      width: 100%;
      display: block;
      border-radius: 24px;
    }

    /* ===== typing SVG ===== */
    .typing-area {
      text-align: center;
      margin: 0.5rem 0 1.2rem;
    }
    .typing-area img {
      max-width: 100%;
      height: auto;
    }

    /* ===== badges ===== */
    .badge-row {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.6rem 1rem;
      margin: 1.2rem 0 0.8rem;
    }
    .badge-row a, .badge-row img {
      display: inline-block;
      vertical-align: middle;
    }
    .badge-row img {
      height: 28px;
    }

    /* ===== snake section ===== */
    .snake-section {
      margin: 2.5rem 0 1.8rem;
      text-align: center;
    }
    .snake-section h3 {
      color: #b0f0e0;
      font-weight: 500;
      letter-spacing: 1px;
      margin-bottom: 0.8rem;
      font-size: 1.2rem;
    }
    .snake-section picture img {
      width: 100%;
      border-radius: 28px;
      background: #0e1a20;
      box-shadow: 0 8px 30px rgba(0, 255, 209, 0.06);
      border: 1px solid rgba(0, 255, 209, 0.06);
    }

    /* ===== divider ===== */
    .divider {
      width: 100%;
      margin: 2rem 0;
      opacity: 0.6;
    }
    .divider img {
      width: 100%;
      display: block;
    }

    /* ===== whoami ===== */
    .whoami {
      background: #101f2b;
      border-radius: 24px;
      padding: 1.8rem 2rem;
      margin: 1.8rem 0 2rem;
      border-left: 4px solid #00FFD1;
    }
    .whoami h2 {
      color: #00FFD1;
      font-weight: 600;
      font-size: 1.8rem;
      margin-bottom: 0.75rem;
      letter-spacing: -0.5px;
    }
    .whoami pre {
      background: #0b161f;
      padding: 1.2rem 1.5rem;
      border-radius: 16px;
      color: #c8e6e0;
      font-size: 0.9rem;
      line-height: 1.7;
      overflow-x: auto;
      white-space: pre-wrap;
      word-break: break-word;
      border: 1px solid #1d3342;
    }
    .whoami table {
      width: 100%;
      margin-top: 1.2rem;
      border-collapse: collapse;
    }
    .whoami td {
      vertical-align: top;
      padding: 0.4rem 0.2rem;
      color: #d0e6e0;
    }
    .whoami ul {
      list-style: none;
      padding-left: 0.2rem;
    }
    .whoami li {
      padding: 0.25rem 0;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .whoami li::before {
      content: "▹";
      color: #00FFD1;
      font-weight: bold;
    }
    .ascii-box {
      background: #0b161f;
      padding: 0.8rem 1rem;
      border-radius: 16px;
      font-size: 0.75rem;
      line-height: 1.5;
      color: #8bb8b0;
      border: 1px solid #1d3342;
      white-space: pre;
      font-family: 'Fira Code', monospace;
    }

    /* ===== experience ===== */
    .exp-block {
      background: #101f2b;
      border-radius: 24px;
      padding: 1.8rem 2rem;
      margin: 2rem 0;
    }
    .exp-block h2 {
      color: #00FFD1;
      font-weight: 600;
      font-size: 1.8rem;
      margin-bottom: 1rem;
    }
    .exp-timeline {
      background: #0b161f;
      padding: 1.5rem;
      border-radius: 20px;
      font-family: 'Fira Code', monospace;
      font-size: 0.85rem;
      color: #b0d4cc;
      white-space: pre-wrap;
      word-break: break-word;
      border: 1px solid #1d3342;
      line-height: 1.6;
    }

    /* ===== tech ===== */
    .tech-section {
      margin: 2rem 0;
      text-align: center;
    }
    .tech-section h2 {
      color: #00FFD1;
      font-weight: 600;
      font-size: 1.8rem;
      margin-bottom: 1.2rem;
    }
    .tech-icons {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.8rem 1.2rem;
      margin: 1rem 0;
    }
    .tech-icons img {
      height: 50px;
      width: auto;
    }
    .tech-badges {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.5rem 0.8rem;
      margin-top: 1rem;
    }
    .tech-badges img {
      height: 28px;
    }

    /* ===== projects ===== */
    .projects {
      margin: 2.5rem 0;
    }
    .projects h2 {
      color: #00FFD1;
      font-weight: 600;
      font-size: 1.8rem;
      margin-bottom: 1.5rem;
    }
    .project-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1.5rem;
    }
    .project-card {
      background: #101f2b;
      padding: 1.5rem;
      border-radius: 24px;
      border: 1px solid #1d3342;
      transition: 0.2s ease;
    }
    .project-card:hover {
      border-color: #00FFD1;
      box-shadow: 0 8px 25px rgba(0, 255, 209, 0.06);
    }
    .project-card h3 {
      color: #e0f0ec;
      font-size: 1.2rem;
      margin-bottom: 0.3rem;
    }
    .project-card p {
      color: #b0c8c2;
      font-size: 0.9rem;
      line-height: 1.5;
      margin: 0.5rem 0 0.8rem;
    }
    .project-card .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem 0.6rem;
      margin: 0.6rem 0;
    }
    .project-card .tags span {
      background: #162b38;
      padding: 0.15rem 0.8rem;
      border-radius: 40px;
      font-size: 0.7rem;
      color: #b0e0d6;
      border: 1px solid #264452;
    }
    .project-card .btn-group {
      display: flex;
      gap: 0.6rem;
      flex-wrap: wrap;
      margin-top: 0.8rem;
    }
    .project-card .btn-group img {
      height: 28px;
    }
    details {
      margin-top: 1.8rem;
      color: #b0d4cc;
      cursor: pointer;
    }
    details summary {
      font-weight: 500;
      font-size: 1rem;
      color: #00FFD1;
    }
    details p {
      margin-top: 0.8rem;
      padding: 0.8rem 1.2rem;
      background: #101f2b;
      border-radius: 20px;
    }
    details a {
      color: #00FFD1;
      text-decoration: none;
    }

    /* ===== github stats ===== */
    .stats-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1.5rem 0;
    }
    .stats-grid img {
      max-width: 48%;
      height: auto;
      border-radius: 20px;
      background: #0e1a20;
      border: 1px solid #1d3342;
    }
    .trophy-row {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      margin: 1.5rem 0 0.5rem;
    }
    .trophy-row img {
      max-width: 100%;
      border-radius: 20px;
    }

    /* ===== contact ===== */
    .contact {
      text-align: center;
      margin: 2.5rem 0 0.5rem;
    }
    .contact h2 {
      color: #00FFD1;
      font-weight: 600;
      font-size: 1.8rem;
      margin-bottom: 1rem;
    }
    .contact-badges {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.6rem 1rem;
      margin: 1rem 0;
    }
    .contact-badges img {
      height: 28px;
    }
    .quote {
      color: #b0d4cc;
      font-size: 0.95rem;
      margin: 1.5rem 0 0.8rem;
      font-style: italic;
    }
    .footer-wave {
      margin-top: 1.5rem;
    }
    .footer-wave img {
      width: 100%;
      display: block;
      border-radius: 0 0 24px 24px;
    }

    /* ===== responsive ===== */
    @media (max-width: 700px) {
      .container { padding: 1.5rem 1rem; }
      .project-grid { grid-template-columns: 1fr; }
      .stats-grid img { max-width: 100%; }
      .whoami td { display: block; width: 100% !important; }
      .whoami table { display: block; }
      .whoami .ascii-box { font-size: 0.65rem; }
    }
  </style>
</head>
<body>
<div class="container">

  <!-- ===== HEADER ===== -->
  <div class="capsule-header">
    <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:00FFD1,100:2C5364&height=250&section=header&text=MANKIRAT%20SINGH&fontSize=55&fontColor=ffffff&fontAlignY=32&desc=Full-Stack%20Developer%20•%20MERN%20%2B%20TypeScript%20•%20AI%20Builder&descAlignY=52&descSize=17&animation=fadeIn" alt="header" />
  </div>

  <!-- ===== TYPING ===== -->
  <div class="typing-area">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=23&duration=2500&pause=800&color=00FFD1&center=true&vCenter=true&width=750&lines=Building+AI-powered+products+%F0%9F%A4%96;MERN+Stack+%2B+TypeScript+Specialist;Real-Time+Apps+%7C+WebSockets+%7C+Clean+Code;GSAP+%26+Framer+Motion+Animation+Nerd;Currently+shipping%3A+AlQuida+AI+%26+OptiTask+AI" alt="typing" />
  </div>

  <!-- ===== BADGES ===== -->
  <div class="badge-row">
    <a href="https://mellow-jalebi-ca7484.netlify.app/" target="_blank"><img src="https://img.shields.io/badge/🌐_PORTFOLIO-Visit_Now-00FFD1?style=for-the-badge&labelColor=0F2027" alt="portfolio" /></a>
    <a href="mailto:mankirat.matharu@gmail.com"><img src="https://img.shields.io/badge/EMAIL-Say_Hi-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0F2027" alt="email" /></a>
    <a href="https://github.com/mankirat657"><img src="https://img.shields.io/badge/GITHUB-Follow-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=0F2027" alt="github" /></a>
    <img src="https://komarev.com/ghpvc/?username=mankirat657&color=00FFD1&style=for-the-badge&label=PROFILE+VIEWS" alt="views" />
  </div>

  <!-- ===== SNAKE ===== -->
  <div class="snake-section">
    <h3><i class="fas fa-snake" style="margin-right: 8px;"></i> Eating My Way Through Every Commit</h3>
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/mankirat657/mankirat657/output/github-contribution-grid-snake-dark.svg" />
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/mankirat657/mankirat657/output/github-contribution-grid-snake.svg" />
      <img alt="Contribution Snake animation" src="https://raw.githubusercontent.com/mankirat657/mankirat657/output/github-contribution-grid-snake.svg" width="100%"/>
    </picture>
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== WHOAMI ===== -->
  <div class="whoami">
    <h2>🧠 `whoami`</h2>
    <pre>name: Mankirat Singh
education: BCA — Guru Gobind Singh Indraprastha University (GGSIPU)
role: Full-Stack Developer (MERN + TypeScript)
currently_building: [AlQuida AI, OptiTask AI]
believes: "An app isn't done until it *feels* smooth."
weapons_of_choice: [React, TypeScript, Node.js, Tailwind, GSAP]
status: 🟢 Open to full-time opportunities</pre>

    <table>
      <tr>
        <td width="60%" valign="top">
          <ul>
            <li>🎓 BCA Graduate, GGSIPU</li>
            <li>💼 2x Software Development Internships (React / React+TypeScript)</li>
            <li>🤖 Building AI-powered products end-to-end — from schema design to pixel-perfect animation</li>
            <li>🎨 Obsessed with motion design — if it doesn't animate, it doesn't ship</li>
            <li>📊 Sharpening backend + SQL chops to go full-stack, full-power</li>
            <li>⚡ Fun fact: I debug CSS faster than I debug my sleep schedule</li>
          </ul>
        </td>
        <td width="40%" valign="top">
          <div class="ascii-box">
   ⚡ current mood ⚡
   ┌─────────────────┐
   │  npm run build  │
   │  ✔ compiled     │
   │  ✔ 0 errors     │
   │  ✔ ship it 🚀   │
   └─────────────────┘
          </div>
        </td>
      </tr>
    </table>
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== EXPERIENCE ===== -->
  <div class="exp-block">
    <h2>💼 Experience Timeline</h2>
    <div class="exp-timeline">
2024 ────────────────────────────────────────────────────►

   ●━━━━━━━━━━━━━━━━━━━━━━━━●
   │                        │
   ▼                        ▼
┌──────────────────┐  ┌───────────────────────┐
│  Domain Expansion │  │       AppKnit         │
│  React Developer  │  │  React + TypeScript   │
│  Maharashtra      │  │  Chandigarh           │
│  💻 Remote         │  │  💻 Remote             │
└──────────────────┘  └───────────────────────┘
   Built & maintained      Shipped type-safe,
   reusable, performant    scalable front-end
   React components        modules in production
    </div>
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== TECH STACK ===== -->
  <div class="tech-section">
    <h2>🛠️ Tech Arsenal</h2>
    <div class="tech-icons">
      <img src="https://skillicons.dev/icons?i=js,ts,react,tailwind,nodejs,express,mongodb,mysql,git,github,vscode,figma&perline=6" alt="tech icons" />
    </div>
    <div class="tech-badges">
      <img src="https://img.shields.io/badge/Framer_Motion-000000?style=for-the-badge&logo=framer&logoColor=white" alt="framer" />
      <img src="https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white" alt="gsap" />
      <img src="https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.io&logoColor=white" alt="socket" />
      <img src="https://img.shields.io/badge/REST_API-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="rest" />
    </div>
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== PROJECTS ===== -->
  <div class="projects">
    <h2>🚀 Featured Builds</h2>
    <div class="project-grid">
      <div class="project-card">
        <h3>🤖 AlQuida AI</h3>
        <p><strong>AI-powered MERN application</strong> delivering an intelligent, seamless user experience — built end-to-end from data layer to UI.</p>
        <div class="tags"><span>React</span><span>TypeScript</span><span>Node.js</span><span>MongoDB</span><span>AI Integration</span></div>
        <div class="btn-group"><img src="https://img.shields.io/badge/View_Project-00FFD1?style=for-the-badge&logo=github&logoColor=black" alt="project" /></div>
      </div>
      <div class="project-card">
        <h3>⚡ OptiTask AI</h3>
        <p><strong>Smart task-management platform</strong> that uses AI to help users prioritize and optimize their daily workflow.</p>
        <div class="tags"><span>React</span><span>Node.js</span><span>Express</span><span>MongoDB</span><span>AI Integration</span></div>
        <div class="btn-group"><img src="https://img.shields.io/badge/View_Project-00FFD1?style=for-the-badge&logo=github&logoColor=black" alt="project" /></div>
      </div>
      <div class="project-card">
        <h3>🌋 Landslide Disaster Management</h3>
        <p>Monitors rainfall, terrain & soil data in real time to predict landslide risk before it happens.</p>
        <div class="tags"><span>MERN</span><span>WebSockets</span><span>Real-Time Alerts</span></div>
        <div class="btn-group"><a href="https://github.com/mankirat657/landslide-disaster-management"><img src="https://img.shields.io/badge/View_Repo-181717?style=for-the-badge&logo=github&logoColor=white" alt="repo" /></a></div>
      </div>
      <div class="project-card">
        <h3>💬 Real-Time Chat App</h3>
        <p>Instant messaging with live, WebSocket-powered updates and zero lag.</p>
        <div class="tags"><span>MERN</span><span>Socket.io</span></div>
        <div class="btn-group"><a href="https://github.com/mankirat657/realtime-chat-app"><img src="https://img.shields.io/badge/View_Repo-181717?style=for-the-badge&logo=github&logoColor=white" alt="repo" /></a></div>
      </div>
    </div>

    <details>
      <summary><b>🔗 More projects</b></summary>
      <p><strong>Favorite Link Setter</strong> — Lightweight productivity tool built with React + LocalStorage to save and access frequently used links.<br/>
      <a href="https://github.com/mankirat657/favorite-links">View Repo →</a></p>
    </details>
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== GITHUB ANALYTICS ===== -->
  <div style="text-align: center; margin: 2rem 0 0.5rem;">
    <h2 style="color: #00FFD1; font-weight: 600; font-size: 1.8rem;">📊 GitHub Analytics</h2>
  </div>
  <div class="stats-grid">
    <img src="https://github-readme-stats.vercel.app/api?username=mankirat657&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" alt="stats" />
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=mankirat657&theme=tokyonight&hide_border=true" alt="streak" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mankirat657&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="langs" />
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=mankirat657&theme=tokyo-night&hide_border=true" alt="graph" />
  </div>
  <div class="trophy-row">
    <img src="https://github-profile-trophy.vercel.app/?username=mankirat657&theme=tokyonight&no-frame=true&column=7&margin-w=8" alt="trophy" />
  </div>

  <!-- ===== DIVIDER ===== -->
  <div class="divider">
    <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" alt="divider" />
  </div>

  <!-- ===== CONTACT ===== -->
  <div class="contact">
    <h2>📫 Let's Build Something Great</h2>
    <div class="contact-badges">
      <a href="https://mellow-jalebi-ca7484.netlify.app/"><img src="https://img.shields.io/badge/🌐_Portfolio-mellow--jalebi-00FFD1?style=for-the-badge&labelColor=0F2027" alt="portfolio" /></a>
      <a href="https://github.com/mankirat657"><img src="https://img.shields.io/badge/GitHub-mankirat657-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=0F2027" alt="github" /></a>
      <a href="mailto:mankirat.matharu@gmail.com"><img src="https://img.shields.io/badge/Email-mankirat.matharu%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0F2027" alt="email" /></a>
    </div>
    <div class="quote">
      ⭐ "Code is like humor. When you have to explain it, it's bad." — but I'll explain it anyway, with great animations.
    </div>
    <div class="footer-wave">
      <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2C5364,50:00FFD1,100:0F2027&height=120&section=footer" alt="footer" />
    </div>
  </div>

</div>
</body>
</html>
