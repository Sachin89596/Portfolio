# Portfolio
I have Designed a detailed portfolio website for me.
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portfolio — Sachin</title>
  <meta name="description" content="Personal portfolio of Your Name — projects, skills and contact." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7c5cff; --glass: rgba(255,255,255,0.04);
      --max-w:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial; background:linear-gradient(180deg,var(--bg) 0%, #071022 100%); color:#e6eef6}
    .container{max-width:var(--max-w);margin:32px auto;padding:24px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#42d4ff);display:grid;place-items:center;font-weight:800;color:#071022}
    nav{display:flex;gap:12px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;padding:8px 12px;border-radius:8px}
    nav a:hover{color:#fff;background:var(--glass)}
    .cta{background:linear-gradient(90deg,var(--accent),#42d4ff);color:#071022;padding:8px 14px;border-radius:10px;font-weight:600;text-decoration:none}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center;margin-top:28px}
    .intro h1{font-size:clamp(28px,4vw,44px);margin:0 0 8px 0}
    .intro p{color:var(--muted);line-height:1.6}
    .socials{margin-top:18px;display:flex;gap:8px}
    .btn-ghost{padding:10px 14px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted);text-decoration:none}

    /* Card */
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:14px;padding:18px;box-shadow:0 6px 20px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}
    .profile-pic{width:100%;height:320px;border-radius:10px;background:linear-gradient(180deg,#122033,#0b1726);display:flex;align-items:center;justify-content:center;color:var(--muted);font-weight:700}

    /* Sections */
    section{margin-top:28px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .projects{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:14px}
    .project{padding:14px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.015), transparent);border:1px solid rgba(255,255,255,0.03)}
    .project h4{margin:8px 0}
    .skill-list{display:flex;flex-wrap:wrap;gap:8px}
    .skill{background:var(--glass);padding:6px 10px;border-radius:999px;color:var(--muted);font-size:14px}

    footer{margin-top:42px;text-align:center;color:var(--muted);font-size:14px;padding:24px}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr}
      .profile-pic{height:220px}
      .grid-3{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:520px){
      nav{display:none}
      header{gap:12px}
      .grid-3{grid-template-columns:1fr}
    }

    /* Simple modal */
    .modal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(2,6,23,0.6);padding:20px}
    .modal.open{display:flex}
    .modal .modal-card{width:100%;max-width:720px}

    /* small helpers */
    .muted{color:var(--muted)}
    .row{display:flex;gap:12px;align-items:center}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">
          S
        </div>
        <div>
          <div style="font-weight:700">Sachin</div>
          <div class="muted" style="font-size:13px">Java Developer • Designer • Problem Solver</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
        <a class="cta" href="#contact">Hire me</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="intro">
          <div class="card">
            <h1>Hi — I&#39;m Sachin.</h1>
            <p>I build beautiful, accessible web Server and web apps. I enjoy turning complex problems into simple, elegant experiences — mostly using Java, UI/UX, and Springboot.</p>
            <div class="socials">
              <a class="btn-ghost" href="#projects">View projects</a>
              <a class="btn-ghost" href="#contact">Get in touch</a>
            </div>
            <div style="margin-top:16px;display:flex;gap:10px;align-items:center">
              <div class="row muted"><strong>📧</strong><span style="margin-left:8px">sachinsaggu7@gmail.com</span></div>
              <div class="row muted"><strong>📍</strong><span style="margin-left:8px">Haryana, India</span></div>
            </div>
          </div>

          <section id="about">
            <div class="card" style="margin-top:16px">
              <h3>About me</h3>
              <p class="muted">I am a web developer with X years of experience building user-friendly applications. My focus is Front-end and Back-end engineering, performance, and delightful user interactions. When I&#39;m not coding I enjoy photography and hiking.</p>
            </div>
          </section>

          <section id="skills">
            <div class="card" style="margin-top:16px">
              <h3>Skills</h3>
              <div class="skill-list" style="margin-top:10px">
                <span class="skill">HTML</span>
                <span class="skill">CSS</span>
                <span class="skill">JavaScript</span>
                <span class="skill">java</span>
                <span class="skill">Spring Boot</span>
                <span class="skill">Mysql</span>
                <span class="skill">MongoDB</span>
              </div>
            </div>
          </section>

        </div>

        <aside>
          <div class="card">
            <div class="profile-pic">
              <div>
                <div style="font-size:22px"><img src="c:\Users\hp\Downloads\Sachin formals pic.png" width="300" length="300"></div>
                <div class="muted" style="font-size:13px;margin-top:6px"></div>
              </div>
            </div>

            <div style="margin-top:12px">
              <h4>Contact</h4>
              <p class="muted" style="margin:6px 0">Feel free to reach out for freelance projects or full-time opportunities.</p>
              <div style="display:flex;gap:8px;margin-top:8px"><a class="btn-ghost" href="#contact">Message</a><a class="btn-ghost" href="#projects">Resume</a></div>
            </div>
          </div>
        </aside>
      </section>

      <section id="projects">
        <h2 style="margin-bottom:12px">Selected projects</h2>
        <div class="projects">
          <article class="project card">
            <h4>Project One</h4>
            <p class="muted">A short description of the project — what it does and what technologies were used.</p>
            <div style="margin-top:10px;display:flex;gap:8px">
              <button onclick="openModal('Project One','This project is a responsive web app built with HTML, CSS and vanilla JS. It features responsive layouts and accessible components.')" class="btn-ghost">Details</button>
              <a class="btn-ghost" href="#">Live</a>
            </div>
          </article>

          <article class="project card">
            <h4>Project Two</h4>
            <p class="muted">Short summary — e.g. a React SPA with authentication and an API backend.</p>
            <div style="margin-top:10px;display:flex;gap:8px">
              <button onclick="openModal('Project Two','React + Node.js app with user auth, database and deploy workflows.')" class="btn-ghost">Details</button>
              <a class="btn-ghost" href="#">Code</a>
            </div>
          </article>

          <article class="project card">
            <h4>Project Three</h4>
            <p class="muted">Short description highlighting the problem solved and the outcome.</p>
            <div style="margin-top:10px;display:flex;gap:8px">
              <button onclick="openModal('Project Three','Design-focused project with prototypes and handoff to developers.')" class="btn-ghost">Details</button>
              <a class="btn-ghost" href="#">Case study</a>
            </div>
          </article>
        </div>
      </section>

      <section id="contact">
        <h2 style="margin-top:20px">Contact</h2>
        <div class="card" style="margin-top:10px;display:flex;gap:12px;flex-wrap:wrap">
          <form id="contactForm" onsubmit="submitForm(event)" style="flex:1;min-width:260px">
            <label class="muted" style="font-size:13px">Name</label>
            <input name="name" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);margin-top:6px;background:transparent;color:inherit">
            <label class="muted" style="font-size:13px;margin-top:12px;display:block">Email</label>
            <input name="email" type="email" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);margin-top:6px;background:transparent;color:inherit">
            <label class="muted" style="font-size:13px;margin-top:12px;display:block">Message</label>
            <textarea name="message" rows="4" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);margin-top:6px;background:transparent;color:inherit"></textarea>
            <div style="margin-top:12px">
              <button type="submit" class="cta">Send message</button>
            </div>
          </form>

          <div style="min-width:220px;max-width:320px">
            <div class="card">
              <h4>Other ways to contact</h4>
              <p class="muted">Email: sachinsaggu7@gmail.com</p>
              <p class="muted">LinkedIn: /https:/LinkedIn.com/sachin-</p>
              <p class="muted">GitHub: /sachin89596</p>
            </div>
          </div>
        </div>
      </section>

    </main>

    <footer>
      © <span id="year"></span> Your Name — Built with ❤️ • <span class="muted">Made responsive & accessible</span>
    </footer>
  </div>

  <div id="modal" class="modal" onclick="closeModal(event)">
    <div class="modal-card card" role="dialog" aria-modal="true" aria-labelledby="modalTitle" onclick="event.stopPropagation()">
      <h3 id="modalTitle"></h3>
      <p id="modalBody" class="muted"></p>
      <div style="margin-top:12px;text-align:right"><button class="btn-ghost" onclick="closeModal()">Close</button></div>
    </div>
  </div>

  <script>
    // small helpers
    document.getElementById('year').textContent = new Date().getFullYear();

    function openModal(title, body){
      document.getElementById('modalTitle').textContent = title;
      document.getElementById('modalBody').textContent = body;
      document.getElementById('modal').classList.add('open');
    }
    function closeModal(e){
      if(e===undefined || e.target) document.getElementById('modal').classList.remove('open');
    }

    // contact form demo handler (replace with real endpoint)
    function submitForm(e){
      e.preventDefault();
      const f = e.target;
      const data = {name: f.name.value, email: f.email.value, message: f.message.value};
      // demo behaviour: show success modal
      openModal('Thanks, ' + (data.name||'there') + '!', 'Message sent (demo). I will get back to you at ' + data.email + '.');
      f.reset();
    }

    // Smooth scroll for internal links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const href = a.getAttribute('href');
        if(href.length>1){
          e.preventDefault();
          document.querySelector(href).scrollIntoView({behavior:'smooth',block:'start'});
        }
      });
    });
  </script>
</body>
</html>

