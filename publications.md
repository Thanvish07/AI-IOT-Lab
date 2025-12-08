---
title: ""
permalink: publications.html
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Year"
---

<style>
  /* 1. HIDE AUTHOR PROFILE (Left Sidebar) */
  .page__sidebar { display: none !important; }

  /* 2. MAIN CONTAINER (Widespread) */
  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important;
    max-width: 1600px !important;
    padding: 0 20px;
    box-sizing: border-box;
  }

  /* 3. SPLIT SCREEN LOGIC (Desktop Only) */
  @media (min-width: 64em) {
    .layout--single .page {
      width: 100% !important;
      padding-right: 0 !important;
    }

    /* Content Area: Takes 75% of width */
    .page__content {
      width: 75% !important;
      float: left !important;
      padding-right: 40px !important; /* Safety gap */
      box-sizing: border-box;
    }

    /* TOC Sidebar: Takes 25% of width */
    .sidebar__right {
      width: 25% !important;
      float: right !important;
      display: block !important;
      margin-left: 0 !important;
      opacity: 0; /* Fade in animation for TOC too */
      animation: fadeUp 1s ease-out 0.5s forwards;
    }
    
    /* Ensure sticky works */
    .sidebar__right.sticky { top: 20px; }
  }

  /* 4. CARD STYLING (Alive & Interactive) */
  .pub-card {
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 12px; /* Smooth corners */
    padding: 25px;
    margin-bottom: 25px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
    border-left: 5px solid #d9d9d9;
    position: relative;
  }

  /* Hover Effect: Lift up + Highlight */
  .pub-card:hover {
    transform: translateY(-7px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    border-left-color: #007bff;
    border-color: #b8daff;
  }

  /* 5. TYPOGRAPHY */
  .pub-title {
    font-size: 1.25em;
    font-weight: 700;
    color: #222;
    margin-bottom: 8px;
    display: block;
    line-height: 1.4;
  }
  
  .pub-meta {
    font-size: 0.95em;
    color: #666;
    margin-bottom: 15px;
    font-style: italic;
  }

  /* 6. INTERACTIVE DETAILS (Abstract) */
  details {
    margin-top: 15px;
    margin-bottom: 15px;
    background: #f8f9fa;
    border-radius: 6px;
    padding: 12px;
    cursor: pointer;
    border: 1px solid #eee;
    transition: background 0.2s;
  }
  
  details:hover { background: #f1f3f5; }

  summary {
    font-weight: 600;
    color: #0056b3;
    outline: none;
    list-style: none; /* Hide default triangle */
  }
  
  /* Add custom icon */
  summary::-webkit-details-marker { display: none; }
  summary:before {
    content: "+";
    display: inline-block;
    width: 20px;
    font-weight: bold;
  }
  details[open] summary:before { content: "-"; }

  /* 7. WATERFALL ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .pub-card {
    opacity: 0; /* Start hidden */
    animation: fadeUp 0.7s cubic-bezier(0.2, 0.8, 0.2, 1) forwards;
  }

  /* Stagger delays */
  .pub-card:nth-of-type(1) { animation-delay: 0.1s; }
  .pub-card:nth-of-type(2) { animation-delay: 0.2s; }
  .pub-card:nth-of-type(3) { animation-delay: 0.3s; }
  .pub-card:nth-of-type(4) { animation-delay: 0.4s; }
  .pub-card:nth-of-type(5) { animation-delay: 0.5s; }
  .pub-card:nth-of-type(6) { animation-delay: 0.6s; }

</style>

# Publications
---

## 2025

<div class="pub-card">
  <span class="pub-title">Mix-BEATS: Mixer-enhanced Basis Expansion Analysis for Load Forecasting</span>
  <div class="pub-meta">
    Anuj Kumar, Harish Kumar Saravanan, Shivam Dwivedi, Pandarasamy Arjunan. <br>
    <em>Proceedings of the 16th ACM International Conference on Future and Sustainable Energy Systems</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      Short-term load forecasting (STLF) is crucial for energy management and integrating renewables, but traditional models often fail to generalize across diverse buildings. While Time Series Foundation Models (TSFM) offer potential, most are transformer-based, making them computationally heavy and unsuitable for edge deployment. We introduce Mix-BEATS, a lightweight and accurate model combining N-BEATS and TSMixer architectures for building-level energy prediction.
    </p>
  </details>

  <a href="https://dl.acm.org/doi/full/10.1145/3679240.3734632" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://dl.acm.org/doi/pdf/10.1145/3679240.3734632" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>

<div class="pub-card">
  <span class="pub-title">Are Time Series Foundation models good for Energy Anomaly Detection?</span>
  <div class="pub-meta">
    Basu Hela, Praveen Prasad Handigol, Pandarasamy Arjunan. <br>
    <em>Proceedings of the 16th ACM International Conference on Future and Sustainable Energy Systems</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      Smart energy meters generate large volumes of fine-grained time series data that captures building’s energy consumption patterns. This data can be leveraged to detect anomalous energy consumption patterns and reduce energy waste in buildings. Traditional anomaly detection methods for smart meter data rely on statistical and machine learning techniques, which often struggle to model complex temporal patterns, require extensive feature engineering, and have poor scalability.
    </p>
  </details>

  <a href="https://dl.acm.org/doi/full/10.1145/3679240.3734633" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://dl.acm.org/doi/pdf/10.1145/3679240.3734633" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>

<div class="pub-card">
  <span class="pub-title">MixForecast: Mixer-Enhanced Foundation Model for Load Forecasting</span>
  <div class="pub-meta">
    Anuj Kumar, Harish Kumar Saravanan, Shivam Dwivedi, Pandarasamy Arjunan. <br>
    <em>Proceedings of the 2nd International Workshop on Foundation Models for Cyber-Physical Systems & Internet of Things</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      Short-term Load Forecasting (STLF) for buildings is essential for optimizing energy management and supporting renewable energy integration, but traditional models often struggle with generalization across diverse building profiles. While recent Time Series Foundation Models (TSFMs) show promise, they remain underexplored for STLF. In this paper, we introduce MixForecast, a novel TSFM for universal energy forecasting.
    </p>
  </details>

  <a href="https://dl.acm.org/doi/abs/10.1145/3722565.3727193" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://dl.acm.org/doi/pdf/10.1145/3722565.3727193" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>

## 2024

<div class="pub-card">
  <span class="pub-title">Analyzing the performance of time series foundation models for short-term load forecasting</span>
  <div class="pub-meta">
    Harish Kumar Saravanan, Shivam Dwivedi, P Praveen, Pandarasamy Arjunan. <br>
    <em>Proceedings of the 11th ACM International Conference on Systems for Energy-Efficient Buildings, Cities, and Transportation</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      Recent advancements in Time Series Foundation Models (TSFMs), pre-trained on extensive time series data from diverse domains, offer a promising domain-agnostic solution that can handle universal forecasting tasks without requiring task-specific training. In this paper, we analyze the performance of four open-source TSFMs - Chronos, Lag-Llama, Moirai, and TimesFM - for STLF in both commercial and residential buildings.
    </p>
  </details>

  <a href="https://dl.acm.org/doi/abs/10.1145/3671127.3698708" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://dl.acm.org/doi/pdf/10.1145/3671127.3699536" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>

<div class="pub-card">
  <span class="pub-title">BD3: Building Defects Detection Dataset for Benchmarking Computer Vision Techniques</span>
  <div class="pub-meta">
    Praveen Kottari, Pandarasamy Arjunan. <br>
    <em>Proceedings of the 11th ACM International Conference on Systems for Energy-Efficient Buildings, Cities, and Transportation</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      The current manual visual inspection of built environments is time-consuming, labor-intensive, prone to errors, costly, and lacks scalability. To address these limitations, automated building inspection techniques have emerged in recent years, leveraging low-cost computer vision systems, drones and mobile robots. However, the practical implementation of these systems is hindered by the lack of robust and generalizable models trained on comprehensive defect image datasets. In this paper, we present BD3: Building Defects Detection Dataset, a comprehensive image dataset designed to benchmark computer vision techniques aimed at improving the robustness and generalizability of automated building inspection systems.
    </p>
  </details>

  <a href="https://dl.acm.org/doi/abs/10.1145/3671127.3698789" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://dl.acm.org/doi/pdf/10.1145/3671127.3698789" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>

<div class="pub-card">
  <span class="pub-title">Generative Adversarial Network with Soft-Dynamic Time Warping and Parallel Reconstruction</span>
  <div class="pub-meta">
    Hardik Prabhu, Jayaraman Valadi, Pandarasamy Arjunan. <br>
    <em>arXiv:2402.14384</em>
  </div>
  
  <details>
    <summary>Read Abstract</summary>
    <p style="margin-top: 10px; font-size: 0.95em; color: #444; line-height: 1.6;">
      In this paper, we employ a 1D deep convolutional generative adversarial network (DCGAN) for sequential anomaly detection in energy time series data. Anomaly detection involves gradient descent to reconstruct energy sub-sequences, identifying the noise vector that closely generates them through the generator network. Soft-DTW is used as a differentiable alternative for the reconstruction loss and is found to be superior to Euclidean distance.
    </p>
  </details>

  <a href="https://arxiv.org/abs/2402.14384" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://arxiv.org/pdf/2402.14384" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>
