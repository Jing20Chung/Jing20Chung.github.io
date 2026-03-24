---
layout: default
title: "Xhaler"
date: 2025-01-12
image: "/assets/images/projects/xhaler/thumbnail.png"
description_title: "A VR game exploring breathing as a core mechanic."
description: "Xhaler is a VR adventure game that explores breathing as a core mechanic to enhance immersion and interactivity in virtual reality. Using alternative input devices, including a wind sensor and a respiration belt, the game creates novel gameplay experiences driven by the player's own breath. The project was developed by a team of five graduate students at Carnegie Mellon University's Entertainment Technology Center (ETC)."
contribution: 
  - Core VR Framework Development
  - Breathing Data System
  - Locomotion System Design
  - Physics System & Interactions
  - Performance Optimization
  - Project Management
team: 
  - 2 Programmers
  - 1 Sound/ Narrative Designer
  - 2 Artists
  - 2 Producers
role:
  - Producer
  - Technical Designer
  - Programmer
timeline: Jan 2025 - May 2025 (14 weeks)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/TrailerCompressed.mp4"
trialer_video: "https://www.youtube.com/embed/fUHDFnX35RE?si=zJSbzG5uehWPiTsR"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include media-block-styles.html %}
{% include content-block-styles.html %}
{% include feature-grid-styles.html %}
{% include layered-card-styles.html %}
{% include callout-style.html %}


{% capture design_problem_01 %}
Have you ever imagined controlling a breath of fire with your own breathing? 

Take a deep breath now — picture a brilliant light shining before your eyes, then exhale, and flames pour from your mouth, burning everything in sight.
{% endcapture %}
{% capture design_problem_02 %}
This simple question sparked the project: when breath becomes the input of a game, what kind of gameplay can emerge from it — and what kind of experience might that create?
{% endcapture %}
{% capture the_medium_01 %}
To answer this question, we explored 2D PC games, and we found ourselves drawn toward a more immersive experience. 
{% endcapture %}
{% capture the_medium_02 %}
We ultimately chose VR (Meta Quest 3) as our medium — a platform where the connection between breath and gameplay could feel truly embodied.
{% endcapture %}
{% capture belt_explain %}
Since our focus was exploring breathing as a game mechanic rather than building hardware from scratch, we prioritized a reliable, off-the-shelf solution — choosing the Vernier Go Direct Respiration Belt for its stable data output, plug-and-play setup, and SDK support.
{% endcapture %}
{% capture windsensor_explain %}
Added later in development, the wind sensor kit was purpose-built for the Meta Quest 3 to enable real-time airflow capture during gameplay. Our teammate Alex Hall designed and 3D-printed a custom enclosure, allowing the kit to mount directly onto the HMD for seamless data collection.
{% endcapture %}
{% capture data_flow %}
Sensor data is collected through two parallel pipelines: the respiration belt streams data via its SDK, while the wind sensor transmits through an Arduino over Wi-Fi. 

Both streams are received and processed by a Python script on PC, then forwarded to the Unity application (C#) running on Meta Quest 3 via UDP socket. 

Since breath data is continuous, occasional packet loss is acceptable — making UDP a practical choice over TCP for this use case.
{% endcapture %}

{% capture dtw %}
The core challenge is recognizing the trend of a breathing pattern within a given window, rather than matching exact timestamps. 

Since the timing of data capture rarely aligns perfectly with the actual breathing cycle, DTW (Dynamic Time Warping) was chosen for its ability to handle these temporal misalignments while still identifying the underlying pattern.
{% endcapture %}

<div class="project-content">
{% include project-info.html %}

<div class="project-section" style="background-color: #F2F2F2F2"> 
    <div class="content-wrapper-80">
      <h4 style="text-align:center;">Design Problem</h4>
      <h3 style="text-align:center;margin:0 auto;">Can breathing be a game input?</h3>
      {% include content-block.html 
        content=design_problem_01
        reversed=true 
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
        text_align="center"
      %}
      {% include content-block.html 
        image="assets/images/projects/xhaler/fireBreathe.png" 
        reversed=false 
        color="#006ba0"
        img_width="50%"
        left_offset="25%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
      {% include content-block.html 
        content=design_problem_02
        reversed=true 
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
        text_align="center"
      %}
    </div>
  </div>
  <div class="project-section" style="background-color: #ffffff"> 
    <div class="content-wrapper-80">
      <h4 style="text-align:center;">Design Decision 1</h4>
      <h3 style="text-align:center;margin:0 auto;">The medium</h3>
      <br><br>
      <h5 style="text-align:center;margin:0 auto;">Question: Which platform would best allow us to explore breathing as a game input? </h5>
      <br><br>
      {% include content-block.html 
        content=the_medium_01
        reversed=true 
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="50%"
        width="100%"
        text_align="left"
        video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/Combined2DPrototypes2.mp4"
      %}

      {% include content-block.html 
        image="assets/images/projects/xhaler/LawrenceShooting.jpg" 
        content=the_medium_02
        reversed=false 
        color="#006ba0"
        img_width="50%"
        left_offset="0%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
    </div>
  </div>
  
  <!-- Tech Exploration -->
  <div class="project-section" style="background-color: #F5F5F5"> 
    <div class="content-wrapper-80">
      <h4 style="text-align:center;">Tech Exploration</h4>
      <h3 style="text-align:center;margin:0 auto;">Capture the breathe</h3>
      <br><br>
      <div style="background-color:#D6D6D6">
        <h4 style="text-align:center;margin:5px auto;">Devices</h4>
      </div>
      {% include callout.html 
        background_color="#000"
        section_color="#F5F5F5"
        body_color="#e0e0e0"
        title="Vernier Go Direct Respiration Belt"
        body="Reliable Solution   →   Focus on development"
      %}
      <div class="icon-grid-bg" style="margin: 0 auto; background-color:#F5F5F5; margin-bottom: px;">
        <div class="icon-grid-container" style="grid-template-columns: repeat(2, 1fr);">
          {% include feature-grid-item.html 
              title="respiration belt"
              hide_title=true
              content=belt_explain
              image="assets/images/projects/xhaler/respirationBelt.png"
              color="#57ac5d"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=true
              width="100%"
          %}
          {% include feature-grid-item.html 
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/belt_shrink.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
        </div>
      </div>

      <br>
      <br>
      <br>

      {% include callout.html 
        section_color="#F5F5F5"
        background_color="#fff"
        title_color="#000"
        body_color="#363636"
        title="Custom Wind Sensor Kit"
        body="Customized Solution   →   Detect Blowing"
      %}
      <div class="icon-grid-bg" style="margin: 0 auto; background-color:#F5F5F5; margin-bottom: 5px;">
        <div class="icon-grid-container" style="grid-template-columns: repeat(2, 1fr);">
          {% include feature-grid-item.html 
              title="windsensor kit"
              hide_title=true
              content=windsensor_explain
              image="assets/images/projects/xhaler/windsensor_kit.png"
              color="#6478ce"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=true
              width="100%"
          %}
          {% include feature-grid-item.html 
              image="assets/images/projects/xhaler/windSensorHMD.jpg"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
        </div>
      </div>
      <br><br>
      <div style="background-color:#D6D6D6">
        <h4 style="text-align:center;margin:50px auto;">Data Flow</h4>
      </div>
      {% include content-block.html 
        image="assets/images/projects/xhaler/XhalerSystem.png" 
        reversed=false 
        color="#006ba0"
        img_width="100%"
        left_offset="0%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
      
      {% include content-block.html
        content=data_flow
        reversed=false 
        color="#006ba0"
        left_offset="0%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
    </div>
  </div>

  <div class="project-section" style="background-color: #ffffff"> 
    <div class="content-wrapper-80">
      <h4 style="text-align:center;">Tech Exploration</h4>
      <h3 style="text-align:center;margin:0 auto;">Design the breathing system</h3>
      <br><br>
      {% include content-block.html 
        image="assets/images/projects/xhaler/dtw.png" 
        reversed=false 
        color="#006ba0"
        img_width="100%"
        left_offset="0%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
      <br><br>
      {% include callout.html 
        section_color="#ffffff"
        background_color="#fffee4"
        tag_color="#aeaeae"
        title_color="#000"
        tag="Strategy: pattern matching"
        title="Dynamic Time Warping (DTW)"
        body_color="#363636"
        body="Identifies breathing trends despite timing variations."
      %}
      {% include content-block.html 
        video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/belt.mp4"
        reversed=true
        content=dtw
        left_offset="0%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="50%"
        left_offset="0%"
        width="100%"
        text_align="left"
      %}

      <div class="icon-grid-bg" style="margin: 0 auto; background-color:#F5F5F5; margin-bottom: 40px;">
        <div class="icon-grid-container" style="grid-template-columns: repeat(3, 1fr);">
          {% include feature-grid-item.html 
              title="Inhale"
              hide_title=false
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Inhale.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
          {% include feature-grid-item.html 
              title="Exhale"
              hide_title=false
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Exhale.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
          {% include feature-grid-item.html 
              title="Hold"
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Hold.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
        </div>
      </div>

      <div class="icon-grid-bg" style="margin: 0 auto; background-color:#F5F5F5; margin-bottom: 5px;">
        <div class="icon-grid-container" style="grid-template-columns: repeat(3, 1fr);">
          {% include feature-grid-item.html 
              title="Gentle"
              hide_title=false
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Gentle.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
          {% include feature-grid-item.html 
              title="Intermittent"
              hide_title=false
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Intermittent.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
          {% include feature-grid-item.html 
              title="Expansive"
              video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/xhaler/patterns/Expansive.mp4"
              reversed=true 
              img_width="100%"
              enable_scroll=false
              enable_modal=false
              width="100%"
          %}
        </div>
      </div>
    </div>
  </div>
</div>
