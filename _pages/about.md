---
permalink: /
title: "Om Bhatt"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<h2 style="margin-top: 0; font-size: 1.8em;"><span id="typed-text" class="tech-text"></span></h2>

<script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>

<script>
  var typed = new Typed('#typed-text', {
    strings: [
      'A Robotics Engineer.', 
      'A Robotics Researcher.'
    ],
    typeSpeed: 50,      // Speed of typing
    backSpeed: 30,      // Speed of backspacing
    backDelay: 1500,    // How long it pauses before deleting
    loop: true,         // Keeps it repeating forever
    showCursor: true,   // Shows the blinking cursor
    cursorChar: '|'     // The character for the cursor
  });
</script>

Welcome to my academic portfolio! I am a well-rounded student with strong academics and extracurricular experience. 

I am passionate about robotics, particularly autonomous and intelligent systems. Currently, I am seeking to expand my engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society.

## Education
**Texas A&M University** (2024-2028)
* B.S. Mechatronics Engineering
* Minor: Embedded Systems

Feel free to explore my [Portfolio](/portfolio/) and [CV](/cv/).

## Featured Projects

{% assign featured_paths = "/portfolio/2024-01-01-dron,/portfolio/robomasters,/portfolio/aeop-research,/portfolio/hatchling,/portfolio/ecotrack,/portfolio/watonobus" | split: "," %}
<div style="display:flex;flex-wrap:wrap;gap:20px;margin-top:16px;">
  {% for p in featured_paths %}
    {% assign matches = site.portfolio | where: "url", p %}
    {% if matches and matches.size > 0 %}
      {% assign item = matches[0] %}
      <div class="hover-card" style="flex:1 1 220px;max-width:320px;border:1px solid rgba(128,128,128,0.3);padding:10px;box-shadow:0 1px 0 rgba(0,0,0,0.02);">
        <a href="{{ item.url }}" style="text-decoration:none;color:inherit;">
          {% if item.header and item.header.teaser %}
            <img src="{{ item.header.teaser }}" alt="{{ item.title }}" style="width:100%;height:160px;object-fit:cover;border-radius:4px;">
          {% endif %}
          <h3 style="margin:10px 0 0 0;font-size:1.05rem;">{{ item.title }}</h3>
          {% if item.excerpt %}
            <p style="margin:6px 0 0;opacity:0.8;font-size:0.95rem;">{{ item.excerpt | strip_html | truncate:120 }}</p>
          {% endif %}
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>

<style>
  /* 1. Levitating Project Cards */
  .hover-card {
    transition: transform 0.3s cubic-bezier(0.25, 0.8, 0.25, 1), box-shadow 0.3s cubic-bezier(0.25, 0.8, 0.25, 1), background-color 0.3s ease !important;
    border-radius: 8px !important;
    background-color: transparent; /* Adapt seamlessly to light mode */
  }
  .hover-card:hover {
    transform: translateY(-8px) !important;
    box-shadow: 0 14px 28px rgba(0,0,0,0.15), 0 10px 10px rgba(0,0,0,0.1) !important;
  }

  /* 2. Interactive Profile Picture */
  .author__avatar img {
    transition: transform 0.4s ease, box-shadow 0.4s ease !important;
  }
  .author__avatar img:hover {
    transform: scale(1.05) !important;
    box-shadow: 0 0 20px rgba(128, 0, 0, 0.4) !important;
  }

  /* 3. Tech Gradient Highlight */
  .tech-text {
    background: linear-gradient(90deg, #800000, #ff4d4d);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: bold;
  }

  /* 4. Dark Theme Card Fixes */
  /* Applies the subtle glass effect ONLY when dark mode is active */
  html[data-theme="dark"] .hover-card, 
  body.dark-theme .hover-card { 
    background-color: rgba(255, 255, 255, 0.05) !important;
    backdrop-filter: blur(5px);
  }
</style>