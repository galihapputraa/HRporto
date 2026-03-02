<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Galih — People Ops Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Mono:wght@300;400;500&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --cream: #F5F0E8;
    --ink: #1A1714;
    --rust: #C4572A;
    --sage: #6B8C6E;
    --warm-gray: #8C8278;
    --light-line: #DDD6C8;
  }

  body {
    background: var(--cream);
    color: var(--ink);
    font-family: 'DM Sans', sans-serif;
    font-weight: 300;
    min-height: 100vh;
    overflow-x: hidden;
  }

  /* HEADER */
  header {
    padding: 60px 60px 40px;
    display: grid;
    grid-template-columns: 1fr auto;
    align-items: end;
    border-bottom: 1px solid var(--light-line);
    position: relative;
  }

  .header-tag {
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--rust);
    margin-bottom: 12px;
  }

  h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(36px, 5vw, 64px);
    font-weight: 400;
    line-height: 1.1;
    letter-spacing: -0.02em;
  }

  h1 em {
    font-style: italic;
    color: var(--rust);
  }

  .header-meta {
    text-align: right;
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    color: var(--warm-gray);
    line-height: 1.8;
  }

  .header-meta strong {
    display: block;
    color: var(--ink);
    font-size: 13px;
    font-weight: 500;
    margin-bottom: 6px;
    font-family: 'DM Sans', sans-serif;
  }

  /* INTRO STRIP */
  .intro-strip {
    padding: 24px 60px;
    background: var(--ink);
    color: var(--cream);
    display: flex;
    gap: 60px;
    align-items: center;
    overflow-x: auto;
  }

  .stat {
    flex-shrink: 0;
    display: flex;
    align-items: baseline;
    gap: 10px;
  }

  .stat-num {
    font-family: 'Playfair Display', serif;
    font-size: 32px;
    color: var(--rust);
  }

  .stat-label {
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: rgba(245,240,232,0.6);
    max-width: 100px;
    line-height: 1.4;
  }

  .divider-v {
    width: 1px;
    height: 40px;
    background: rgba(245,240,232,0.2);
    flex-shrink: 0;
  }

  /* MAIN GRID */
  main {
    padding: 60px;
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 40px;
  }

  /* SECTION LABEL */
  .section-label {
    font-family: 'DM Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--warm-gray);
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .section-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: var(--light-line);
  }

  /* PROJECT CARDS */
  .projects-col { display: flex; flex-direction: column; gap: 24px; }

  .project-card {
    border: 1px solid var(--light-line);
    padding: 28px 32px;
    position: relative;
    transition: border-color 0.2s, transform 0.2s;
    cursor: default;
    background: rgba(255,255,255,0.4);
  }

  .project-card:hover {
    border-color: var(--rust);
    transform: translateX(4px);
  }

  .project-card::before {
    content: '';
    position: absolute;
    left: 0; top: 0; bottom: 0;
    width: 3px;
    background: var(--rust);
    opacity: 0;
    transition: opacity 0.2s;
  }

  .project-card:hover::before { opacity: 1; }

  .card-top {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 12px;
  }

  .card-category {
    font-family: 'DM Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--rust);
    background: rgba(196,87,42,0.08);
    padding: 3px 8px;
    border-radius: 2px;
  }

  .card-tools {
    display: flex;
    gap: 6px;
    flex-wrap: wrap;
    justify-content: flex-end;
  }

  .tool-tag {
    font-family: 'DM Mono', monospace;
    font-size: 9px;
    color: var(--warm-gray);
    border: 1px solid var(--light-line);
    padding: 2px 7px;
    border-radius: 2px;
    letter-spacing: 0.05em;
  }

  .card-title {
    font-family: 'Playfair Display', serif;
    font-size: 20px;
    font-weight: 700;
    margin-bottom: 8px;
    line-height: 1.2;
  }

  .card-desc {
    font-size: 13px;
    line-height: 1.7;
    color: #4A4440;
    margin-bottom: 16px;
  }

  .card-outcome {
    display: flex;
    align-items: flex-start;
    gap: 10px;
    padding: 12px 16px;
    background: rgba(107,140,110,0.08);
    border-left: 2px solid var(--sage);
  }

  .outcome-icon {
    font-size: 14px;
    margin-top: 1px;
    flex-shrink: 0;
  }

  .outcome-text {
    font-size: 12px;
    color: var(--sage);
    font-weight: 500;
    line-height: 1.5;
    font-family: 'DM Mono', monospace;
    letter-spacing: 0.02em;
  }

  /* SIDEBAR */
  .sidebar { display: flex; flex-direction: column; gap: 32px; }

  .sidebar-block {
    border: 1px solid var(--light-line);
    padding: 24px;
    background: rgba(255,255,255,0.4);
  }

  .tools-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
    margin-top: 4px;
  }

  .tool-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 14px 10px;
    border: 1px solid var(--light-line);
    text-align: center;
    transition: border-color 0.2s, background 0.2s;
    cursor: default;
  }

  .tool-item:hover {
    border-color: var(--rust);
    background: rgba(196,87,42,0.04);
  }

  .tool-emoji { font-size: 20px; margin-bottom: 6px; }
  .tool-name {
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    color: var(--ink);
    letter-spacing: 0.05em;
  }
  .tool-use {
    font-size: 10px;
    color: var(--warm-gray);
    margin-top: 3px;
    line-height: 1.3;
  }

  /* TIPS BLOCK */
  .tips-list { list-style: none; margin-top: 4px; }
  .tips-list li {
    font-size: 12px;
    line-height: 1.6;
    color: #4A4440;
    padding: 10px 0;
    border-bottom: 1px solid var(--light-line);
    display: flex;
    gap: 10px;
    align-items: flex-start;
  }
  .tips-list li:last-child { border-bottom: none; }
  .tip-dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--rust);
    flex-shrink: 0;
    margin-top: 5px;
  }

  /* TIMELINE / APPROACH */
  .timeline { margin-top: 4px; }
  .tl-item {
    display: flex;
    gap: 14px;
    padding-bottom: 18px;
    position: relative;
  }
  .tl-item:not(:last-child)::before {
    content: '';
    position: absolute;
    left: 11px;
    top: 22px;
    bottom: 0;
    width: 1px;
    background: var(--light-line);
  }
  .tl-num {
    width: 22px;
    height: 22px;
    border-radius: 50%;
    background: var(--ink);
    color: var(--cream);
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    position: relative;
    z-index: 1;
  }
  .tl-content { flex: 1; }
  .tl-title {
    font-size: 12px;
    font-weight: 500;
    margin-bottom: 3px;
  }
  .tl-desc {
    font-size: 11px;
    color: var(--warm-gray);
    line-height: 1.5;
    font-family: 'DM Mono', monospace;
  }

  /* FOOTER */
  footer {
    margin: 0 60px 60px;
    padding: 24px 32px;
    background: var(--ink);
    color: var(--cream);
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 16px;
  }

  .footer-text {
    font-family: 'Playfair Display', serif;
    font-style: italic;
    font-size: 16px;
    color: rgba(245,240,232,0.7);
  }

  .footer-text strong {
    color: var(--rust);
    font-style: normal;
  }

  .footer-cta {
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--cream);
    border: 1px solid rgba(245,240,232,0.3);
    padding: 10px 20px;
  }

  @media (max-width: 900px) {
    header, .intro-strip, main, footer { padding-left: 24px; padding-right: 24px; }
    main { grid-template-columns: 1fr; }
    footer { margin-left: 24px; margin-right: 24px; }
  }

  /* ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  header { animation: fadeUp 0.5s ease both; }
  .intro-strip { animation: fadeUp 0.5s 0.1s ease both; }
  .project-card:nth-child(1) { animation: fadeUp 0.5s 0.2s ease both; }
  .project-card:nth-child(2) { animation: fadeUp 0.5s 0.3s ease both; }
  .project-card:nth-child(3) { animation: fadeUp 0.5s 0.4s ease both; }
  .project-card:nth-child(4) { animation: fadeUp 0.5s 0.5s ease both; }
  .sidebar { animation: fadeUp 0.5s 0.3s ease both; }
</style>
</head>
<body>

<header>
  <div>
    <div class="header-tag">Portfolio Guide · People Operations & HR Admin</div>
    <h1>What to Build &<br><em>How to Show It</em></h1>
  </div>
  <div class="header-meta">
    <strong>Galih</strong>
    Malang, Indonesia · UTC+7<br>
    6+ yrs · Asia-wide<br>
    $10/hr · Remote
  </div>
</header>

<div class="intro-strip">
  <div class="stat">
    <span class="stat-num">6+</span>
    <span class="stat-label">Years Experience</span>
  </div>
  <div class="divider-v"></div>
  <div class="stat">
    <span class="stat-num">C2</span>
    <span class="stat-label">English Proficiency</span>
  </div>
  <div class="divider-v"></div>
  <div class="stat">
    <span class="stat-num">5</span>
    <span class="stat-label">Portfolio Projects to Build</span>
  </div>
  <div class="divider-v"></div>
  <div class="stat">
    <span class="stat-num">3+</span>
    <span class="stat-label">Countries Coordinated</span>
  </div>
</div>

<main>

  <!-- LEFT: PROJECT CARDS -->
  <div class="projects-col">
    <div class="section-label">Portfolio Projects</div>

    <div class="project-card">
      <div class="card-top">
        <span class="card-category">HR Admin</span>
        <div class="card-tools">
          <span class="tool-tag">Google Docs</span>
          <span class="tool-tag">Canva</span>
        </div>
      </div>
      <div class="card-title">Remote Onboarding Packet</div>
      <div class="card-desc">A complete new hire kit: welcome guide, first-week checklist, tools access list, and FAQ doc. Design it for a fictional remote company spanning 3 time zones.</div>
      <div class="card-outcome">
        <span class="outcome-icon">📌</span>
        <span class="outcome-text">Show case study: "Reduced time-to-productivity from 2 weeks → 5 days"</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-top">
        <span class="card-category">SOPs & Systems</span>
        <div class="card-tools">
          <span class="tool-tag">Google Docs</span>
          <span class="tool-tag">Google Forms</span>
        </div>
      </div>
      <div class="card-title">SOP Library — 5-Doc Sample</div>
      <div class="card-desc">Build a mini SOP hub with 5 procedures: leave requests, expense submissions, IT escalation, vendor onboarding, and offboarding checklist. Document how each process flows through Odoo.</div>
      <div class="card-outcome">
        <span class="outcome-icon">📌</span>
        <span class="outcome-text">Demonstrates SOP writing + Odoo workflow knowledge — rare and in-demand combo</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-top">
        <span class="card-category">Remote Coordination</span>
        <div class="card-tools">
          <span class="tool-tag">MS Teams</span>
          <span class="tool-tag">Google Sheets</span>
        </div>
      </div>
      <div class="card-title">Time Zone Sync Protocol</div>
      <div class="card-desc">A visual meeting schedule + async communication protocol for a team spread across Indonesia, Singapore, and India. Include a weekly cadence doc and a "how we work" guide built for Teams.</div>
      <div class="card-outcome">
        <span class="outcome-icon">📌</span>
        <span class="outcome-text">Directly reflects your real Asia-wide coordination experience — very credible</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-top">
        <span class="card-category">Operations</span>
        <div class="card-tools">
          <span class="tool-tag">Monday.com</span>
          <span class="tool-tag">Google Sheets</span>
        </div>
      </div>
      <div class="card-title">HR Admin Dashboard</div>
      <div class="card-desc">A Monday.com board tracking headcount, onboarding pipeline, open roles, and vendor contracts — with a paired Google Sheets summary for reporting. Screenshot + walkthrough.</div>
      <div class="card-outcome">
        <span class="outcome-icon">📌</span>
        <span class="outcome-text">Shows you can manage data and ops systems — not just execute tasks</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-top">
        <span class="card-category">Employee Experience</span>
        <div class="card-tools">
          <span class="tool-tag">Canva</span>
          <span class="tool-tag">Google Drive</span>
        </div>
      </div>
      <div class="card-title">Remote Team Handbook</div>
      <div class="card-desc">A polished 10–15 page handbook in Canva covering communication norms, time-off policy, performance expectations, and cultural values — designed for an async-first distributed team.</div>
      <div class="card-outcome">
        <span class="outcome-icon">📌</span>
        <span class="outcome-text">Signals strategic thinking — not just admin work, but culture-building</span>
      </div>
    </div>
  </div>

  <!-- RIGHT: SIDEBAR -->
  <div class="sidebar">

    <div class="sidebar-block">
      <div class="section-label">Tools to Feature</div>
      <div class="tools-grid">
        <div class="tool-item">
          <div class="tool-emoji">📋</div>
          <div class="tool-name">Google Workspace</div>
          <div class="tool-use">Docs, Sheets, Forms, Drive</div>
        </div>
        <div class="tool-item">
          <div class="tool-emoji">🔧</div>
          <div class="tool-name">Odoo</div>
          <div class="tool-use">HR & ops management</div>
        </div>
        <div class="tool-item">
          <div class="tool-emoji">✅</div>
          <div class="tool-name">Monday.com</div>
          <div class="tool-use">Project & task tracking</div>
        </div>
        <div class="tool-item">
          <div class="tool-emoji">🎨</div>
          <div class="tool-name">Canva</div>
          <div class="tool-use">Visual docs & handbooks</div>
        </div>
        <div class="tool-item">
          <div class="tool-emoji">💬</div>
          <div class="tool-name">MS Teams</div>
          <div class="tool-use">Team comms & meetings</div>
        </div>
        <div class="tool-item">
          <div class="tool-emoji">📧</div>
          <div class="tool-name">Email / Mail</div>
          <div class="tool-use">Vendor & stakeholder comms</div>
        </div>
      </div>
    </div>

    <div class="sidebar-block">
      <div class="section-label">How to Present Each Project</div>
      <div class="timeline">
        <div class="tl-item">
          <div class="tl-num">1</div>
          <div class="tl-content">
            <div class="tl-title">State the Problem</div>
            <div class="tl-desc">What was broken or missing before you built this?</div>
          </div>
        </div>
        <div class="tl-item">
          <div class="tl-num">2</div>
          <div class="tl-content">
            <div class="tl-title">Show What You Built</div>
            <div class="tl-desc">Live Notion link, PDF export, or screenshot walkthrough</div>
          </div>
        </div>
        <div class="tl-item">
          <div class="tl-num">3</div>
          <div class="tl-content">
            <div class="tl-title">Quantify the Result</div>
            <div class="tl-desc">Time saved, errors reduced, headcount managed, etc.</div>
          </div>
        </div>
        <div class="tl-item">
          <div class="tl-num">4</div>
          <div class="tl-content">
            <div class="tl-title">Name Tools Used</div>
            <div class="tl-desc">Signals tool fluency directly to the client</div>
          </div>
        </div>
      </div>
    </div>

    <div class="sidebar-block">
      <div class="section-label">Pro Tips</div>
      <ul class="tips-list">
        <li><div class="tip-dot"></div><span>Use <strong>anonymized real work</strong> — far more credible than fictional samples</span></li>
        <li><div class="tip-dot"></div><span>Host everything on one <strong>Notion portfolio page</strong> — signals the exact tools they want</span></li>
        <li><div class="tip-dot"></div><span>Add a <strong>Loom walkthrough</strong> to at least 1 project — shows communication skills</span></li>
        <li><div class="tip-dot"></div><span>Your UTC+7 coverage is a <strong>genuine selling point</strong> — mention it in each project context</span></li>
      </ul>
    </div>

  </div>
</main>

<footer>
  <div class="footer-text">Build systems. <strong>Support people.</strong> Show both.</div>
  <div class="footer-cta">5 Projects · 1 Notion Page · Ready to Pitch</div>
</footer>

</body>
</html>
