---
permalink: /
title: "Om Bhatt"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my academic portfolio! I am a well-rounded student with strong academics and extracurricular experience. 

I am passionate about robotics, particularly autonomous and intelligent systems. Currently, I am seeking to expand my engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society.

## Education
**Texas A&M University** (2024-2028)
* B.S. Mechatronics Engineering
* Minor: Embedded Systems

Feel free to explore my [Portfolio](/portfolio/) and [CV](/cv/).

## Featured Projects

<div style="display:flex;flex-wrap:wrap;gap:20px;margin-top:16px;">
  {% for item in site.portfolio limit:4 %}
    <div style="flex:1 1 220px;max-width:320px;border:1px solid #e6e6e6;padding:10px;box-shadow:0 1px 0 rgba(0,0,0,0.02);">
      <a href="{{ item.url }}" style="text-decoration:none;color:inherit;">
        {% if item.header and item.header.teaser %}
          <img src="{{ item.header.teaser }}" alt="{{ item.title }}" style="width:100%;height:160px;object-fit:cover;border-radius:4px;">
        {% endif %}
        <h3 style="margin:10px 0 0 0;font-size:1.05rem;">{{ item.title }}</h3>
        {% if item.excerpt %}
          <p style="margin:6px 0 0 0;color:#555;font-size:0.95rem;">{{ item.excerpt | strip_html | truncate:120 }}</p>
        {% endif %}
      </a>
    </div>
  {% endfor %}
</div>