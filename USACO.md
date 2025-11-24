---
layout: default
title: USACO Training
title_zh: USACO 培训
description: USA Computing Olympiad Competition Preparation
description_zh: 美国计算机奥林匹克竞赛准备
---

<style>
  /* Premium Animations */
  @keyframes gradientWave {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-10px) rotate(-1deg); }
    75% { transform: translateY(10px) rotate(1deg); }
  }

  @keyframes shimmer {
    0% { left: -100%; }
    100% { left: 100%; }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50% { transform: scale(1.05); opacity: 0.9; }
  }

  @keyframes slideInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes rotateGlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes trophyBounce {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 25%, #FF6B6B 50%, #4ECDC4 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.4);
    min-height: 400px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🏆';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: trophyBounce 6s ease-in-out infinite;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotateGlow 20s linear infinite;
  }

  /* Floating medals background */
  .course-hero .medals-bg {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .course-hero .medal {
    position: absolute;
    font-size: 3rem;
    opacity: 0.1;
    animation: float 10s ease-in-out infinite;
  }

  .medal:nth-child(1) { left: 10%; top: 20%; animation-delay: 0s; }
  .medal:nth-child(2) { left: 80%; top: 30%; animation-delay: 2s; }
  .medal:nth-child(3) { left: 20%; top: 70%; animation-delay: 4s; }
  .medal:nth-child(4) { left: 70%; top: 60%; animation-delay: 6s; }

  .course-hero h1 {
    color: white !important;
    font-size: 4rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out;
  }

  .course-hero p {
    color: white !important;
    font-size: 1.5rem;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.2s backwards;
  }

  /* Level Cards - Premium Design */
  .level-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 4rem auto;
    max-width: 1600px; /* Increased from 1400px */
    padding: 0 2rem;
  }

  @media (max-width: 1400px) {
    .level-cards {
      grid-template-columns: repeat(2, 1fr);
      gap: 2.5rem;
    }
  }

  @media (max-width: 768px) {
    .level-cards {
      grid-template-columns: 1fr;
    }
  }

  .level-card {
    background: white;
    padding: 2rem 1.5rem; /* Adjusted padding */
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: flex;
    flex-direction: column;
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
    min-width: 0; /* Prevent overflow */
  }

  .level-card:nth-child(1) { animation-delay: 0.1s; }
  .level-card:nth-child(2) { animation-delay: 0.2s; }
  .level-card:nth-child(3) { animation-delay: 0.3s; }
  .level-card:nth-child(4) { animation-delay: 0.4s; }

  .level-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
    animation: shimmer 3s infinite;
  }

  .level-card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
  }

  .bronze { 
    border-top: 6px solid #CD7F32;
    background: linear-gradient(to bottom, rgba(205, 127, 50, 0.08) 0%, white 40%);
  }
  
  .bronze:hover {
    box-shadow: 0 30px 60px rgba(205, 127, 50, 0.3);
  }
  
  .silver { 
    border-top: 6px solid #C0C0C0;
    background: linear-gradient(to bottom, rgba(192, 192, 192, 0.08) 0%, white 40%);
  }
  
  .silver:hover {
    box-shadow: 0 30px 60px rgba(192, 192, 192, 0.3);
  }
  
  .gold { 
    border-top: 6px solid #FFD700;
    background: linear-gradient(to bottom, rgba(255, 215, 0, 0.08) 0%, white 40%);
  }
  
  .gold:hover {
    box-shadow: 0 30px 60px rgba(255, 215, 0, 0.4);
  }
  
  .platinum { 
    border-top: 6px solid;
    border-image: linear-gradient(90deg, #E5E4E2, #B8B8B8, #E5E4E2) 1;
    background: linear-gradient(to bottom, rgba(229, 228, 226, 0.1) 0%, white 40%);
  }
  
  .platinum:hover {
    box-shadow: 0 30px 60px rgba(184, 184, 184, 0.3);
  }

  .level-header {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .level-icon {
    font-size: 3.5rem;
    margin-bottom: 0.8rem;
    display: inline-block;
    animation: pulse 3s ease-in-out infinite;
  }

  .bronze .level-icon { animation-delay: 0s; }
  .silver .level-icon { animation-delay: 0.5s; }
  .gold .level-icon { animation-delay: 1s; }
  .platinum .level-icon { animation-delay: 1.5s; }

  .level-name {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
    white-space: nowrap;
  }

  .level-subtitle {
    font-size: 0.95rem;
    font-weight: 500;
    color: #6B7280;
    margin-bottom: 1.2rem;
    white-space: nowrap;
  }

  .level-topics {
    color: #6B7280;
    line-height: 1.6;
    flex-grow: 1;
  }

  .level-topics ul {
    padding-left: 0;
    margin: 0;
    list-style: none;
  }

  .level-topics li {
    margin: 0.5rem 0;
    font-size: 0.9rem;
    padding-left: 1.5rem;
    position: relative;
    white-space: nowrap; /* Prevent text wrapping */
    overflow: hidden;
    text-overflow: ellipsis;
  }

  /* Allow wrapping on smaller screens */
  @media (max-width: 1600px) {
    .level-topics li {
      white-space: normal;
      font-size: 0.85rem;
    }
  }

  .level-topics li::before {
    content: '→';
    position: absolute;
    left: 0;
    color: #9CA3AF;
    font-weight: bold;
  }

  .bronze .level-topics li::before { color: #CD7F32; }
  .silver .level-topics li::before { color: #C0C0C0; }
  .gold .level-topics li::before { color: #FFD700; }
  .platinum .level-topics li::before { color: #B8B8B8; }

  /* Section Headers - Premium */
  .section-header {
    text-align: center;
    color: #1F2937;
    margin: 5rem 0 3rem;
    position: relative;
  }

  .section-header h2 {
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .section-header p {
    color: #6B7280;
    font-size: 1.2rem;
  }

  /* Timeline - Premium Design */
  .timeline-section {
    padding: 4rem 0;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .timeline {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    max-width: 1000px;
    margin: 3rem auto;
    padding: 0 2rem;
  }

  .timeline::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 5%;
    right: 5%;
    height: 4px;
    background: linear-gradient(90deg, #CD7F32 0%, #C0C0C0 33%, #FFD700 66%, #E5E4E2 100%);
    z-index: 0;
    border-radius: 2px;
  }

  .timeline-item {
    background: white;
    padding: 1.5rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    z-index: 1;
    position: relative;
    text-align: center;
    flex: 1;
    margin: 0 1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
  }

  .timeline-item:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .timeline-item:nth-child(1):hover { border-color: #CD7F32; }
  .timeline-item:nth-child(2):hover { border-color: #C0C0C0; }
  .timeline-item:nth-child(3):hover { border-color: #FFD700; }
  .timeline-item:nth-child(4):hover { border-color: #E5E4E2; }

  .timeline-level {
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
    font-size: 1.2rem;
  }

  .timeline-duration {
    font-size: 0.9rem;
    color: #6B7280;
  }

  @media (max-width: 768px) {
    .timeline {
      flex-direction: column;
      gap: 2rem;
    }
    
    .timeline::before {
      top: 0;
      bottom: 0;
      left: 50%;
      width: 4px;
      height: 90%;
    }
  }

  /* Training Features - Premium Grid */
  .training-features {
    background: white;
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
  }

  .training-features::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #FFD700, #FFA500, #FF6B6B);
    animation: shimmer 3s infinite;
  }

  .training-features h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 3rem;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin-top: 3rem;
  }

  @media (max-width: 968px) {
    .features-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .features-grid {
      grid-template-columns: 1fr;
    }
  }

  .feature-item {
    text-align: center;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 2.5rem;
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
  }

  .feature-item::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 215, 0, 0.1), transparent);
    transition: left 0.5s;
  }

  .feature-item:hover::before {
    left: 100%;
  }

  .feature-item:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 15px 30px rgba(255, 165, 0, 0.2);
    border-color: #FFD700;
    background: white;
  }

  .feature-icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
    display: inline-block;
    animation: float 6s ease-in-out infinite;
  }

  .feature-item:nth-child(odd) .feature-icon {
    animation-delay: 0s;
  }

  .feature-item:nth-child(even) .feature-icon {
    animation-delay: 3s;
  }

  .feature-title {
    color: #1F2937;
    font-size: 1.3rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
  }

  .feature-description {
    color: #6B7280;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* Success Stories - Premium Stats */
  .success-section {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.3);
    position: relative;
    overflow: hidden;
  }

  .success-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .success-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 3rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 3rem;
    margin: 2rem 0;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 968px) {
    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .stats-grid {
      grid-template-columns: 1fr;
    }
  }

  .stat-item {
    text-align: center;
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .stat-item:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .stat-number {
    font-size: 3rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    display: inline-block;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #6B7280;
    font-size: 1rem;
    margin-top: 0.5rem;
    font-weight: 600;
  }

  /* Contest Dates Section */
  .contest-dates {
    background: white;
    padding: 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .contest-dates h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
  }

  .contest-calendar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 1200px) {
    .contest-calendar {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .contest-calendar {
      grid-template-columns: 1fr;
    }
  }

  .contest-month {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 1.5rem;
    border-radius: 15px;
    border-left: 4px solid #FFD700;
    transition: all 0.3s;
  }

  .contest-month:hover {
    transform: translateX(5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .contest-month h3 {
    color: #1F2937;
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }

  .contest-month p {
    color: #6B7280;
    font-size: 0.95rem;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 25%, #FF6B6B 50%, #4ECDC4 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 4rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.4);
    margin-top: 4rem;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 60%);
    animation: rotateGlow 12s linear infinite;
  }

  .cta-section h2 {
    color: white !important;
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
  }

  .cta-section p {
    color: white !important;
    font-size: 1.3rem;
    margin: 1.5rem 0;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .cta-button {
    background: white;
    color: #FFA500;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    margin-top: 1.5rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
    overflow: hidden;
  }

  .cta-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 165, 0, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #FF8C00;
  }

  /* Responsive adjustments */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2.5rem;
    }
    
    .section-header h2 {
      font-size: 2rem;
    }
    
    .cta-section h2 {
      font-size: 2rem;
    }
  }
</style>

<div class="course-hero">
  <div class="medals-bg">
    <span class="medal">🥉</span>
    <span class="medal">🥈</span>
    <span class="medal">🥇</span>
    <span class="medal">💎</span>
  </div>
  <h1>
    <span class="en-content">USACO Training Program</span>
    <span class="zh-content">USACO 培训计划</span>
  </h1>
  <p>
    <span class="en-content">Your Path from Bronze to Platinum</span>
    <span class="zh-content">从铜牌到白金的进阶之路</span>
  </p>
</div>

<!-- Course Overview -->
<div class="section-header">
  <h2>
    <span class="en-content">Complete Competition Curriculum</span>
    <span class="zh-content">完整竞赛课程体系</span>
  </h2>
  <p>
    <span class="en-content">Progressive training through all USACO divisions with proven results</span>
    <span class="zh-content">通过所有USACO级别的渐进式培训，成果显著</span>
  </p>
</div>

<!-- Level Cards -->
<div class="level-cards">
  <!-- Bronze Level -->
  <div class="level-card bronze">
    <div class="level-header">
      <div class="level-icon">🥉</div>
      <h3 class="level-name">
        <span class="en-content">Bronze Division</span>
        <span class="zh-content">铜牌组</span>
      </h3>
      <p class="level-subtitle">
        <span class="en-content">Foundation Building</span>
        <span class="zh-content">基础构建</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">USACO Contest Format</span>
          <span class="zh-content">USACO 竞赛格式</span>
        </li>
        <li>
          <span class="en-content">File I/O & Edge Cases</span>
          <span class="zh-content">文件输入输出与边界情况</span>
        </li>
        <li>
          <span class="en-content">Complete Search</span>
          <span class="zh-content">完全搜索</span>
        </li>
        <li>
          <span class="en-content">Greedy Algorithms</span>
          <span class="zh-content">贪心算法</span>
        </li>
        <li>
          <span class="en-content">Ad Hoc Problems</span>
          <span class="zh-content">特殊问题</span>
        </li>
        <li>
          <span class="en-content">Basic Sorting</span>
          <span class="zh-content">基础排序</span>
        </li>
        <li>
          <span class="en-content">Simulation</span>
          <span class="zh-content">模拟</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Silver Level -->
  <div class="level-card silver">
    <div class="level-header">
      <div class="level-icon">🥈</div>
      <h3 class="level-name">
        <span class="en-content">Silver Division</span>
        <span class="zh-content">银牌组</span>
      </h3>
      <p class="level-subtitle">
        <span class="en-content">Core Algorithms</span>
        <span class="zh-content">核心算法</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Graph Traversal (DFS/BFS)</span>
          <span class="zh-content">图遍历（深搜/广搜）</span>
        </li>
        <li>
          <span class="en-content">Flood Fill Algorithms</span>
          <span class="zh-content">洪水填充算法</span>
        </li>
        <li>
          <span class="en-content">Binary Search</span>
          <span class="zh-content">二分搜索</span>
        </li>
        <li>
          <span class="en-content">Two Pointers</span>
          <span class="zh-content">双指针技术</span>
        </li>
        <li>
          <span class="en-content">Prefix Sums</span>
          <span class="zh-content">前缀和</span>
        </li>
        <li>
          <span class="en-content">Custom Sorting</span>
          <span class="zh-content">自定义排序</span>
        </li>
        <li>
          <span class="en-content">Tree Algorithms</span>
          <span class="zh-content">树算法</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Gold Level -->
  <div class="level-card gold">
    <div class="level-header">
      <div class="level-icon">🥇</div>
      <h3 class="level-name">
        <span class="en-content">Gold Division</span>
        <span class="zh-content">金牌组</span>
      </h3>
      <p class="level-subtitle">
        <span class="en-content">Advanced Techniques</span>
        <span class="zh-content">高级技术</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Dynamic Programming</span>
          <span class="zh-content">动态规划</span>
        </li>
        <li>
          <span class="en-content">Dijkstra's Algorithm</span>
          <span class="zh-content">Dijkstra 算法</span>
        </li>
        <li>
          <span class="en-content">Minimum Spanning Tree</span>
          <span class="zh-content">最小生成树</span>
        </li>
        <li>
          <span class="en-content">Disjoint Set Union</span>
          <span class="zh-content">并查集</span>
        </li>
        <li>
          <span class="en-content">Topological Sort</span>
          <span class="zh-content">拓扑排序</span>
        </li>
        <li>
          <span class="en-content">Hashing Techniques</span>
          <span class="zh-content">哈希技术</span>
        </li>
        <li>
          <span class="en-content">Point Update Range Sum</span>
          <span class="zh-content">点更新区间求和</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Platinum Level -->
  <div class="level-card platinum">
    <div class="level-header">
      <div class="level-icon">💎</div>
      <h3 class="level-name">
        <span class="en-content">Platinum Division</span>
        <span class="zh-content">白金组</span>
      </h3>
      <p class="level-subtitle">
        <span class="en-content">Expert Mastery</span>
        <span class="zh-content">专家精通</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Advanced DP & Optimization</span>
          <span class="zh-content">高级动态规划与优化</span>
        </li>
        <li>
          <span class="en-content">Network Flow</span>
          <span class="zh-content">网络流</span>
        </li>
        <li>
          <span class="en-content">Computational Geometry</span>
          <span class="zh-content">计算几何</span>
        </li>
        <li>
          <span class="en-content">Segment Trees</span>
          <span class="zh-content">线段树</span>
        </li>
        <li>
          <span class="en-content">Heavy-Light Decomposition</span>
          <span class="zh-content">树链剖分</span>
        </li>
        <li>
          <span class="en-content">String Algorithms (KMP, Z)</span>
          <span class="zh-content">字符串算法（KMP, Z）</span>
        </li>
        <li>
          <span class="en-content">FFT & Number Theory</span>
          <span class="zh-content">FFT 与数论</span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- Timeline Section -->
<div class="timeline-section">
  <div class="section-header">
    <h2 style="color: #1F2937;">
      <span class="en-content">Your Journey to Success</span>
      <span class="zh-content">您的成功之路</span>
    </h2>
    <p>
      <span class="en-content">Typical progression with dedicated practice</span>
      <span class="zh-content">通过专注练习的典型进阶</span>
    </p>
  </div>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-level">
        <span class="en-content">Bronze</span>
        <span class="zh-content">铜牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">3-6 months</span>
        <span class="zh-content">3-6个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-level">
        <span class="en-content">Silver</span>
        <span class="zh-content">银牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">6-12 months</span>
        <span class="zh-content">6-12个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-level">
        <span class="en-content">Gold</span>
        <span class="zh-content">金牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">12-18 months</span>
        <span class="zh-content">12-18个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-level">
        <span class="en-content">Platinum</span>
        <span class="zh-content">白金</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">18+ months</span>
        <span class="zh-content">18个月+</span>
      </div>
    </div>
  </div>
</div>

<!-- Training Features -->
<div class="training-features">
  <h2>
    <span class="en-content">Our Training Excellence</span>
    <span class="zh-content">我们的培训优势</span>
  </h2>
  
  <div class="features-grid">
    <div class="feature-item">
      <div class="feature-icon">📚</div>
      <h3 class="feature-title">
        <span class="en-content">1000+ Problems</span>
        <span class="zh-content">1000+ 题目</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Comprehensive problem bank with detailed solutions</span>
        <span class="zh-content">配有详细解答的综合题库</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">🎯</div>
      <h3 class="feature-title">
        <span class="en-content">Strategic Training</span>
        <span class="zh-content">策略培训</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Contest tactics and time optimization</span>
        <span class="zh-content">竞赛策略和时间优化</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">💻</div>
      <h3 class="feature-title">
        <span class="en-content">Weekly Contests</span>
        <span class="zh-content">每周竞赛</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Simulated USACO contests every week</span>
        <span class="zh-content">每周模拟USACO竞赛</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">📊</div>
      <h3 class="feature-title">
        <span class="en-content">Performance Analytics</span>
        <span class="zh-content">成绩分析</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Detailed progress tracking and insights</span>
        <span class="zh-content">详细的进度跟踪和洞察</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">🏆</div>
      <h3 class="feature-title">
        <span class="en-content">Competition Coaching</span>
        <span class="zh-content">竞赛辅导</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Personal guidance from USACO finalists</span>
        <span class="zh-content">USACO决赛选手的个人指导</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">👥</div>
      <h3 class="feature-title">
        <span class="en-content">Elite Small Groups</span>
        <span class="zh-content">精英小班</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Max 4 students for personalized attention</span>
        <span class="zh-content">最多4人确保个性化关注</span>
      </p>
    </div>
  </div>
</div>

<!-- Contest Dates -->
<div class="contest-dates">
  <h2>
    <span class="en-content">2024-2025 Contest Schedule</span>
    <span class="zh-content">2024-2025 竞赛日程</span>
  </h2>
  
  <div class="contest-calendar">
    <div class="contest-month">
      <h3>
        <span class="en-content">December Contest</span>
        <span class="zh-content">12月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Dec 20-23, 2024</span>
        <span class="zh-content">2024年12月20-23日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span class="en-content">January Contest</span>
        <span class="zh-content">1月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Jan 24-27, 2025</span>
        <span class="zh-content">2025年1月24-27日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span class="en-content">February Contest</span>
        <span class="zh-content">2月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Feb 21-24, 2025</span>
        <span class="zh-content">2025年2月21-24日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span class="en-content">US Open</span>
        <span class="zh-content">美国公开赛</span>
      </h3>
      <p>
        <span class="en-content">March 14-17, 2025</span>
        <span class="zh-content">2025年3月14-17日</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stories -->
<div class="success-section">
  <h2>
    <span class="en-content">Proven Track Record</span>
    <span class="zh-content">卓越成绩</span>
  </h2>
  
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">300+</div>
      <div class="stat-label">
        <span class="en-content">Students Trained</span>
        <span class="zh-content">培训学生</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">92%</div>
      <div class="stat-label">
        <span class="en-content">Promotion Rate</span>
        <span class="zh-content">晋级率</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">85+</div>
      <div class="stat-label">
        <span class="en-content">Gold & Above</span>
        <span class="zh-content">金牌及以上</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">23</div>
      <div class="stat-label">
        <span class="en-content">Platinum Students</span>
        <span class="zh-content">白金学生</span>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Your USACO Journey Today!</span>
    <span class="zh-content">今天开始您的USACO之旅！</span>
  </h2>
  <p>
    <span class="en-content">Join the ranks of our Gold and Platinum achievers</span>
    <span class="zh-content">加入我们金牌和白金获得者的行列</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Begin Training Now</span>
    <span class="zh-content">立即开始培训</span>
  </a>
</div>
