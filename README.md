# Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Portfolio of Muhammed Nihal C K - Computer Science Engineering student, programmer and cybersecurity enthusiast.">
  <title>Muhammed Nihal C K | Portfolio</title>
  <style>
    :root{
      --bg:#08111f;
      --bg2:#0d1a2d;
      --card:rgba(18,32,53,.72);
      --text:#eef5ff;
      --muted:#a9b8cc;
      --accent:#5ee7ff;
      --accent2:#7c6cff;
      --border:rgba(255,255,255,.10);
      --shadow:0 20px 60px rgba(0,0,0,.30);
    }
    *{box-sizing:border-box;margin:0;padding:0}
    html{scroll-behavior:smooth}
    body{
      font-family:Inter,Segoe UI,Arial,sans-serif;
      background:
        radial-gradient(circle at 10% 10%, rgba(124,108,255,.18), transparent 28%),
        radial-gradient(circle at 90% 20%, rgba(94,231,255,.13), transparent 25%),
        linear-gradient(135deg,var(--bg),#050b14 70%);
      color:var(--text);
      line-height:1.6;
    }
    a{color:inherit;text-decoration:none}
    .container{width:min(1120px,92%);margin:auto}
    nav{
      position:fixed;top:0;left:0;right:0;z-index:100;
      background:rgba(5,11,20,.72);
      backdrop-filter:blur(16px);
      border-bottom:1px solid var(--border);
    }
    .nav-inner{
      min-height:70px;display:flex;align-items:center;justify-content:space-between;
    }
    .logo{font-weight:800;font-size:1.15rem;letter-spacing:.4px}
    .logo span{color:var(--accent)}
    .nav-links{display:flex;gap:26px;list-style:none}
    .nav-links a{color:var(--muted);font-size:.95rem;transition:.25s}
    .nav-links a:hover{color:var(--accent)}
    .hero{min-height:100vh;display:grid;place-items:center;padding:120px 0 70px}
    .hero-grid{display:grid;grid-template-columns:1.35fr .85fr;gap:55px;align-items:center}
    .eyebrow{
      display:inline-block;padding:7px 13px;border:1px solid rgba(94,231,255,.28);
      border-radius:999px;color:var(--accent);background:rgba(94,231,255,.07);
      font-size:.85rem;margin-bottom:20px;
    }
    h1{font-size:clamp(2.8rem,7vw,5.7rem);line-height:.98;letter-spacing:-3px}
    h1 .gradient{
      background:linear-gradient(90deg,var(--accent),#b5a8ff);
      -webkit-background-clip:text;background-clip:text;color:transparent;
    }
    .hero p{max-width:680px;color:var(--muted);font-size:1.08rem;margin:25px 0}
    .buttons{display:flex;gap:14px;flex-wrap:wrap}
    .btn{
      display:inline-flex;align-items:center;justify-content:center;padding:12px 19px;
      border-radius:12px;border:1px solid var(--border);font-weight:700;transition:.25s;
    }
    .btn-primary{background:linear-gradient(135deg,var(--accent2),#3d9dff);border:none}
    .btn-secondary{background:rgba(255,255,255,.04)}
    .btn:hover{transform:translateY(-2px);box-shadow:0 10px 30px rgba(0,0,0,.25)}
    .hero-card{
      padding:30px;border:1px solid var(--border);border-radius:26px;background:var(--card);
      box-shadow:var(--shadow);position:relative;overflow:hidden;
    }
    .hero-card:before{
      content:"";position:absolute;width:180px;height:180px;border-radius:50%;
      background:rgba(94,231,255,.14);filter:blur(10px);top:-80px;right:-60px;
    }
    .terminal{font-family:"Courier New",monospace;color:#cfe4ff}
    .terminal .prompt{color:var(--accent)}
    .terminal .cmd{color:#fff}
    .terminal-line{margin:10px 0}
    .stat-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:22px}
    .stat{padding:17px;border-radius:16px;background:rgba(255,255,255,.045);border:1px solid var(--border)}
    .stat strong{font-size:1.35rem;display:block;color:var(--accent)}
    .stat small{color:var(--muted)}
    section{padding:95px 0}
    .section-title{font-size:2.2rem;margin-bottom:10px}
    .section-subtitle{color:var(--muted);margin-bottom:35px}
    .grid{display:grid;gap:20px}
    .skills-grid{grid-template-columns:repeat(4,1fr)}
    .skill-card,.project-card,.cert-card,.timeline-item{
      background:var(--card);border:1px solid var(--border);border-radius:20px;padding:24px;
      box-shadow:0 12px 35px rgba(0,0,0,.16);
    }
    .skill-card h3{margin-bottom:10px}
    .skill-card p{color:var(--muted);font-size:.95rem}
    .tags{display:flex;flex-wrap:wrap;gap:8px;margin-top:14px}
    .tag{
      padding:6px 10px;border-radius:999px;background:rgba(124,108,255,.11);
      border:1px solid rgba(124,108,255,.22);font-size:.82rem;color:#d9d4ff;
    }
    .project-card{display:grid;grid-template-columns:1fr auto;gap:25px;align-items:start}
    .project-card h3{font-size:1.4rem;margin-bottom:10px}
    .project-card p{color:var(--muted)}
    .project-icon{
      width:65px;height:65px;border-radius:18px;display:grid;place-items:center;
      background:linear-gradient(135deg,rgba(94,231,255,.18),rgba(124,108,255,.2));
      font-size:1.8rem;border:1px solid var(--border)
    }
    .cert-grid{grid-template-columns:repeat(3,1fr)}
    .cert-card{position:relative}
    .cert-card .date{color:var(--accent);font-size:.82rem;font-weight:700}
    .cert-card h3{margin:8px 0;color:#fff}
    .cert-card p{color:var(--muted)}
    .achievement-list{display:grid;gap:14px;list-style:none}
    .achievement-list li{
      padding:18px 20px;border-left:3px solid var(--accent);background:rgba(255,255,255,.035);
      border-radius:0 14px 14px 0;color:#dce7f5;
    }
    .timeline{display:grid;gap:18px}
    .timeline-item{display:flex;justify-content:space-between;gap:25px}
    .timeline-item h3{color:#fff}
    .timeline-item p{color:var(--muted)}
    .timeline-item .year{white-space:nowrap;color:var(--accent);font-weight:700}
    .contact-box{
      text-align:center;padding:50px 25px;border:1px solid var(--border);border-radius:25px;
      background:linear-gradient(135deg,rgba(124,108,255,.13),rgba(94,231,255,.07));
    }
    .contact-box p{color:var(--muted);max-width:650px;margin:12px auto 25px}
    .contact-links{display:flex;justify-content:center;gap:12px;flex-wrap:wrap}
    footer{padding:30px 0;border-top:1px solid var(--border);color:var(--muted);text-align:center}
    @media(max-width:850px){
      .hero-grid{grid-template-columns:1fr}
      .skills-grid{grid-template-columns:repeat(2,1fr)}
      .cert-grid{grid-template-columns:1fr}
      .nav-links{display:none}
    }
    @media(max-width:560px){
      h1{letter-spacing:-1.5px}
      .skills-grid{grid-template-columns:1fr}
      .project-card{grid-template-columns:1fr}
      .timeline-item{flex-direction:column;gap:6px}
      section{padding:70px 0}
    }
  </style>
</head>
<body>

<nav>
  <div class="container nav-inner">
    <a class="logo" href="#home">Nihal<span>.</span></a>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#certifications">Certifications</a></li>
      <li><a href="#achievements">Achievements</a></li>
      <li><a href="#education">Education</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</nav>

<main id="home">
  <section class="hero">
    <div class="container hero-grid">
      <div>
        <span class="eyebrow">Computer Science Engineering Student • Cybersecurity Enthusiast</span>
        <h1>Muhammed <span class="gradient">Nihal C K</span></h1>
        <p>
          A passionate Computer Science Engineering student focused on programming,
          web technologies and cybersecurity. I enjoy building practical projects,
          solving coding problems and continuously learning new technologies.
        </p>
        <div class="buttons">
          <a class="btn btn-primary" href="#projects">View My Projects</a>
          <a class="btn btn-secondary" href="mailto:mn7145676@gmail.com">Contact Me</a>
        </div>
      </div>

      <div class="hero-card">
        <div class="terminal">
          <div class="terminal-line"><span class="prompt">$</span> <span class="cmd">whoami</span></div>
          <div class="terminal-line">Muhammed Nihal C K</div>
          <div class="terminal-line"><span class="prompt">$</span> <span class="cmd">focus --area</span></div>
          <div class="terminal-line">Cybersecurity + Software Development</div>
          <div class="terminal-line"><span class="prompt">$</span> <span class="cmd">skills --core</span></div>
          <div class="terminal-line">Python | C++ | SQL | HTML | CSS | JavaScript</div>
          <div class="terminal-line"><span class="prompt">$</span> <span class="cmd">status</span></div>
          <div class="terminal-line">Learning • Building • Improving_</div>
        </div>
        <div class="stat-grid">
          <div class="stat"><strong>250+</strong><small>DSA problems solved</small></div>
          <div class="stat"><strong>3</strong><small>Professional certifications</small></div>
          <div class="stat"><strong>1</strong><small>Featured hardware project</small></div>
          <div class="stat"><strong>2025</strong><small>B.Tech started</small></div>
        </div>
      </div>
    </div>
  </section>

  <section id="about">
    <div class="container">
      <h2 class="section-title">About Me</h2>
      <p class="section-subtitle">A quick introduction.</p>
      <div class="project-card">
        <div>
          <h3>Building skills for the future of technology</h3>
          <p>
            I am pursuing a Bachelor of Technology in Computer Science and Engineering
            at Lovely Professional University. My interests include cybersecurity,
            programming, web development, networking and practical problem-solving.
            I like turning concepts into working projects and strengthening my skills
            through coding challenges and hands-on learning.
          </p>
        </div>
        <div class="project-icon">💻</div>
      </div>
    </div>
  </section>

  <section id="skills">
    <div class="container">
      <h2 class="section-title">Skills</h2>
      <p class="section-subtitle">Technologies and areas I work with.</p>
      <div class="grid skills-grid">
        <div class="skill-card">
          <h3>Programming</h3>
          <p>Languages used for problem-solving and application development.</p>
          <div class="tags"><span class="tag">Python</span><span class="tag">C++</span><span class="tag">C</span><span class="tag">SQL</span></div>
        </div>
        <div class="skill-card">
          <h3>Web Development</h3>
          <p>Building responsive and interactive web experiences.</p>
          <div class="tags"><span class="tag">HTML</span><span class="tag">CSS</span><span class="tag">JavaScript</span></div>
        </div>
        <div class="skill-card">
          <h3>Cybersecurity</h3>
          <p>Foundational knowledge in systems, networks and security tools.</p>
          <div class="tags"><span class="tag">Kali Linux</span><span class="tag">Nmap</span><span class="tag">Networking</span><span class="tag">Linux</span></div>
        </div>
        <div class="skill-card">
          <h3>Tools & Platforms</h3>
          <p>Development and database tools used for projects and learning.</p>
          <div class="tags"><span class="tag">Git</span><span class="tag">GitHub</span><span class="tag">VS Code</span><span class="tag">PostgreSQL</span><span class="tag">MySQL</span></div>
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <div class="container">
      <h2 class="section-title">Featured Project</h2>
      <p class="section-subtitle">A practical project combining programming and embedded systems.</p>
      <div class="project-card">
        <div>
          <h3>Smart Home Automation System</h3>
          <p>
            An Arduino-based project designed to automate and monitor household
            appliances using sensors and relay modules. Arduino UNO acts as the main
            controller, receiving sensor inputs and controlling devices such as lights
            and fans through relay modules.
          </p>
          <p style="margin-top:12px">
            The project integrates embedded systems, sensor technology, C programming
            and automation to create a low-cost and scalable smart-home solution.
            It can be extended with Wi-Fi connectivity, mobile applications, voice
            control, gas detection and IoT-based remote monitoring.
          </p>
          <div class="tags">
            <span class="tag">Arduino UNO</span>
            <span class="tag">C Programming</span>
            <span class="tag">DHT11 Sensor</span>
            <span class="tag">PIR Sensor</span>
            <span class="tag">Relay Module</span>
          </div>
          <div class="buttons" style="margin-top:20px">
            <a class="btn btn-secondary" href="https://github.com/nihal-creator338" target="_blank" rel="noopener">GitHub Profile ↗</a>
          </div>
        </div>
        <div class="project-icon">🏠</div>
      </div>
    </div>
  </section>

  <section id="certifications">
    <div class="container">
      <h2 class="section-title">Certifications</h2>
      <p class="section-subtitle">Recent learning and professional development.</p>
      <div class="grid cert-grid">
        <div class="cert-card">
          <div class="date">AUG 2026</div>
          <h3>Introduction to Python</h3>
          <p>Infosys Springboard</p>
        </div>
        <div class="cert-card">
          <div class="date">MAR 2026</div>
          <h3>Introduction to Artificial Intelligence</h3>
          <p>Infosys Springboard</p>
        </div>
        <div class="cert-card">
          <div class="date">AUG 2026</div>
          <h3>Networking and Web Technology</h3>
          <p>Infosys Springboard</p>
        </div>
      </div>
    </div>
  </section>

  <section id="achievements">
    <div class="container">
      <h2 class="section-title">Achievements</h2>
      <p class="section-subtitle">Highlights from coding and extracurricular activities.</p>
      <ul class="achievement-list">
        <li>🏆 Solved <strong>250+ DSA problems</strong> on LeetCode and other coding platforms.</li>
        <li>🌐 Developed practical projects using modern web technologies, strengthening problem-solving and hands-on development skills.</li>
        <li>🥊 Actively participated in boxing training and competitions, demonstrating discipline, consistency, physical fitness, confidence and a strong competitive mindset.</li>
      </ul>
    </div>
  </section>

  <section id="education">
    <div class="container">
      <h2 class="section-title">Education</h2>
      <p class="section-subtitle">Academic journey.</p>
      <div class="timeline">
        <div class="timeline-item">
          <div>
            <h3>Lovely Professional University</h3>
            <p>Bachelor of Technology — Computer Science and Engineering</p>
          </div>
          <div class="year">Aug 2025 – Present<br>Phagwara, Punjab</div>
        </div>
        <div class="timeline-item">
          <div>
            <h3>Govt. Higher Secondary School Chavassery</h3>
            <p>Intermediate — PCM • Percentage: 91.5%</p>
          </div>
          <div class="year">Jun 2023 – May 2025<br>Kannur, Kerala</div>
        </div>
        <div class="timeline-item">
          <div>
            <h3>Iritty Higher Secondary School</h3>
            <p>Matriculation • Percentage: 100%</p>
          </div>
          <div class="year">Jun 2022 – May 2023<br>Kannur, Kerala</div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="container">
      <div class="contact-box">
        <h2 class="section-title">Let's Connect</h2>
        <p>
          Interested in technology, programming and cybersecurity? Feel free to connect
          with me for opportunities, collaborations or technical discussions.
        </p>
        <div class="contact-links">
          <a class="btn btn-primary" href="mailto:mn7145676@gmail.com">Email</a>
          <a class="btn btn-secondary" href="https://www.linkedin.com/in/muhammed-nihal-770546318/" target="_blank" rel="noopener">LinkedIn ↗</a>
          <a class="btn btn-secondary" href="https://github.com/nihal-creator338" target="_blank" rel="noopener">GitHub ↗</a>
          <a class="btn btn-secondary" href="tel:+917025507649">Call</a>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="container">© 2026 Muhammed Nihal C K • Built with HTML & CSS</div>
</footer>

</body>
</html>
