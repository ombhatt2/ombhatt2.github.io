---
permalink: /
title: "Portfolio"
author_profile: true
image: https://ombhatt2.github.io/images/portfolio-preview.jpg
excerpt: "Welcome to my academic portfolio! I am a well-rounded student with strong academics and extracurricular experience. I am passionate about robotics, particularly autonomous and intelligent systems. Currently, I am seeking to expand my engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society."
redirect_from: 
  - /about/
  - /about.html
---

<div class="hero-section" data-aos="fade-up">
  <h1 class="intro-header">
    Hello, I'm Om.<br>
    <span style="font-size: 0.65em; opacity: 0.9; font-weight: 700;">A Robotics <span id="typed-text" class="tech-text"></span></span>
  </h1>

  <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
  <script>
    function startTyping() {
      if (typeof Typed !== 'undefined') {
        new Typed('#typed-text', {
          strings: ['Engineer.', 'Researcher.', 'Developer.'],
          typeSpeed: 60, backSpeed: 40, backDelay: 2000, loop: true, showCursor: true, cursorChar: '|'
        });
      } else {
        setTimeout(startTyping, 100);
      }
    }
    startTyping();
  </script>

  <p class="intro-text">
    Welcome to my academic portfolio! I am a well-rounded student with strong academics and extracurricular experience. 
  </p>
  
  <p class="intro-text">
    I am passionate about robotics, particularly autonomous and intelligent systems. Currently, I am seeking to expand my engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society.
  </p>

  <div style="margin-top: 2.5rem; margin-bottom: 4rem;">
    <a href="/files/Om_Bhatt_Resume.pdf" class="modern-resume-btn" target="_blank">
      View My Resume <i class="fas fa-arrow-right"></i>
    </a>
  </div>
</div>

<nav class="floating-nav">
  <ul>
    <li><a href="#featured-projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#leadership">Leadership</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<h2 id="featured-projects">Featured Projects</h2>

{% assign featured_paths = "/portfolio/2024-01-01-dron,/portfolio/robomasters,/portfolio/aeop-research,/portfolio/hatchling,/portfolio/ecotrack,/portfolio/watonobus" | split: "," %}
<div style="display:flex;flex-wrap:wrap;gap:25px;margin-top:16px;" class="project-grid">
  {% for p in featured_paths %}
    {% assign matches = site.portfolio | where: "url", p %}
    {% if matches and matches.size > 0 %}
      {% assign item = matches[0] %}
      <div class="hover-card" style="flex:1 1 300px;max-width:400px;border:1px solid rgba(128,128,128,0.3);padding:18px;box-shadow:0 1px 0 rgba(0,0,0,0.02);">
        <a href="{{ item.url }}" style="text-decoration:none;color:inherit;">
          {% if item.header and item.header.teaser %}
            <img src="{{ item.header.teaser }}" alt="{{ item.title }}" style="width:100%;height:220px;object-fit:cover;border-radius:6px;">
          {% endif %}
          <h3 style="margin:15px 0 0 0;font-size:1.3rem;">{{ item.title }}</h3>
          {% if item.excerpt %}
            <p style="margin:10px 0 0;opacity:0.85;font-size:1rem;line-height:1.5;">{{ item.excerpt | strip_html | truncate:140 }}</p>
          {% endif %}
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>

<h2 id="education">Education</h2>

<div data-aos="fade-up" class="glass-card">
    <div class="card-header">
        <h3 class="role">B.S. Mechatronics Engineering</h3>
        <span class="date">2024 - 2028</span>
    </div>
    <h4 class="company">Texas A&M University | Minor: Embedded Systems</h4>
    
    <div class="coursework-tags">
        <span class="course-tag">Embedded Systems in C</span>
        <span class="course-tag">Analog & Digital Electronics</span>
        <span class="course-tag">Circuit Analysis</span>
        <span class="course-tag">Engineering Mechanics</span>
        <span class="course-tag">Calculus I-III & DiffEq</span>
    </div>
</div>

<h2 id="experience">Relevant Experience</h2>

<div data-aos="fade-up" class="glass-card clickable-card">
  <a href="/portfolio/2024-01-01-dron" class="card-link-wrapper">
    <div class="card-header">
        <h3 class="role">R&D Robotics Engineer</h3>
        <span class="date">Sep 2025 - Present</span>
    </div>
    <h4 class="company">T.U.R.T.L.E Robotics, Texas A&M</h4>
    <p class="description">Collaborating to research and implement ROS 2 Humble, PX4, and MAVROS frameworks in simulation environments for a UAV swarm platform designed to assist first responders.</p>
    <div class="coursework-tags" style="margin-top: 15px;">
        <span class="course-tag">ROS 2 Humble</span>
        <span class="course-tag">PX4</span>
        <span class="course-tag">MAVROS</span>
    </div>
  </a>
</div>

<div data-aos="fade-up" class="glass-card clickable-card" data-aos-delay="100">
  <a href="/portfolio/robomasters" class="card-link-wrapper">
    <div class="card-header">
        <h3 class="role">Hardware Team Member</h3>
        <span class="date">Sep 2025 - Present</span>
    </div>
    <h4 class="company">TAMU Robomasters</h4>
    <p class="description">Designing robust structural components using OnShape CAD and integrating NVIDIA Jetson Orin, LiDAR, and cameras for a fully autonomous Sentry Robot.</p>
    <div class="coursework-tags" style="margin-top: 15px;">
        <span class="course-tag">OnShape CAD</span>
        <span class="course-tag">NVIDIA Jetson Orin</span>
        <span class="course-tag">LiDAR & Vision</span>
    </div>
  </a>
</div>

<div data-aos="fade-up" class="glass-card clickable-card" data-aos-delay="150">
  <a href="/portfolio/aeop-research" class="card-link-wrapper">
    <div class="card-header">
        <h3 class="role">Summer Robotics Research Intern</h3>
        <span class="date">Jun 2025 - Aug 2025</span>
    </div>
    <h4 class="company">Center for Autonomy, UT Austin (AEOP)</h4>
    <p class="description">Architected a 1/16 scale autonomous RC car using a C++/ROS2 software stack, achieving precise Ackerman steering and validating SLAM algorithms for complex drift and jump navigation.</p>
    <div class="coursework-tags" style="margin-top: 15px;">
        <span class="course-tag">C++ / ROS2</span>
        <span class="course-tag">SLAM Algorithms</span>
        <span class="course-tag">Low-Level Controls</span>
    </div>
  </a>
</div>

<div data-aos="fade-up" class="glass-card clickable-card" data-aos-delay="200">
  <a href="/portfolio/hatchling" class="card-link-wrapper">
    <div class="card-header">
        <h3 class="role">Hatchling Team Member</h3>
        <span class="date">Jan 2025 - Sep 2025</span>
    </div>
    <h4 class="company">T.U.R.T.L.E Robotics, Texas A&M</h4>
    <p class="description">Designed mechanical components including a forklift-style lift in SolidWorks, and programmed an ESP32/Arduino stack for vehicle navigation. Won 2nd Place out of 30+ teams at the 2025 Hatchling Competition.</p>
    <div class="coursework-tags" style="margin-top: 15px;">
        <span class="course-tag">SolidWorks</span>
        <span class="course-tag">ESP32 & Arduino</span>
        <span class="course-tag">C/C++</span>
    </div>
  </a>
</div>

<div data-aos="fade-up" class="glass-card clickable-card" data-aos-delay="300">
  <a href="/portfolio/watonobus" class="card-link-wrapper">
    <div class="card-header">
        <h3 class="role">Mechatronics Research Intern</h3>
        <span class="date">Jun 2021 - Sep 2021</span>
    </div>
    <h4 class="company">Mechatronics Vehicle Systems Lab, Univ. of Waterloo</h4>
    <p class="description">Designed, fabricated, and programmed an LED display module for the WATonoBus autonomous shuttle to communicate vehicle intentions to non-ego agents.</p>
    <div class="coursework-tags" style="margin-top: 15px;">
        <span class="course-tag">Embedded Systems</span>
        <span class="course-tag">Prototyping</span>
    </div>
  </a>
</div>

<h2 id="leadership">Leadership & Involvement</h2>

<div data-aos="fade-up" class="glass-card">
    <div class="card-header">
        <h3 class="role">Design Review Officer</h3>
        <span class="date">Jan 2026 - Present</span>
    </div>
    <h4 class="company">T.U.R.T.L.E Robotics</h4>
    <p class="description">Providing specialized technical input during design reviews and managing Q/A channels to ensure robust project progression and strict engineering standards.</p>
</div>

<div data-aos="fade-up" class="glass-card" data-aos-delay="100">
    <div class="card-header">
        <h3 class="role">Science and Engineering Fair Judge</h3>
        <span class="date">Mar 2025 - Present</span>
    </div>
    <h4 class="company">Texas Science and Engineering Fair (TXSEF)</h4>
    <p class="description">Evaluating 20+ student research projects annually in the Energy: Sustainable Materials and Robotics categories, mentoring the next generation of engineers.</p>
</div>

<p style="margin-top: 30px; font-size: 1.1em;">Feel free to explore my full <a href="/portfolio/">Portfolio</a>, <a href="/leadership/">Leadership Experience</a>, and <a href="/cv/">CV</a>.</p>

<h2 id="skills">Technical Skills</h2>

<h3 style="font-size: 1.1rem; margin-bottom: 0.8rem; color: #800000;">Programming</h3>
<div class="skill-cloud" data-aos="fade-up">
  <div class="skill-badge"><i class="fas fa-code"></i> C/C++</div>
  <div class="skill-badge"><i class="fab fa-python"></i> Python</div>
  <div class="skill-badge"><i class="fas fa-robot"></i> ROS2</div>
  <div class="skill-badge"><i class="fab fa-linux"></i> Linux</div>
  <div class="skill-badge"><i class="fas fa-terminal"></i> Shell (Bash/Zsh)</div>
  <div class="skill-badge"><i class="fas fa-subscript"></i> LaTeX</div>
</div>

<h3 style="font-size: 1.1rem; margin-top: 1.5rem; margin-bottom: 0.8rem; color: #800000;">Hardware & Prototyping</h3>
<div class="skill-cloud" data-aos="fade-up">
  <div class="skill-badge"><i class="fas fa-microchip"></i> ESP32 & STM32</div>
  <div class="skill-badge"><i class="fas fa-satellite-dish"></i> Arduino & RPi</div>
  <div class="skill-badge"><i class="fas fa-eye"></i> LiDARs & Cameras</div>
  <div class="skill-badge"><i class="fas fa-bolt"></i> Soldering</div>
  <div class="skill-badge"><i class="fas fa-network-wired"></i> PCB Design</div>
</div>

<h3 style="font-size: 1.1rem; margin-top: 1.5rem; margin-bottom: 0.8rem; color: #800000;">Simulation & CAD</h3>
<div class="skill-cloud" style="margin-bottom: 2rem;" data-aos="fade-up">
  <div class="skill-badge"><i class="fas fa-cube"></i> SolidWorks</div>
  <div class="skill-badge"><i class="fas fa-drafting-compass"></i> Onshape & Inventor</div>
  <div class="skill-badge"><i class="fas fa-print"></i> Bambu Studio</div>
  <div class="skill-badge"><i class="fas fa-microchip"></i> Eagle & Multisim</div>
  <div class="skill-badge"><i class="fas fa-laptop-code"></i> MATLAB</div>
</div>

<p style="font-size: 0.95rem; opacity: 0.8; margin-bottom: 1rem;" data-aos="fade-up"><em>Prefer the command line? Run <code>ls</code> to view my environment.</em></p>
<div class="terminal-window" data-aos="fade-up">
  <div class="terminal-header">
    <div class="terminal-buttons">
      <span class="term-btn close"></span>
      <span class="term-btn minimize"></span>
      <span class="term-btn maximize"></span>
    </div>
    <div class="terminal-title">obhatt@tamu: ~/skills</div>
  </div>
  <div class="terminal-body" id="terminal-body" onclick="document.getElementById('term-input').focus()">
    <div class="term-output" id="term-output">
      Loading OM_OS kernel... [OK]<br>
      Accessing skill databases... [OK]<br>
      Type <span class="term-highlight">'help'</span> to see a list of available commands.<br><br>
    </div>
    <div class="term-input-line">
      <span class="term-prompt">obhatt@tamu:~$</span>
      <input type="text" id="term-input" autocomplete="off" spellcheck="false">
    </div>
  </div>
</div>

<script>
  const termInput = document.getElementById('term-input');
  const termOutput = document.getElementById('term-output');
  const termBody = document.getElementById('terminal-body');

  const skillsData = {
    'programming.txt': 'C/C++, Python, ROS2, Linux, Shell (Bash/Zsh), LaTeX',
    'hardware.txt': 'ESP32 & STM32, Arduino & RPi, LiDARs & Cameras, Soldering, PCB Design',
    'simulation.txt': 'SolidWorks, Onshape, Inventor, Bambu Studio, Eagle, MATLAB'
  };

  termInput.addEventListener('keypress', function(e) {
    if (e.key === 'Enter') {
      const cmd = this.value.trim().toLowerCase();
      let response = '';
      
      if (cmd === 'help') {
        response = 'Available commands:<br><span class="term-highlight">ls</span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- List directory contents<br><span class="term-highlight">cat [file]</span> - View file contents<br><span class="term-highlight">clear</span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Clear the terminal screen';
      } else if (cmd === 'ls') {
        response = '<span class="term-file">programming.txt</span>&nbsp;&nbsp;<span class="term-file">hardware.txt</span>&nbsp;&nbsp;<span class="term-file">simulation.txt</span>';
      } else if (cmd.startsWith('cat ')) {
        const file = cmd.split(' ')[1];
        if (skillsData[file]) {
          response = `<span style="color: #f1fa8c;">${skillsData[file]}</span>`;
        } else {
          response = `cat: ${file}: No such file or directory`;
        }
      } else if (cmd === 'clear') {
        termOutput.innerHTML = '';
        this.value = '';
        return;
      } else if (cmd === 'sudo') {
        response = 'Nice try. This incident will be reported.';
      } else if (cmd === '') {
        response = '';
      } else {
        response = `Command not found: ${cmd}. Type 'help' for available commands.`;
      }

      const prevLine = `<div><span class="term-prompt">obhatt@tamu:~$</span> ${this.value}</div>`;
      const resLine = response ? `<div style="margin-bottom: 15px;">${response}</div>` : '';
      
      termOutput.innerHTML += prevLine + resLine;
      this.value = '';
      
      termBody.scrollTop = termBody.scrollHeight;
    }
  });
</script>

<div id="contact" class="modern-contact-section" data-aos="fade-up">
  <div class="contact-header">
    <h2>Get In Touch</h2>
    <p>I'm always open to discussing new projects, creative ideas, or opportunities - whether it's research, robotics, or anything in between. Feel free to reach out.</p>
  </div>

  <div class="contact-grid">
    <div class="contact-info-column">
      <div class="glass-info-card">
        <div class="info-icon">✉</div>
        <div class="info-text">
          <span>EMAIL ME</span>
          <strong>ombhatt2@gmail.com</strong>
        </div>
      </div>

      <div class="glass-info-card">
        <div class="info-icon">📍</div>
        <div class="info-text">
          <span>LOCATION</span>
          <strong>College Station, TX</strong>
        </div>
      </div>

      <div class="social-buttons-row">
        <a href="https://www.linkedin.com/in/ombhattofficial/" class="glass-social-btn">LinkedIn</a>
        <a href="https://github.com/ombhatt2" class="glass-social-btn">GitHub</a>
      </div>
    </div>

    <div class="glass-form-card">
      <form action="https://formspree.io/f/mzdqypyb" method="POST">
        <div class="form-row">
          <div class="input-group">
            <label>Your Name</label>
            <input type="text" name="name" placeholder="John Doe" required>
          </div>
          <div class="input-group">
            <label>Your Email</label>
            <input type="email" name="email" placeholder="john@example.com" required>
          </div>
        </div>
        
        <div class="input-group">
          <label>Subject</label>
          <input type="text" name="subject" placeholder="How can I help you?">
        </div>
        
        <div class="input-group">
          <label>Message</label>
          <textarea name="message" rows="5" placeholder="Tell me about your project..." required></textarea>
        </div>
        
        <button type="submit" class="submit-btn">Send Message ↗</button>
      </form>
    </div>
  </div>
</div>

<style>
  /* --- Smooth Scrolling --- */
  html {
    scroll-behavior: smooth;
  }

  /* --- Floating Right-Side Navigation --- */
  .floating-nav {
    position: fixed;
    top: 50%;
    right: 30px; /* Pins it to the right side of the window */
    transform: translateY(-50%); /* Centers it vertically */
    background: rgba(128, 128, 128, 0.05);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border: 1px solid rgba(128, 128, 128, 0.15);
    border-radius: 12px;
    padding: 20px 25px;
    z-index: 1000;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  }

  .floating-nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }

  .floating-nav a {
    text-decoration: none !important;
    font-weight: 700;
    font-size: 0.95rem;
    color: #555;
    transition: color 0.3s ease, transform 0.2s ease;
    display: block;
    text-align: right;
  }

  /* Hover effect: text turns maroon and bumps slightly left */
  .floating-nav a:hover {
    color: #800000;
    transform: translateX(-5px);
  }

  /* Dark Mode Adjustments */
  html[data-theme="dark"] .floating-nav,
  body.dark-theme .floating-nav {
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid rgba(255, 255, 255, 0.05);
  }

  html[data-theme="dark"] .floating-nav a,
  body.dark-theme .floating-nav a {
    color: #aaa;
  }

  html[data-theme="dark"] .floating-nav a:hover,
  body.dark-theme .floating-nav a:hover {
    color: #ff4d4d;
  }

  /* Hide on smaller screens (tablets/phones) so it doesn't cover text */
  @media (max-width: 1300px) {
    .floating-nav {
      display: none;
    }
  }

  /* --- Section Spacing & Centered Headings --- */
  h2 {
    text-align: center;
    font-size: 2.2rem;
    font-weight: 800;
    margin-top: 80px !important; /* Huge whitespace above sections */
    margin-bottom: 40px !important; /* Space between title and content */
    position: relative;
    padding-bottom: 15px;
  }

  /* The maroon accent line under the section titles */
  h2::after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 4px;
    background-color: #800000;
    border-radius: 2px;
  }

  /* Brighten the accent line in dark mode */
  html[data-theme="dark"] h2::after, 
  body.dark-theme h2::after {
    background-color: #ff4d4d;
  }

  /* --- Hide Auto-Generated Theme Title --- */
  h1.page__title {
    display: none !important;
  }

  /* --- Hero Section & Typography --- */
  .hero-section {
    padding-top: 10px;
  }

  .intro-header {
    font-size: 3.5rem !important;
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 25px;
    letter-spacing: -1px;
    color: var(--text-default);
  }

  @media (max-width: 768px) {
    .intro-header { font-size: 2.5rem !important; }
  }

  /* Force Intro Text to be Larger */
  .intro-text {
    font-size: 1.4rem !important; 
    line-height: 1.8 !important;
    opacity: 0.9;
    max-width: 800px; 
    margin-bottom: 20px;
  }

  /* --- Bigger Profile Picture with Tech Ring --- */
  .author__avatar img {
    max-width: 170px !important; 
    width: 100%;
    border: 3px solid #800000 !important; 
    padding: 4px; 
    background-color: transparent;
    border-radius: 50%;
    transition: transform 0.4s ease, box-shadow 0.4s ease;
  }

  .author__avatar img:hover {
    transform: scale(1.08) !important;
    box-shadow: 0 0 25px rgba(128, 0, 0, 0.5) !important;
  }

  /* 1. Levitating Project Cards */
  .hover-card {
    transition: transform 0.3s cubic-bezier(0.25, 0.8, 0.25, 1), box-shadow 0.3s cubic-bezier(0.25, 0.8, 0.25, 1), background-color 0.3s ease;
    border-radius: 8px !important;
    background-color: transparent; 
  }
  .hover-card:hover {
    transform: translateY(-8px) !important;
    box-shadow: 0 14px 28px rgba(0,0,0,0.15), 0 10px 10px rgba(0,0,0,0.1) !important;
  }

  /* 3. Tech Gradient Highlight */
  .tech-text {
    background: linear-gradient(90deg, #800000, #ff4d4d);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: bold;
  }

  /* 4. Experience & Education Glass Cards */
  .glass-card {
      background: rgba(128, 128, 128, 0.05);
      border: 1px solid rgba(128, 128, 128, 0.15);
      border-left: 4px solid #800000;
      border-radius: 8px;
      margin-bottom: 20px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
      transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
      padding: 25px;
  }

  .glass-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 30px rgba(128, 0, 0, 0.15);
      border-left: 4px solid #ff4d4d; 
  }

  /* Make whole card clickable without messing up padding */
  .clickable-card {
      padding: 0;
      overflow: hidden;
  }
  .card-link-wrapper {
      display: block;
      padding: 25px;
      text-decoration: none !important;
      color: inherit !important;
  }

  .card-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 5px;
  }

  .card-header h3 {
      margin: 0;
      font-size: 1.4em;
      font-weight: 700;
  }

  .card-header .date {
      font-family: monospace;
      color: #ff4d4d;
      font-size: 0.9em;
      letter-spacing: 1px;
  }

  .company {
      margin: 0 0 15px 0;
      font-size: 1.1em;
      opacity: 0.8;
      font-weight: 500;
  }

  .description {
      margin: 0;
      line-height: 1.6;
      font-size: 0.95em;
  }

  .coursework-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 15px;
  }

  .course-tag {
      background: rgba(128, 0, 0, 0.08);
      border: 1px solid rgba(128, 0, 0, 0.3);
      color: #b30000;
      padding: 5px 12px;
      border-radius: 4px;
      font-size: 0.8em;
      font-family: monospace;
      transition: background 0.2s ease;
  }
  
  .course-tag:hover {
      background: rgba(128, 0, 0, 0.15);
  }

  /* 5. Terminal CSS */
  .terminal-window {
      background-color: #1e1e1e;
      border-radius: 8px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
      overflow: hidden;
      font-family: 'Courier New', Courier, monospace;
      margin-bottom: 3rem;
  }

  .terminal-header {
      background-color: #323233;
      padding: 10px;
      display: flex;
      align-items: center;
      border-bottom: 1px solid #111;
  }

  .terminal-buttons {
      display: flex;
      gap: 8px;
  }

  .term-btn {
      width: 12px;
      height: 12px;
      border-radius: 50%;
  }

  .term-btn.close { background-color: #ff5f56; }
  .term-btn.minimize { background-color: #ffbd2e; }
  .term-btn.maximize { background-color: #27c93f; }

  .terminal-title {
      flex-grow: 1;
      text-align: center;
      color: #ccc;
      font-size: 0.85rem;
      letter-spacing: 1px;
      margin-right: 44px; /* Balance the buttons */
  }

  .terminal-body {
      padding: 20px;
      color: #d4d4d4;
      font-size: 0.95rem;
      height: 300px;
      overflow-y: auto;
      cursor: text;
  }

  .term-prompt {
      color: #800000;
      font-weight: bold;
      margin-right: 8px;
  }

  .term-highlight { color: #ff4d4d; font-weight: bold; }
  .term-file { color: #50fa7b; font-weight: bold; }

  .term-input-line {
      display: flex;
      align-items: center;
  }

  #term-input {
      background: transparent;
      border: none;
      color: #f1fa8c;
      font-family: 'Courier New', Courier, monospace;
      font-size: 0.95rem;
      flex-grow: 1;
      outline: none;
  }

  /* 6. Dark Theme Overrides */
  html[data-theme="dark"] .hover-card, 
  body.dark-theme .hover-card { 
    background-color: rgba(255, 255, 255, 0.05) !important;
    backdrop-filter: blur(5px);
  }
  
  html[data-theme="dark"] .glass-card, 
  body.dark-theme .glass-card {
      background: rgba(255, 255, 255, 0.02);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-left: 4px solid #800000;
  }
  
  html[data-theme="dark"] .course-tag, 
  body.dark-theme .course-tag {
      color: #ff9999;
      border-color: rgba(255, 153, 153, 0.3);
  }

  html[data-theme="dark"] .term-prompt {
      color: #ff4d4d;
  }

  @media (max-width: 768px) {
      .card-header {
          flex-direction: column;
          align-items: flex-start;
          gap: 5px;
      }
  }

/* ========================================================
     MODERN CONTACT CARD (GLASSMORPHISM + MAROON THEME)
     ======================================================== */
  
  .modern-contact-section {
    max-width: 900px;
    margin: 60px auto 100px auto;
    padding: 0 20px;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  }

  .contact-header {
    text-align: center;
    margin-bottom: 40px;
  }

  .contact-header h2 {
    font-size: 3rem !important;
    font-weight: 800;
    margin-bottom: 10px !important;
    margin-top: 0 !important;
    padding-bottom: 0 !important;
    letter-spacing: -1px;
  }
  
  .contact-header h2::after {
    display: none; /* Removes the maroon line just for this header to keep it clean */
  }

  .contact-header p {
    font-size: 1.15rem;
    opacity: 0.8;
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.6;
  }

  .contact-grid {
    display: grid;
    grid-template-columns: 1fr 1.5fr;
    gap: 30px;
    margin-top: 40px;
  }

  /* --- LEFT COLUMN: INFO CARDS --- */
  .contact-info-column {
    display: flex;
    flex-direction: column;
    gap: 15px;
  }

  .glass-info-card {
    background: rgba(128, 128, 128, 0.05);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border: 1px solid rgba(128, 128, 128, 0.15);
    border-radius: 12px;
    padding: 20px;
    display: flex;
    align-items: center;
    gap: 15px;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.04);
    transition: transform 0.2s ease, border-color 0.2s ease;
  }

  .glass-info-card:hover {
    transform: translateY(-3px);
    border-color: rgba(128, 0, 0, 0.3);
  }

  .info-icon {
    font-size: 1.5rem;
    color: #800000;
    background: rgba(128, 0, 0, 0.08);
    width: 50px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px;
  }

  .info-text span {
    display: block;
    font-size: 0.75rem;
    font-weight: 700;
    color: #888888;
    letter-spacing: 1px;
    text-transform: uppercase;
    margin-bottom: 3px;
  }

  .info-text strong {
    font-size: 1rem;
    color: var(--text-default);
  }

  .social-buttons-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
    margin-top: 5px;
  }

  .glass-social-btn {
    background: rgba(128, 128, 128, 0.05);
    backdrop-filter: blur(12px);
    border: 1px solid rgba(128, 128, 128, 0.15);
    border-radius: 12px;
    padding: 15px;
    text-align: center;
    font-weight: 700;
    color: var(--text-default);
    text-decoration: none !important;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.04);
    transition: all 0.2s ease;
  }

  .glass-social-btn:hover {
    background: #800000;
    color: #ffffff !important;
    transform: translateY(-3px);
  }

  /* --- RIGHT COLUMN: CONTACT FORM --- */
  .glass-form-card {
    background: rgba(128, 128, 128, 0.05);
    backdrop-filter: blur(12px);
    border: 1px solid rgba(128, 128, 128, 0.15);
    border-radius: 16px;
    padding: 35px;
    box-shadow: 0 12px 35px rgba(0, 0, 0, 0.06);
  }

  .form-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }

  .input-group {
    margin-bottom: 20px;
  }

  .input-group label {
    display: block;
    font-size: 0.85rem;
    font-weight: 600;
    color: var(--text-default);
    margin-bottom: 8px;
  }

  .input-group input, 
  .input-group textarea {
    width: 100%;
    padding: 14px;
    background: rgba(128, 128, 128, 0.05);
    border: 1px solid rgba(128, 128, 128, 0.2);
    border-radius: 8px;
    font-family: inherit;
    font-size: 0.95rem;
    color: var(--text-default);
    transition: all 0.2s ease;
    box-sizing: border-box;
  }

  .input-group input:focus, 
  .input-group textarea:focus {
    outline: none;
    background: rgba(255, 255, 255, 0.8);
    border-color: #800000;
    box-shadow: 0 0 0 3px rgba(128, 0, 0, 0.1);
  }

  .submit-btn {
    width: 100%;
    background: #800000;
    color: #ffffff;
    border: none;
    border-radius: 8px;
    padding: 16px;
    font-size: 1rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.2s ease;
  }

  .submit-btn:hover {
    background: #600000;
    box-shadow: 0 6px 20px rgba(128, 0, 0, 0.2);
    transform: translateY(-2px);
  }

  /* Responsive Design for Mobile */
  @media (max-width: 768px) {
    .contact-grid {
      grid-template-columns: 1fr;
    }
    .form-row {
      grid-template-columns: 1fr;
    }
    .glass-form-card {
      padding: 25px;
    }
  }

  /* ========================================================
     CYBERPUNK / NEON BACKGROUND & GLOW EFFECTS (DARK MODE)
     ======================================================== */
     
  /* 1. Add Neon Glow Behind the Contact Section */
  html[data-theme="dark"] .modern-contact-section,
  body.dark-theme .modern-contact-section {
    position: relative;
    z-index: 1;
  }

  html[data-theme="dark"] .modern-contact-section::before,
  body.dark-theme .modern-contact-section::before {
    content: "";
    position: absolute;
    top: -50px; left: -50px; right: -50px; bottom: -50px;
    z-index: -1;
    background-image: 
      radial-gradient(circle at 15% 50%, rgba(255, 77, 77, 0.15), transparent 40%),
      radial-gradient(circle at 85% 50%, rgba(128, 0, 0, 0.2), transparent 40%),
      linear-gradient(rgba(255, 77, 77, 0.05) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255, 77, 77, 0.05) 1px, transparent 1px);
    background-size: 100% 100%, 100% 100%, 30px 30px, 30px 30px;
    pointer-events: none;
    border-radius: 20px;
  }

  /* 2. Text Brightness Fixes */
  html[data-theme="dark"] .contact-header h2,
  body.dark-theme .contact-header h2,
  html[data-theme="dark"] .contact-header p,
  body.dark-theme .contact-header p {
    color: #e0e0e0 !important;
    text-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
  }
  
  html[data-theme="dark"] .info-text span,
  body.dark-theme .info-text span {
    color: #aaaaaa !important;
  }

  html[data-theme="dark"] .info-text strong,
  body.dark-theme .info-text strong,
  html[data-theme="dark"] .glass-social-btn,
  body.dark-theme .glass-social-btn,
  html[data-theme="dark"] .input-group label,
  body.dark-theme .input-group label {
    color: #ffffff !important; 
  }

  /* 3. Neon Edge-Glow for the Left Info Cards */
  html[data-theme="dark"] .glass-info-card,
  body.dark-theme .glass-info-card,
  html[data-theme="dark"] .glass-social-btn,
  body.dark-theme .glass-social-btn {
    background: rgba(15, 15, 20, 0.7) !important;
    border: 1px solid rgba(255, 77, 77, 0.3) !important;
    box-shadow: 0 0 15px rgba(255, 77, 77, 0.1), inset 0 0 10px rgba(255, 77, 77, 0.05) !important;
  }

  /* Intense Neon Flare on Hover */
  html[data-theme="dark"] .glass-info-card:hover,
  body.dark-theme .glass-info-card:hover,
  html[data-theme="dark"] .glass-social-btn:hover,
  body.dark-theme .glass-social-btn:hover {
    border-color: #ff4d4d !important;
    box-shadow: 0 0 25px rgba(255, 77, 77, 0.5), inset 0 0 15px rgba(255, 77, 77, 0.2) !important;
  }

  /* 4. Neon Edge-Glow for the Main Form Box */
  html[data-theme="dark"] .glass-form-card,
  body.dark-theme .glass-form-card {
    background: rgba(15, 15, 20, 0.7) !important;
    border: 1px solid rgba(255, 77, 77, 0.2) !important;
    box-shadow: 0 0 40px rgba(255, 77, 77, 0.15), inset 0 0 20px rgba(255, 77, 77, 0.05) !important;
  }

  /* 5. Cyberpunk Input Fields */
  html[data-theme="dark"] .input-group input,
  body.dark-theme .input-group input,
  html[data-theme="dark"] .input-group textarea,
  body.dark-theme .input-group textarea {
    background: rgba(0, 0, 0, 0.5) !important;
    border: 1px solid rgba(255, 255, 255, 0.15) !important;
    color: #ffffff !important;
  }

  html[data-theme="dark"] .input-group input::placeholder,
  body.dark-theme .input-group input::placeholder,
  html[data-theme="dark"] .input-group textarea::placeholder,
  body.dark-theme .input-group textarea::placeholder {
    color: rgba(255, 255, 255, 0.4) !important;
  }
  
  html[data-theme="dark"] .input-group input:focus,
  body.dark-theme .input-group input:focus,
  html[data-theme="dark"] .input-group textarea:focus,
  body.dark-theme .input-group textarea:focus {
    background: rgba(0, 0, 0, 0.8) !important;
    border-color: #ff4d4d !important;
    box-shadow: 0 0 15px rgba(255, 77, 77, 0.4) !important;
  }
  
</style>