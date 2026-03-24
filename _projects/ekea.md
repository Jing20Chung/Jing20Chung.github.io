---
layout: default
title: "EKEA"
date: 2024-08-24
image: "assets/images/projects/ekea/thumbnail.png"
description_title: "Innovative Interface for Game Experience"
description: "A rhythm game featuring an innovative interface that utilizes the Xbox Adaptive Controller, designed to deliver an intuitive gaming experience. The game was developed in two weeks, incorporating feedback from interim playtests and iterations."
team: 
  - 2 Programmer
  - 1 Sound Designer
  - 2 Artists
role:
  - Gameplay Systems Programmer
timeline: Aug 2024 (2 weeks)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/ekea/hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/ekea/gameplay_compressed.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Architecture & Game Flow**
- Built scene transition management
- Designed event-based object communication system
- Implemented game state logic

**Gameplay Mechanics**
- Developed core sawing gameplay mechanics

**Visual Effects & Cinematics**
- Authored cutscenes using Cinemachine
- Implemented visual feedback through wood animation
{% endcapture %}

<div class="project-content">
  {% include project-info.html %}

<div class="project-section" style="padding-top: 00px; background-color: #eeeeee"> 
    <div class="content-wrapper-80">
      <h3 style="text-align:center;margin:0 auto;">Contributions</h3>
      {% include content-block.html 
        content=contribution
        reversed=true 
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
        text_align="left"
      %}
    </div>
  </div>

</div>
