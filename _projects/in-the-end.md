---
layout: default
title: "In The End"
date: 2025-08-06
image: "/assets/images/projects/InTheEnd/InTheEnd-ThumbNail.jpg"
description_title: "An immersive VR experience where physical sensations shape an emotional arc."
description: "In The End is an immersive VR experience uses haptic gloves to fuse context into tactile sensation that drives an emotional arc."
timeline: Aug 2025 - Dec 2025 (14 weeks)
team: 
  - 2 Programmers
  - 1 Narrative/ Sound Designer
  - 1 Producer
  - 2 Artists
contribution:
  - Developed Event-Based Haptic System Architecture
  - Created customizable shader to create 8+ visual effects
  - Full Experience Integration & Delivery
role:
  - System Architect
  - Technical Designer
  - Technical Artist
  - Game Play Programmer
video: "/assets/videos/projects/InTheEnd/hero.mp4"
---
{% include hero-video.html %}
{% include project-styles.html %}
{% include project-scripts.html %}
{% include media-block-styles.html %}
{% include content-block-styles.html %}
{% include feature-grid-styles.html %}
{% include layered-card-styles.html %}


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

{% capture rain_content %}
In this prototype, I primarily tested whether the sensitivity of collision detection and haptic triggering was sufficient. The results showed that single-point collision is viable; however, the limitation still lies in Unity's physics engine detection quality — if the raindrop moves too fast, it cannot be detected. On the visual side, I also found an interesting insight about general perception: most people associate raindrops with a nearly linear shape, which was a notable finding about common mental models.
{% endcapture %}


{% capture crush_content %}
This prototype required the use of the Interactor module from the Meta SDK. Since the module didn't offer fine-grained control over finger curl degree for gesture detection, we went deeper into the Meta SDK and modified the relevant source code directly to make the interaction possible.
The biggest challenge, however, was optimizing for the wide variation in how people crush objects — both in terms of speed and motion range. One key issue we encountered was that users with prior VR experience would instinctively "grab" or "pinch" objects, rather than naturally conforming their hand shape to the object as they would in real life. To handle this, we implemented several nuanced conditions: for instance, if a user's fingers were already beyond the curl threshold upon first contact with the object, the Crush interaction would not trigger immediately — instead, it would wait until the user opened their hand again before resuming detection. These refinements ensured that users could fully experience the haptic feedback throughout the crush motion, and this logic was carried forward into our final Crush Heart interaction.
{% endcapture %}

{% capture heartbeat_content %}
For this prototype, we initially used the Inspector to adjust the heartbeat frequency, then asked players how they would interpret each variation and how it made them feel. This testing process revealed that heartbeat carries a broadly shared meaning across users, and because it is so closely tied to life itself, it tends to evoke emotion more readily. As a result, this interaction became the centerpiece of our experience.
{% endcapture %}


{% capture problem_content %}
I originated and pitched this project at CMU’s Entertainment Technology Center, assembling a team to explore a core question from my previous VR game, Monkeying Around: Can haptics convey profound emotion, rather than just physical sensation?
{% endcapture %}

{% capture problem_content_2 %}
A key inspiration for this exploration was the game Before Your Eyes. Its core mechanic uses eye-blinking to fast-forward the narrative; when the webcam detects a blink, time leaps ahead. This creates a unique emotional tension: when you desperately want to witness a moment but are physically forced to blink, the resulting frustration and longing are entirely different from the feelings evoked by traditional keyboard or controller inputs. We aim to achieve this same level of visceral, non-traditional emotional engagement through haptics.
{% endcapture %}

{% capture bHapticGloves %}
We used bHaptics’ TactGlove DK2, which feature six vibration points across the fingers and wrist. Their well-designed interface and Unity-friendly API made them ideal for our initial exploration without overly complex haptic implementation.
{% endcapture %}

{% capture bottomUp %}
Taking a bottom-up approach, we began by experimenting with fundamental haptic patterns—slap, elastic band, pinch, small human touch, and more. Through multiple prototypes and playtests, we discovered that heartbeat was the pattern most capable of directly evoking emotion, making it the core tactile element of our final experience.
{% endcapture %}


<div class="project-content">
  {% include project-info.html %}
  <div class="project-section" style="background-color: #F2F2F2F2"> 
    <div class="content-wrapper-80">
      <h4>Inspiration</h4>
      <h3>Can haptic be the motor driving emotional response?</h3>
      {% include content-block.html 
        image="assets/images/projects/monkeying-around/thumbnail.png"
        content=problem_content
        reversed=true 
        color="#006ba0"
        img_width="30%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="48%"
      %}
      {% include content-block.html 
        image="assets/images/projects/InTheEnd/BeforeYourEyes.png" 
        content=problem_content_2
        reversed=true 
        color="#006ba0"
        img_width="30%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="48%"
      %}
    </div>
  </div>

  <div class="project-section" style="background-color: #ffffff"> 
    <div class="content-wrapper-80">
      <h4>Medium</h4>
      <h3>bHaptics’ TactGlove DK2</h3>
      {% include content-block.html 
        image="assets/images/projects/InTheEnd/tactGloveDK2.png" 
        content=bHapticGloves
        reversed=true 
        color="#006ba0"
        img_width="30%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="0px"
        width="100%"
      %}
    </div>
  </div>

  <div class="project-section" style="background-color: #f2f2f2"> 
    <div class="content-wrapper-80">
      <h4>Explore</h4>
      <h3>Bottom-up approach: investigate what works</h3>
      {% include content-block.html 
        image="assets/images/projects/InTheEnd/bottom-up.png" 
        content=bottomUp
        reversed=true 
        color="#006ba0"
        img_width="50%"
        enable_scroll=false
        enable_modal=false
        margin_bottom="50px"
        width="100%"
      %}
    </div>
  </div>

  <div class="icon-grid-bg">
    <div class="icon-grid-container">
      {% include feature-grid-item.html 
        video="/assets/videos/projects/InTheEnd/elastic-band-haptic-visual.mp4" 
        color="green"
        title="Elastic Band"
        content=elastic_band_content
        reversed=true 
        img_width="100%"
        enable_scroll=false
        enable_modal=true
        width="100%"
    %}
    {% include feature-grid-item.html 
      video="/assets/videos/projects/InTheEnd/stoke-1.mp4" 
      title="Stroke"
      content=stroke_content
      reversed=false 
      color="#6e0035"
      img_width="100%"
      enable_scroll=false
      enable_modal=true
      width="100%"
    %}
    {% include feature-grid-item.html 
      video="/assets/videos/projects/InTheEnd/slap-haptic-visual.mp4" 
      title="Slap"
      content=slap_content
      reversed=false 
      color="#ce5200"
      img_width="100%"
      enable_scroll=false
      enable_modal=true
      width="100%"
    %}
    {% include feature-grid-item.html 
      video="/assets/videos/projects/InTheEnd/rain2.mp4" 
      title="Rain"
      content=rain_content
      reversed=true 
      color="#1d60f0"
      img_width="100%"
      enable_scroll=false
      enable_modal=true
      width="100%"
    %}
    </div>
  </div>

  <div class="icon-grid-bg">
    <div class="icon-grid-container">
      {% include feature-grid-item.html 
        video="/assets/videos/projects/InTheEnd/teleknesis.mp4" 
        title="Telekinesis"
        content=teleknesis_content
        reversed=true 
        color="#1d60f0"
        img_width="100%"
        enable_scroll=false
        enable_modal=true
        width="20%"
      %}

      {% include feature-grid-item.html 
        video="/assets/videos/projects/InTheEnd/pinch-1.mp4" 
        title="Pinch"
        content=pinch_content
        reversed=true 
        color="#006ba0"
        img_width="100%"
        enable_scroll=false
        enable_modal=true
        width="20%"
      %}

      {% include feature-grid-item.html 
        video="/assets/videos/projects/InTheEnd/heartbeat-1.mp4" 
        title="Heartbeat"
        content=heartbeat_content
        reversed=true 
        color="#006ba0"
        img_width="100%"
        enable_scroll=false
        enable_modal=true
        width="20%"
      %}

      {% include feature-grid-item.html 
        video="/assets/videos/projects/InTheEnd/crush-1.mp4" 
        title="Crush"
        content=crush_content
        reversed=true 
        color="#006ba0"
        img_width="100%"
        enable_scroll=false
        enable_modal=true
        width="20%"
      %}
    </div>
  </div>

  <div class="project-section" style="padding-top: 100px; background-color: #ffffff"> 
    <div class="content-wrapper-80">
      <div class="layered-card">
        <span class="card-label">Distill</span>
        <h3>A Universal Abstract Concept: The Heartbeat</h3>
        <p style="text-align: left;">After experimenting with various haptic interactions, we noticed that while people have different interpretations of abstract concepts like telekinesis, they share a unanimous understanding of the heartbeat. Everyone instinctively associates a fast heartbeat with tension and a slow one with peace—even the transitions between them carry inherent meaning. We realized that this intuitive connection is the perfect medium for haptics. Instead of over-engineering new associations, we utilize these existing biological links to trigger authentic emotional states in the user.</p>
      </div>
    </div>
  </div>





{% capture dd_01 %}
With a limited 7-week timeframe and the need to optimize for Meta Quest 3 performance, we drew inspiration from Return of the Obra Dinn. We decided to present our final experience through static, frozen-in-time scenes, ensuring a seamless performance that prioritizes our core haptic mechanics.
{% endcapture %}

{% capture dd_02 %}
By utilizing a frozen scene, we effectively minimized visual noise to direct the player's focus toward the primary objective. 
This minimalist art style significantly reduces cognitive load and eliminates distractions, ensuring players remain focused on the heart, the central source of information, and its heartbeat.
{% endcapture %}

{% capture dd_03 %}
With the beating heart as the only animated element, the design intuitively signals that it is the sole interactable object. 
{% endcapture %}

  <div class="project-section" style="background-color: #ffffff"> 
    <div class="content-wrapper-80">
      <h4>Design Decisions</h4>
      <h3>Knowing The Constraint</h3>
      {% include content-block.html 
        content=dd_01
        reversed=true
        image="assets/images/projects/InTheEnd/ObraDinn.png"
      %}
      {% include content-block.html 
        title="Minimized Visual Noise"
        content=dd_02
        img_width="40%"
        reversed=false
        image="assets/images/projects/InTheEnd/Act2.png"
      %}
      {% include content-block.html 
        title="Emphasize Quietly"
        img_width="20%"
        content=dd_03
        reversed=true
        image="assets/images/projects/InTheEnd/Heart.png"
      %}
    </div>
  </div>

  {% capture sys_01 %}
  To validate the haptic-driven, event-based architecture, I developed this early-stage framework prior to the semester. Using Meta Quest 3 controllers, I prototyped an elastic band interaction to explore the relationship between physical tension and haptic intensity. This system served as the technical backbone for our subsequent complex interactions. 
  {% endcapture %}
  <div class="project-section" style="background-color: #90f0ff45"> 
    <div class="content-wrapper-80">
      <h4>System Architecture</h4>
      <h3>System Behind the Beating Heart</h3>
      {% include content-block.html 
        image="assets/images/projects/InTheEnd/System.png"
        img_width="100%"
      %}
      <p style="text-align: center; max-width: 80%; margin: 0 auto; margin-bottom: 100px;">Game-side triggers send event data to an abstract layer, which translates high-level requests into low-level hardware API commands for haptic output.</p>
      {% include content-block.html 
        title="Pre-Semester Technical Foundations"
        img_width="20%"
        content=sys_01
        reversed=true
        image="assets/images/projects/InTheEnd/metaController.png"
      %}
    </div>

  </div>
  <div class="project-section" style="background-color: #ffffff; margin: 200px 0;"> 
    <div class="content-wrapper-80" style="display: flex; flex-direction: column; align-items: center;">
      <h3>What does it feel like in the end?</h3>
      <div class="video-responsive" style="width: 80%;">
          <iframe src="https://www.youtube.com/embed/gU48gWbiNd4?rel=0" frameborder="10" allowfullscreen></iframe>
      </div>
    </div>
  </div>

{% capture future_01 %}
Sense Memory gives Haptics meaning, and that meaning can in turn evoke emotion. Some highly recognizable Haptics — such as a heartbeat — can be identified on their own and interpreted through Sense Memory, naturally carrying emotional weight.
{% endcapture %}

{% capture future_02 %}
Haptics that are too generic may require additional context — such as visual or audio cues — to help the meaning become recognizable, and from there, connect to Sense Memory. Once that connection is made, emotion can follow just the same.
{% endcapture %}
{% capture future_03 %}
The way the human brain stores memories is often not an accurate recording of reality. Take the heartbeat, for example — not everyone has actually felt a heart beating with their own hands, yet it feels like universally shared knowledge. This is because that Sense Memory has been simplified and reinforced through stories and films. The corresponding Haptic is equally simplified, yet it still successfully builds a memory association. This means that if you want to create a Haptic for something that doesn't exist in the real world, you simply need to first teach players the memory link — and from then on, the Haptic can trigger the emotion on the other end of that connection.
{% endcapture %}

{% capture future_04 %}
The heartbeat is a non-literal, universally shared Haptic that generates Sense Memory and effectively evokes emotion. When designing interactions, if you can find a pattern that is already universally understood, don't hesitate — use it. Leveraging existing shared perception can significantly reduce the cost of building that understanding from scratch.
{% endcapture %}

{% capture future_05 %}
Humans are multi-sensory beings, and the experiences we form are typically the result of multiple senses working together. Designing an experience flow that evokes the right emotions requires a broader orchestration of context — much like filmmaking. Haptics are absolutely qualified to be part of that ensemble, and they don't have to play just a supporting role.
{% endcapture %}

  <div class="project-section" style="background-color: #fff7b950; margin: 200px 0;"> 
    <div class="content-wrapper-80">
      <h4>Future Work</h4>
      <h3>The possible tools in the future</h3>
      <p>After a semester of exploration, we arrived at several key takeaways:</p>
      {% include content-block.html 
        img_width="80%"
        left_offset="10%"
        image="assets/images/projects/InTheEnd/HapticDiagram.png"
      %}
      {% include content-block.html 
        has_shadow=true
        title="Sense Memory is the source through which Haptics trigger emotion."
        content=future_01
        img_width="50%"
        image="assets/images/projects/InTheEnd/251101A_Fall_Playtest_ETC_sm_083.jpg"
      %}
      {% include content-block.html 
        has_shadow=true
        title="Context can help define ambiguous Haptics and link them to Sense Memory."
        content=future_02
        img_width="50%"
        reversed=true
        image="assets/images/projects/InTheEnd/Act3.png"
      %}
      {% include content-block.html 
        has_shadow=true
        title="Sense Memory doesn't have to be factual."
        content=future_03
        img_width="50%"
        image="assets/images/projects/InTheEnd/YingjiePlaytest.jpg"
      %}
      {% include content-block.html 
        has_shadow=true
        title="Hitch a ride when you can — find Haptic language that is universal and intuitive."
        content=future_04
        img_width="30%"
        image="assets/images/projects/InTheEnd/20251021_164423.jpg"
      %}
      {% include content-block.html 
        has_shadow=true
        title="Haptics driving emotion is absolutely achievable."
        content=future_05
        img_width="50%"
        image="assets/images/projects/InTheEnd/glovesEngagement.jpg"
      %}
    </div>
  </div>
</div>