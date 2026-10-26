<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#0b1020">
  <meta name="description" content="Suraj Singh Chauhan — Data Science, SQL, Business Intelligence and automation portfolio.">
  <title>Suraj Singh Chauhan | Data & Analytics Portfolio</title>
  <style>
    :root {
      --bg: #080c18;
      --surface: rgba(18, 25, 45, .82);
      --surface-2: #111a2d;
      --text: #edf3ff;
      --muted: #a3b1ca;
      --mint: #9fe1cb;
      --violet: #a99bff;
      --line: rgba(173, 190, 225, .16);
      --shadow: 0 22px 70px rgba(0,0,0,.28);
      --radius: 22px;
      --max: 1120px;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; scroll-padding-top: 88px; }
    body {
      margin: 0; color: var(--text);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      line-height: 1.65;
      background:
        radial-gradient(ellipse at 12% 0%, rgba(94, 73, 190, .22), transparent 35rem),
        radial-gradient(ellipse at 92% 20%, rgba(30, 132, 111, .15), transparent 32rem),
        var(--bg);
    }
    a { color: inherit; text-decoration: none; }
    a:focus-visible, button:focus-visible { outline: 3px solid var(--mint); outline-offset: 4px; }
    .container { width: min(var(--max), calc(100% - 40px)); margin-inline: auto; }
    .nav-wrap { position: sticky; top: 0; z-index: 10; backdrop-filter: blur(18px); background: rgba(8,12,24,.78); border-bottom: 1px solid var(--line); }
    nav { min-height: 72px; display: flex; align-items: center; justify-content: space-between; gap: 20px; }
    .brand { font-weight: 800; letter-spacing: -.04em; font-size: 1.05rem; }
    .brand span { color: var(--mint); }
    .nav-links { display: flex; align-items: center; gap: 24px; color: var(--muted); font-size: .92rem; }
    .nav-links a:hover { color: var(--mint); }
    .menu-btn { display: none; border: 1px solid var(--line); background: var(--surface-2); color: var(--text); border-radius: 10px; padding: 8px 12px; }
    .hero { padding: 86px 0 72px; display: grid; grid-template-columns: 1.3fr .7fr; gap: 44px; align-items: center; }
    .eyebrow { display: inline-flex; align-items: center; gap: 9px; border: 1px solid rgba(159,225,203,.25); background: rgba(159,225,203,.07); color: var(--mint); border-radius: 999px; padding: 7px 13px; font-size: .82rem; font-weight: 700; }
    .pulse { width: 7px; height: 7px; border-radius: 50%; background: #65e3ad; box-shadow: 0 0 0 5px rgba(101,227,173,.12); }
    h1 { margin: 22px 0 16px; font-size: clamp(2.7rem, 6vw, 5.2rem); line-height: 1.02; letter-spacing: -.065em; }
    h1 .gradient { background: linear-gradient(100deg, var(--mint), #c7c0ff 75%); -webkit-background-clip: text; background-clip: text; color: transparent; }
    .lead { color: var(--muted); max-width: 650px; font-size: clamp(1.03rem, 1.7vw, 1.2rem); }
    .hero-actions { display: flex; flex-wrap: wrap; gap: 12px; margin: 28px 0 22px; }
    .btn { display: inline-flex; align-items: center; justify-content: center; gap: 9px; border-radius: 12px; padding: 12px 17px; font-weight: 750; border: 1px solid var(--line); transition: transform .2s, border-color .2s, background .2s; }
    .btn:hover { transform: translateY(-2px); border-color: rgba(159,225,203,.5); }
    .btn-primary { background: var(--mint); color: #08151a; border-color: transparent; }
    .btn-secondary { background: rgba(255,255,255,.035); }
    .socials { display: flex; flex-wrap: wrap; gap: 18px; color: var(--muted); font-size: .92rem; }
    .socials a:hover { color: var(--mint); }
    .hero-card { position: relative; padding: 26px; border: 1px solid var(--line); background: linear-gradient(145deg, rgba(25,35,60,.95), rgba(13,19,35,.85)); border-radius: 28px; box-shadow: var(--shadow); overflow: hidden; }
    .hero-card:before { content: ""; position: absolute; width: 190px; height: 190px; border-radius: 50%; right: -70px; top: -80px; background: rgba(169,155,255,.15); filter: blur(2px); }
    .mini-label { color: var(--muted); font-size: .78rem; text-transform: uppercase; letter-spacing: .12em; font-weight: 800; }
    .metric { padding: 18px 0; border-bottom: 1px solid var(--line); position: relative; }
    .metric:last-child { border-bottom: 0; padding-bottom: 0; }
    .metric strong { display: block; font-size: 1.3rem; letter-spacing: -.025em; }
    .metric span { color: var(--muted); font-size: .9rem; }
    section { padding: 54px 0; }
    .section-head { display: flex; align-items: end; justify-content: space-between; gap: 24px; margin-bottom: 26px; }
    .section-kicker { color: var(--mint); text-transform: uppercase; letter-spacing: .14em; font-weight: 800; font-size: .75rem; }
    h2 { font-size: clamp(1.8rem, 3vw, 2.65rem); line-height: 1.15; letter-spacing: -.045em; margin: 7px 0 0; }
    .section-desc { color: var(--muted); max-width: 520px; margin: 0; }
    .grid { display: grid; gap: 18px; }
    .grid-3 { grid-template-columns: repeat(3, minmax(0, 1fr)); }
    .grid-2 { grid-template-columns: repeat(2, minmax(0, 1fr)); }
    .panel { background: var(--surface); border: 1px solid var(--line); border-radius: var(--radius); padding: 23px; box-shadow: 0 10px 35px rgba(0,0,0,.10); }
    .panel h3 { margin: 8px 0 9px; font-size: 1.12rem; letter-spacing: -.02em; }
    .panel p { color: var(--muted); margin: 0; }
    .icon-box { width: 43px; height: 43px; display: grid; place-items: center; border-radius: 13px; background: rgba(159,225,203,.09); border: 1px solid rgba(159,225,203,.15); font-size: 1.25rem; }
    .skill-group { margin-bottom: 17px; }
    .skill-group:last-child { margin-bottom: 0; }
    .skill-top { display: flex; justify-content: space-between; gap: 14px; margin-bottom: 9px; font-weight: 700; }
    .skill-top span:last-child { color: var(--muted); font-size: .82rem; font-weight: 500; }
    .tags { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 15px; }
    .tag { color: #d8e2f7; background: rgba(169,155,255,.08); border: 1px solid rgba(169,155,255,.16); padding: 5px 10px; border-radius: 999px; font-size: .79rem; }
    .project { display: flex; flex-direction: column; min-height: 100%; }
    .project-top { display: flex; justify-content: space-between; gap: 14px; align-items: start; }
    .project-number { color: var(--mint); font: 800 .8rem ui-monospace, SFMono-Regular, Menlo, monospace; }
    .project-meta { margin-top: auto; padding-top: 20px; }
    .note { border-left: 3px solid var(--mint); padding: 12px 15px; color: var(--muted); background: rgba(159,225,203,.05); border-radius: 0 12px 12px 0; margin-top: 18px; font-size: .9rem; }
    .timeline { display: grid; gap: 14px; }
    .timeline-item { display: grid; grid-template-columns: 130px 1fr; gap: 18px; padding: 20px 0; border-bottom: 1px solid var(--line); }
    .timeline-item:last-child { border-bottom: 0; }
    .timeline-date { color: var(--mint); font-weight: 800; font-size: .86rem; }
    .timeline-item h3 { margin: 0 0 4px; font-size: 1.02rem; }
    .timeline-item p { margin: 0; color: var(--muted); }
    .contact { padding: 34px; border: 1px solid rgba(159,225,203,.23); background: linear-gradient(125deg, rgba(28,65,63,.42), rgba(30,26,63,.55)); border-radius: 28px; display: flex; align-items: center; justify-content: space-between; gap: 24px; }
    .contact h2 { margin-bottom: 10px; }
    .contact p { margin: 0; color: var(--muted); max-width: 600px; }
    footer { border-top: 1px solid var(--line); padding: 26px 0 36px; color: var(--muted); font-size: .88rem; }
    .footer-inner { display: flex; justify-content: space-between; gap: 16px; flex-wrap: wrap; }
    .muted { color: var(--muted); }
    .small { font-size: .85rem; }
    @media (max-width: 850px) {
      .hero { grid-template-columns: 1fr; padding-top: 60px; }
      .hero-card { max-width: 620px; }
      .grid-3 { grid-template-columns: repeat(2, minmax(0, 1fr)); }
      .section-head { align-items: start; flex-direction: column; }
    }
    @media (max-width: 620px) {
      .container { width: min(100% - 28px, var(--max)); }
      .nav-links { display: none; position: absolute; top: 71px; left: 0; right: 0; padding: 18px 22px 22px; flex-direction: column; align-items: start; background: #0c1222; border-bottom: 1px solid var(--line); }
      .nav-links.open { display: flex; }
      .menu-btn { display: inline-flex; }
      .hero { padding: 48px 0 42px; gap: 28px; }
      .grid-3, .grid-2 { grid-template-columns: 1fr; }
      section { padding: 38px 0; }
      .timeline-item { grid-template-columns: 1fr; gap: 5px; }
      .contact { padding: 24px; flex-direction: column; align-items: start; }
      .hero-card { padding: 21px; }
    }
    @media (prefers-reduced-motion: reduce) { html { scroll-behavior: auto; } *, *::before, *::after { transition-duration: .01ms !important; animation-duration: .01ms !important; } }
  </style>
</head>
<body>
  <div class="nav-wrap">
    <nav class="container" aria-label="Main navigation">
      <a class="brand" href="#home">Suraj<span>.</span></a>
      <button class="menu-btn" id="menuBtn" aria-expanded="false" aria-controls="navLinks">Menu ☰</button>
      <div class="nav-links" id="navLinks">
        <a href="#about">About</a><a href="#skills">Skills</a><a href="#projects">Projects</a><a href="#education">Education</a><a href="#contact">Contact</a>
      </div>
    </nav>
  </div>

  <main>
    <header class="container hero" id="home">
      <div>
        <div class="eyebrow"><span class="pulse"></span> Open to opportunities</div>
        <h1>Suraj Singh<br><span class="gradient">Chauhan.</span></h1>
        <p class="lead">Data Science &amp; Analytics aspirant turning raw data into clearer decisions through Python, SQL, business intelligence, and workflow automation.</p>
        <div class="hero-actions">
          <a class="btn btn-primary" href="#projects">Explore my work <span aria-hidden="true">↗</span></a>
          <a class="btn btn-secondary" href="mailto:ssc799978@gmail.com">Contact me <span aria-hidden="true">✉</span></a>
        </div>
        <div class="socials">
          <a href="https://www.linkedin.com/in/suraj-singh-chauhan" target="_blank" rel="noopener noreferrer">LinkedIn ↗</a>
          <a href="https://github.com/SJ563" target="_blank" rel="noopener noreferrer">GitHub ↗</a>
          <a href="mailto:ssc799978@gmail.com">Email ↗</a>
        </div>
      </div>
      <aside class="hero-card" aria-label="Portfolio highlights">
        <div class="mini-label">At a glance</div>
        <div class="metric"><strong>Data Analytics</strong><span>EDA · reporting · business insights</span></div>
        <div class="metric"><strong>Machine Learning</strong><span>Predictive modelling · segmentation</span></div>
        <div class="metric"><strong>Automation</strong><span>Power Automate Desktop · ETL workflows</span></div>
        <div class="metric"><strong>Lucknow, India</strong><span>Open to remote opportunities</span></div>
      </aside>
    </header>

    <section id="about">
      <div class="container">
        <div class="section-head">
          <div><div class="section-kicker">A little about me</div><h2>Commerce foundation.<br>Data-driven mindset.</h2></div>
          <p class="section-desc">I’m pursuing a B.Com (NEP) while building practical analytics skills through coursework and project work. I enjoy turning messy information into useful insights, dashboards, and repeatable processes.</p>
        </div>
        <div class="grid grid-3">
          <article class="panel"><div class="icon-box">📊</div><h3>Analytics &amp; BI</h3><p>Explore datasets, identify trends, and communicate findings with visualisations and dashboards.</p></article>
          <article class="panel"><div class="icon-box">🧠</div><h3>Applied Machine Learning</h3><p>Practice supervised learning, clustering, feature engineering, and model evaluation.</p></article>
          <article class="panel"><div class="icon-box">⚙️</div><h3>Workflow Automation</h3><p>Build structured data-processing workflows to reduce repetitive manual effort.</p></article>
        </div>
      </div>
    </section>

    <section id="skills">
      <div class="container">
        <div class="section-head">
          <div><div class="section-kicker">Toolkit</div><h2>Skills &amp; technologies</h2></div>
          <p class="section-desc">A working toolkit across data preparation, analysis, databases, reporting, and automation.</p>
        </div>
        <div class="grid grid-2">
          <article class="panel">
            <h3>Data &amp; Programming</h3>
            <div class="tags"><span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">NumPy</span><span class="tag">Matplotlib</span><span class="tag">Seaborn</span><span class="tag">Scikit-learn</span><span class="tag">EDA</span><span class="tag">Feature Engineering</span></div>
            <div class="note">Focus: data cleaning, exploratory analysis, model evaluation, and clear documentation.</div>
          </article>
          <article class="panel">
            <h3>Databases &amp; BI</h3>
            <div class="tags"><span class="tag">MySQL</span><span class="tag">PostgreSQL</span><span class="tag">SQL Joins</span><span class="tag">Aggregations</span><span class="tag">Power BI</span><span class="tag">Tableau</span><span class="tag">Excel</span><span class="tag">Data Modelling</span></div>
            <div class="note">Focus: querying, reporting, KPI dashboards, and business-oriented insights.</div>
          </article>
          <article class="panel">
            <h3>Automation &amp; Cloud</h3>
            <div class="tags"><span class="tag">Power Automate Desktop</span><span class="tag">ETL workflows</span><span class="tag">AWS S3</span><span class="tag">AWS EC2</span><span class="tag">Git</span><span class="tag">GitHub</span></div>
          </article>
          <article class="panel">
            <h3>Web &amp; Productivity</h3>
            <div class="tags"><span class="tag">HTML</span><span class="tag">CSS</span><span class="tag">JavaScript</span><span class="tag">PHP</span><span class="tag">MS Office</span><span class="tag">SharePoint</span><span class="tag">Teams</span><span class="tag">Outlook</span></div>
          </article>
        </div>
      </div>
    </section>

    <section id="projects">
      <div class="container">
        <div class="section-head">
          <div><div class="section-kicker">Selected work</div><h2>Projects &amp; practical experience</h2></div>
          <p class="section-desc">Coursework and academic projects that demonstrate a growing range of analytics, database, and automation skills.</p>
        </div>
        <div class="grid grid-2">
          <article class="panel project">
            <div class="project-top"><div class="icon-box">📈</div><span class="project-number">PROJECT 01</span></div>
            <h3>Data Science Coursework Projects</h3>
            <p>Explored sales, finance, and marketing datasets; practised data cleaning, exploratory analysis, customer churn prediction, segmentation, and BI reporting as part of the Kaish Computer Institute programme.</p>
            <div class="project-meta"><div class="tags"><span class="tag">Python</span><span class="tag">EDA</span><span class="tag">Random Forest</span><span class="tag">K-Means</span><span class="tag">Power BI</span></div></div>
          </article>
          <article class="panel project">
            <div class="project-top"><div class="icon-box">🗃️</div><span class="project-number">PROJECT 02</span></div>
            <h3>Institute Management System</h3>
            <p>Designed a relational database concept for student records, fee tracking, and administrative workflows, with validation, role-based access concepts, documentation, and functional testing.</p>
            <div class="project-meta"><div class="tags"><span class="tag">Database Design</span><span class="tag">SQL</span><span class="tag">RBAC</span><span class="tag">Testing</span><span class="tag">Documentation</span></div></div>
          </article>
          <article class="panel project">
            <div class="project-top"><div class="icon-box">🤖</div><span class="project-number">PROJECT 03</span></div>
            <h3>RPA Automation — Power Automate Desktop</h3>
            <p>Built an Excel-based data-processing workflow using extraction, transformation, looping, record updates, and exception handling. The source profile reports approximately 70% less manual processing effort.</p>
            <div class="project-meta"><div class="tags"><span class="tag">Power Automate</span><span class="tag">Excel</span><span class="tag">ETL</span><span class="tag">Exception Handling</span></div></div>
          </article>
          <article class="panel project">
            <div class="project-top"><div class="icon-box">📊</div><span class="project-number">PROJECT 04</span></div>
            <h3>Business Intelligence Dashboards</h3>
            <p>Practised translating metrics into stakeholder-friendly reporting views using Power BI and Tableau, including KPI measures and visual summaries.</p>
            <div class="project-meta"><div class="tags"><span class="tag">Power BI</span><span class="tag">Tableau</span><span class="tag">KPI Reporting</span><span class="tag">Data Visualisation</span></div></div>
          </article>
        </div>
        <p class="muted small" style="margin-top:16px">Tip: Add links to repositories, dashboards, screenshots, and project write-ups as you publish them.</p>
      </div>
    </section>

    <section id="education">
      <div class="container">
        <div class="section-head">
          <div><div class="section-kicker">Learning journey</div><h2>Education &amp; certifications</h2></div>
          <p class="section-desc">Academic background and training listed in my profile.</p>
        </div>
        <div class="grid grid-2">
          <article class="panel">
            <h3>🎓 Education</h3>
            <div class="timeline">
              <div class="timeline-item"><div class="timeline-date">2026 – Present</div><div><h3>B.Com (NEP), pursuing</h3><p>Lucknow Public College of Professional Studies · University of Lucknow</p></div></div>
              <div class="timeline-item"><div class="timeline-date">2024</div><div><h3>Class XII — Commerce, Economics &amp; Computer Science</h3><p>Nirmala Convent Inter College · ISC</p></div></div>
              <div class="timeline-item"><div class="timeline-date">2021</div><div><h3>Class X · 80%</h3><p>Nirmala Convent Inter College · ICSE</p></div></div>
            </div>
          </article>
          <article class="panel">
            <h3>📜 Certifications &amp; training</h3>
            <div class="timeline">
              <div class="timeline-item"><div class="timeline-date">2026 – Present</div><div><h3>Data Science Programme</h3><p>Kaish Computer Institute, Lucknow · Python, ML, EDA, SQL, Power BI, Tableau, AWS</p></div></div>
              <div class="timeline-item"><div class="timeline-date">Jun 2025</div><div><h3>Data Analytics Job Simulation</h3><p>Deloitte via Forage</p></div></div>
              <div class="timeline-item"><div class="timeline-date">Feb 2025</div><div><h3>Branch Banking Executive</h3><p>NSDC / Skill India</p></div></div>
              <div class="timeline-item"><div class="timeline-date">2023 – 2024</div><div><h3>Web Designing &amp; Development</h3><p>Kaish Computer Institute, Lucknow</p></div></div>
              <div class="timeline-item"><div class="timeline-date">Sep 2023</div><div><h3>Diploma in Computer Applications (DCA)</h3><p>STP Computer Education, Lucknow</p></div></div>
            </div>
          </article>
        </div>
        <article class="panel" style="margin-top:18px">
          <h3>🌟 Leadership &amp; volunteering</h3>
          <p><strong style="color:var(--text)">Volunteer — Youth Utsav 2024</strong> · Nehru Yuva Kendra, Lucknow · Jan 2025</p>
          <p style="margin-top:7px">Supported event logistics, multi-stakeholder communication, and structured activity documentation.</p>
        </article>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="contact">
          <div><div class="section-kicker">Let’s connect</div><h2>Have a data problem to solve?</h2><p>I’m interested in Data Analyst opportunities, junior data science pathways, and internships where I can keep learning and contribute to meaningful work.</p></div>
          <div style="display:flex;flex-wrap:wrap;gap:10px">
            <a class="btn btn-primary" href="mailto:ssc799978@gmail.com">Email me ↗</a>
            <a class="btn btn-secondary" href="https://github.com/SJ563" target="_blank" rel="noopener noreferrer">View GitHub ↗</a>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container footer-inner">
      <span>© <span id="year"></span> Suraj Singh Chauhan</span>
      <span>Designed for clarity, curiosity &amp; continuous learning.</span>
    </div>
  </footer>
  <script>
    const menuBtn = document.getElementById('menuBtn');
    const navLinks = document.getElementById('navLinks');
    menuBtn.addEventListener('click', () => {
      const open = navLinks.classList.toggle('open');
      menuBtn.setAttribute('aria-expanded', String(open));
    });
    navLinks.querySelectorAll('a').forEach(link => link.addEventListener('click', () => {
      navLinks.classList.remove('open');
      menuBtn.setAttribute('aria-expanded', 'false');
    }));
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
