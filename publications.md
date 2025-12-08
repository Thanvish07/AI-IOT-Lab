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
  /* 1. LAYOUT LOGIC (Wide Center + Right TOC) */
  
  /* Hide the LEFT sidebar (Author profile) only */
  .page__sidebar { display: none !important; }

  /* Allow the container to use full width */
  .page__inner-wrap {
    float: none !important;
    margin: 0 auto !important;
    width: 95% !important;
    max-width: 1600px !important;
  }

  /* On Desktop: Split screen between Content (Left) and TOC (Right) */
  @media (min-width: 64em) {
    .layout--single .page {
      width: 100% !important;
      padding-right: 0 !important;
    }

    /* Main Content takes 75% width */
    .page__content {
      width: 75% !important;
      float: left !important;
      padding-right: 30px !important; /* Buffer space between text and TOC */
    }

    /* TOC Sidebar takes 25% width */
    .sidebar__right {
      width: 25% !important;
      float: right !important;
      display: block !important; /* Force TOC to show */
      margin-left: 0 !important;
    }
    
    /* Fix sticky positioning */
    .sidebar__right.sticky {
      top: 20px;
    }
  }

  /* 2. CARD STYLING */
  .pub-card {
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border-left: 4px solid #d9d9d9;
  }

  .pub-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    border-left-color: #007bff;
  }

  .pub-title {
    font-size: 1.2em;
    font-weight: bold;
    color: #333;
    margin-bottom: 5px;
    display: block;
  }
  
  .pub-meta {
    font-size: 0.95em;
    color: #666;
    margin-bottom: 15px;
    font-style: italic;
  }

  /* 3. INTERACTIVE DETAILS */
  details {
    margin-top: 10px;
    margin-bottom: 15px;
    background: #f9f9f9;
    border-radius: 4px;
    padding: 10px;
    cursor: pointer;
  }

  summary { font-weight: bold; color: #0056b3; outline: none; }
  summary:hover { text-decoration: underline; }

  /* 4. ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .pub-card { opacity: 0; animation: fadeUp 0.6s ease-out forwards; }
  .pub-card:nth-of-type(1) { animation-delay: 0.1s; }
  .pub-card:nth-of-type(2) { animation-delay: 0.2s; }
  .pub-card:nth-of-type(3) { animation-delay: 0.3s; }
  .pub-card:nth-of-type(4) { animation-delay: 0.4s; }
  .pub-card:nth-of-type(5) { animation-delay: 0.5s; }
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      Short-term load forecasting (STLF) is crucial for energy management and integrating renewables, but traditional models often fail to generalize across diverse buildings. We introduce Mix-BEATS, a lightweight and accurate model combining N-BEATS and TSMixer architectures for building-level energy prediction.
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      Smart energy meters generate large volumes of fine-grained time series data that captures building’s energy consumption patterns. This data can be leveraged to detect anomalous energy consumption patterns and reduce energy waste in buildings.
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      Short-term Load Forecasting (STLF) for buildings is essential for optimizing energy management. While recent Time Series Foundation Models (TSFMs) show promise, they remain underexplored for STLF. In this paper, we introduce MixForecast, a novel TSFM for universal energy forecasting.
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      Recent advancements in Time Series Foundation Models (TSFMs), pre-trained on extensive time series data from diverse domains, offer a promising domain-agnostic solution. In this paper, we analyze the performance of four open-source TSFMs - Chronos, Lag-Llama, Moirai, and TimesFM.
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      We present BD3: Building Defects Detection Dataset, a comprehensive image dataset designed to benchmark computer vision techniques aimed at improving the robustness and generalizability of automated building inspection systems.
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
    <p style="margin-top: 10px; font-size: 0.95em; color: #444;">
      In this paper, we employ a 1D deep convolutional generative adversarial network (DCGAN) for sequential anomaly detection in energy time series data using Soft-DTW as a differentiable alternative for the reconstruction loss.
    </p>
  </details>

  <a href="https://arxiv.org/abs/2402.14384" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://arxiv.org/pdf/2402.14384" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>
