---
layout: default
title: Projects
permalink: /projects/
---

<style>
  .projects-gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
    margin-top: 30px;
    padding: 0 20%
  }
  
  .project-card {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    overflow: hidden;
    background: #fff;
    cursor: pointer;
  }
  
  .project-card-link {
    display: block;
    text-decoration: none;
    color: inherit;
    height: 100%;
  }
  
  .project-image-wrapper {
    position: relative;
    width: 100%;
    height: 200px;
    background: #f0f0f0;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #999;
    font-size: 14px;
    overflow: hidden;
  }
  
  .project-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
  }
  
  .project-card:hover .project-image {
    transform: scale(1.05);
  }
  
  .project-overlay {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.6);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s ease;
  }
  
  .project-card:hover .project-overlay {
    opacity: 1;
  }
  
  .overlay-content {
    color: white;
    text-align: center;
    padding: 20px;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  
  .overlay-title {
    font-size: 24px;
    font-weight: 700;
    margin: 0;
  }
  
  .overlay-description {
    font-size: 14px;
    line-height: 1.5;
    margin: 0;
  }
  
  h1 {
    padding: 1% 20% 0% 20%;
  }
</style>

{% assign sorted_projects = site.projects | sort: "date" | reverse %}

<h1>Projects</h1>
<div class="projects-gallery">
  
  {% for project in sorted_projects %}
    <a href="{{ project.url | relative_url }}" class="project-card-link">
      <div class="project-card">
        <div class="project-image-wrapper">
          {% if project.image %}
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
          {% else %}
            <span>No image</span>
          {% endif %}
          <div class="project-overlay">
            <div class="overlay-content">
              <h3 class="overlay-title">{{ project.title }}</h3>
            </div>
          </div>
        </div>
      </div>
    </a>
  {% endfor %}
</div>