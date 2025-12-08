---
title: ""
permalink: /projects.html
layout: single
author_profile: false
toc: true
toc_sticky: false
toc_label: "Active Projects"
---

<style>
  /* 1. LAYOUT STYLE (Standardized Center) */
  .sidebar, .page__sidebar { display: none !important; }
  
  .page__inner-wrap { 
    float: none !important; 
    margin: 0 auto !important; 
    width: 95% !important; 
    max-width: 1600px !important; /* Visual pages get more width */
    padding: 0 20px;
    box-sizing: border-box;
  }
  
  .page__content { width: 100% !important; }
  
  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* 2. CARD STYLING */
  .feature__row {
    display: flex !important;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    margin-top: 30px;
  }

  .feature__item {
    flex: 1 1 300px;
    max-width: 450px;
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 0;
    padding-bottom: 20px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    position: relative;
    overflow: hidden;
    margin-bottom: 0 !important;
    display: flex;
    flex-direction: column;
  }

  .feature__item:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
    border-color: #007bff;
  }

  .archive__item-teaser {
    background: #f1f1f1;
    margin: 0;
    overflow: hidden;
    height: 220px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #eee;
  }

  .archive__item-teaser img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.6s ease;
  }

  .feature__item:hover .archive__item-teaser img { transform: scale(1.1); }

  .feature__item-content {
    padding: 25px;
    flex: 1;
    display: flex;
    flex-direction: column;
  }

  .feature__item-title {
    font-size: 1.35em;
    font-weight: 700;
    margin-bottom: 10px;
    color: #222;
  }
  
  .feature__item-content p {
    color: #555;
    font-size: 0.95em;
    line-height: 1.6;
    flex-grow: 1;
  }

  .btn--small { align-self: flex-start; margin-top: 15px; }

  /* 3. ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .feature__item { opacity: 0; animation: fadeUp 0.8s ease-out forwards; }
  .feature__item:nth-child(1) { animation-delay: 0.1s; }
  .feature__item:nth-child(2) { animation-delay: 0.2s; }
  .feature__item:nth-child(3) { animation-delay: 0.3s; }
  .feature__item:nth-child(4) { animation-delay: 0.4s; }
</style>

# Research Projects
---

We focus on a variety of themes at the intersection of **Cyber-Physical Systems** and **Data Science**, spanning from theoretical frameworks to real-world deployment.

## Active Projects

<div class="feature__row">

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/anomaly.png" alt="Energy Anomaly Detection">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Energy Anomaly Detection (LEAD)</h3>
      <p>Developing techniques and a Large-scale Anomaly Detection (LEAD) dataset for building energy consumption analysis.</p>
      <a href="#" class="btn btn--primary btn--small">View Details</a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/fault.png" alt="Fault Detection">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Fault Detection (FDD)</h3>
      <p>Using data-driven methods for fault detection and diagnosis (FDD) in commercial chiller systems to improve efficiency.</p>
      <a href="#" class="btn btn--primary btn--small">View Details</a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/infrared.png" alt="Infrared Thermography">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Infrared Thermography (IRT)</h3>
      <p>Leveraging Infrared Thermography for city-scale building diagnostics, occupant behaviour, and energy auditing.</p>
      <a href="#" class="btn btn--primary btn--small">View Details</a>
    </div>
  </div>

  <div class="feature__item">
    <div class="archive__item-teaser">
      <img src="/AI-IOT-Lab/assets/images/benchmarking.png" alt="Building Benchmarking">
    </div>
    <div class="feature__item-content">
      <h3 class="feature__item-title">Building Benchmarking</h3>
      <p>Creating more accurate and explanatory building energy benchmarking systems for Singapore and India.</p>
      <a href="#" class="btn btn--primary btn--small">View Details</a>
    </div>
  </div>

</div>
