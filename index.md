---
layout: home
permalink: /
classes: wide
header:
  overlay_image: /assets/images/bg_2.png
  overlay_filter: "0.5"
  caption: "AIM-Lab @ RBCCPS, IISC"
  actions:
    - label: "Explore Our Research"
      url: "/themes.html"
      btn_class: "btn--primary"

feature_row:
  - icon: "fas fa-chart-line"
    title: "Data Science"
    excerpt: "Developing advanced machine learning and deep learning models for time-series analysis, prediction, and anomaly detection."
    url: "/themes.html" 
  - icon: "fas fa-bolt"
    title: "Energy Sustainability"
    excerpt: "Focusing on smart building energy efficiency, benchmarking, and fault detection and diagnosis (FDD) for HVAC systems."
    url: "/themes.html"
  - icon: "fas fa-microchip"
    title: "IoT & CPS"
    excerpt: "Bridging the gap between physical sensors and digital analysis through Cyber-Physical Systems and Internet of Things."
    url: "/themes.html"
---

<style>
  /* --- 1. LAYOUT FIX: FORCE CENTER ALIGNMENT --- */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; }
  
  #main { margin: 0 !important; padding: 0 !important; width: 100% !important; }

  /* This fixes the "Left-Sided" issue */
  .page__inner-wrap {
    float: none !important; /* Stops it from sticking to the left */
    margin-left: auto !important; /* Pushes from left */
    margin-right: auto !important; /* Pushes from right */
    width: 100% !important; 
    max-width: 1200px !important; /* Matches Themes.md width */
    padding: 0 20px;
    box-sizing: border-box;
  }
  
  .page__content { 
    width: 100% !important; 
    max-width: 100% !important; 
    margin: 0 auto !important;
  }

  @media (min-width: 64em) { 
    .page { 
      width: 100% !important; 
      padding: 0 !important; 
      float: none !important; /* Double check for large screens */
    } 
  }

  /* --- 2. MISSION STATEMENT (CENTERED TEXT) --- */
  .notice--info { 
    font-size: 1.15em; 
    text-align: center !important; /* Center the text inside */
    margin: 40px 0 50px 0;
    width: 100%; /* Fill container */
    max-width: 100%; 
    box-sizing: border-box;
    border-left: 5px solid #007bff;
    background: #f4f9ff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    transition: transform 0.3s ease;
  }

  .notice--info:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 15px rgba(0,0,0,0.1);
  }

  /* --- 3. FEATURE GRID (3 BOXES, 1 ROW, CENTERED) --- */
  .feature__wrapper {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 3 Equal Columns */
    gap: 30px;
    width: 100%;
    margin: 0 auto;
    box-sizing: border-box;
  }

  /* Stack on mobile */
  @media (max-width: 768px) {
    .feature__wrapper { grid-template-columns: 1fr; }
  }

  /* --- 4. CARD STYLING (Matches Themes.md) --- */
  .feature__item {
    background: #ffffff;
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 16px; 
    padding: 0; 
    box-shadow: 0 10px 30px rgba(0,0,0,0.04);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    text-align: center; /* Center text inside cards */
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  /* Gradient Border */
  .feature__item::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; height: 4px;
    background: linear-gradient(90deg, #007bff, #00d4ff);
    transform: scaleX(0);
    transform-origin: center;
    transition: transform 0.4s ease;
  }
  .feature__item:hover::before { transform: scaleX(1); }

  .feature__item:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 0 20px 40px rgba(0,123,255,0.15);
    border-color: transparent;
    z-index: 2;
  }

  /* --- 5. ICON STYLING --- */
  .feature__item-teaser {
    background: #f8faff; 
    padding: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #f0f0f0;
  }

  .feature__item-teaser i {
    font-size: 3.5em; 
    color: #007bff;
    transition: transform 0.5s ease;
    filter: drop-shadow(0 5px 15px rgba(0,0,0,0.1));
  }

  @keyframes pulseIcon {
    0% { transform: scale(1); }
    50% { transform: scale(1.15); }
    100% { transform: scale(1); }
  }

  .feature__item:hover .feature__item-teaser i {
    animation: pulseIcon 1.5s infinite;
    color: #00d4ff; 
  }

  /* --- 6. CONTENT STYLING --- */
  .feature__item-body {
    padding: 25px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .archive__item-title {
    font-size: 1.4em;
    font-weight: 800;
    margin-bottom: 12px;
    color: #2c3e50;
  }
  
  .archive__item-excerpt {
    font-size: 0.95em;
    line-height: 1.7;
    color: #555;
    margin-bottom: 20px;
    flex-grow: 1;
  }

  /* Interactive Arrow */
  .read-more-arrow {
    margin-top: auto;
    font-weight: bold;
    color: #007bff;
    text-decoration: none !important;
    display: inline-block;
    transition: transform 0.3s ease;
  }

  .feature__item:hover .read-more-arrow {
    transform: scale(1.1);
    color: #0056b3;
  }

  /* Typography Polish */
  h1 { 
    font-size: 2.2em !important; 
    border-bottom: 2px solid #eee; 
    padding-bottom: 10px; 
    margin-bottom: 30px; 
    width: 100%;
    text-align: center; /* Center the Title */
  }
  
  /* Animations */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .feature__item, .notice--info, h1 { animation: fadeUp 0.8s ease-out forwards; opacity: 0; }
  h1 { animation-delay: 0s; }
  .notice--info { animation-delay: 0.2s; }
  .feature__item:nth-child(1) { animation-delay: 0.3s; }
  .feature__item:nth-child(2) { animation-delay: 0.4s; }
  .feature__item:nth-child(3) { animation-delay: 0.5s; }
</style>

# About the Lab
---

<div class="notice--info" markdown="1">
**Mission Statement**
* We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**.
* Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

<div class="feature__wrapper">
  {% for feature in page.feature_row %}
    <div class="feature__item">
      <div class="feature__item-teaser">
        <i class="{{ feature.icon }}"></i>
      </div>
      <div class="feature__item-body">
        <h2 class="archive__item-title">{{ feature.title }}</h2>
        <div class="archive__item-excerpt">
          <p>{{ feature.excerpt }}</p>
        </div>
        <a href="{{ feature.url }}" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
      </div>
    </div>
  {% endfor %}
</div>

<br>

# <i class="fas fa-newspaper"></i> What's New
