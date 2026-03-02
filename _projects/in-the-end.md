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
{% include project-scripts.html %}
{% include media-block-styles.html %}


{% capture elastic_band_content %}
I started developing this prototype during the summer, implementing the elastic band stretching effect through code. Since the haptic gloves hadn't arrived yet, I initially prototyped using the built-in haptics of Meta Quest controllers. Once the gloves arrived, thanks to the modular Haptic System I had established, I only needed to swap out the hardware interface layer—all the upper-level software implementation remained unchanged, allowing seamless transition to glove-based haptic playback.

User feedback on this prototype was positive—players enjoyed the tension effect when stretching the elastic band. I designed the haptic feedback in three distinct phases: grabbing the band, stretching it, and the sharp 'snap' impact upon release. Testing confirmed that adding haptics increased user immersion, though the emotional impact wasn't particularly pronounced.
{% endcapture %}

{% capture slap_content %}
This experiment explored impact-based haptics through balloon slapping. I implemented floaty balloon physics that reacted naturally to hits while maintaining upward drift. Users found the 'pop' satisfying and instinctively continued interacting.

Our Sound Designer, Michaecle, added switchable audio—realistic vs. cartoon. The emotional shift was dramatic: cartoon sounds transformed the experience into something playful and laughter-inducing.

While engaging, the haptic impact on emotion still needed strengthening.
{% endcapture %}


{% capture stroke_content %}
In this interaction, I explored multiple dimensions:

1. **Ray-cast detection**: Using ray-cast to detect contact points, so that individual fingertips trigger vibrations based on whether they are touching an object.
2. **Dynamic intensity**: Weakening or strengthening haptic feedback based on finger distance to simulate light vs. firm strokes.
3. **Indirect control**: Experimenting with how haptic feedback can serve as negative feedback.

One of the core design challenges in VR is that virtual objects have no physical presence...

## No Way to Stop the Hand
You cannot physically prevent a user's hand from "passing through" an object. How to communicate to users what the "correct" action is, especially for something as nuanced as stroking, is a genuinely interesting topic.

## Can Haptics Say "Wrong"?
From the early exploration phase, we found that shock-like haptic sensations caused users to recoil and feel discomfort — though at that point, we had not yet investigated whether this discomfort would actually lead users to avoid such contact.
This gave rise to an initial hypothesis: that an extremely intense haptic feedback could be used to convey a signal of "wrong" or erroneous behavior.

## More Rock, Less Talk
Based on this hypothesis, I designed an interaction in which, when a user touches the "interior" of an object (i.e., passes beyond its surface), the haptic feedback intensity increases sharply, prompting users to notice the discomfort and withdraw their hand.

## What the Playtesters Taught Me
After having playtesters try it, the results were not significant. Users did not interpret intense haptic feedback as an error signal, and the perceived intensity of the haptics varied considerably across age groups — for example, Playtester A found the vibration very strong, while Playtester B found it barely noticeable. This led me to understand that normalizing haptic feedback is inherently difficult, and that people's interpretation of haptics requires further research before it can reliably serve as a feedback guide.
{% endcapture %}
{% capture teleknesis_content %}
This prototype explores how individuals conceptualize abstract phenomena. Our findings reveal that mental models vary significantly: some users envision subtle vibrations, while others imagine energy flowing from their fingertips to their wrists. This diversity highlights a key challenge in hand gesture prediction—since there is no universal 'standard' for telekinesis, users naturally employ a wide range of intuitive gestures. This experience underscored that for abstract, non-standardized mechanics (unlike the well-established 'magic wand' trope), continuous playtesting and behavioral analysis are indispensable.
{% endcapture %}
{% capture pinch_content %}
How would you pinch your father?' This prototype investigates how social context and empathy reshape physical interactions with virtual entities. Beyond testing haptic feedback for the 'pinch' gesture, we examined how shifting the identity of a virtual character—assigned via dynamic text labels—altered user behavior. Our study revealed that users were reluctant to use a pinch gesture on figures of authority, such as a 'King,' preferring instead to support them in their palms. Furthermore, many participants expressed moral hesitation to pinch virtual humans altogether. These findings underscore that empathy and social hierarchy significantly dictate interaction paradigms, suggesting that context is essential for creating truly intuitive and culturally resonant XR experiences.
{% endcapture %}
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
    enable_scroll=false
    width="100%"
    margin_bottom="100px"
  %}

  <div class="lego-row">

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/elastic-band-haptic-visual.mp4" 
    title="Elastic Band" 
    color="green"
    content=elastic_band_content
    reversed=true 
    img_width="50%"
    enable_scroll=false
    enable_modal=true
    margin_bottom="50px"
    width="49%"
  %}

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/stoke-1.mp4" 
    title="Stroke"
    content=stroke_content
    reversed=false 
    color="#6e0035"
    img_width="50%"
    enable_scroll=false
    enable_modal=true
    margin_bottom="50px"
    width="48%"
  %}

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/slap-haptic-visual.mp4" 
    title="Slap" 
    content=slap_content
    reversed=false 
    color="#ce5200"
    img_width="60%"
    enable_scroll=false
    enable_modal=true
    margin_bottom="50px"
    width="40%"
  %}

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/teleknesis.mp4" 
    title="Teleknisis" 
    content=teleknesis_content
    reversed=true 
    color="#1d60f0"
    img_width="45%"
    enable_scroll=false
    enable_modal=true
    margin_bottom="50px"
    width="58%"
  %}

  {% include lego-block.html 
    video="/assets/videos/projects/InTheEnd/pinch-1.mp4" 
    title="Pinch" 
    content=pinch_content
    reversed=true 
    color="#006ba0"
    img_width="50%"
    enable_scroll=false
    enable_modal=true
    margin_bottom="50px"
    width="48%"
  %}
  </div>


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


