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
      My journey began with a basketball tactics training system in VR, sparking my passion for creating experiences that blend the physical and virtual. Since then, I've explored diverse approaches to immersion:
    </p>
    <p>
      Go!KartVR paired motion chair feedback with kart racing gameplay for physical sensation. Monkeying Around broke physical space limitations by letting players climb as a toy monkey searching for family. In The End used haptic gloves to create an emotionally resonant storytelling experience centered on human connection. Xhaler transformed breathing into a game mechanic using a respiration belt and wind sensors for intuitive, body-driven gameplay.
    </p>
    <p>
      Each project reflects my core interest: finding new ways for players to feel truly present in virtual worlds.
    </p>
    <p>
      When I'm not developing, you'll find me experimenting in the kitchen, on the basketball court setting up the perfect pass, or hanging out with cats.
    </p>
  </div>
  
  <div class="about-image">
    <img src="/assets/images/about/me.jpg" alt="About Me">
  </div>
</div>