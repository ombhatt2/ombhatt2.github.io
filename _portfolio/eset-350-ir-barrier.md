---
title: "ESET 350: Infrared Light Barrier"
excerpt: "Constructed and analyzed a MK120 infrared alarm system utilizing a 4.8 kHz modulated IR beam to act as a reliable tripwire security system."
date: 2026-05-10
header:
  teaser: /images/7.jpg
sidebar:
  - title: "Course"
    text: "ESET 350"
  - title: "Skills"
    text: "PCB Assembly, Waveform Analysis, Astable Multivibrators, Phototransistors, Circuit Troubleshooting"
  - title: "Team Members"
    text: "Om Bhatt, Anirudh Subramaniam"
---

For our ESET 350 final project, we constructed and analyzed the MK120 Infrared Alarm System. This system is designed to establish an invisible, continuous optical link between a dedicated transmitter board and a receiver circuit, acting as a reliable tripwire security system. 

To operate effectively without false triggering from ambient sunlight or room lighting, the transmitter modulates an infrared (IR) light beam at a specific high frequency of roughly 4.8 kHz using an astable multivibrator circuit. The receiver utilizes a phototransistor to constantly monitor for this exact frequency. As long as the receiver detects the pulsed IR light, the system remains in a passive state. However, when an object breaks the line of sight, the system immediately emits a loud audible alert and visual warning.

Beyond physical through-hole PCB assembly, this project involved extensive circuit analysis and validation. We captured detailed DC bench measurements and oscilloscope waveforms to analyze the performance of the astable multivibrator, LED driver transistors, and phototransistor outputs under various conditions.

### Project Report

<div style="margin-bottom: 20px;">
  <a href="/files/ESET%20350%20Project%20Report.pdf" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #800000; color: white; text-decoration: none; border-radius: 5px; font-weight: bold;">📄 Open Full Project Report in New Tab</a>
</div>

<iframe src="/files/ESET%20350%20Project%20Report.pdf" width="100%" height="600px" style="border: 1px solid rgba(128,128,128,0.3); border-radius: 8px; margin-bottom: 40px;">
  This browser does not support PDFs. Please download the PDF to view it: <a href="/files/ESET%20350%20Project%20Report.pdf">Download PDF</a>.
</iframe>

### Project Demonstrations

<div style="display: flex; flex-wrap: wrap; gap: 20px; margin-top: 20px;">
  <iframe width="400" height="225" src="https://www.youtube.com/embed/2-2afXlnSuU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 8px; flex: 1 1 300px;"></iframe>

  <iframe width="400" height="225" src="https://www.youtube.com/embed/qvinB1lXy3U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 8px; flex: 1 1 300px;"></iframe>
</div>