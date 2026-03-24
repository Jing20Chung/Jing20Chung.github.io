---
layout: default
title: "Go! KartVR"
date: 2018-10-30
image: "assets/images/projects/go-kart-vr/thumbnail.png"
description_title: "Experience the Ultimate Thrill of Virtual Racing!"
description: "GO! KartVR is an exhilarating VR racing game that syncs virtual car movements with a real-world racing chair, creating an immersive experience."
team: 
  - 2 Programmer
  - 1 Producer
  - 2 Artists
role:
  - Gameplay Systems Programmer
timeline: Oct 2018 - Dec 2019
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/go-kart-vr/go-kart-vr-hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/go-kart-vr/gameplay.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture contribution %}
**Multiplayer & Networking**
- Developed online multiplayer features and connectivity
- Implemented lobby system for player matchmaking

**Live Streaming System**
- Built real-time live-streaming system

**Interactive Systems**
- Designed and implemented interactive event systems
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

        <h3 style="text-align: center;"> Lobby & Broadcast Demo </h3>
      {% include content-block.html 
        video="https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/go-kart-vr/GO!KartVR-MultiplayerDemo.mp4"
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="100%"
        width="100%"
        text_align="left"
      %}
      {% include content-block.html 
        title="Exhibitions"
        content="GO! KartVR was showcased at a VR exhibition in South Korea and later exhibited in Taipei, Taiwan, in 2019, where it garnered positive attention from both players and industry professionals."
        image="assets/images/projects/go-kart-vr/OurArea.jpg"
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="50%"
        width="100%"
        text_align="left"
      %}

      {% include content-block.html 
        title=""
        image="assets/images/projects/go-kart-vr/child.png"
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="70%"
        width="100%"
        text_align="left"
      %}
      {% include content-block.html 
        title=""
        image="assets/images/projects/go-kart-vr/player1.jpg"
        color="#006ba0"
        reversed=true 
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="70%"
        width="100%"
        text_align="left"
      %}
      {% include content-block.html 
        title=""
        image="assets/images/projects/go-kart-vr/television.jpg"
        color="#006ba0"
        reversed=false 
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="70%"
        width="100%"
        text_align="left"
      %}
      {% include content-block.html 
        title=""
        image="assets/images/projects/go-kart-vr/three.jpg"
        color="#006ba0"
        reversed=false 
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        img_width="100%"
        width="100%"
        text_align="left"
      %}
  </div>

</div>
