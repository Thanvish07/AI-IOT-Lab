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
  /* 1. Hide Sidebar Completely */
  .sidebar, .page__sidebar, .sidebar__right { display: none !important; }

  /* 2. Force Content to Center and take Full Width */
  .page__inner-wrap {
    float: none !important;
    margin-left: auto !important; margin-right: auto !important;
    width: 100% !important; max-width: 1200px !important;
    padding-right: 20px; padding-left: 20px;
  }
  .page__content { width: 100% !important; max-width: 100% !important; }
  
  /* 3. Fix Layout logic for large screens */
  @media (min-width: 64em) {
    .layout--single .page, .layout--home .page, .layout--archive .page {
      padding-left: 0 !important; padding-right: 0 !important;
      width: 100% !important;
    }
  }

  /* 4. Animations (Make it Alive) */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  .feature__item, .notice--info, h1, h2, .page__content p {
    animation: fadeUp 0.8s ease-out forwards;
  }
  
  /* 5. Typography Polish */
  h1 { font-size: 2.2em !important; border-bottom: 2px solid #eee; padding-bottom: 10px; }
  .notice--info { font-size: 1.1em; text-align: center; }
</style>

# About the Lab

<div class="notice--info" markdown="1">
### Mission Statement
* We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**.
* Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

{% include feature_row %}

# <i class="fas fa-newspaper"></i> What's New

<div style="text-align: center; margin-top: 40px;">
  <a href="/year-archive/" class="btn btn--inverse btn--large">View News Archive</a>
</div>
