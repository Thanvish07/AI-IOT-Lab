---
layout: home
permalink: /
header:
  overlay_image: /assets/images/bg_2.png
  overlay_filter: "0.5"
  caption: "AI-IOT Lab @ RBCCPS, IISC"
  actions:
    - label: "Explore Research"
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
  
  /* 4. General Typography Fixes */
  h1 { font-size: 2.2em !important; border-bottom: 2px solid #eee; padding-bottom: 10px; }
  .notice--info { font-size: 1.1em; text-align: center; }
</style>

# About the Lab

<div class="notice--info" markdown="1">
  * We focus on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**. <br>
  * Our goal is to build data-driven solutions that solve real-world challenges in smart built environments.
</div>

{% include feature_row %}

# <i class="fas fa-newspaper"></i> What's New

<div style="text-align: center; margin-top: 30px;">
  <a href="/year-archive/" class="btn btn--inverse">View News Archive</a>
</div>
