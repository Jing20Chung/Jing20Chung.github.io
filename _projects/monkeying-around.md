---
layout: default
title: "Monkeying Around"
date: 2024-09-01
image: "assets/images/projects/monkeying-around/thumbnail.png"
description_title: "Alternative Interface for Game Experience"
description: "Hospital Rush is a 2v2 cooperative game that uses adaptive controllers to stimulate the effect of a rotating hospital stretcher carrying a slippery patient. Work with your partner to race through a hospital and get your patient to the last available emergency room before your opponents!"
team: 
  - 2 Programmer
  - 1 Sound Designer
  - 2 Artists
role:
  - Gameplay Systems Programmer
timeline: Sept 2024 (2 weeks)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/monkeying-around/hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/monkeying-around/gameplay.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Gameplay Mechanics**
- Implemented touch angle detection for climbing mechanics
- Developed hand-tracking system for camera movement
- Built attachment and detachment rule logic

**Architecture & Game Flow**
- Built scene transition management
- Designed event-based object communication system
- Implemented game state logic

**Visual Effects**
- Designed visual cues to indicate climbing status
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
