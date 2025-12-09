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
  - icon: "fas fa-bolt"
    title: "Energy Sustainability"
    excerpt: "Focusing on smart building energy efficiency, benchmarking, and fault detection and diagnosis (FDD) for HVAC systems."
  - icon: "fas fa-microchip"
    title: "IoT & CPS"
    excerpt: "Bridging the gap between physical sensors and digital analysis through Cyber-Physical Systems and Internet of Things."
---

<style>
  /* 1. LAYOUT: CENTERED 1200px (Fixes Line Length & Alignment) */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; }
  
  #main { margin: 0 !important; padding: 0 !important; width: 100% !important; }

  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 100% !important; 
    max-width: 1200px !important; /* This aligns Header lines, Mission, and Cards perfectly */
    padding: 0 20px;
    box-sizing: border-box;
  }
  
  .page__content { width: 100% !important; max-width: 100% !important; }

  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* 2. MISSION STATEMENT STYLING */
  .notice--info { 
    font-size: 1.15em; 
    text-align: left !important;
    margin: 40px 0 40px 0; /* Adjusted margins */
    width: 75%; 
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

  /* 3. FEATURE CARD STYLING */
  .feature__wrapper {
    display: flex !important;
    flex-wrap: wrap;
    justify-content: space-between; /* Ensures they fill the 1200px exactly like the Mission box */
    gap: 20px;
    margin-bottom: 0 !important; /* Removes bottom spacing that might look like a gap */
    padding-bottom: 0 !important;
  }

  .feature__item {
    flex: 1; /* Equal width */
    min-width: 300px;
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 30px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    text-align: center;
    margin-bottom: 0 !important;
  }

  .feature__item:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
    border-color: #007bff;
  }

  /* Icon Animation */
  .feature__item-teaser {
    margin-bottom: 20px;
    color: #007bff;
  }
  
  .feature__item-teaser i { transition: transform 0.4s ease; }
  .feature__item:hover .feature__item-teaser i { transform: scale(1.2) rotate(5deg); }

  /* Text Styling */
  .archive__item-title { font-size: 1.3em; font-weight: 700; margin-bottom: 15px; }
  .archive__item-excerpt { font-size: 0.95em; line-height: 1.6; color: #555; }

  /* 4. ANIMATIONS */
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
  h1 { 
    font-size: 2.2em !important; 
    border-bottom: 2px solid #eee; 
    padding-bottom: 10px; 
    margin-bottom: 30px; 
    width: 100%; /* Obey the 1200px limit */
  }
</style>

# About the Lab
---

<div class="notice--info" markdown="1">
**Mission Statement**
* We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**.
* Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

{% include feature_row %}

<br>

# <i class="fas fa-newspaper"></i> What's New
