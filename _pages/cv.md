---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="cv-download-links">
  <a href="{{ base_path }}/files/Om_Bhatt_CV.pdf" class="btn btn--primary">Download CV as PDF</a>
</div>

College Station, TX ⋄ [{{ site.data.cv.basics.email }}](mailto:{{ site.data.cv.basics.email }}) ⋄ {{ site.data.cv.basics.phone }}

{% for profile in site.data.cv.basics.profiles %}{% if profile.url %}[{{ profile.network }}]({{ profile.url }}){% else %}{{ profile.network }}{% endif %}{% if forloop.last == false %} ⋄ {% endif %}{% endfor %}

Professional Summary
======
Well-rounded student with strong academics and extracurricular experience. Passionate about robotics, particularly autonomous and intelligent systems. Seeking to expand engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society.

Education
======
* Texas A&M University — B.S. Mechatronics Engineering, 2024–2028
  * Minor: Embedded Systems
  * Relevant Coursework: Calculus I–III, Differential Equations, Electricity & Magnetism, Engineering Mechanics, Metallic Materials, Circuit Analysis, Analog Electronics, Digital Electronics, Embedded Systems Development in C
  * Certification: Introduction to Programming using Python

Relevant Experience
======
* R&D Robotics Engineer — Software Subteam, T.U.R.T.L.E Robotics, Disaster Response Observation Network, Texas A&M University, Sep 2025–Present
  * Researched and implemented ROS 2 Humble, PX4, and MAVROS frameworks in simulation environments.
  * Supported UAV swarm platform development for first responder visual data, mapping, and low-human-input disaster response missions.

* Hardware Team Member, TAMU Robomasters, Texas A&M University, Sep 2025–Present
  * Contributed to the Sentry Robot’s fully autonomous ground vehicle design using OnShape CAD.
  * Integrated NVIDIA Jetson Orin, LiDAR sensors, and cameras for real-time perception and decision-making.

* AEOP Summer Robotics Research Intern — LLMs for Safe Navigation REU, Oden Institute, UT Austin, Jun 2025–Aug 2025
  * Architected a low-cost 1/16 scale autonomous RC rally car research platform using ROS 2.
  * Designed and soldered custom PCBs to integrate Raspberry Pi 5/Jetson Nano, motor controllers, and power systems.
  * Programmed a low-level controller in C++/ROS 2 for Ackerman steering and throttle control.
  * Established teleoperation capabilities and validated SLAM and control algorithms in the F1Tenth simulator.

* Hatchling Team Member, T.U.R.T.L.E Robotics, Jan 2025–Sep 2025
  * Won 2nd place out of 30+ teams at the 2025 TURTLE Robotics Hatchling Competition.
  * Designed mechanical components in SolidWorks, including a forklift-style lift and gripper mechanism.
  * Programmed ESP32 and Arduino controllers for precise navigation and multi-stage lift operation.

* Student Researcher — Engineering Science Fairs, Dual-axis Solar Tracker, Science Fair Club, Vista Ridge High School, Sep 2022–Mar 2024
  * Developed EcoTrack, a phototropic solar tracker using thermoresponsive polymers and no electrical tracking components.
  * Demonstrated 87% more net energy than a traditional dual-axis tracker and 119% more than a fixed panel system.
  * Earned first place at the Austin Regional Science Fair and advanced to TXSEF State Fair.
  * Received the Jacobs Engineering tuition scholarship and RICOH Sustainable Development Award.

* Mechatronics Research Intern — WATonoBus Autonomous Shuttle, Mechatronics Vehicle Systems Lab, University of Waterloo, Jun 2021–Sep 2021
  * Designed, fabricated, and programmed an LED display module to communicate shuttle intent to other road users.
  * Completed over 60 hours of development under the guidance of Professor Amir Khajepour.

Publications
======
* I. Wilhite, A. Briggs, C. Ambroziak, R. Kato, D. Wheaton, O. Bhatt, A. Talal, J. Shouba, C. Xu, O. Thomas, S. Ahn, “Disaster Response Observation Network (DRON)”, TURTLE Robotics, Nov 21st, 2025 [Showcase Poster]

Volunteering and Leadership
======
* Design Review Officer, T.U.R.T.L.E Robotics, Jan 2026–Present
  * Provide specialized input during design reviews and Q/A discussions to improve project direction.

* Sponsorship Committee Member, T.U.R.T.L.E Robotics, Sep 2025–Jan 2026
  * Secured corporate sponsorships through a Corporate Sponsor Outreach Initiative.
  * Developed outreach strategies to support workshops, social events, and advanced technical projects.

* Texas Science and Engineering Fair Judge, Texas A&M University College of Engineering, Mar 2025–Present
  * Evaluated 20+ student research projects annually in Energy: Sustainable Materials & Designs and Robotics & Intelligent Machines.
  * Provided constructive feedback to future engineers.

* Student Council Member, Vista Ridge High School, Sep 2022–Sep 2024
  * Contributed 20+ hours of community service through event organization, fundraising, and outreach.

Skills
======
* Hardware and Prototyping: ESP32, Arduino, Raspberry Pi, STM32, LiDARs, cameras, soldering, PCB design
* Programming: Python, C#, C++, ROS 2, Linux, Shell (Bash/Zsh), LaTeX
* Simulation and CAD: SolidWorks, Autodesk Inventor, Onshape, Bambu Studio, Eagle, Multisim, MATLAB

Awards
======
* AEOP Summer Robotics Research REU Scholarship, Oden Institute, Jul 2025
* 2nd Place, 2025 TURTLE Robotics Hatchling Competition
* AP Scholar, College Board, May 2024
* Vista Ridge High School Scholar: “A” Honor Roll, May 2024
* 2nd Place, Austin Regional Science Fair, Feb 2024
* Vista Ridge High School Scholar: “A” Honor Roll, May 2023
* 1st Place, Austin Regional Science Fair, Feb 2023
* Jacobs Engineering Tuition Scholarship ($2000), Feb 2023
* RICOH Sustainable Development Award, Feb 2023
* Summer Intern Scholarship, University of Waterloo, Jun 2021
