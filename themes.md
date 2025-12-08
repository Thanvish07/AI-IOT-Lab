---
title: ""
permalink: /themes.html
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Themes"
---

<style>
  /* 1. Hide Sidebar Completely */
  .sidebar, .page__sidebar { display: none !important; }

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

  /* 4. Grid Card Styling */
  .feature__item { margin-bottom: 30px; }
  .archive__item-teaser img { 
    max-height: 200px; 
    object-fit: contain; /* Keeps the whole image visible */
    width: 100%; 
    border-radius: 6px;
    background: #f8f8f8; /* Subtle background for transparent PNGs */
    padding: 10px;
  }
</style>

# Research Themes
---

Our research philosophy is grounded in the convergence of **Data Science** and **Cyber-Physical Systems**.

## Core Methodologies

We primarily leverage **smart meter time series** and other opportunistic data sources to develop systems and techniques for the following key areas:

---

<div class="feature__row feature__row--left">

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EA.png" alt="Energy Monitoring">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Monitoring</h3>
      <p>We develop systems to collect and process high-frequency <strong>smart meter time-series data</strong>. By monitoring consumption patterns at granular levels, we enable real-time visibility into building performance and identify opportunistic data sources.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EB.png" alt="Energy Benchmarking">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Benchmarking</h3>
      <p>Comparing raw energy consumption is often unfair due to varying building sizes and operations. We build <strong>data-driven benchmarking models</strong> that normalize for weather and occupancy, allowing for accurate peer-to-peer comparison.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/PA.png" alt="Energy Prediction">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Prediction</h3>
      <p>Forecasting future energy demand is critical for grid stability. We apply statistical and machine learning techniques to <strong>predict load profiles</strong> based on historical smart meter data, weather forecasts, and calendar variables.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/AD.png" alt="Anomaly Detection">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Anomaly Detection</h3>
      <p>Buildings often waste energy due to unnoticed irregularities. We research unsupervised learning algorithms to automatically scan time-series data and <strong>detect point and contextual anomalies</strong>, flagging unusual consumption spikes.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/fault.png" alt="Fault Detection (FDD)">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Fault Detection (FDD)</h3>
      <p>Going beyond simple anomalies, we focus on identifying specific equipment failures. Our FDD research utilizes system-level data to <strong>diagnose root causes</strong> of inefficiencies in HVAC components like Chillers and AHUs.</p>
    </div>
  </div>

</div>
