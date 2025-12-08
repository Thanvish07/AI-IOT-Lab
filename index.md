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
  /* -----------------------------------------------------------
     1. AGGRESSIVE LAYOUT RESET (Fixing the Left Space) 
     ----------------------------------------------------------- */
  /* Remove sidebar completely from layout calculation */
  .sidebar, .page__sidebar, .sidebar__right { 
    display: none !important; 
    width: 0 !important;
  }

  /* Force the main container to touch the left edge */
  #main {
    margin-left: 0 !important; margin-right: 0 !important;
    padding-left: 0 !important; padding-right: 0 !important;
    width: 100% !important; max-width: 100% !important;
  }

  /* Expand the content wrapper to 95% of the screen */
  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important; 
    max-width: 1800px !important; /* Huge cap for wide monitors */
    padding: 0 !important;
  }

  /* Ensure the theme's grid logic doesn't add left padding */
  @media (min-width: 64em) {
    .layout--home .page {
      padding-left: 0 !important; padding-right: 0 !important;
      width: 100% !important;
      float: none !important;
    }
  }

  /* -----------------------------------------------------------
     2. MAKING IT ALIVE (Interactivity) 
     ----------------------------------------------------------- */
  
  /* Feature Cards (The 3 icons) - Base Style */
  .feature__item {
    background: #fff;
    border-radius: 12px;
    padding: 30px;
    transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1); /* Smooth physics-like motion */
    border: 1px solid transparent; 
    box-shadow: 0 4px 6px rgba(0,0,0,0.02); /* Subtle initial shadow */
  }

  /* Hover Effect: Lift up + Deep Shadow */
  .feature__item:hover {
    transform: translateY(-12px); /* Lifts the card */
    box-shadow: 0 20px 30px rgba(0,0,0,0.1), 0 10px 10px rgba(0,0,0,0.05);
    border-color: #eee;
    z-index: 10;
  }

  /* Icon Animation on Hover */
  .feature__item:hover .feature__item-teaser i {
    color: #d9534f; /* Change to brand color (adjust as needed) */
    transform: scale(1.2) rotate(8deg); /* Grow and tilt slightly */
    transition: transform 0.3s ease, color 0.3s ease;
  }

  /* Mission Statement Box Styling */
  .notice--info { 
    font-size: 1.25em; 
    text-align: center; 
    margin: 40px auto 60px auto; 
    max-width: 85%; 
    border-left: 6px solid #007bff;
    background: #f4f9ff;
    padding: 25px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    transition: transform 0.3s ease;
  }
  
  /* Make the mission box pulse slightly on hover */
  .notice--info:hover {
    transform: scale(1.02);
    background: #e6f2ff;
  }

  /* -----------------------------------------------------------
     3. STAGGERED ENTRANCE ANIMATIONS (Waterfall Effect)
     ----------------------------------------------------------- */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  /* Hide elements initially */
  .feature__item, .notice--info, h1 { opacity: 0; }

  /* Apply animations with delays */
  h1 { animation: fadeUp 0.8s ease-out forwards; }
  .notice--info { animation: fadeUp 0.8s ease-out 0.2s forwards; }
  
  /* Stagger the 3 feature cards so they appear one by one */
  .feature__wrapper .feature__item:nth-child(1) { animation: fadeUp 0.8s ease-out 0.4s forwards; }
  .feature__wrapper .feature__item:nth-child(2) { animation: fadeUp 0.8s ease-out 0.6s forwards; }
  .feature__wrapper .feature__item:nth-child(3) { animation: fadeUp 0.8s ease-out 0.8s forwards; }

</style>

# About the Lab
---

<div class="notice--info" markdown="1">
**Mission Statement**
* We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**.
* Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

{% include feature_row %}

# <i class="fas fa-newspaper"></i> What's New
---
