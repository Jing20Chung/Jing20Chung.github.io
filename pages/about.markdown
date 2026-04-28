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

  .pdf-preview-container {
    width: 80%;
    margin: 40px auto;
    border-top: 1px solid #eee;
    padding-top: 20px;
  }

  .pdf-wrapper {
    position: relative;
    width: 100%; 
    padding-top: 100%;
    background: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 4px;
    overflow: hidden;
  }

  .pdf-wrapper iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: none;
  }

  .download-link {
    display: inline-block;
    margin-top: 12px;
    font-size: 14px;
    color: #2a7ae2;
    text-decoration: none;
    font-weight: 500;
  }

  .download-link:hover {
    text-decoration: underline;
  }
  .pdf-full-width {
    grid-column: 1 / span 2;
    width: 100%;
    margin-top: 50px;
  }

  @media (max-width: 768px) {
    .pdf-full-width {
      grid-column: 1;
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
<div class="pdf-preview-container">
  <h3 style="margin-top: 0;">Resume</h3>
  <div class="pdf-wrapper">
    <iframe src="{{ 'assets/pdfs/Ming-Fen_Jing_Chung_Resume.pdf' | relative_url }}">
      This browser does not support PDF previews. Please 
      <a href="{{ 'assets/pdfs/Ming-Fen_Jing_Chung_Resume.pdf' | relative_url }}">click here to download the PDF</a>.
    </iframe>
  </div>
  <a href="{{ 'assets/pdfs/Ming-Fen_Jing_Chung_Resume.pdf' | relative_url }}" class="download-link" target="_blank">
    <i class="fas fa-external-link-alt"></i> Open in New Window / Download Full Version
  </a>
</div>
