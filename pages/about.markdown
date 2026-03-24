---
layout: default
title: About
permalink: /about/
---

<style>
  .about-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
    align-items: start;
    min-height: 500px;
    padding: 5% 20%;
  }

  .about-text {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  
  .about-text h2 {
    font-size: 36px;
    font-weight: 700;
    white-space: normal;
    margin: 0 0 15px 0;
  }
  
  .about-text p {
    font-size: 16px;
    line-height: 1.8;
    color: #555;
    margin: 0 0 15px 0;
  }
  
  .about-image {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .about-image img {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  }
  
  @media (max-width: 768px) {
    .about-container {
      grid-template-columns: 1fr;
      gap: 30px;
    }
  }
</style>

<div class="about-container">
  <div class="about-text">
    <h2>Hi! I'm a VR enthusiast, basketball player, and cat lover.</h2>
    <p>
      I am a VR/XR engineer with a background that cuts across hardware and experience design. Before coming to games, I spent four years as a Principal Firmware Engineer in Taiwan, building real expertise in the system layer from driver behavior to hardware timing. I left that career behind to pursue the question that had been pulling at me for years: what can VR become when the body is fully part of the experience?
    </p>
    <p>
      Since arriving at Carnegie Mellon's Entertainment Technology Center, that question has driven every project I have taken on. I have built a breath-controlled VR experience, originated and led a haptic-glove narrative piece exploring whether physical sensation can carry emotional weight, and designed a mixed reality system that turns real physical objects into interactive elements. Across all of it, I keep returning to the same intersection: immersive technology and non-traditional input. My firmware foundation lets me work close to the hardware, and my time at ETC sharpened my instinct to ask the right question before reaching for a solution. I build systems that serve experiences, and I am always asking whether they do.
    </p>
    <p>
      When I'm not developing, you'll find me experimenting in the kitchen, on the basketball court setting up the perfect pass, or hanging out with cats.
    </p>
  </div>
  
  <div class="about-image">
    <img src="{{ '/assets/images/about/me.jpg' | relative_url }}" alt="About Me">
  </div>
</div>