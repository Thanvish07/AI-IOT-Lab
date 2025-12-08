---
title: ""
permalink: publications.html
layout: single
author_profile: false
toc: true
toc_sticky: True
toc_label: "Year"
---

<style>
  /* --- 1. LAYOUT MATCHING JOINING-US.MD --- */
  .sidebar, .page__sidebar { display: none !important; }
  
  .page__inner-wrap { 
    float: none !important; 
    margin: 0 auto !important; 
    width: 100% !important; 
    max-width: 1200px !important; /* Matches joining-us.md exactly */
  }
  
  .page__content { width: 100% !important; }
  
  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* --- 2. CARD STYLING --- */
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

  /* Interactive Abstract */
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

  /* Animations */
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
      Short-term load forecasting (STLF) is crucial for energy management...
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
      Smart energy meters generate large volumes of fine-grained time series data...
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
      Short-term Load Forecasting (STLF) for buildings is essential...
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
      Recent advancements in Time Series Foundation Models (TSFMs)...
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
      The current manual visual inspection of built environments...
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
      In this paper, we employ a 1D deep convolutional generative adversarial network...
    </p>
  </details>

  <a href="https://arxiv.org/abs/2402.14384" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://arxiv.org/pdf/2402.14384" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>
