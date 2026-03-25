---
layout: default
title: "Basketball Tactic Training System"
date: 2017-07-07
image: "assets/images/projects/basketball-tactic-training-system/defender_mode_3PP.PNG"
description_title: "VR-BTB — Immersive Basketball Tactic Training"
description: "The Basketball Tactic Training System offers an immersive VR training experience, accelerating players' familiarity with basketball tactics. The system is designed to generate real-time 3D simulations by seamlessly converting 2D tactical data from a digital tablet into a dynamic 3D environment.This tactical information is sent to the VR system via socket, creating an immersive experience in virtual reality."
team: 
  - 1 Programmer
role:
  - Programmer
timeline: June 2015 - July 2017
video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/basketball-tactic-training-system/hero.mp4"
trialer_video: "https://pub-ff65b495204a4a92b2eb66af1e701a7e.r2.dev/projects/basketball-tactic-training-system/hero.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include content-block-styles.html %}


{% capture features %}
**Normal Mode**
Standard tactic simulation viewable in first-person or third-person perspective

**Learning Mode**
Head pose-guided training that pauses progression until the player looks at the correct target

**Defender Mode**
Auto-generates virtual defenders using positional formula based on offensive player, ball, and hoop locations
{% endcapture %}

{% capture tech_implementation %}
**2D-to-3D Tactic Pipeline**
- Developed an Android tablet app (E-BTB) for coaches to draw and record offensive player trajectories and orientations
- Transmitted tactic data to a 3D rendering server via TCP socket communication
- Converted 2D player trajectories into real-time 3D animations using Unreal Engine 4, displayed via HTC Vive

**Tactic Recommendation System**
- Implemented Dynamic Time Warping (DTW) algorithm for trajectory similarity matching
- Compared DTW against EDR and selected DTW for its direction-sensitive accuracy

**Player & Defender Animation**
- Designed state machine for player animation (No Ball → Catch Ball → Hold Ball → Pass Ball)
- Implemented defender positioning using the formula `0.62Otk + 0.11Bt + 0.27H`
- Resolved defender animation jitter via a 4-state animation state machine (Idle → Start → Running → Stop)

**Learning Mode System**
- Built head pose detection using dot product and inverse cosine to determine if target is within 40° field of view
- Used Unreal Engine 4's Inverse Transform Location to determine left/right directional hints
{% endcapture %}

<div class="project-content">
  {% include project-info.html %}

<div class="project-section" style="padding-top: 00px; background-color: #eeeeee"> 
    <div class="content-wrapper-80">
      <h3 style="text-align:center;margin:0 auto;">Features</h3>
      {% include content-block.html 
        content=features
        reversed=true 
        color="#006ba0"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
        text_align="left"
      %}
      <h3 style="text-align:center;margin:0 auto;">Technical Implementation</h3>
      {% include content-block.html 
        content=tech_implementation
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
