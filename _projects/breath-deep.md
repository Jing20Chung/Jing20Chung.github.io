---
layout: default
title: "Breath Deep"
date: 2025-01-30
image: "/assets/images/projects/breath-deep/thumbnail.png"
description_title: "GGJ 2025 | < 48 hours | Jammer's Choice Award"
description: "Breathe Deep is a 1v1 strategy survival game where precision, adaptability, and cunning determine the victor. You and your opponent are rival pirates of a sunken ship, racing to collect bubbles for oxygen while battling each other in the depths. But beware—danger lurks in every corner of the deep sea, and only the craftiest pirate will survive."
contribution: 
  - Designed event-driven architecture with ScriptableObjects
  - Implemented all game mechanics (bubble fight, portal teleportation, collectibles, dynamic pitfall)
  - Integrated event-triggered animation transitions
team: 
  - 2 Programmers
  - 1 Sound Designer
  - 2 Artists
  - 1 Producer
role:
  - Gameplay Systems Programmer
timeline: 26 Jan - 1 Feb 2026 (48 hours)
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/breath-deep/BreathDeepTitle.mp4"
trialer_video: "https://www.youtube.com/embed/Qp9gI5iN9wY?si=yqpsjCnrmWcL4n5_"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Architecture & Game Flow**
- Designed an event-driven architecture using ScriptableObjects to manage game state
- Implemented win/lose conditions and replay logic

**Gameplay Mechanics**
- Built raycast-based collision detection and dynamic pitfall activation
- Developed randomized portal teleportation and countdown timer systems
- Created collectible spawn and identification systems with player-specific effects

**Visual Effects**
- Integrated event-triggered animation transitions tied to game state changes
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
