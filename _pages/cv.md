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
Well-rounded student with strong academics and extracurricular experience. Passionate about robotics, particularly autonomous and intelligent systems. Seeking to expand engineering knowledge and experience to design, develop, and optimize mechatronic and robotic systems that advance automation and contribute to the betterment of society. U.S. Person (No Sponsorship Required).

Education
======
* Texas A&M University — B.S. Mechatronics Engineering, 2024–2028
  * Minor: Embedded Systems
  * Relevant Coursework: Calculus I–III, Differential Equations, Electricity & Magnetism, Engineering Mechanics, Strength of Materials, Metallic Materials, Fluid Mechanics & Power, Circuit Analysis, Analog Electronics, Digital Electronics, Embedded Systems Development in C, Microcontroller Architecture, Applied Dynamic Systems
  * Certification: Introduction to Programming using Python
  * Organizations: IEEE TAMU, ASME TAMU, TURTLE Robotics, Texas Aimbots, SOMTECH, TAMUHACK, SASE

Relevant Experience
======
* R&D Robotics Engineer — Software Subteam, T.U.R.T.L.E Robotics, Disaster Response Observation Network, Texas A&M University, Sep 2025–Present
  * Researched and programmed autonomous flight algorithms (offboard_control_square_2) using PX4 and MAVROS over ROS 2 Humble to command UAVs for a 10-member team's autonomous UAV swarm platform assisting first responders during structural fires.
  * Co-authored and presented the "Disaster Response Observation Network (DRON)" research poster across two university showcases (Nov 2025, Apr 2026), detailing autonomous swarm progress and system architecture to an audience of engineering faculty and peers.

* Hardware Team Member, Texas Aimbots, Texas A&M University, Sep 2025–Present
  * Contributing to Sentry, a fully autonomous ground robot that traverses the field and engages targets using computer vision.
  * Designed 4+ structural components, including the gimbal housing, in Onshape CAD.
  * Integrated the NVIDIA Jetson Orin, LiDAR sensors, and cameras for real-time perception and autonomous decision-making ahead of the 2026 ARC Championship, an international collegiate robotics competition.

* AEOP Summer Robotics Research Intern — LLMs for Safe Navigation REU, Oden Institute, UT Austin, Jun 2025–Aug 2025
  * Researched autonomous off-road navigation and drift/jump control dynamics under Dr. Ufuk Topcu, Dr. Christian Ellis, and PhD student Rwik Rana to architect a low-cost, 1/16 scale autonomous RC rally car research platform using ROS 2.
  * Designed and soldered custom PCBs to integrate a Raspberry Pi 5/Jetson Nano, motor controllers, and power systems.
  * Programmed a low-level controller in C++/ROS 2 for precise Ackerman steering and throttle control.
  * Established teleoperation capabilities and validated SLAM and control algorithms in the F1Tenth simulator with IMU fusion for post-jump re-localization.

* Hatchling Team Member, T.U.R.T.L.E Robotics, Jan 2025–Sep 2025
  * Won 2nd place out of 30+ teams at the 2025 TURTLE Robotics Hatchling Competition.
  * Designed mechanical components in SolidWorks, including a forklift-style lift and gripper mechanism engineered for rapid block acquisition.
  * Programmed ESP32 and Arduino controllers for precise navigation and multi-stage lift operation.

* Student Researcher — Engineering Science Fairs, Dual-axis Solar Tracker, Science Fair Club, Vista Ridge High School, Sep 2022–Mar 2024
  * Developed EcoTrack, a phototropic solar tracker using thermoresponsive polymers and no electrical tracking components.
  * Demonstrated 87% more net energy than a traditional dual-axis tracker and 119% more than a fixed panel system.
  * Earned first place at the Austin Regional Science Fair and advanced to TXSEF State Fair.
  * Received the Jacobs Engineering tuition scholarship and RICOH Sustainable Development Award.
  * Elected officer to mentor other students on their projects and showcase the school's achievements to attract sponsors.

* Mechatronics Research Intern — WATonoBus Autonomous Shuttle, Mechatronics Vehicle Systems Lab, University of Waterloo, Jun 2021–Sep 2021
  * Designed, fabricated, and programmed an LED display module to communicate shuttle intent to other road users.
  * Completed over 60 hours of development under the guidance of Professor Amir Khajepour.
  * Awarded a scholarship from MVS Lab for demonstrated excellence.

Publications
======
* I. Wilhite, C. Ambroziak, A. Briggs, R. Kato, O. Bhatt, L. Breedlove, V. So, R. Shah, M. Shi, J. Shouba, O. Thomas, C. Weatherspoon, and D. Wheaton, "Disaster Response Observation Network (DRON)," TURTLE Robotics, Apr. 2026. [Conference Poster]
* I. Wilhite, A. Briggs, C. Ambroziak, R. Kato, D. Wheaton, O. Bhatt, A. Talal, J. Shouba, C. Xu, O. Thomas, and S. Ahn, "Disaster Response Observation Network (DRON)," TURTLE Robotics, Nov. 2025. [Conference Poster]
* O. Bhatt, "Autonomous RC Rally Car for Jump and Drift Racing," under the guidance of Dr. U. Topcu, Dr. C. Ellis, and R. Rana, AEOP Summer Robotics Research REU, UT Austin, Aug. 2025. [Research Presentation & Abstract]

Volunteering and Leadership
======
* Autodesk Ambassador Program, Autodesk, Texas A&M University, Jan 2026–Present
  * Selected for a competitive ambassador program to represent Autodesk, promoting CAD tools through campus events and workshops.

* Design Review Officer, T.U.R.T.L.E Robotics, Project Branch, Jan 2026–Present
  * Provide specialized input during design reviews and Q/A discussions to improve project direction.
  * Evaluate system requirements, CAD/electronics documentation, and BOMs across 20+ projects over 3 Design Review sessions.

* Sponsorship Committee Member, T.U.R.T.L.E Robotics, External Branch, Sep 2025–Jan 2026
  * Secured corporate sponsorships through a new Corporate Sponsor Outreach Initiative.
  * Developed outreach strategies to support workshops, social events, and advanced technical projects.

* Texas Science and Engineering Fair Judge, Texas A&M University College of Engineering, Mar 2025–Present
  * Evaluated 20+ student research projects annually in the Energy: Sustainable Materials & Designs (2025) and Robotics & Intelligent Machines (2026) categories at TXSEF, providing constructive feedback to future engineers.
  * As part of judge appreciation, toured the Research Integration Center at the George H.W. Bush Combat Development Complex.

* Student Council Member, Vista Ridge High School, Sep 2022–Sep 2024
  * Contributed 20+ hours of community service through event organization, fundraising, and outreach.

Skills
======
* Robotics & Autonomy: ROS 2, PX4, MAVROS, SLAM, OpenCV, PWM/PID Control, Teleoperation, Gazebo, RViz, Point Clouds
* Hardware and Prototyping: ESP32, Arduino, Raspberry Pi, STM32, FPGA, LiDAR, Cameras, PCB Design, Soldering, Analog Electronics, Oscilloscope & DMM Testing, Data Acquisition Systems
* Programming Languages: Python, C/C++, Embedded C, Linux, Shell (Bash/Zsh), LaTeX, HTML, CSS
* Simulation and CAD: SolidWorks, FEA, Autodesk Inventor, Onshape, Bambu Studio, Eagle, Multisim, MATLAB/Simulink
* AI & Software Tools: Git/GitHub, Visual Studio Code, Workspace, Microsoft Office, LLM Integration (ChatGPT, Claude, Gemini)

Awards
======
* AEOP Summer Robotics Research REU Scholarship ($6,000), Oden Institute, Jul 2025
* 2nd Place, 2025 TURTLE Robotics Hatchling Competition, T.U.R.T.L.E Robotics, May 2025
* AP Scholar, College Board, May 2024
* Vista Ridge High School Scholar: "A" Honor Roll, May 2024
* Texas Science & Engineering Fair Finalist, TXSEF, Mar 2024
* 2nd Place, Austin Regional Science Fair, Feb 2024
* Vista Ridge High School Scholar: "A" Honor Roll, May 2023
* Texas Science & Engineering Fair Finalist, TXSEF, Mar 2023
* 1st Place, Austin Regional Science Fair, Feb 2023
* Jacobs Engineering Tuition Scholarship ($2,000), Feb 2023
* RICOH Sustainable Development Award, Feb 2023
* Summer Intern Scholarship, University of Waterloo, Jun 2021