---
layout: default
title: USACO Training
description: USA Computing Olympiad Competition Preparation
---

<style>
  .course-hero {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    padding: 4rem 2rem;
    border-radius: 20px;
    color: white;
    text-align: center;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .course-hero::before {
    content: '🏆';
    position: absolute;
    font-size: 15rem;
    opacity: 0.1;
    right: -50px;
    top: -50px;
    transform: rotate(-15deg);
  }

  .level-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
  }

  .level-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 2px solid #E5E7EB;
    transition: all 0.3s;
    text-align: center;
  }

  .level-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
  }

  .bronze { border-top: 4px solid #CD7F32; }
  .silver { border-top: 4px solid #C0C0C0; }
  .gold { border-top: 4px solid #FFD700; }
  .platinum { border-top: 4px solid #E5E4E2; }

  .level-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .level-name {
    font-size: 1.5rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .level-topics {
    color: #6B7280;
    line-height: 1.6;
    text-align: left;
  }
</style>

<div class="course-hero">
  <h1>USACO Training Program</h1>
  <p>Your Path from Bronze to Platinum</p>
</div>

<!-- Course Content Structure -->
<h2 style="text-align: center; color: #1F2937; margin-bottom: 3rem;">
  <span class="en-content">Complete Competition Curriculum</span>
  <span class="zh-content">完整竞赛课程体系</span>
</h2>

<div class="level-cards">
  <!-- Bronze Level -->
  <div class="level-card bronze">
    <div class="level-icon">🥉</div>
    <h3 class="level-name">Bronze Division</h3>
    <div class="level-topics">
      <p><strong>Getting Started</strong></p>
      <ul>
        <li>Introduction to USACO</li>
        <li>Input/Output handling</li>
        <li>Complete Search</li>
        <li>Greedy Algorithms basics</li>
        <li>Simulation problems</li>
        <li>Basic sorting</li>
      </ul>
    </div>
  </div>

  <!-- Silver Level -->
  <div class="level-card silver">
    <div class="level-icon">🥈</div>
    <h3 class="level-name">Silver Division</h3>
    <div class="level-topics">
      <p><strong>Core Algorithms</strong></p>
      <ul>
        <li>Graph Theory (DFS, BFS)</li>
        <li>Flood Fill</li>
        <li>Binary Search</li>
        <li>Two Pointers</li>
        <li>Prefix Sums</li>
        <li>Custom Comparators</li>
      </ul>
    </div>
  </div>

  <!-- Gold Level -->
  <div class="level-card gold">
    <div class="level-icon">🥇</div>
    <h3 class="level-name">Gold Division</h3>
    <div class="level-topics">
      <p><strong>Advanced Techniques</strong></p>
      <ul>
        <li>Dynamic Programming</li>
        <li>Shortest Paths (Dijkstra, SPFA)</li>
        <li>Minimum Spanning Trees</li>
        <li>Disjoint Set Union</li>
        <li>Topological Sort</li>
        <li>Euler Paths</li>
      </ul>
    </div>
  </div>

  <!-- Platinum Level -->
  <div class="level-card platinum">
    <div class="level-icon">💎</div>
    <h3 class="level-name">Platinum Division</h3>
    <div class="level-topics">
      <p><strong>Expert Level</strong></p>
      <ul>
        <li>Advanced DP & Optimization</li>
        <li>Network Flow</li>
        <li>Computational Geometry</li>
        <li>Advanced Data Structures</li>
        <li>String Algorithms</li>
        <li>Number Theory</li>
      </ul>
    </div>
  </div>
</div>

<!-- Training Features -->
<div style="background: #F9FAFB; padding: 3rem; border-radius: 15px; margin: 3rem 0;">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 2rem;">
    <span class="en-content">Our Training Approach</span>
    <span class="zh-content">我们的培训方法</span>
  </h2>
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem;">
    <div style="text-align: center;">
      <div style="font-size: 2rem; margin-bottom: 1rem;">📝</div>
      <h3 style="color: #1F2937;">1000+ Problems</h3>
      <p style="color: #6B7280;">Curated problem sets for each level</p>
    </div>
    
    <div style="text-align: center;">
      <div style="font-size: 2rem; margin-bottom: 1rem;">🎯</div>
      <h3 style="color: #1F2937;">Contest Strategy</h3>
      <p style="color: #6B7280;">Time management and problem selection</p>
    </div>
    
    <div style="text-align: center;">
      <div style="font-size: 2rem; margin-bottom: 1rem;">💻</div>
      <h3 style="color: #1F2937;">Mock Contests</h3>
      <p style="color: #6B7280;">Regular practice competitions</p>
    </div>
    
    <div style="text-align: center;">
      <div style="font-size: 2rem; margin-bottom: 1rem;">📊</div>
      <h3 style="color: #1F2937;">Progress Tracking</h3>
      <p style="color: #6B7280;">Personalized improvement plans</p>
    </div>
  </div>
</div>

<!-- CTA -->
<div style="background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%); padding: 3rem; border-radius: 15px; text-align: center; color: white;">
  <h2>Start Your USACO Journey Today!</h2>
  <p style="font-size: 1.1rem; margin: 1rem 0;">Join hundreds of students who have achieved Gold and Platinum</p>
  <a href="../aicoding/contact.html" style="background: white; color: #FFA500; padding: 1rem 2rem; border-radius: 10px; text-decoration: none; display: inline-block; font-weight: 600; margin-top: 1rem;">Enroll Now</a>
</div>
