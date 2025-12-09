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
  /* --- 1. LAYOUT: EXACT MATCH WITH THEMES.MD --- */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; }
  
  #main { margin: 0 !important; padding: 0 !important; width: 100% !important; }

  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 100% !important; 
    max-width: 1200px !important; /* Strictly 1200px like Themes.md */
    padding: 0 20px;
    box-sizing: border-box;
  }
  
  .page__content { width: 100% !important; max-width: 100% !important; }

  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* --- 2. MISSION STATEMENT ALIGNMENT --- */
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

  /* --- 3. FLEX CARD CONTAINER (Copied from Themes.md) --- */
  .feature__wrapper {
    display: flex !important;
    flex-wrap: wrap;
    justify-content: center;
    gap: 25px; /* Matches Themes.md spacing */
    width: 100%;
    margin-bottom: 0 !important;
  }

  /* --- 4. CARD STYLING (Copied from Themes.md) --- */
  .feature__item {
    flex: 1 1 300px;
    max-width: 350px; /* Exact width from Themes.md */
    background: #ffffff;
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 16px; 
    padding: 25px; /* Added padding back to match Themes.md style */
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    position: relative;
    overflow: hidden;
    text-align: center; /* Center aligned text like Themes.md */
    display: flex;
    flex-direction: column;
    margin-bottom: 0 !important;
  }

  /* Hover Effect: Lift Up */
  .feature__item:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    border-color: #007bff;
  }

  /* --- 5. ICON STYLING (Adapted to match Image Box in Themes.md) --- */
  .feature__item-teaser {
    background: #f8faff; /* Matches image background */
    border-radius: 8px;
    padding: 15px;
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100px; /* Fixed height to mimic image area */
  }

  .feature__item-teaser i {
    font-size: 3.5em; 
    color: #007bff;
    transition: transform 0.5s ease;
    filter: drop-shadow(0 5px 10px rgba(0,0,0,0.1));
  }

  /* Pulse Animation */
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
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .archive__item-title {
    font-size: 1.3em;
    font-weight: 700;
    margin-bottom: 10px;
    color: #333;
  }
  
  .archive__item-excerpt {
    font-size: 0.95em;
    line-height: 1.6;
    color: #555;
    margin-bottom: 20px;
    flex-grow: 1;
  }

  /* Interactive Arrow */
  .read-more-arrow {
    margin-top: auto;
    font-weight: bold;
    color: #007bff !important;
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
  
  .read-more-arrow:hover { color: #0056b3 !important; }

  /* --- 7. ANIMATIONS --- */
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

  /* Typography Polish */
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
