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
      Short-term load forecasting (STLF) is crucial for energy management and integrating renewables, but traditional models often fail to generalize across diverse buildings. While Time Series Foundation Models (TSFM) offer potential, most are transformer-based, making them computationally heavy and unsuitable for edge deployment. We introduce Mix-BEATS, a lightweight and accurate model combining N-BEATS and TSMixer architectures for buildinglevel energy prediction. Adapting TSMixer originated from MLPMixer, originally designed for vision tasks using pure MLP blocks for patchwise and spatial mixing, we leverage its principles for temporal forecasting. Mix-BEATS is trained on hourly smart-meter data from 38,956 buildings and evaluated on a held-out set of 1,000 buildings using the NRMSE metric. We compare Mix-BEATS againststate-of-the-art TSFMs such as Lag-Llama, Moirai, Chronos, and Tiny Time Mixers in zero-shot and fine-tuned settings, as well as generic models including Autoformer, N-BEATS, TS-Mixer, etc., under domain-specific training and testing. In both comparisons, Mix-BEATS consistently outperforms the baselines, demonstrating robust generalization and efficiency for real-world STLF tasks. Code: https://github.com/AI-IoT-Lab/Mix-BEATS.
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
      Smart energy meters generate large volumes of fine-grained time series data that captures building’s energy consumption patterns. This data can be leveraged to detect anomalous energy consumption patterns and reduce energy waste in buildings. Traditional anomaly detection methods for smart meter data rely on statistical and machine learning techniques, which often struggle to model complex temporal patterns, require extensive feature engineering, and have poor scalability. Foundation models for time series, which are pretrained on massive volumes of time series data from diverse domains, have recently emerged as a versatile and scalable tool for time series analysis. They are capable of handling multiple tasks, including anomaly detection, and demonstrating superior performance compared to traditional models in various domains. Despite their potential for cross-domain applications, their applicability to the energy domain and their performance compared to traditional machine learning models remain largely unexplored.
Therefore, in this paper, we analyze the applicability and performance of Time Series Foundation Models (TSFMs) for unsupervised energy anomaly detection. Specifically, we compare the performance of two widely used state-of-the-art TSFMs, TimeGPT and MOMENT, against existing anomaly detection techniques in the literature: (a) two statistical methods (Interquartile Range (IQR) and Modified Z-Score (mZ-Score)), (b) two unsupervised machine learning techniques (Isolation Forest and Local Outlier Factor), and (c) a deep learning-based technique, Variational Autoencoder (VAE). Our experimental results, conducted using the LEAD 1.0 dataset, which consists of annotated hourly energy readings of 200 buildings, show that MOMENT outperforms both traditional statistical methods and unsupervised machine learning methods. Our results reveal that fine-tuning of MOMENT marginally improves its performance. VAE trained from scratch surpasses TSFMs in performance despite having a smaller model size. We also analyze the trade-off between performance, scalability, and compute requirements of these models. Our analysis also provides new research directions for using TSFMs in the energy domain.
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
      Short-term Load Forecasting (STLF) for buildings is essential for optimizing energy management and supporting renewable energy integration, but traditional models often struggle with generalization across diverse building profiles. While recent Time Series Foundation Models (TSFMs) show promise, they remain underexplored for STLF. In this paper, we introduce MixForecast, a novel TSFM for universal energy forecasting. The MixForecast architecture is based on the TSMixer block ensembling technique to provide accurate and robust load forecasting for smart meter time series. In particular, MixForecast is designed with fewer parameters approx 0.19M than existing TSFMs, making it efficient and suitable for deployment in individual buildings. We trained MixForecast using hourly energy data from 63K buildings and evaluated its performance on a test set of 1,000 commercial and residential buildings around the world. We compared MixForecast against pre-trained TSFMs such as Tiny Time Mixers, Lag-Llama, Moirai, and Chronos, in both zero-shot and fine-tuned settings, as well as against traditional models. The model demonstrates superior accuracy and adaptability, excelling in various building profiles. Its lightweight design, combined with strong forecasting performance, establishes MixForecast as a versatile and efficient model for STLF, advancing energy management while promoting sustainable energy practices.
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
      The recent advancements in Time Series Foundation Models (TSFMs), which are pre-trained on vast time series corpus from diverse domains and designed to handle universal forecasting tasks without the need for task-specific training, present a promising domain-agnostic, one-size-fits-all solution. In this paper, we analyze the performance of four open-source TSFMs - Chronos, Lag-Llama, Moirai, and TimesFM - for short-term load forecasting (STLF) in both commercial and residential buildings. Specifically, we benchmark these models' zero-shot prediction capabilities, assessing their ability to perform STLF on unseen buildings, and compare them to state-of-the-art models. Our experimental results, conducted on a large-scale dataset of over 1,900 real-world residential and commercial buildings, reveal that the Chronos model achieves the lowest Normalized Root Mean Squared Error (NRMSE) compared to the contemporary models and demonstrates comparable performance with an existing pre-trained TSFM for the energy domain from the BuildingsBench platform.
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
      The current manual visual inspection of built environments is time-consuming, labor-intensive, prone to errors, costly, and lacks scalability. To address these limitations, automated building inspection techniques have emerged in recent years, leveraging low-cost computer vision systems, drones and mobile robots. However, the practical implementation of these systems is hindered by the lack of robust and generalizable models trained on comprehensive defect image datasets. In this paper, we present BD3: Building Defects Detection Dataset, a comprehensive image dataset designed to benchmark computer vision techniques aimed at improving the robustness and generalizability of automated building inspection systems. The BD3 dataset contains 3,965 high-quality, manually collected, and annotated images. Unlike other datasets that primarily focus on crack and non-crack images, BD3 includes images of six distinct building defects (algae, major crack, minor crack, peeling, spalling, and stain), as well as images representing normal building conditions. We benchmarked the BD3 using five state-of-the-art computer vision models to classify defect and normal images. The experimental results indicate that the Vision Transformer (ViT) model achieved the highest F1-scores of 0.9342 and 0.9879 on the original and augmented datasets, respectively. The BD3 dataset and its accompanying reproducible codebase are publicly available for benchmarking other defect detection algorithms.
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
      In this paper, we employ a 1D deep convolutional generative adversarial network (DCGAN) for sequential anomaly detection in energy time series data. Anomaly detection involves gradient descent to reconstruct energy sub-sequences, identifying the noise vector that closely generates them through the generator network. Soft-DTW is used as a differentiable alternative for the reconstruction loss and is found to be superior to Euclidean distance. Combining reconstruction loss and the latent space's prior probability distribution serves as the anomaly score. Our novel method accelerates detection by parallel computation of reconstruction of multiple points and shows promise in identifying anomalous energy consumption in buildings, as evidenced by performing experiments on hourly energy time series from 15 buildings.
    </p>
  </details>

  <a href="https://arxiv.org/abs/2402.14384" class="btn btn--primary btn--x-small">Link</a>
  <a href="https://arxiv.org/pdf/2402.14384" class="btn btn--inverse btn--x-small"><i class="fas fa-file-pdf"></i> PDF</a>
</div>
