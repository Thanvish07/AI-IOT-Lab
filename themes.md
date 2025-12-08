---
title: "Research Themes"
permalink: /themes.html
classes: wide
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Core Themes"

# Defining the 5 core themes
themes_list:
  - image: "/assets/images/EA.png"
    title: "Energy Monitoring"
    excerpt: "We develop systems to collect and process high-frequency **smart meter time-series data**. By monitoring consumption patterns at granular levels, we enable real-time visibility into building performance and identify opportunistic data sources for deeper analysis."

  - image: "/assets/images/EB.png"
    title: "Energy Benchmarking"
    excerpt: "Comparing raw energy consumption is often unfair due to varying building sizes and operations. We build **data-driven benchmarking models** that normalize for weather and occupancy, allowing for accurate peer-to-peer comparison and efficiency ranking."

  - image: "/assets/images/PA.png"
    title: "Energy Prediction"
    excerpt: "Forecasting future energy demand is critical for grid stability. We apply statistical and machine learning techniques to **predict load profiles** based on historical smart meter data, weather forecasts, and calendar variables."

  - image: "/assets/images/AD.png"
    title: "Anomaly Detection"
    excerpt: "Buildings often waste energy due to unnoticed irregularities. We research unsupervised learning algorithms to automatically scan time-series data and **detect point and contextual anomalies**, flagging unusual consumption spikes in real-time."
    
  - image: "/assets/images/fault.png" 
    title: "Fault Detection (FDD)"
    excerpt: "Going beyond simple anomalies, we focus on identifying specific equipment failures. Our FDD research utilizes system-level data to **diagnose root causes** of inefficiencies in HVAC components like Chillers and Air Handling Units."
---

<style>
  /* -----------------------------------------------------
     1. FIX LEFT SPACE (Make page full width)
     ----------------------------------------------------- */
  .sidebar, .page__sidebar { display: none !important; }

  @media (min-width: 64em) {
    .layout--single .page {
      display: block !important;
      padding-left: 0 !important; padding-right: 0 !important;
      margin-left: 0 !important; margin-right: 0 !important;
    }
  }

  .page__inner-wrap {
    float: none !important; margin: 0 !important;
    width: 100% !important; max-width: 100% !important;
    padding: 0 20px !important;
  }

  .page__content { width: 100% !important; max-width: 100% !important; }

  /* -----------------------------------------------------
     2. THEMES SPECIFIC: LIST VIEW (Line after Line)
     ----------------------------------------------------- */
  
  /* Force the grid wrapper to be a single column */
  .feature__wrapper {
    display: flex !important;
    flex-direction: column !important; /* Stack vertically */
    gap: 30px; /* Space between rows */
  }

  /* Make each item take full width and look like a row */
  .feature__item {
    width: 100% !important;
    max-width: 100% !important;
    display: flex; /* Use flexbox for Image Left / Text Right layout */
    flex-direction: row;
    align-items: flex-start;
    background: #f9f9f9; /* Light grey background for separation */
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  }
  
  /* Style the inner teaser container to work with flex */
  .feature__item .archive__item-teaser {
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 100%;
    text-align: left; /* Ensure text aligns left */
  }

  /* Style the Image */
  .feature__item img {
    width: 150px !important; /* Fixed width for consistency */
    height: auto;
    margin-right: 30px !important; /* Space between image and text */
    margin-bottom: 0 !important;
    object-fit: contain;
  }

  /* Style the Text Area */
  .feature__item-content {
    flex: 1; /* Take remaining space */
  }

  /* Mobile Responsive: Stack them on small screens */
  @media (max-width: 768px) {
    .feature__item .archive__item-teaser {
      flex-direction: column;
      text-align: center;
    }
    .feature__item img {
      margin-right: 0 !important;
      margin-bottom: 20px !important;
    }
  }
</style>

# Research Themes
---

Our current research interests lie in the intersection of **Cyber-Physical Systems** and **Data Science**, specifically applied to smart built environments and energy sustainability. 


## Core Methodologies

We primarily leverage **smart meter time series** and other opportunistic data sources to develop systems and techniques for the following key areas:

{% include custom_feature_row.html id="themes_list" type="left" %}
