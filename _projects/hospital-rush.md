---
layout: default
title: "Hospital Rush"
date: 2024-10-01
image: "assets/images/projects/hospital-rush/thumbnail.png"
description_title: "Alternative Interface for Game Experience"
description: "Hospital Rush is a 2v2 cooperative game that uses adaptive controllers to stimulate the effect of a rotating hospital stretcher carrying a slippery patient. Work with your partner to race through a hospital and get your patient to the last available emergency room before your opponents!"
contribution: 
  - Designed event-driven architecture with ScriptableObjects
  - Implemented all game mechanics (bubble fight, portal teleportation, collectibles, dynamic pitfall)
  - Integrated event-triggered animation transitions
team: 
  - 2 Programmer
  - 1 Sound Designer
  - 2 Artists
role:
  - Gameplay Systems Programmer
timeline: Oct 2024 (1 week)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/hospital-rush/hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/hospital-rush/HospitalRushDescription.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Architecture & Game Flow**
1. Designed event-based object communication system
2. Implemented win/lose conditions and replay logic

**Gameplay Mechanics**
1. Developed hospital stretcher rotation system
2. Implemented patient collision detection and behavior
3. Built rigid body collision handling (patients, tables, obstacles)
4. Created multi-input device mapping system
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
