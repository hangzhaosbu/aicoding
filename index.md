---
layout: default
title: AIcoding Academy
title_zh: AIcoding 学院
description: Elite Programming Education for Future Tech Leaders
description_zh: 为未来科技领袖提供的精英编程教育
---

<style>
  /* ========================================
     Animations
  ======================================== */
  @keyframes gradientFlow {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 0.8; }
    50% { transform: scale(1.05); opacity: 1; }
  }

  @keyframes slideInUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes starTwinkle {
    0%, 100% { opacity: 0.3; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.3); }
  }

  @keyframes arrowPulse {
    0%, 100% { transform: translateX(0); opacity: 0.6; }
    50% { transform: translateX(5px); opacity: 1; }
  }

  /* ========================================
     Hero Section
  ======================================== */
  .hero-section {
    min-height: 85vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, #1e1b4b 0%, #312e81 25%, #4338ca 50%, #6366f1 75%, #4338ca 100%);
    background-size: 400% 400%;
    animation: gradientFlow 15s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
  }

  .hero-stars {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
  }

  .hero-star {
    position: absolute;
    width: 4px;
    height: 4px;
    background: white;
    border-radius: 50%;
    animation: starTwinkle 3s ease-in-out infinite;
  }

  .hero-star:nth-child(1) { left: 5%; top: 15%; animation-delay: 0s; }
  .hero-star:nth-child(2) { left: 15%; top: 45%; animation-delay: 0.5s; }
  .hero-star:nth-child(3) { left: 25%; top: 75%; animation-delay: 1s; }
  .hero-star:nth-child(4) { left: 45%; top: 20%; animation-delay: 1.5s; }
  .hero-star:nth-child(5) { left: 65%; top: 70%; animation-delay: 0.3s; }
  .hero-star:nth-child(6) { left: 80%; top: 35%; animation-delay: 0.8s; }
  .hero-star:nth-child(7) { left: 90%; top: 60%; animation-delay: 1.2s; }

  .hero-content {
    position: relative;
    z-index: 2;
    text-align: center;
    animation: slideInUp 1s ease-out;
  }

  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    padding: 0.6rem 1.5rem;
    border-radius: 50px;
    margin-bottom: 2rem;
    border: 1px solid rgba(255, 255, 255, 0.3);
  }

  .hero-badge-dot {
    width: 8px;
    height: 8px;
    background: #10B981;
    border-radius: 50%;
    animation: pulse 2s ease-in-out infinite;
  }

  .hero-badge-text {
    color: white;
    font-size: 0.9rem;
    font-weight: 600;
  }

  .hero-title {
    font-size: 4.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 4px 30px rgba(0, 0, 0, 0.4);
    margin-bottom: 1.5rem;
    letter-spacing: -2px;
  }

  .hero-subtitle {
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.95);
    margin-bottom: 1rem;
    font-weight: 400;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
  }

  .hero-description {
    font-size: 1.1rem;
    color: rgba(255, 255, 255, 0.85);
    margin-bottom: 2.5rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .hero-btn {
    padding: 1.1rem 2.5rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.05rem;
    text-decoration: none;
    transition: all 0.4s ease;
  }

  .hero-btn-primary {
    background: white;
    color: #4338ca;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.25);
  }

  .hero-btn-primary:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    color: #4338ca;
  }

  .hero-btn-secondary {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.4);
  }

  .hero-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.25);
    transform: translateY(-5px);
    color: white;
  }

  /* ========================================
     Section Styles
  ======================================== */
  .section-header {
    text-align: center;
    margin-bottom: 4rem;
  }

  .section-eyebrow {
    display: inline-block;
    font-size: 0.85rem;
    font-weight: 700;
    color: #6366f1;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin-bottom: 1rem;
    padding: 0.5rem 1.5rem;
    background: rgba(99, 102, 241, 0.1);
    border-radius: 50px;
  }

  .section-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.2rem;
    max-width: 650px;
    margin: 0 auto;
    line-height: 1.7;
  }

  /* ========================================
     Learning Paths Section
  ======================================== */
  .paths-section {
    margin: 6rem 0;
    padding: 4rem 0;
  }

  .path-container {
    margin-bottom: 3rem;
    background: white;
    border-radius: 24px;
    box-shadow: 0 10px 50px rgba(0, 0, 0, 0.08);
    overflow: hidden;
    border: 1px solid #E5E7EB;
  }

  .path-header {
    padding: 1.5rem 2rem;
    display: flex;
    align-items: center;
    gap: 1rem;
    color: white;
    position: relative;
  }

  .path-header-icon {
    font-size: 2rem;
    filter: drop-shadow(0 2px 8px rgba(0, 0, 0, 0.2));
  }

  .path-header-content {
    flex: 1;
  }

  .path-header-title {
    font-size: 1.4rem;
    font-weight: 800;
    margin-bottom: 0.2rem;
    text-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
  }

  .path-header-subtitle {
    font-size: 0.9rem;
    opacity: 0.9;
  }

  .path-header-goal {
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 0.5rem 1rem;
    border-radius: 50px;
    font-size: 0.85rem;
    font-weight: 600;
    border: 1px solid rgba(255, 255, 255, 0.3);
  }

  /* Path Colors */
  .path-ap { background: linear-gradient(135deg, #3B82F6, #1D4ED8); }
  .path-acsl { background: linear-gradient(135deg, #8B5CF6, #6D28D9); }
  .path-usaco { background: linear-gradient(135deg, #10B981, #059669); }
  .path-ml { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .path-math { background: linear-gradient(135deg, #EF4444, #DC2626); }
  .path-wq { background: linear-gradient(135deg, #06B6D4, #0891B2); }
  .path-himcm { background: linear-gradient(135deg, #EC4899, #DB2777); }

  /* Timeline */
  .path-timeline {
    padding: 2rem;
    display: flex;
    align-items: stretch;
    gap: 0;
    overflow-x: auto;
    position: relative;
  }

  .timeline-step {
    flex: 1;
    min-width: 180px;
    display: flex;
    flex-direction: column;
    position: relative;
  }

  .timeline-connector {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 0.5rem;
    min-width: 50px;
  }

  .timeline-arrow {
    font-size: 1.5rem;
    color: #D1D5DB;
    animation: arrowPulse 2s ease-in-out infinite;
  }

  .step-card {
    background: #F9FAFB;
    border-radius: 16px;
    padding: 1.5rem;
    height: 100%;
    border: 2px solid #E5E7EB;
    transition: all 0.3s ease;
    position: relative;
  }

  .step-card:hover {
    border-color: #C7D2FE;
    transform: translateY(-3px);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  }

  .step-number {
    position: absolute;
    top: -12px;
    left: 1rem;
    width: 28px;
    height: 28px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.8rem;
    font-weight: 700;
    color: white;
  }

  .step-ap .step-number { background: #3B82F6; }
  .step-acsl .step-number { background: #8B5CF6; }
  .step-usaco .step-number { background: #10B981; }
  .step-ml .step-number { background: #F59E0B; }
  .step-math .step-number { background: #EF4444; }
  .step-wq .step-number { background: #06B6D4; }
  .step-himcm .step-number { background: #EC4899; }

  .step-duration {
    display: inline-block;
    padding: 0.3rem 0.8rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
    background: #E5E7EB;
    color: #4B5563;
  }

  .step-title {
    font-size: 1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .step-description {
    font-size: 0.85rem;
    color: #6B7280;
    line-height: 1.5;
  }

  /* Final Goal Step */
  .step-goal {
    background: linear-gradient(135deg, #FEF3C7, #FDE68A);
    border-color: #F59E0B;
  }

  .step-goal .step-number {
    background: linear-gradient(135deg, #F59E0B, #D97706);
  }

  .step-goal .step-title {
    color: #92400E;
  }

  .step-goal .step-description {
    color: #A16207;
    font-weight: 600;
  }

  /* ========================================
     Why Choose Us Section
  ======================================== */
  .why-section {
    margin: 6rem 0;
    padding: 4rem 2rem;
    background: linear-gradient(180deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 30px;
  }

  .why-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 3rem;
  }

  .why-card {
    background: white;
    border-radius: 20px;
    padding: 2rem;
    text-align: center;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.05);
    border: 1px solid #E5E7EB;
    transition: all 0.4s ease;
  }

  .why-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.1);
  }

  .why-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .why-title {
    font-size: 1.15rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .why-description {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* ========================================
     Stats Section
  ======================================== */
  .stats-section {
    background: linear-gradient(135deg, #1e1b4b 0%, #312e81 50%, #4338ca 100%);
    border-radius: 30px;
    padding: 4rem 3rem;
    margin: 6rem 0;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 3rem;
  }

  .stat-item {
    text-align: center;
  }

  .stat-icon {
    font-size: 2.5rem;
    margin-bottom: 0.8rem;
  }

  .stat-number {
    font-size: 3.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
    margin-bottom: 0.3rem;
  }

  .stat-label {
    color: rgba(255, 255, 255, 0.85);
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
  }

  /* ========================================
     CTA Section
  ======================================== */
  .cta-section {
    background: white;
    border-radius: 30px;
    padding: 5rem 3rem;
    margin: 6rem 0;
    text-align: center;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.08);
    border: 1px solid #E5E7EB;
    position: relative;
    overflow: hidden;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #a855f7, #ec4899);
  }

  .cta-icon {
    font-size: 4rem;
    margin-bottom: 1.5rem;
    animation: float 4s ease-in-out infinite;
  }

  .cta-title {
    font-size: 2.8rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .cta-description {
    font-size: 1.2rem;
    color: #6B7280;
    margin-bottom: 2.5rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-btn {
    padding: 1.1rem 2.5rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.05rem;
    text-decoration: none;
    transition: all 0.4s ease;
  }

  .cta-btn-primary {
    background: linear-gradient(135deg, #6366f1, #8b5cf6);
    color: white;
    box-shadow: 0 10px 40px rgba(99, 102, 241, 0.4);
  }

  .cta-btn-primary:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 50px rgba(99, 102, 241, 0.5);
    color: white;
  }

  .cta-btn-secondary {
    background: #F3F4F6;
    color: #4B5563;
  }

  .cta-btn-secondary:hover {
    background: #E5E7EB;
    transform: translateY(-5px);
    color: #1F2937;
  }

  /* ========================================
     Responsive Design
  ======================================== */
  @media (max-width: 1200px) {
    .path-timeline {
      flex-wrap: nowrap;
      overflow-x: auto;
      padding-bottom: 1rem;
    }
    
    .timeline-step {
      min-width: 160px;
    }
  }

  @media (max-width: 900px) {
    .why-grid {
      grid-template-columns: repeat(2, 1fr);
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
    }

    .path-header {
      flex-wrap: wrap;
    }

    .path-header-goal {
      width: 100%;
      text-align: center;
      margin-top: 0.5rem;
    }
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 3rem;
    }

    .section-title {
      font-size: 2.2rem;
    }

    .why-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
    }

    .cta-title {
      font-size: 2rem;
    }

    .path-timeline {
      flex-direction: column;
      gap: 1rem;
    }

    .timeline-connector {
      transform: rotate(90deg);
      padding: 0.5rem 0;
      min-width: auto;
    }

    .timeline-step {
      min-width: 100%;
    }
  }

  @media (max-width: 480px) {
    .hero-buttons,
    .cta-buttons {
      flex-direction: column;
      align-items: center;
    }

    .hero-btn,
    .cta-btn {
      width: 100%;
      max-width: 280px;
      justify-content: center;
    }

    .stats-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<!-- Hero Section -->
<section class="hero-section">
  <div class="hero-stars">
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
  </div>
  
  <div class="hero-content">
    <div class="hero-badge">
      <span class="hero-badge-dot"></span>
      <span class="hero-badge-text">
        <span class="en-content">Now Enrolling for 2025</span>
        <span class="zh-content">2025年招生进行中</span>
      </span>
    </div>
    
    <h1 class="hero-title">
      <span class="en-content">AIcoding Academy</span>
      <span class="zh-content">AIcoding 学院</span>
    </h1>
    
    <p class="hero-subtitle">
      <span class="en-content">Empowering Future Tech Leaders</span>
      <span class="zh-content">培养未来科技领袖</span>
    </p>
    
    <p class="hero-description">
      <span class="en-content">7 specialized learning tracks for programming, competitions, and research. Choose your path to excellence.</span>
      <span class="zh-content">7条专业学习路线，涵盖编程、竞赛和研究。选择您的卓越之路。</span>
    </p>
    
    <div class="hero-buttons">
      <a href="./course.html" class="hero-btn hero-btn-primary">
        <span class="en-content">🚀 Explore Programs</span>
        <span class="zh-content">🚀 探索课程</span>
      </a>
      <a href="./contact.html" class="hero-btn hero-btn-secondary">
        <span class="en-content">📞 Free Consultation</span>
        <span class="zh-content">📞 免费咨询</span>
      </a>
    </div>
  </div>
</section>

<!-- Learning Paths Section -->
<section class="paths-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Learning Paths</span>
      <span class="zh-content">学习路径</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">7 Tracks to Excellence</span>
      <span class="zh-content">7条卓越之路</span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Each track has a clear progression from fundamentals to mastery. Find the path that matches your goals.</span>
      <span class="zh-content">每条路线都有清晰的从基础到精通的进阶路径。找到符合您目标的路线。</span>
    </p>
  </div>

  <!-- Track 1: AP Computer Science -->
  <div class="path-container">
    <div class="path-header path-ap">
      <span class="path-header-icon">📘</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">AP Computer Science Track</span>
          <span class="zh-content">AP计算机科学路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">Master AP CSA & AP CSP for college credit</span>
          <span class="zh-content">掌握AP CSA和AP CSP获得大学学分</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Score 5 on AP Exams</span>
        <span class="zh-content">🎯 目标：AP考试满分5分</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Java Fundamentals</span>
            <span class="zh-content">Java基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Variables, loops, arrays, OOP basics, methods</span>
            <span class="zh-content">变量、循环、数组、面向对象基础、方法</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AP CSP Prep</span>
            <span class="zh-content">AP CSP备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Computing concepts, data, algorithms, internet, impact</span>
            <span class="zh-content">计算概念、数据、算法、互联网、影响</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AP CSA Prep</span>
            <span class="zh-content">AP CSA备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced OOP, inheritance, recursion, ArrayLists</span>
            <span class="zh-content">高级OOP、继承、递归、ArrayList</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2 months</span>
            <span class="zh-content">2个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Exam Practice</span>
            <span class="zh-content">模拟考试</span>
          </h4>
          <p class="step-description">
            <span class="en-content">FRQ training, mock exams → Score 5!</span>
            <span class="zh-content">FRQ训练、模拟考试 → 满分5分！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 2: ACSL -->
  <div class="path-container">
    <div class="path-header path-acsl">
      <span class="path-header-icon">💻</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">ACSL Competition Track</span>
          <span class="zh-content">ACSL竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">American Computer Science League</span>
          <span class="zh-content">美国计算机科学联赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: ACSL Finals</span>
        <span class="zh-content">🎯 目标：ACSL决赛</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Programming Basics</span>
            <span class="zh-content">编程基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python/Java basics, problem-solving fundamentals</span>
            <span class="zh-content">Python/Java基础，问题解决入门</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Junior</span>
            <span class="zh-content">ACSL初级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Number systems, Boolean algebra, graph theory basics</span>
            <span class="zh-content">数制、布尔代数、图论基础</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Intermediate</span>
            <span class="zh-content">ACSL中级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Bit manipulation, regex, prefix/postfix notation</span>
            <span class="zh-content">位运算、正则表达式、前缀/后缀表示法</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Senior</span>
            <span class="zh-content">ACSL高级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced topics → Qualify for Finals!</span>
            <span class="zh-content">高级主题 → 进入决赛！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 3: USACO -->
  <div class="path-container">
    <div class="path-header path-usaco">
      <span class="path-header-icon">🐄</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">USACO Competition Track</span>
          <span class="zh-content">USACO竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">USA Computing Olympiad</span>
          <span class="zh-content">美国计算机奥林匹克</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Platinum Division</span>
        <span class="zh-content">🎯 目标：白金级</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">C++ & Basics</span>
            <span class="zh-content">C++与基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">C++ fundamentals, STL, time complexity</span>
            <span class="zh-content">C++基础，STL，时间复杂度</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Bronze → Silver</span>
            <span class="zh-content">铜级 → 银级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Simulation, sorting, binary search, greedy</span>
            <span class="zh-content">模拟、排序、二分查找、贪心</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">6-8 months</span>
            <span class="zh-content">6-8个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Silver → Gold</span>
            <span class="zh-content">银级 → 金级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">DFS/BFS, DP basics, DSU, trees</span>
            <span class="zh-content">DFS/BFS、DP基础、并查集、树</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">8-12 months</span>
            <span class="zh-content">8-12个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Gold → Platinum</span>
            <span class="zh-content">金级 → 白金级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced DP, segment trees → Platinum!</span>
            <span class="zh-content">高级DP、线段树 → 白金级！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 4: Machine Learning / AI -->
  <div class="path-container">
    <div class="path-header path-ml">
      <span class="path-header-icon">🤖</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">AI/ML Competition Track</span>
          <span class="zh-content">AI/ML竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">USAAIO & Kaggle Competitions</span>
          <span class="zh-content">USAAIO和Kaggle竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Kaggle Medal / USAAIO Award</span>
        <span class="zh-content">🎯 目标：Kaggle奖牌 / USAAIO获奖</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Python & Data</span>
            <span class="zh-content">Python与数据</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python, NumPy, Pandas, data visualization</span>
            <span class="zh-content">Python、NumPy、Pandas、数据可视化</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Machine Learning</span>
            <span class="zh-content">机器学习</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Sklearn, regression, classification, clustering</span>
            <span class="zh-content">Sklearn、回归、分类、聚类</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Deep Learning</span>
            <span class="zh-content">深度学习</span>
          </h4>
          <p class="step-description">
            <span class="en-content">PyTorch, CNN, RNN, transformers</span>
            <span class="zh-content">PyTorch、CNN、RNN、Transformer</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Competition Prep</span>
            <span class="zh-content">竞赛备战</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Kaggle projects → Medal / USAAIO Award!</span>
            <span class="zh-content">Kaggle项目 → 奖牌 / USAAIO获奖！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 5: Math Competition -->
  <div class="path-container">
    <div class="path-header path-math">
      <span class="path-header-icon">🔢</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">Math Competition Track</span>
          <span class="zh-content">数学竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">AMC → AIME → USAMO</span>
          <span class="zh-content">AMC → AIME → USAMO</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: AIME Qualification / USAMO</span>
        <span class="zh-content">🎯 目标：AIME资格 / USAMO</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AMC 8 Prep</span>
            <span class="zh-content">AMC 8备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Number sense, basic geometry, counting</span>
            <span class="zh-content">数感、基础几何、计数</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AMC 10/12</span>
            <span class="zh-content">AMC 10/12</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Algebra, geometry, probability, number theory</span>
            <span class="zh-content">代数、几何、概率、数论</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">6-8 months</span>
            <span class="zh-content">6-8个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AIME Prep</span>
            <span class="zh-content">AIME备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced techniques, proof strategies</span>
            <span class="zh-content">高级技巧、证明策略</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">6-12 months</span>
            <span class="zh-content">6-12个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">USAMO Prep</span>
            <span class="zh-content">USAMO备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Olympiad problems → USAMO Qualifier!</span>
            <span class="zh-content">奥赛问题 → USAMO资格！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 6: WorldQuant -->
  <div class="path-container">
    <div class="path-header path-wq">
      <span class="path-header-icon">📈</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">WorldQuant Challenge Track</span>
          <span class="zh-content">WorldQuant挑战赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">Quantitative Finance Competition</span>
          <span class="zh-content">量化金融竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Gold Badge / Top 100</span>
        <span class="zh-content">🎯 目标：金牌徽章 / 前100名</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Python & Stats</span>
            <span class="zh-content">Python与统计</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python, statistics, probability basics</span>
            <span class="zh-content">Python、统计学、概率基础</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Finance Basics</span>
            <span class="zh-content">金融基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Markets, trading, financial data analysis</span>
            <span class="zh-content">市场、交易、金融数据分析</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Alpha Research</span>
            <span class="zh-content">Alpha研究</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Factor modeling, alpha generation, backtesting</span>
            <span class="zh-content">因子建模、Alpha生成、回测</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Competition</span>
            <span class="zh-content">竞赛</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Submit alphas → Gold Badge!</span>
            <span class="zh-content">提交Alpha → 金牌徽章！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 7: HiMCM -->
  <div class="path-container">
    <div class="path-header path-himcm">
      <span class="path-header-icon">📋</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">HiMCM Modeling Track</span>
          <span class="zh-content">HiMCM数学建模路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">High School Mathematical Contest in Modeling</span>
          <span class="zh-content">高中数学建模竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Outstanding Award</span>
        <span class="zh-content">🎯 目标：杰出奖</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Math & Python</span>
            <span class="zh-content">数学与Python</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Calculus, statistics, Python for data analysis</span>
            <span class="zh-content">微积分、统计、Python数据分析</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Modeling Basics</span>
            <span class="zh-content">建模基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Optimization, simulation, differential equations</span>
            <span class="zh-content">优化、模拟、微分方程</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Paper Writing</span>
            <span class="zh-content">论文写作</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Technical writing, LaTeX, report structure</span>
            <span class="zh-content">技术写作、LaTeX、报告结构</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2 months</span>
            <span class="zh-content">2个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Competition</span>
            <span class="zh-content">竞赛</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Practice problems → Outstanding Award!</span>
            <span class="zh-content">练习问题 → 杰出奖！</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Why Choose Us Section -->
<section class="why-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Why AIcoding</span>
      <span class="zh-content">为什么选择AIcoding</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">The AIcoding Difference</span>
      <span class="zh-content">AIcoding的独特优势</span>
    </h2>
  </div>
  
  <div class="why-grid">
    <div class="why-card">
      <div class="why-icon">👨‍🏫</div>
      <h4 class="why-title">
        <span class="en-content">Expert Instructors</span>
        <span class="zh-content">专家导师</span>
      </h4>
      <p class="why-description">
        <span class="en-content">PhD holders, FAANG engineers, and competition gold medalists</span>
        <span class="zh-content">博士、FAANG工程师和竞赛金牌得主</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">👥</div>
      <h4 class="why-title">
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h4>
      <p class="why-description">
        <span class="en-content">Maximum 8 students per class for personalized attention</span>
        <span class="zh-content">每班最多8名学生，确保个性化关注</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">📈</div>
      <h4 class="why-title">
        <span class="en-content">Proven Results</span>
        <span class="zh-content">成果显著</span>
      </h4>
      <p class="why-description">
        <span class="en-content">90% success rate in competitions and AP exams</span>
        <span class="zh-content">竞赛和AP考试90%成功率</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">🎯</div>
      <h4 class="why-title">
        <span class="en-content">Clear Roadmap</span>
        <span class="zh-content">清晰路线</span>
      </h4>
      <p class="why-description">
        <span class="en-content">Structured progression with milestone tracking</span>
        <span class="zh-content">结构化进阶，里程碑跟踪</span>
      </p>
    </div>
  </div>
</section>

<!-- Stats Section -->
<section class="stats-section">
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-icon">👨‍🎓</div>
      <div class="stat-number">50+</div>
      <div class="stat-label">
        <span class="en-content">Students</span>
        <span class="zh-content">学生</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">🏆</div>
      <div class="stat-number">20+</div>
      <div class="stat-label">
        <span class="en-content">Awards</span>
        <span class="zh-content">奖项</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">📈</div>
      <div class="stat-number">90%</div>
      <div class="stat-label">
        <span class="en-content">Success Rate</span>
        <span class="zh-content">成功率</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">🛤️</div>
      <div class="stat-number">7</div>
      <div class="stat-label">
        <span class="en-content">Learning Tracks</span>
        <span class="zh-content">学习路线</span>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-icon">🚀</div>
  <h2 class="cta-title">
    <span class="en-content">Ready to Start Your Journey?</span>
    <span class="zh-content">准备好开始您的旅程了吗？</span>
  </h2>
  <p class="cta-description">
    <span class="en-content">Choose your track and begin your path to excellence. Schedule a free consultation to find the perfect fit.</span>
    <span class="zh-content">选择您的路线，开始卓越之旅。预约免费咨询，找到最适合您的路径。</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-btn cta-btn-primary">
      <span class="en-content">📞 Free Consultation</span>
      <span class="zh-content">📞 免费咨询</span>
    </a>
    <a href="./course.html" class="cta-btn cta-btn-secondary">
      <span class="en-content">📚 View All Courses</span>
      <span class="zh-content">📚 查看所有课程</span>
    </a>
  </div>
</section>
