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
  .feature__item:nth-child(4) { animation-delay: 0.4s; }
  .feature__item:nth-child(5) { animation-delay: 0.5s; }

</style>

# Research Themes
---

Our research philosophy is grounded in the convergence of **Data Science** and **Cyber-Physical Systems**.

## Core Methodologies

We primarily leverage **smart meter time series** and other opportunistic data sources to develop systems and techniques for the following key areas:

<div class="feature__row">

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EA.png" alt="Energy Monitoring">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Monitoring</h3>
      <p>We develop systems to collect and process high-frequency <strong>smart meter time-series data</strong>. By monitoring consumption patterns at granular levels, we enable real-time visibility into building performance.</p>
      
      <a href="#" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/EB.png" alt="Energy Benchmarking">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Benchmarking</h3>
      <p>Comparing raw energy consumption is often unfair. We build <strong>data-driven benchmarking models</strong> that normalize for weather and occupancy, allowing for accurate peer-to-peer comparison.</p>
      
      <a href="#" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/PA.png" alt="Energy Prediction">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Prediction</h3>
      <p>Forecasting future energy demand is critical. We apply statistical and machine learning techniques to <strong>predict load profiles</strong> based on historical smart meter data and weather forecasts.</p>
      
      <a href="#" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/AD.png" alt="Anomaly Detection">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Anomaly Detection</h3>
      <p>We research unsupervised learning algorithms to automatically scan time-series data and <strong>detect point and contextual anomalies</strong>, flagging unusual consumption spikes.</p>
      
      <a href="#" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/fault.png" alt="Fault Detection (FDD)">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Fault Detection (FDD)</h3>
      <p>Going beyond simple anomalies, we focus on specific failures. Our FDD research utilizes system-level data to <strong>diagnose root causes</strong> of inefficiencies in HVAC components.</p>
      
      <a href="#" class="read-more-arrow">Explore <i class="fas fa-arrow-right"></i></a>
    </div>
  </div>

</div>
