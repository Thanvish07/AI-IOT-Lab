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
  /* --- 1. LAYOUT: WIDER (1600px) --- */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; }
  
  #main { margin: 0 !important; padding: 0 !important; width: 100% !important; }

  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important; 
    max-width: 1600px !important; /* Increased width to use right-side space */
    padding: 0 20px;
    box-sizing: border-box;
  }
  
  .page__content { width: 100% !important; max-width: 100% !important; }

  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* --- 2. MISSION STATEMENT --- */
  .notice--info { 
    font-size: 1.15em; 
    text-align: left !important;
    margin: 40px 0 50px 0;
    width: 100%; 
    max-width: 100%; 
    box-sizing: border-box;
    border-left: 5px solid #007bff;
    background: #f4f9ff;
    padding: 25px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    transition: transform 0.3s ease;
  }

  .notice--info:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 15px rgba(0,0,0,0.1);
  }

  /* --- 3. GRID LAYOUT (ONE ROW) --- */
  .feature__wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between; /* Spreads them evenly */
    gap: 30px;
    width: 100%;
  }

  /* --- 4. PREMIUM CARD STYLING --- */
  .feature__item {
    flex: 1 1 300px; /* Allow them to grow */
    max-width: 500px; /* Increased max-width so they fill the 1600px space without wrapping */
    background: #ffffff;
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 16px; 
    padding: 0; 
    box-shadow: 0 10px 30px rgba(0,0,0,0.04);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    text-align: left; 
    display: flex;
    flex-direction: column;
    margin-bottom: 0 !important;
  }

  /* Mobile: Stack them */
  @media (max-width: 1000px) {
    .feature__item { max-width: 100%; flex-basis: 100%; }
  }

  /* Gradient Border Effect */
  .feature__item::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; height: 4px;
    background: linear-gradient(90deg, #007bff, #00d4ff);
    transform: scaleX(0);
    transform-origin: left;
    transition: transform 0.4s ease;
  }

  .feature__item:hover::before { transform: scaleX(1); }

  /* Hover State */
  .feature__item:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 0 20px 40px rgba(0,123,255,0.15);
    border-color: transparent;
    z-index: 2;
  }

  /* --- 5. CONTENT STYLING --- */
  .feature__item-teaser {
    background: #f8faff; 
    padding: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #f0f0f0;
  }

  .feature__item-teaser i {
    font-size: 3em; 
    color: #007bff;
    transition: transform 0.5s ease;
    filter: drop-shadow(0 5px 10px rgba(0,0,0,0.1));
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

  .feature__item-body {
    padding: 30px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .archive__item-title {
    font-size: 1.4em;
    font-weight: 800;
    margin-bottom: 15px;
    color: #2c3e50;
  }
  
  .archive__item-excerpt {
    font-size: 1em;
    line-height: 1.7;
    color: #555;
    margin-bottom: 25px;
    flex-grow: 1;
  }

  /* Interactive Arrow */
  .read-more-arrow {
    margin-top: auto;
    font-weight: bold;
    color: #007bff;
    opacity: 0;
    transform: translateX(-10px);
    transition: all 0.3s ease;
    font-size: 0.9em;
    text-transform: uppercase;
    letter-spacing: 1px;
    display: inline-block;
    text-decoration: none !important;
  }

  .feature__item:hover .read-more-arrow {
    opacity: 1;
    transform: translateX(0);
  }
  
  .read-more-arrow:hover { color: #0056b3; }

  /* --- 6. ANIMATIONS --- */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  .feature__item, .notice--info, h1, .page__content p { 
    animation: fadeUp 0.8s ease-out forwards; 
    opacity: 0; 
  }
  
  h1 { animation-delay: 0s; }
  .notice--info { animation-delay: 0.2s; }
  .feature__item:nth-child(1) { animation-delay: 0.3s; }
  .feature__item:nth-child(2) { animation-delay: 0.4s; }
  .feature__item:nth-child(3) { animation-delay: 0.5s; }

  /* Typography */
  h1 { font-size: 2.2em !important; border-bottom: 2px solid #eee; padding-bottom: 10px; margin-bottom: 30px; width: 100%; }
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
