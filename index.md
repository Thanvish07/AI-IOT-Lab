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
  /* --- 1. LAYOUT CONSISTENCY --- */
  .sidebar, .page__sidebar { display: none !important; }
  
  .page__inner-wrap { 
    float: none !important; 
    margin: 0 auto !important; 
    width: 100% !important; 
    max-width: 1200px !important; 
    padding: 0 20px;
    box-sizing: border-box;
  }
  .page__content { width: 100% !important; }
  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* --- 2. ADVANCED CARD STYLING --- */
  .feature__row {
    display: flex !important;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    margin-top: 40px;
  }

  .feature__item {
    flex: 1 1 320px; 
    max-width: 360px;
    background: #ffffff;
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 16px; 
    padding: 0; 
    box-shadow: 0 10px 30px rgba(0,0,0,0.04); 
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); 
    position: relative;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    text-align: left; 
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

  .feature__item:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 0 20px 40px rgba(0,123,255,0.15);
    border-color: transparent;
  }

  /* --- 3. IMAGE & ICON STYLING --- */
  .archive__item-teaser {
    background: #f8faff; 
    padding: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #f0f0f0;
    position: relative;
  }

  .archive__item-teaser img {
    height: 120px;
    width: auto;
    object-fit: contain;
    transition: transform 0.5s ease;
    filter: drop-shadow(0 5px 15px rgba(0,0,0,0.1));
  }

  @keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); }
  }

  .feature__item:hover .archive__item-teaser img {
    animation: pulse 1.5s infinite;
  }

  /* --- 4. CONTENT STYLING --- */
  .feature__item-content {
    padding: 25px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .feature__item-title {
    font-size: 1.4em;
    font-weight: 800;
    margin-bottom: 12px;
    color: #2c3e50;
    letter-spacing: -0.5px;
  }
  
  .feature__item-content p {
    color: #555;
    font-size: 0.95em;
    line-height: 1.7;
    margin-bottom: 20px;
  }

  /* Interactive Arrow Link Styling */
  .read-more-arrow {
    margin-top: auto;
    font-weight: bold;
    color: #007bff !important; /* Force color */
    opacity: 0;
    transform: translateX(-10px);
    transition: all 0.3s ease;
    font-size: 0.9em;
    text-transform: uppercase;
    letter-spacing: 1px;
    text-decoration: none !important; /* No underline */
    cursor: pointer;
    display: inline-block;
  }

  .feature__item:hover .read-more-arrow {
    opacity: 1;
    transform: translateX(0);
  }

  .read-more-arrow:hover {
    color: #0056b3 !important;
  }

  /* --- 5. WATERFALL ENTRANCE --- */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .feature__item { opacity: 0; animation: fadeUp 0.8s ease-out forwards; }
  .feature__item:nth-child(1) { animation-delay: 0.1s; }
  .feature__item:nth-child(2) { animation-delay: 0.2s; }
  .feature__item:nth-child(3) { animation-delay: 0.3s; }

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
