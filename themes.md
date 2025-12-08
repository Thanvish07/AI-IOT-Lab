---
title: ""
permalink: /themes.html
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Core Themes"
---

<style>
  /* 1. AGGRESSIVE LAYOUT RESET (Full Width) */
  .sidebar, .page__sidebar { display: none !important; }
  
  #main { margin: 0 !important; padding: 0 !important; width: 100% !important; max-width: 100% !important; }

  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important; 
    max-width: 1600px !important;
    padding: 0 20px !important;
    box-sizing: border-box;
  }
  
  .page__content { width: 100% !important; max-width: 100% !important; }

  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* 2. THEME CARD STYLING */
  /* Override the default feature row to be a flexible grid */
  .feature__row {
    display: flex !important;
    flex-wrap: wrap;
    justify-content: center; /* Center cards if they don't fill the row */
    gap: 30px;
    margin-top: 30px;
  }

  .feature__item {
    flex: 1 1 300px; /* Grow, Shrink, Basis (Min width 300px) */
    max-width: 400px; /* Don't get too wide on huge screens */
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 25px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    position: relative;
    overflow: hidden;
    margin-bottom: 0 !important; /* CSS Grid handles gap */
    text-align: center; /* Center align content for better look */
  }

  /* Hover Effect: Lift & Shadow */
  .feature__item:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
    border-color: #007bff;
  }

  /* 3. IMAGE STYLING & ZOOM EFFECT */
  .archive__item-teaser {
    background: #f8f9fa;
    border-radius: 8px;
    padding: 15px;
    margin-bottom: 20px;
    overflow: hidden; /* Contains the zoom */
  }

  .archive__item-teaser img {
    max-height: 160px;
    object-fit: contain;
    width: 100%;
    transition: transform 0.5s ease; /* Smooth zoom */
  }

  /* Zoom image on card hover */
  .feature__item:hover .archive__item-teaser img {
    transform: scale(1.1);
  }

  /* 4. TEXT STYLING */
  .feature__item-title {
    font-size: 1.4em;
    font-weight: 700;
    margin-bottom: 10px;
    color: #333;
  }
  
  .feature__item-content p {
    color: #555;
    font-size: 0.95em;
    line-height: 1.6;
  }

  /* 5. ANIMATIONS (Waterfall Effect) */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .feature__item {
    opacity: 0; /* Start hidden */
    animation: fadeUp 0.8s ease-out forwards;
  }

  /* Stagger delays */
  .feature__item:nth-child(1) { animation-delay: 0.1s; }
  .feature__item:nth-child(2) { animation-delay: 0.2s; }
  .feature__item:nth-child(3) { animation-delay: 0.3s; }
  .feature__item:nth-child(4) { animation-delay: 0.4s; }
  .feature__item:nth-child(5) { animation-delay: 0.5s; }

</style>

# Research Themes
---

Our research philosophy is grounded in the convergence of **Data Science** and **Cyber-Physical Systems**.

## Core Methodologies

We primarily leverage **smart meter time series** and other opportunistic data sources to develop systems and techniques for the following key areas:

---

<div class="feature__row">

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EA.png" alt="Energy Monitoring">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Monitoring</h3>
      <p>We develop systems to collect and process high-frequency <strong>smart meter time-series data</strong>. By monitoring consumption patterns at granular levels, we enable real-time visibility into building performance.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EB.png" alt="Energy Benchmarking">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Benchmarking</h3>
      <p>Comparing raw energy consumption is often unfair. We build <strong>data-driven benchmarking models</strong> that normalize for weather and occupancy, allowing for accurate peer-to-peer comparison.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/PA.png" alt="Energy Prediction">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Prediction</h3>
      <p>Forecasting future energy demand is critical. We apply statistical and machine learning techniques to <strong>predict load profiles</strong> based on historical smart meter data and weather forecasts.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/AD.png" alt="Anomaly Detection">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Anomaly Detection</h3>
      <p>We research unsupervised learning algorithms to automatically scan time-series data and <strong>detect point and contextual anomalies</strong>, flagging unusual consumption spikes.</p>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/fault.png" alt="Fault Detection (FDD)">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Fault Detection (FDD)</h3>
      <p>Going beyond simple anomalies, we focus on specific failures. Our FDD research utilizes system-level data to <strong>diagnose root causes</strong> of inefficiencies in HVAC components.</p>
    </div>
  </div>

</div>
