---
layout: default
title: "In The End"
date: 2025-08-06
image: "/assets/images/projects/InTheEnd/InTheEnd-ThumbNail.jpg"
description: "An immersive VR experience where physical sensations shape an emotional arc."
contribution: 
  - Developed Event-Based Haptic System Architecture
  - Created customizable shader to create 8+ visual effects
  - Full Experience Integration & Delivery
role:
  - Technical Designer
  - Technical Artist
  - Programmer
video: "/assets/videos/projects/InTheEnd/in-the-end-hero.mp4"
permalink: "/projects/in-the-end"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include media-block-styles.html %}

<div class="project-content">
  {% include project-info.html %}

  {% include lego-block.html 
    video="assets/videos/projects/InTheEnd/Death-1.mp4" 
    title="A Journey Through Pulse" 
    content="You are a novice Grim Reaper. Your task is to sense people's heartbeats, identify who is nearing death, and guide them onward. Throughout this journey, a voice accompanies you—until you discover its true identity..." 
    reversed=true 
    img_width="45%"
    color="#9b0669"
    enable_scroll=false
    margin_bottom="50px"
  %}

  
  {% include lego-block.html 
    image="assets/images/projects/InTheEnd/tactGloveDK2.png" 
    title="Tools of Touch" 
    external=true
    content="We used bHaptics' TactGlove DK2, which feature six vibration points across the fingers and wrist. Their well-designed interface and Unity-friendly API made them ideal for our initial exploration without overly complex haptic implementation." 
    reversed=true 
    color="#018358"
    img_width="30%"
    width="100%"
    enable_scroll=false
  %}
  {% include lego-block.html 
    image="/assets/images/projects/InTheEnd/bottom-up.png" 
    title="From Sensation to Story" 
    content="Taking a bottom-up approach, we began by experimenting with fundamental haptic patterns—slap, elastic band, pinch, small human touch, and more. Through multiple prototypes and playtests, we discovered that heartbeat was the pattern most capable of directly evoking emotion, making it the core tactile element of our final experience." 
    reversed=true 
    color="#ffa78c"
    img_width="60%"
    enable_scroll=false
    margin_bottom="50px"
  %}
  {% include lego-block.html 
    image="assets/images/projects/monkeying-around/thumbnail.png" 
    title="Where It All Began" 
    link='/projects/xhaler'
    content="I originated and pitched this project at CMU's Entertainment Technology Center, assembling a team to explore a question from my previous VR game, Monkeying Around: Can haptic feedback convey emotion, not just physical sensation? As Technical Designer and Programmer, I focused on development—building the modular haptic system and shader library—while collaborating with our producer on the broader vision." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}

  
  {% include lego-block.html 
    title="Prototypes"
    text_align="center"
    content="Iterating toward emotional haptics." 
    color="#322d6b"
    scroll_height="1000px"  
    height="200px"
    reversed=false 
    enable_scroll=true
    width="100%"
    margin_bottom="100px"
  %}

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/elastic-band-haptic-visual.mp4" 
    title="Elastic Band" 
    color="green"
    content="I started developing this prototype during the summer, implementing the elastic band stretching effect through code. Since the haptic gloves hadn't arrived yet, I initially prototyped using the built-in haptics of Meta Quest controllers. Once the gloves arrived, thanks to the modular Haptic System I had established, I only needed to swap out the hardware interface layer—all the upper-level software implementation remained unchanged, allowing seamless transition to glove-based haptic playback.<br><br>
    User feedback on this prototype was positive—players enjoyed the tension effect when stretching the elastic band. I designed the haptic feedback in three distinct phases: grabbing the band, stretching it, and the sharp 'snap' impact upon release. Testing confirmed that adding haptics increased user immersion, though the emotional impact wasn't particularly pronounced." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}
  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/slap-haptic-visual.mp4" 
    title="Slap" 
    content="This experiment explored impact-based haptics through balloon slapping. I implemented floaty balloon physics that reacted naturally to hits while maintaining upward drift. Users found the 'pop' satisfying and instinctively continued interacting.<br><br>Our Sound Designer, Michaecle, added switchable audio—realistic vs. cartoon. The emotional shift was dramatic: cartoon sounds transformed the experience into something playful and laughter-inducing.<br><br>While engaging, the haptic impact on emotion still needed strengthening." 
    reversed=false 
    color="#ce5200"
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}

</div>
<!-- 
  {% include media-block.html 
    image="assets/images/projects/InTheEnd/tactGloveDK2.png" 
    title="Tools of Touch" 
    external=true
    link='https://www.bhaptics.com/'
    content="We used bHaptics' TactGlove DK2, which feature six vibration points across the fingers and wrist. Their well-designed interface and Unity-friendly API made them ideal for our initial exploration without overly complex haptic implementation." 
    reversed=true 
    img_width="30%"
    enable_scroll=false
    margin_bottom="50px"
  %}



  {% include media-block.html 
    image="/assets/images/projects/InTheEnd/bottom-up.png" 
    title="From Sensation to Story" 
    content="Taking a bottom-up approach, we began by experimenting with fundamental haptic patterns—slap, elastic band, pinch, small human touch, and more. Through multiple prototypes and playtests, we discovered that heartbeat was the pattern most capable of directly evoking emotion, making it the core tactile element of our final experience." 
    reversed=true 
    img_width="30%"
    enable_scroll=false
    margin_bottom="50px"
  %}



  {% include media-block.html 
    video="assets/videos/projects/InTheEnd/Death.mov" 
    title="A Journey Through Pulse" 
    content="You are a novice Grim Reaper. Your task is to sense people's heartbeats, identify who is nearing death, and guide them onward. Throughout this journey, a voice accompanies you—until you discover its true identity..." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}



  {% include media-block.html 
    image="/assets/images/projects/InTheEnd/Tacit-logo.png" 
    title="When Touch Moves the Heart" 
    content="The experience proved emotionally compelling enough that one professor couldn't bring themselves to continue playing. We successfully achieved our goal of eliciting complex emotions—not just simple feelings, but layered, profound responses. This demonstrated the potential of haptic feedback as a medium for deep emotional storytelling, which is precisely what we set out to explore." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}


  {% include media-block.html 
    image="assets/images/projects/monkeying-around/thumbnail.png" 
    title="Where It All Began" 
    link='/projects/xhaler'
    content="We are a student team from CMU's Entertainment Technology Center. This pitch project originated from my first-semester VR climbing game, Monkeying Around. While developing it, I wondered: What if I could feel what I'm gripping? How would that transform the experience? This semester, I gathered teammates to embark on this exploration together." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}

    {% include media-block.html 
    image="/assets/images/projects/InTheEnd/Tacit-logo.png" 
    title="Sharing the Pulse" 
    content="We've shared our work at multiple conferences: selected for Sona Film Festival, submitted to Laval Virtual and SIGGRAPH. We hope this unique journey will raise awareness of haptic technology's potential and expand possibilities for the VR/MR industry." 
    reversed=true 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}


  {% include media-block.html 
    image="/assets/images/projects/InTheEnd/Tacit-logo.png" 
    title="Meet our team!" 
    link='https://projects.etc.cmu.edu/tacit/'
    content="“TACIT”, which means understood or implied without being stated, is our aspiration for how the haptic interactions we carefully experimented can enhance the subtle yet layered emotions within the VR journey. As a student pitch team passionate about innovating how touch can drive gameplay, we secretly hope that TACIT might also mean, Totally Awesome Creative Innovation on Tactileness!" 
    reversed=false 
    img_width="50%"
    enable_scroll=false
    margin_bottom="50px"
  %}

{% include media-block.html 
   title="" 
   content="" 
   youtube_id="gU48gWbiNd4"
   img_width="30%" 
   enable_scroll=false 
%}

  {% include lego-block.html 
    text-align="center"
    external=true
    link="https://www.youtube.com/watch?v=jax5KGOHjuE"
    title="What does it feel like in the end?" 
    content=""
    height="10%"
    width="100%" 
    left_offset="0%" 
    color="yellow" 
    enable_scroll=false 
  %} -->


