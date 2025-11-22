---
layout: default
title: AIcoding Academy
description: Elite Programming Education for Future Tech Leaders
---

<style>
  /* Hero Section */
  .hero-section {
    text-align: center;
    padding: 3rem 0;
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    border-radius: 20px;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
  }

  .hero-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    top: -50%;
    left: -50%;
    background: radial-gradient(circle, rgba(79, 70, 229, 0.1) 0%, transparent 70%);
    animation: pulse 15s ease-in-out infinite;
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.1); }
  }

  .hero-title {
    font-size: 2.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 1rem;
    position: relative;
  }

  .hero-subtitle {
    font-size: 1.2rem;
    color: #4B5563;
    margin-bottom: 2rem;
    position: relative;
  }

  /* Feature Cards */
  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
  }

  .feature-card {
    background: white;
    border-radius: 15px;
    padding: 2rem;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    transition: all 0.3s ease;
    border: 1px solid #E5E7EB;
  }

  .feature-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.1);
    border-color: #4F46E5;
  }

  .feature-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .feature-title {
    font-size: 1.3rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .feature-description {
    color: #6B7280;
    line-height: 1.6;
  }

  /* Course Categories */
  .category-section {
    margin: 4rem 0;
  }

  .section-header {
    text-align: center;
    margin-bottom: 3rem;
  }

  .section-title {
    font-size: 2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.1rem;
  }

  .categories-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
  }

  .category-card {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 15px;
    padding: 2rem;
    color: white;
    text-align: center;
    transition: transform 0.3s ease;
    cursor: pointer;
  }

  .category-card:hover {
    transform: scale(1.05);
  }

  .category-card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
  }

  .category-card p {
    opacity: 0.95;
    line-height: 1.6;
  }

  /* Competition Section */
  .competition-badges {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: center;
    margin: 2rem 0;
  }

  .badge {
    background: #F3F4F6;
    padding: 0.5rem 1.5rem;
    border-radius: 25px;
    font-weight: 500;
    color: #4B5563;
    border: 2px solid transparent;
    transition: all 0.3s;
  }

  .badge:hover {
    border-color: #4F46E5;
    color: #4F46E5;
    background: #EEF2FF;
  }

  .badge-gold {
    background: linear-gradient(135deg, #FFD700, #FFA500);
    color: white;
  }

  /* Instructor Section */
  .instructor-highlights {
    background: #F9FAFB;
    border-radius: 15px;
    padding: 3rem;
    margin: 3rem 0;
  }

  .highlight-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .highlight-item {
    text-align: center;
  }

  .highlight-number {
    font-size: 2.5rem;
    font-weight: 700;
    color: #4F46E5;
  }

  .highlight-label {
    color: #6B7280;
    margin-top: 0.5rem;
  }

  /* CTA Section */
  .cta-section {
    background: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%);
    border-radius: 20px;
    padding: 3rem;
    text-align: center;
    color: white;
    margin: 4rem 0;
  }

  .cta-title {
    font-size: 2rem;
    margin-bottom: 1rem;
  }

  .cta-description {
    font-size: 1.1rem;
    margin-bottom: 2rem;
    opacity: 0.95;
  }

  .cta-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-button {
    background: white;
    color: #4F46E5;
    padding: 0.8rem 2rem;
    border-radius: 10px;
    text-decoration: none;
    font-weight: 600;
    transition: transform 0.3s;
    display: inline-block;
  }

  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  }

  .cta-button-secondary {
    background: transparent;
    color: white;
    border: 2px solid white;
  }

  .cta-button-secondary:hover {
    background: rgba(255, 255, 255, 0.1);
  }

  /* Language Toggle */
  .language-section {
    text-align: center;
    margin: 2rem 0;
  }

  .language-toggle {
    display: inline-flex;
    background: #F3F4F6;
    border-radius: 10px;
    padding: 0.25rem;
  }

  .lang-btn {
    padding: 0.5rem 1.5rem;
    border-radius: 8px;
    background: transparent;
    border: none;
    cursor: pointer;
    font-weight: 500;
    transition: all 0.3s;
  }

  .lang-btn.active {
    background: white;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .hero-title {
      font-size: 2rem;
    }
    
    .features-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<!-- Language Toggle -->
<div class="language-section">
  <div class="language-toggle">
    <button class="lang-btn active" onclick="setLanguage('en')">English</button>
    <button class="lang-btn" onclick="setLanguage('zh')">中文</button>
  </div>
</div>

<!-- Hero Section -->
<section class="hero-section">
  <h1 class="hero-title">
    <span class="en-content">Welcome to AIcoding Academy</span>
    <span class="zh-content" style="display:none;">欢迎来到 AIcoding 学院</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Where Future Tech Leaders Begin Their Journey</span>
    <span class="zh-content" style="display:none;">未来科技领袖的起点</span>
  </p>
</section>

<!-- Features Grid -->
<section class="features-grid">
  <div class="feature-card">
    <div class="feature-icon">🎯</div>
    <h3 class="feature-title">
      <span class="en-content">Personalized Learning</span>
      <span class="zh-content" style="display:none;">个性化学习</span>
    </h3>
    <p class="feature-description">
      <span class="en-content">Tailored curriculum designed to match your goals and learning pace</span>
      <span class="zh-content" style="display:none;">根据您的目标和学习节奏量身定制的课程</span>
    </p>
  </div>
  
  <div class="feature-card">
    <div class="feature-icon">🏆</div>
    <h3 class="feature-title">
      <span class="en-content">Competition Excellence</span>
      <span class="zh-content" style="display:none;">竞赛卓越</span>
    </h3>
    <p class="feature-description">
      <span class="en-content">Proven track record in USACO, USAAIO, AMC, and more</span>
      <span class="zh-content" style="display:none;">在 USACO、USAAIO、AMC 等竞赛中成绩斐然</span>
    </p>
  </div>
  
  <div class="feature-card">
    <div class="feature-icon">👨‍🏫</div>
    <h3 class="feature-title">
      <span class="en-content">Expert Instructors</span>
      <span class="zh-content" style="display:none;">专家导师</span>
    </h3>
    <p class="feature-description">
      <span class="en-content">PhD holders and industry professionals from top tech companies</span>
      <span class="zh-content" style="display:none;">来自顶尖科技公司的博士和行业专家</span>
    </p>
  </div>
</section>

<!-- Course Categories -->
<section class="category-section">
  <div class="section-header">
    <h2 class="section-title">
      <span class="en-content">Our Programs</span>
      <span class="zh-content" style="display:none;">我们的课程</span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Comprehensive courses from fundamentals to advanced topics</span>
      <span class="zh-content" style="display:none;">从基础到高级的全面课程</span>
    </p>
  </div>
  
  <div class="categories-grid">
    <div class="category-card">
      <h3>💻 Programming Languages</h3>
      <p>Python, Java, C++, JavaScript, R</p>
    </div>
    
    <div class="category-card" style="background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);">
      <h3>📊 Data & Algorithms</h3>
      <p>Data Structures, Algorithms, MySQL</p>
    </div>
    
    <div class="category-card" style="background: linear-gradient(135deg, #F59E0B 0%, #EF4444 100%);">
      <h3>🤖 AI & Machine Learning</h3>
      <p>Deep Learning, Neural Networks, AI Projects</p>
    </div>
  </div>
</section>

<!-- Competition Badges -->
<section class="competition-section">
  <div class="section-header">
    <h2 class="section-title">
      <span class="en-content">Competition Training</span>
      <span class="zh-content" style="display:none;">竞赛培训</span>
    </h2>
  </div>
  
  <div class="competition-badges">
    <span class="badge badge-gold">USACO Gold & Platinum</span>
    <span class="badge">USAAIO</span>
    <span class="badge">AMC 8/10/12</span>
    <span class="badge">AIME</span>
    <span class="badge">ACSL</span>
    <span class="badge">WorldQuant</span>
    <span class="badge">HiMCM</span>
    <span class="badge">AP CSA</span>
    <span class="badge">AP CSP</span>
  </div>
</section>

<!-- Instructor Highlights -->
<section class="instructor-highlights">
  <div class="section-header">
    <h2 class="section-title">
      <span class="en-content">Why Choose AIcoding?</span>
      <span class="zh-content" style="display:none;">为什么选择 AIcoding？</span>
    </h2>
  </div>
  
  <div class="highlight-grid">
    <div class="highlight-item">
      <div class="highlight-number">500+</div>
      <div class="highlight-label">
        <span class="en-content">Students Taught</span>
        <span class="zh-content" style="display:none;">学生人数</span>
      </div>
    </div>
    
    <div class="highlight-item">
      <div class="highlight-number">95%</div>
      <div class="highlight-label">
        <span class="en-content">Success Rate</span>
        <span class="zh-content" style="display:none;">成功率</span>
      </div>
    </div>
    
    <div class="highlight-item">
      <div class="highlight-number">50+</div>
      <div class="highlight-label">
        <span class="en-content">Competition Awards</span>
        <span class="zh-content" style="display:none;">竞赛奖项</span>
      </div>
    </div>
    
    <div class="highlight-item">
      <div class="highlight-number">10+</div>
      <div class="highlight-label">
        <span class="en-content">Years Experience</span>
        <span class="zh-content" style="display:none;">年经验</span>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <h2 class="cta-title">
    <span class="en-content">Ready to Start Your Coding Journey?</span>
    <span class="zh-content" style="display:none;">准备开始您的编程之旅了吗？</span>
  </h2>
  <p class="cta-description">
    <span class="en-content">Join hundreds of successful students who have achieved their tech dreams</span>
    <span class="zh-content" style="display:none;">加入数百名成功实现科技梦想的学生行列</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-button">
      <span class="en-content">Get Started Today</span>
      <span class="zh-content" style="display:none;">立即开始</span>
    </a>
    <a href="./course.html" class="cta-button cta-button-secondary">
      <span class="en-content">View All Courses</span>
      <span class="zh-content" style="display:none;">查看所有课程</span>
    </a>
  </div>
</section>

<script>
  function setLanguage(lang) {
    const enContent = document.querySelectorAll('.en-content');
    const zhContent = document.querySelectorAll('.zh-content');
    const langBtns = document.querySelectorAll('.lang-btn');
    
    langBtns.forEach(btn => btn.classList.remove('active'));
    
    if (lang === 'zh') {
      enContent.forEach(el => el.style.display = 'none');
      zhContent.forEach(el => el.style.display = 'inline');
      langBtns[1].classList.add('active');
    } else {
      enContent.forEach(el => el.style.display = 'inline');
      zhContent.forEach(el => el.style.display = 'none');
      langBtns[0].classList.add('active');
    }
  }
</script>
