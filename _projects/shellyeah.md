---
layout: default
title: "Shell Yeah!"
date: 2024-11-01
image: "assets/images/projects/shell-yeah/thumbnail.png"
description_title: "3 vs 1 Co-op Game"
description: "Shell Yeah! is a 3-vs-1 co-op party game where three players team up to control a crab by pressing buttons in sequence to maintain its speed, while the fourth player becomes an octopus, using laser beams to disrupt their progress. The crab's goal is to reach three checkpoints, gather weapons, and defeat the octopus, creating a thrilling battle of teamwork and strategy."
contribution: 
  - Designed event-driven architecture with ScriptableObjects
  - Implemented all game mechanics (bubble fight, portal teleportation, collectibles, dynamic pitfall)
  - Integrated event-triggered animation transitions
team: 
  - 1 Programmer
  - 1 Sound Designer
  - 2 Artists
role:
  - Gameplay Systems Programmer
timeline: Nov – Dec 2024 (2 weeks)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/shell-yeah/hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/shell-yeah/48_ShellYeah.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Architecture & Game Flow**
1. Designed event-based object communication system
2. Implemented win/lose conditions and replay logic
3. Built scene transition management

**Gameplay Mechanics**
1. Developed spline-based crab movement system
2. Implemented combo-key input behavior
3. Integrated Timeline Director for cutscene triggers
4. Created randomized step order generator

**Visual Effects & Cinematics**
1. Authored intro cutscene using Unity Timeline
2. Designed glowing visual effect for cutscene trigger area
3. Implemented mini-screen view from Octopus's perspective
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
