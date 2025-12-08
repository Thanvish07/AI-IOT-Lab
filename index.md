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
  /* 1. Hide the sidebar container completely */
  .sidebar, .page__sidebar {
    display: none !important;
  }

  /* 2. FORCE the page to ignore the sidebar grid layout */
  @media (min-width: 64em) {
    .layout--single .page, 
    .layout--home .page, 
    .layout--archive .page {
      display: block !important; /* Kills the grid */
      padding-left: 0 !important;
      padding-right: 0 !important;
      margin-left: 0 !important;
      margin-right: 0 !important;
    }
  }

  /* 3. Force the content wrapper to touch the edges */
  .page__inner-wrap {
    float: none !important;
    margin-left: 0 !important;
    margin-right: 0 !important;
    width: 100% !important;
    max-width: 100% !important;
    padding-left: 20px !important; /* Small padding so text doesn't touch screen edge */
    padding-right: 20px !important;
  }

  /* 4. Fix the Content Width itself */
  .page__content {
    width: 100% !important;
    max-width: 100% !important;
  }
</style>

# About the Lab
---

<div class="notice--info">
  <h4 class="no_toc">Mission Statement</h4>
  <p>Our lab is part of the <strong>Robert Bosch Centre for Cyber-Physical Systems (RBCCPS)</strong> at the <strong>Indian Institute of Science (IISc)</strong>. We focus on the intersection of <strong>Machine Learning</strong>, <strong>IoT</strong>, and <strong>Sustainability</strong> to build data-driven solutions for smart built environments.</p>
</div>

{% include feature_row %}

# <i class="fas fa-newspaper"></i> What's New

<div style="text-align: center; margin-top: 20px;">
  <a href="/year-archive/" class="btn btn--inverse">View News Archive</a>
</div>
