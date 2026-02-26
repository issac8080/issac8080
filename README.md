<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Issac Sunny — Professional Card-based README</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&family=JetBrains+Mono:wght@600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0d1117; --card:#0f1720; --muted:#94a3b8; --accent:#00d9ff; --accent-2:#64ffda; --pink:#ff6b9d;
      --glass: rgba(255,255,255,0.04);
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#071028 0%, #0b1020 60%);font-family:Inter,system-ui,Segoe UI,Roboto,"Helvetica Neue",Arial;}
    .wrap{max-width:1100px;margin:32px auto;padding:28px;display:grid;gap:22px;grid-template-columns:1fr;}

    /* Header */
    .header{display:flex;gap:18px;align-items:center}
    .hero-img{flex:0 0 100%;border-radius:12px;overflow:hidden;box-shadow:0 8px 30px rgba(2,6,23,0.7)}
    .title{display:flex;flex-direction:column;gap:8px}
    .name{font-family:'JetBrains Mono',monospace;font-size:28px;color:var(--accent);letter-spacing:0.8px}
    .role{font-weight:600;color:var(--accent-2)}
    .subtitle{color:var(--muted);font-size:14px}

    /* Grid of cards */
    .grid{display:grid;grid-template-columns:repeat(12,1fr);gap:18px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:14px;padding:18px;box-shadow:0 6px 18px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}
    .card--full{grid-column:span 12}
    .card--left{grid-column:span 4}
    .card--mid{grid-column:span 4}
    .card--right{grid-column:span 4}

    @media(max-width:900px){.card--left,.card--mid,.card--right{grid-column:span 12}.header{flex-direction:column}}

    h3{margin:0 0 10px 0;color:var(--accent);font-size:16px}
    p{margin:0;color:var(--muted);line-height:1.5}

    /* tech badges grid */
    .badges{display:flex;flex-wrap:wrap;gap:8px}
    .badge{padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:13px;color:#fff}

    /* buttons & links */
    .links{display:flex;gap:8px;flex-wrap:wrap}
    .btn{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border-radius:10px;background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#05131a;font-weight:700;text-decoration:none}
    .muted-link{color:var(--muted);font-weight:600;text-decoration:none;padding:8px 10px;border-radius:8px;background:transparent}

    /* stats image sizing */
    .stats{display:flex;gap:12px;flex-direction:column}
    .stats img{width:100%;height:auto;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}

    /* small list */
    ul.meta{padding:0;margin:8px 0 0 0;list-style:none;display:flex;flex-direction:column;gap:6px}
    ul.meta li{color:var(--muted);font-size:14px}

    /* floating/soft animations */
    .float{animation:float 6s ease-in-out infinite}
    @keyframes float{0%{transform:translateY(0)}50%{transform:translateY(-6px)}100%{transform:translateY(0)}}

    /* footer / connectors */
    .connects{display:flex;gap:10px;align-items:center;flex-wrap:wrap}

    /* minimal code block look */
    .mono{font-family:'JetBrains Mono',monospace;font-size:13px;color:var(--muted);background:var(--glass);padding:8px;border-radius:8px}
  </style>
</head>
<body>
  <main class="wrap">

    <!-- Header -->
    <section class="header card card--full">
      <div style="display:flex;gap:18px;align-items:center;width:100%">
        <div style="flex:1">
          <img class="hero-img float" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,16,19&height=140&section=header&text=&fontSize=0&animation=fadeIn" alt="Header" />
        </div>
        <div class="title" style="flex:0 0 420px;min-width:260px">
          <div class="name">&lt;/&gt; ISSAC SUNNY; { Software Engineer }</div>
          <div class="role">Building Digital Experiences — Performance Obsessed</div>
          <div class="subtitle">Crafting fast, maintainable & delightful web applications · Open-source contributor</div>
          <div style="margin-top:10px;display:flex;gap:8px">
            <a class="btn" href="https://github.com/issac8080" target="_blank">GitHub</a>
            <a class="muted-link" href="https://www.linkedin.com/in/issacsunny" target="_blank">LinkedIn</a>
            <a class="muted-link" href="mailto:your.email@example.com">Email</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Top cards: About / Tech / Stats -->
    <section class="grid card--full">

      <article class="card card--left">
        <h3>About</h3>
        <p>Passionate software engineer focused on building scalable, performant user experiences. I write clear, testable code and love optimizing runtime and bundle size. Outside of work I enjoy learning new languages and contributing to open-source tools.</p>

        <ul class="meta">
          <li>🎯 Focus: Frontend architecture, performance & accessibility</li>
          <li>⚡ Strengths: React, TypeScript, Next.js, Web performance</li>
          <li>🌱 Mindset: Continuous learning, mentoring & clean code</li>
        </ul>

      </article>

      <article class="card card--mid">
        <h3>Tech Stack</h3>
        <div class="badges" style="margin-top:8px">
          <!-- keep the badges you already used but presented as neat chips -->
          <span class="badge">React</span>
          <span class="badge">Next.js</span>
          <span class="badge">TypeScript</span>
          <span class="badge">JavaScript</span>
          <span class="badge">Tailwind CSS</span>
          <span class="badge">Node.js</span>
          <span class="badge">PostgreSQL</span>
          <span class="badge">Docker</span>
          <span class="badge">AWS</span>
          <span class="badge">Vercel</span>
        </div>

        <h3 style="margin-top:14px">Currently Learning</h3>
        <div class="badges">
          <span class="badge">Rust</span>
          <span class="badge">Go</span>
          <span class="badge">Three.js</span>
          <span class="badge">Web3.js</span>
        </div>
      </article>

      <article class="card card--right stats">
        <h3>GitHub Stats</h3>
        <img src="https://github-readme-stats.vercel.app/api?username=issac8080&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0D1117&title_color=00D9FF&icon_color=64FFDA" alt="GitHub stats" />
        <img style="margin-top:10px" src="https://github-readme-stats.vercel.app/api/top-langs/?username=issac8080&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00D9FF&text_color=64FFDA" alt="Top languages" />
      </article>

    </section>

    <!-- Middle row: Activity / Projects / Insights -->
    <section class="grid card--full">
      <article class="card card--left">
        <h3>Activity</h3>
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=issac8080&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=00D9FF&line=64FFDA&point=FF6B9D&area=true&area_color=00D9FF" alt="Activity graph" />
        <p style="margin-top:8px" class="mono">Contributions · Commits · Issues · PRs</p>
      </article>

      <article class="card card--mid">
        <h3>Projects</h3>
        <p>Open-source projects & prototypes focused on UX, performance and developer tooling.</p>
        <ul class="meta" style="margin-top:8px">
          <li>• Urban Place — AI-governed home services marketplace</li>
          <li>• Performance analyzer — bundle & runtime insights</li>
          <li>• Component library — accessible, themeable UI</li>
        </ul>
        <div style="margin-top:12px" class="links">
          <a class="muted-link" href="https://github.com/issac8080">View repos</a>
          <a class="muted-link" href="#projects">Case studies</a>
        </div>
      </article>

      <article class="card card--right">
        <h3>Insights</h3>
        <p>I write about performance best-practices, front-end architecture and practical optimizations.</p>
        <div style="margin-top:12px" class="connects">
          <a class="muted-link" href="#blog">Latest posts</a>
          <a class="muted-link" href="#notes">Notes & snippets</a>
        </div>
      </article>
    </section>

    <!-- Lower row: Connect / Contact / Jokes / Visitor -->
    <section class="grid card--full">
      <article class="card card--left">
        <h3>Connect</h3>
        <div class="connects" style="margin-top:8px">
          <a class="muted-link" href="https://www.linkedin.com/in/issacsunny">LinkedIn</a>
          <a class="muted-link" href="mailto:your.email@example.com">Email</a>
          <a class="muted-link" href="https://github.com/issac8080">GitHub</a>
        </div>

        <h3 style="margin-top:12px">Contact</h3>
        <p class="mono">your.email@example.com · Available for freelance & collaborations</p>
      </article>

      <article class="card card--mid">
        <h3>Fun</h3>
        <p>Visitor counter and a rotating joke card to keep things friendly and approachable.</p>
        <div style="margin-top:8px">
          <img src="https://komarev.com/ghpvc/?username=issac8080&color=00D9FF&style=for-the-badge" alt="Profile Views" />
        </div>
        <div style="margin-top:8px">
          <img src="https://readme-jokes.vercel.app/api?theme=tokyonight&hideBorder=true&bgColor=0D1117&textColor=64FFDA&qColor=00D9FF&aColor=FF6B9D" alt="Random Joke" />
        </div>
      </article>

      <article class="card card--right">
        <h3>Quick Links</h3>
        <ul class="meta">
          <li><a class="muted-link" href="#resume">Resume</a></li>
          <li><a class="muted-link" href="#projects">Projects</a></li>
          <li><a class="muted-link" href="#blog">Blog</a></li>
        </ul>
      </article>
    </section>

    <!-- Footer animation -->
    <section class="card card--full" style="text-align:center">
      <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,16,19&height=110&section=footer&text=Thanks+for+visiting!+%F0%9F%9A%80&fontSize=28&animation=fadeIn&fontColor=ffffff" alt="footer" style="border-radius:10px;" />
    </section>

  </main>
</body>
</html>
