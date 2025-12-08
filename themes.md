---
title: ""
permalink: /themes.html
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Core Themes"

themes_list:
  - image: "/assets/images/EA.png"
    title: "Energy Monitoring"
    excerpt: "We develop systems to collect and process high-frequency **smart meter time-series data**. By monitoring consumption patterns at granular levels, we enable real-time visibility into building performance and identify opportunistic data sources."
  
  - image: "/assets/images/EB.png"
    title: "Energy Benchmarking"
    excerpt: "Comparing raw energy consumption is often unfair due to varying building sizes and operations. We build **data-driven benchmarking models** that normalize for weather and occupancy, allowing for accurate peer-to-peer comparison."
  
  - image: "/assets/images/PA.png"
    title: "Energy Prediction"
    excerpt: "Forecasting future energy demand is critical for grid stability. We apply statistical and machine learning techniques to **predict load profiles** based on historical smart meter data, weather forecasts, and calendar variables."
  
  - image: "/assets/images/AD.png"
    title: "Anomaly Detection"
    excerpt: "Buildings often waste energy due to unnoticed irregularities. We research unsupervised learning algorithms to automatically scan time-series data and **detect point and contextual anomalies**, flagging unusual consumption spikes."

  - image: "/assets/images/fault.png"
    title: "Fault Detection (FDD)"
    excerpt: "Going beyond simple anomalies, we focus on identifying specific equipment failures. Our FDD research utilizes system-level data to **diagnose root causes** of inefficiencies in HVAC components like Chillers and AHUs."
---

<style>
  /* GLOBAL FIXES */
  .sidebar, .page__sidebar { display: none !important; }
  .page__inner-wrap { float: none !important; margin: 0 auto !important; width: 100% !important; max-width: 1200px !important; }
  .page__content { width: 100% !important; }
  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* THEME LIST SPECIFIC STYLES */
  .feature__wrapper { display: flex; flex-direction: column; gap: 30px; }
  
  .feature__item {
    display: flex; flex-direction: row; align-items: center;
    background: #fff; border: 1px solid #e0e0e0; border-radius: 8px;
    padding: 25px; box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  }
  
  /* Image Styles */
  .feature__item .archive__item-teaser img {
    width: 200px !important; height: auto; object-fit: contain;
    margin-right: 30px; border-radius: 4px;
  }
  
  /* Text Styles */
  .archive__item-title { font-size: 1.5em !important; margin-top: 0 !important; }
  .archive__item-excerpt { font-size: 1.05em; line-height: 1.6; color: #444; }

  /* Mobile Responsive */
  @media (max-width: 768px) {
    .feature__item { flex-direction: column; text-align: center; }
    .feature__item .archive__item-teaser img { margin: 0 0 20px 0; }
  }
</style>

## Research Themes

Our research philosophy is grounded in the convergence of **Data Science** and **Cyber-Physical Systems**.

## Core Methodologies

We primarily leverage **smart meter time series** and other opportunistic data sources to develop systems and techniques for the following key areas:

{% include custom_feature_row.html id="themes_list" type="left" %}
