<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ranjitha J U — Full Stack Developer</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7c3aed; --accent-2:#f59e0b;
      --glass: rgba(255,255,255,0.03);
    }
    [data-theme="light"]{
      --bg:#f6f8fb; --card:#ffffff; --muted:#475569; --accent:#6b21a8; --accent-2:#b45309; --glass: rgba(2,6,23,0.04);
    }

    *{box-sizing:border-box;font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;}
    body{margin:0; min-height:100vh; background:linear-gradient(180deg,var(--bg), #081023 120%); color: #e6eef8; display:flex; align-items:center; justify-content:center; padding:40px;}
    .wrap{width:100%; max-width:920px; background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border-radius:16px; padding:28px; box-shadow:0 10px 30px rgba(2,6,23,0.6); border:1px solid rgba(255,255,255,0.03);}
    .top{display:flex; gap:20px; align-items:center;}
    .avatar{
      width:120px; height:120px; border-radius:20px; overflow:hidden; flex:0 0 120px;
      background:linear-gradient(135deg,var(--accent),var(--accent-2)); display:flex; align-items:center; justify-content:center; color:#fff; font-weight:700; font-size:28px; box-shadow:0 6px 20px rgba(7,12,24,0.6);
    }
    .info h1{margin:0; font-size:28px; letter-spacing:0.2px;}
    .role{margin-top:6px; color:var(--muted); font-weight:600;}
    .badges{margin-top:12px; display:flex; gap:8px; flex-wrap:wrap;}
    .badge{background:var(--glass); padding:6px 10px; border-radius:999px; font-weight:600; color:var(--muted); font-size:13px; border:1px solid rgba(255,255,255,0.02);}
    .badge.highlight{background:linear-gradient(90deg,var(--accent),var(--accent-2)); color:white; box-shadow:0 6px 18px rgba(124,58,237,0.12); border:none;}
    .actions{margin-left:auto; display:flex; gap:8px; align-items:center;}
    .btn{background:transparent; border:1px solid rgba(255,255,255,0.06); padding:8px 12px; border-radius:10px; color:var(--muted); cursor:pointer; font-weight:600;}
    .btn.primary{background:var(--accent); color:white; border:none;}
    .content{display:grid; grid-template-columns:1fr 320px; gap:22px; margin-top:22px;}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005)); padding:18px; border-radius:12px; border:1px solid rgba(255,255,255,0.02);}
    .about p{color:var(--muted); margin:0 0 12px 0; line-height:1.5;}
    .skills{display:flex; gap:8px; flex-wrap:wrap;}
    .skill{padding:8px 10px; border-radius:8px; background:rgba(255,255,255,0.02); color:var(--muted); font-weight:600; font-size:13px; border:1px solid rgba(255,255,255,0.02);}
    .skill.java{background:linear-gradient(90deg,#f59e0b,#d97706); color:#081023; box-shadow:0 6px 15px rgba(213,119,6,0.12);}
    .projects{display:flex; flex-direction:column; gap:10px;}
    .proj{padding:10px; border-radius:10px; background:rgba(255,255,255,0.015); display:flex; justify-content:space-between; align-items:center; border:1px solid rgba(255,255,255,0.02);}
    .proj .meta{color:var(--muted); font-size:14px;}
    .side .section-title{font-weight:700; margin-bottom:12px;}
    .contact a{display:inline-block; margin-right:8px; margin-bottom:8px; font-weight:700; color:var(--muted); text-decoration:none; padding:8px 10px; border-radius:8px; background:rgba(255,255,255,0.02); border:1px solid rgba(255,255,255,0.02);}
    footer{margin-top:18px; color:var(--muted); font-size:13px; text-align:center;}

    /* small screens */
    @media (max-width:820px){
      .content{grid-template-columns:1fr; padding-top:10px;}
      .actions{margin-left:0;}
      .top{flex-direction:column; align-items:flex-start;}
    }
  </style>
</head>
<body data-theme="dark">
  <div class="wrap" role="main" aria-labelledby="title">
    <div class="top">
      <div class="avatar" aria-hidden="true">RJ</div>
      <div class="info">
        <h1 id="title">Ranjitha J U <span style="font-weight:500; color:var(--muted); font-size:16px">— Full Stack Developer</span></h1>
        <div class="role">Building polished web & backend experiences • Passion: clean code & scalable systems</div>
        <div class="badges">
          <span class="badge">Full Stack</span>
          <span class="badge highlight">Java Developer</span>
          <span class="badge">React</span>
          <span class="badge">Node.js</span>
          <span class="badge">SQL & NoSQL</span>
        </div>
      </div>

      <div class="actions" aria-hidden="false">
        <button class="btn" id="themeToggle" title="Toggle theme">Toggle theme</button>
        <a class="btn primary" href="#" id="downloadCV">Download CV</a>
      </div>
    </div>

    <div class="content" role="region" aria-label="Profile content">
      <div>
        <section class="card about" aria-labelledby="aboutTitle">
          <h2 id="aboutTitle">About</h2>
          <p>Hi — I'm <strong>Ranjitha J U</strong>, a Full Stack Developer with a strong emphasis on Java backend development and modern frontend frameworks. I enjoy turning ideas into production-grade features and focusing on developer experience, testability, and performance.</p>
          <p class="muted">Open to collaboration, internships, and opportunities to build impactful products.</p>

          <h3 style="margin-top:14px">Core skills</h3>
          <div class="skills" role="list">
            <span class="skill java" role="listitem">Java</span>
            <span class="skill" role="listitem">Spring Boot</span>
            <span class="skill" role="listitem">REST & GraphQL</span>
            <span class="skill" role="listitem">React</span>
            <span class="skill" role="listitem">Node.js</span>
            <span class="skill" role="listitem">TypeScript</span>
            <span class="skill" role="listitem">Docker</span>
            <span class="skill" role="listitem">CI / CD</span>
          </div>
        </section>

        <section class="card projects" aria-labelledby="projTitle" style="margin-top:14px">
          <h2 id="projTitle">Selected projects</h2>

          <div class="proj">
            <div>
              <div style="font-weight:700">Premium Formal Wear Shop (Demo)</div>
              <div class="meta">React • Tailwind • Node • Stripe</div>
            </div>
            <div><a href="#" style="text-decoration:none; color:var(--muted)">View</a></div>
          </div>

          <div class="proj">
            <div>
              <div style="font-weight:700">TaskManager API</div>
              <div class="meta">Java • Spring Boot • PostgreSQL</div>
            </div>
            <div><a href="#" style="text-decoration:none; color:var(--muted)">View</a></div>
          </div>

          <div class="proj">
            <div>
              <div style="font-weight:700">Portfolio + Blog</div>
              <div class="meta">Gatsby / React • Markdown • Netlify</div>
            </div>
            <div><a href="#" style="text-decoration:none; color:var(--muted)">View</a></div>
          </div>
        </section>
      </div>

      <aside class="side">
        <div class="card contact" aria-labelledby="contactTitle">
          <div class="section-title" id="contactTitle">Contact</div>
          <div style="margin-bottom:10px; color:var(--muted)">Let's connect — available for internships and junior/full-stack roles</div>
          <a href="mailto:your-email@example.com">Email</a>
          <a href="https://www.linkedin.com/in/your-linkedin" target="_blank" rel="noopener">LinkedIn</a>
          <a href="https://github.com/your-github" target="_blank" rel="noopener">GitHub</a>
        </div>

        <div class="card" style="margin-top:12px">
          <div class="section-title">Stats & interests</div>
          <div style="color:var(--muted); font-size:14px; line-height:1.5">
            🔭 Interested in Java microservices and cloud-native design.<br/>
            📚 Learning: distributed systems, design patterns, performance tuning.<br/>
            ⚡ Fun: UI design, minimal animations, and developer tooling.
          </div>
        </div>
      </aside>
    </div>

    <footer>
      Built with ♥ — <strong>Ranjitha J U</strong> • Full Stack & Java Developer
    </footer>
  </div>

  <script>
    // small interactions: theme toggle + dummy CV download
    const themeBtn = document.getElementById('themeToggle');
    const downloadBtn = document.getElementById('downloadCV');
    const root = document.body;

    function setTheme(t){
      root.setAttribute('data-theme', t);
      localStorage.setItem('theme', t);
    }
    themeBtn.addEventListener('click', () => {
      const current = root.getAttribute('data-theme') === 'dark' ? 'dark' : 'dark';
      const next = (localStorage.getItem('theme') === 'dark') ? 'light' : 'dark';
      setTheme(next);
    });
    // initialize
    if(localStorage.getItem('theme')) root.setAttribute('data-theme', localStorage.getItem('theme'));

    downloadBtn.addEventListener('click', (e) => {
      e.preventDefault();
      // simple generated CV file (replace with real link if you have one)
      const cvText = `Ranjitha J U — Full Stack Developer\n\nSkills:\n- Java, Spring Boot\n- React, Node.js\n- Databases, Docker\n\nContact: your-email@example.com`;
      const blob = new Blob([cvText], {type: 'text/plain'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'Ranjitha_JU_CV.txt';
      document.body.appendChild(a); a.click(); a.remove();
      URL.revokeObjectURL(url);
    });
  </script>
</body>
</html>
