---
title: "Lab Members"
permalink: /people.html
layout: single
author_profile: false
toc: true
toc_sticky: true
toc_label: "Team"
---

<style>
  /* 1. LAYOUT RESET (Widespread Fix) */
  .sidebar, .page__sidebar { display: none !important; }
  .page__inner-wrap { float: none !important; margin: 0 auto !important; width: 100% !important; max-width: 1200px !important; }
  .page__content { width: 100% !important; }
  @media (min-width: 64em) { .page { width: 100% !important; padding: 0 !important; } }

  /* 2. PERSON CARD STYLING */
  .person-card {
    display: flex;
    flex-direction: row;
    align-items: center;
    background: #fff;
    border: 1px solid #e0e0e0;
    border-radius: 12px; /* Smooth corners */
    padding: 25px;
    margin-bottom: 30px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    position: relative;
    overflow: hidden; /* Keeps zoom effect inside card */
  }

  /* Hover Effect: Lift & Shadow */
  .person-card:hover {
    transform: translateY(-7px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    border-color: #007bff; /* Highlight border on hover */
  }

  /* 3. AVATAR STYLING */
  .avatar-box {
    flex-shrink: 0;
    width: 150px;
    height: 150px;
    margin-right: 30px;
    overflow: hidden;
    border-radius: 8px; /* Rectangular as requested */
    border: 3px solid #f0f0f0;
  }

  .avatar-box img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease; /* Smooth zoom */
  }

  /* Zoom photo on hover */
  .person-card:hover .avatar-box img {
    transform: scale(1.1);
  }

  /* 4. TEXT CONTENT */
  .person-info { flex: 1; }

  .person-name {
    margin-top: 0;
    margin-bottom: 5px;
    font-size: 1.5em;
    font-weight: 700;
    color: #333;
  }

  .person-role {
    font-size: 0.95em;
    text-transform: uppercase;
    letter-spacing: 1px;
    color: #007bff; /* Brand color */
    font-weight: bold;
    margin-bottom: 10px;
    display: block;
  }

  .person-focus {
    background: #f4f9ff;
    padding: 8px 12px;
    border-radius: 6px;
    font-size: 0.9em;
    color: #444;
    display: inline-block;
    margin-bottom: 15px;
    border-left: 3px solid #007bff;
  }

  /* 5. ANIMATIONS (Waterfall Effect) */
  @keyframes slideIn {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .person-card {
    opacity: 0; /* Start hidden */
    animation: slideIn 0.7s ease-out forwards;
  }

  /* Stagger delays for sequential loading */
  .person-card:nth-of-type(1) { animation-delay: 0.1s; }
  .person-card:nth-of-type(2) { animation-delay: 0.2s; }
  .person-card:nth-of-type(3) { animation-delay: 0.3s; }
  .person-card:nth-of-type(4) { animation-delay: 0.4s; }
  .person-card:nth-of-type(5) { animation-delay: 0.5s; }

  /* Mobile Responsive */
  @media (max-width: 768px) {
    .person-card { flex-direction: column; text-align: center; }
    .avatar-box { margin-right: 0; margin-bottom: 20px; }
  }
</style>

# Lab Members
---

## Lab Head

<div class="person-card">
  <div class="avatar-box">
    <img src="/AI-IOT-Lab/assets/images/speaker_pandarasamy.jpg" alt="Pandarasamy Arjunan">
  </div>
  <div class="person-info">
    <h3 class="person-name">Pandarasamy Arjunan</h3>
    <span class="person-role">Assistant Professor</span>
    <div class="person-focus">
      <strong>Research:</strong> CPS, Data Science, and Energy Sustainability
    </div>
    <div class="author__urls-wrapper">
      <a href="mailto:samy@iisc.ac.in" class="btn btn--inverse btn--small"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://www.linkedin.com/in/pandarasamy-arjunan-5580a215" class="btn btn--primary btn--small"><i class="fab fa-linkedin"></i> LinkedIn</a>
      <a href="https://scholar.google.com/citations?user=6zG4VnQAAAAJ" class="btn btn--info btn--small"><i class="fas fa-graduation-cap"></i> Scholar</a>
    </div>
  </div>
</div>

## PhD Students

<div class="person-card">
  <div class="avatar-box">
    <img src="/AI-IOT-Lab/assets/images/Person.jpg" alt="Jane">
  </div>
  <div class="person-info">
    <h3 class="person-name">Jane</h3>
    <span class="person-role">PhD Student</span>
    <div class="person-focus">
      <strong>Focus:</strong> Energy Anomaly Detection & Deep Learning
    </div>
    <div class="author__urls-wrapper">
      <a href="mailto:Jane@iisc.ac.in" class="btn btn--inverse btn--small"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://linkedin.com/in/Jane" class="btn btn--primary btn--small"><i class="fab fa-linkedin"></i> LinkedIn</a>
    </div>
  </div>
</div>

## M.Tech Students

<div class="person-card">
  <div class="avatar-box">
    <img src="/AI-IOT-Lab/assets/images/Person.jpg" alt="Jack">
  </div>
  <div class="person-info">
    <h3 class="person-name">Jack</h3>
    <span class="person-role">M.Tech Student</span>
    <div class="person-focus">
      <strong>Focus:</strong> Sustainable Energy Solutions & IoT Systems
    </div>
    <div class="author__urls-wrapper">
      <a href="mailto:Jack@iisc.ac.in" class="btn btn--inverse btn--small"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://linkedin.com/in/Jack" class="btn btn--primary btn--small"><i class="fab fa-linkedin"></i> LinkedIn</a>
    </div>
  </div>
</div>

## Project Staff

<div class="person-card">
  <div class="avatar-box">
    <img src="/AI-IOT-Lab/assets/images/Person.jpg" alt="Peter">
  </div>
  <div class="person-info">
    <h3 class="person-name">Peter</h3>
    <span class="person-role">Project Associate</span>
    <div class="person-focus">
      <strong>Focus:</strong> Energy Time-Series Modeling & Analysis
    </div>
    <div class="author__urls-wrapper">
      <a href="mailto:Peter@iisc.ac.in" class="btn btn--inverse btn--small"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://linkedin.com/in/Peter" class="btn btn--primary btn--small"><i class="fab fa-linkedin"></i> LinkedIn</a>
    </div>
  </div>
</div>
