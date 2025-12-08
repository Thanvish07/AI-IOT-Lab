---
layout: home
permalink: /
classes: wide
header:
  overlay_image: /assets/images/bg_2.png
  overlay_filter: "0.5"
  caption: "AI-IOT Lab @ RBCCPS, IISC"
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
  /* 1. AGGRESSIVE LAYOUT RESET */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; width: 0 !important; }
  
  #main {
    margin-left: 0 !important; margin-right: 0 !important;
    padding-left: 0 !important; padding-right: 0 !important;
    width: 100% !important; max-width: 100% !important;
  }

  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important; 
    max-width: 1600px !important;
    padding: 0 20px !important;
  }

  /* 2. MISSION STATEMENT FIX (Left Aligned) */
  .notice--info { 
    font-size: 1.15em; 
    text-align: left !important; /* FIXED: Now Left Aligned */
    margin: 30px 0 50px 0; /* Removed auto margins to stick left */
    max-width: 100%; 
    border-left: 5px solid #007bff;
    background: #f4f9ff;
    padding: 20px;
    border-radius: 4px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
  }

  /* 3. CARD CONTAINER FIX (Prevent Overflow) */
  .feature__wrapper {
    display: flex !important;
    justify-content: space-between;
    gap: 20px; /* Consistent gap between cards */
    flex-wrap: wrap; /* Allows wrapping on small mobile screens */
  }

  /* 4. INDIVIDUAL CARD FIX (Fixed Size & Behavior) */
  .feature__item {
    flex: 1; /* Forces all 3 cards to be equal width */
    min-width: 280px; /* Prevents them from getting too squished */
    max-width: 32%; /* Ensures 3 cards fit perfectly in one row */
    
    background: #fff;
    border-radius: 8px;
    padding: 25px;
    border: 1px solid #eee; 
    box-shadow: 0 4px 6px rgba(0,0,0,0.05);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .feature__item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    border-color: #ddd;
    z-index: 10;
  }

  /* 5. ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  .feature__item, .notice--info, h1 { opacity: 0; }
  h1 { animation: fadeUp 0.8s ease-out forwards; }
  .notice--info { animation: fadeUp 0.8s ease-out 0.2s forwards; }
  
  .feature__wrapper .feature__item:nth-child(1) { animation: fadeUp 0.8s ease-out 0.4s forwards; }
  .feature__wrapper .feature__item:nth-child(2) { animation: fadeUp 0.8s ease-out 0.5s forwards; }
  .feature__wrapper .feature__item:nth-child(3) { animation: fadeUp 0.8s ease-out 0.6s forwards; }

</style>

# About the Lab

<div class="notice--info" markdown="1">
**Mission Statement**
* We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**.
* Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

{% include feature_row %}

# <i class="fas fa-newspaper"></i> What's New
---
