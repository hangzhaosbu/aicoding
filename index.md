---
layout: default
title: AIcoding Academy
title_zh: AIcoding 学院
description: Elite Programming Education for Future Tech Leaders
description_zh: 为未来科技领袖提供的精英编程教育
---

<style>
  /* Advanced Animations */
  @keyframes gradientFlow {
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
    0% { background-position: -1000px 0; }
    100% { background-position: 1000px 0; }
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

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 0.8; }
    50% { transform: scale(1.05); opacity: 1; }
  }

  /* Hero Section - Ultra Premium */
  .hero-section {
    min-height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 75%, #4facfe 100%);
    background-size: 300% 300%;
    animation: gradientFlow 15s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.3);
  }

  .hero-section::before {
    content: '';
    position: absolute;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
    background: radial-gradient(circle at 20% 80%, rgba(120, 119, 198, 0.3), transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 92, 167, 0.3), transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(255, 255, 255, 0.1), transparent 50%);
    animation: pulse 10s ease-in-out infinite;
  }

  .hero-content {
    position: relative;
    z-index: 1;
    text-align: center;
    animation: slideInUp 1s ease-out;
  }

  .hero-title {
    font-size: 4.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
    margin-bottom: 1.5rem;
    letter-spacing: -2px;
    animation: float 6s ease-in-out infinite;
  }

  .hero-subtitle {
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.95);
    margin-bottom: 3rem;
    font-weight: 300;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .hero-btn {
    padding: 1.2rem 3rem;
    border-radius: 50px;
    font-weight: 600;
    font-size: 1.1rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    position: relative;
    overflow: hidden;
  }

  .hero-btn-primary {
    background: white;
    color: #667eea;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  }

  .hero-btn-primary::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.2), transparent);
    transition: left 0.5s;
  }

  .hero-btn-primary:hover::before {
    left: 100%;
  }

  .hero-btn-primary:hover {
    transform: translateY(-3px);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #667eea;
  }

  .hero-btn-secondary {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.5);
  }

  .hero-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.25);
    transform: translateY(-3px);
    color: white;
  }

  /* Animated Background Elements */
  .floating-icons {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 0;
  }

  .floating-icon {
    position: absolute;
    font-size: 3rem;
    opacity: 0.1;
    animation: float 20s infinite ease-in-out;
    color: white;
  }

  .floating-icon:nth-child(1) { top: 10%; left: 10%; animation-delay: 0s; }
  .floating-icon:nth-child(2) { top: 20%; right: 10%; animation-delay: 3s; }
  .floating-icon:nth-child(3) { bottom: 30%; left: 15%; animation-delay: 5s; }
  .floating-icon:nth-child(4) { bottom: 10%; right: 20%; animation-delay: 7s; }
  .floating-icon:nth-child(5) { top: 40%; left: 40%; animation-delay: 2s; }

  /* Features Grid - Premium Cards */
  .features-section {
    margin: 5rem 0;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2.5rem;
    margin: 3rem 0;
  }

  .feature-card {
    background: white;
    border-radius: 25px;
    padding: 3rem;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 1px solid rgba(229, 231, 235, 0.5);
    position: relative;
    overflow: hidden;
  }

  .feature-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    transform: scaleX(0);
    transition: transform 0.5s ease;
  }

  .feature-card:hover::before {
    transform: scaleX(1);
  }

  .feature-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
  }

  .feature-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 2rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    color: white;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
    animation: pulse 3s ease-in-out infinite;
  }

  .feature-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    text-align: center;
  }

  .feature-description {
    color: #6B7280;
    line-height: 1.8;
    text-align: center;
    font-size: 1.05rem;
  }

  /* Course Categories - Ultra Modern */
  .category-section {
    margin: 6rem 0;
    padding: 5rem 0;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 30px;
    position: relative;
    overflow: hidden;
  }

  .category-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(102, 126, 234, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(236, 72, 153, 0.05), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .section-header {
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    z-index: 1;
  }

  .section-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    position: relative;
    display: inline-block;
  }

  .section-title::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 100px;
    height: 4px;
    background: linear-gradient(90deg, #667eea, #764ba2);
    border-radius: 2px;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.3rem;
    font-weight: 300;
  }

  .categories-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2.5rem;
    position: relative;
    z-index: 1;
    padding: 0 2rem;
  }

  .category-card {
    border-radius: 25px;
    padding: 3rem;
    color: white;
    text-align: center;
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    cursor: pointer;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .category-card::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.2), transparent 70%);
    animation: rotate 10s linear infinite;
  }

  @keyframes rotate {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .category-card:hover {
    transform: scale(1.05) translateY(-5px);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.3);
  }

  .category-card h3 {
    font-size: 1.8rem;
    margin-bottom: 1rem;
    color: white !important;
    position: relative;
    z-index: 1;
  }

  .category-card p {
    opacity: 0.95;
    line-height: 1.6;
    color: white !important;
    font-size: 1.1rem;
    position: relative;
    z-index: 1;
  }

  .category-1 {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  }

  .category-2 {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
  }

  .category-3 {
    background: linear-gradient(135deg, #F59E0B 0%, #EF4444 100%);
  }

  /* Competition Section - Luxury Design */
  .competition-section {
    margin: 6rem 0;
    padding: 4rem;
    background: white;
    border-radius: 30px;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
  }

  .competition-badges {
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
    justify-content: center;
    margin: 3rem 0;
  }

  .badge {
    background: linear-gradient(135deg, #F3F4F6 0%, #E5E7EB 100%);
    padding: 1rem 2rem;
    border-radius: 50px;
    font-weight: 600;
    color: #4B5563;
    border: 2px solid transparent;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .badge::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.1), transparent);
    animation: shimmer 3s infinite;
  }

  .badge:hover {
    transform: translateY(-5px) scale(1.1);
    border-color: #667eea;
    color: #667eea;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
  }

  .badge-gold {
    background: linear-gradient(135deg, #FFD700, #FFA500);
    color: white;
    font-size: 1.1rem;
    padding: 1.2rem 2.5rem;
    animation: pulse 2s ease-in-out infinite;
  }

  /* Stats Section - Data Visualization Style */
  .stats-section {
    background: linear-gradient(135deg, #1F2937 0%, #111827 100%);
    border-radius: 30px;
    padding: 5rem 3rem;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 3rem;
    position: relative;
    z-index: 1;
  }

  .stat-item {
    text-align: center;
    animation: slideInUp 1s ease-out;
  }

  .stat-number {
    font-size: 4rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #EC4899 50%, #F59E0B 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.5rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #9CA3AF;
    font-size: 1.2rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 500;
  }

  /* CTA Section - Ultimate Premium */
  .cta-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientFlow 10s ease infinite;
    border-radius: 30px;
    padding: 5rem 3rem;
    text-align: center;
    color: white;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -100%;
    left: -100%;
    width: 300%;
    height: 300%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.1) 0%, transparent 70%);
    animation: rotate 20s linear infinite;
  }

  .cta-content {
    position: relative;
    z-index: 1;
  }

  .cta-title {
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    color: white !important;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
  }

  .cta-description {
    font-size: 1.3rem;
    margin-bottom: 3rem;
    opacity: 0.95;
    color: white !important;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-button {
    background: white;
    color: #667eea;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1.1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
  }

  .cta-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    color: #667eea;
  }

  .cta-button-secondary {
    background: transparent;
    color: white;
    border: 3px solid white;
  }

  .cta-button-secondary:hover {
    background: rgba(255, 255, 255, 0.15);
    color: white;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .hero-title {
      font-size: 2.5rem;
    }
    
    .features-grid {
      grid-template-columns: 1fr;
    }

    .categories-grid {
      grid-template-columns: 1fr;
      padding: 0 1rem;
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
    }

    .cta-title {
      font-size: 2rem;
    }
  }
</style>

<!-- Hero Section -->
<section class="hero-section">
  <div class="floating-icons">
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🚀</span>
    <span class="floating-icon">🎯</span>
    <span class="floating-icon">🏆</span>
    <span class="floating-icon">⚡</span>
  </div>
  
  <div class="hero-content">
    <h1 class="hero-title">
      <span class="en-content">AIcoding Academy</span>
      <span class="zh-content">AIcoding 学院</span>
    </h1>
    <p class="hero-subtitle">
      <span class="en-content">Transforming Students into Tech Innovators</span>
      <span class="zh-content">将学生转变为科技创新者</span>
    </p>
    <div class="hero-buttons">
      <a href="./contact.html" class="hero-btn hero-btn-primary">
        <span class="en-content">Start Your Journey</span>
        <span class="zh-content">开始您的旅程</span>
      </a>
      <a href="./course.html" class="hero-btn hero-btn-secondary">
        <span class="en-content">Explore Courses</span>
        <span class="zh-content">探索课程</span>
      </a>
    </div>
  </div>
</section>

<!-- Features Grid -->
<section class="features-section">
  <div class="features-grid">
    <div class="feature-card">
      <div class="feature-icon">🎯</div>
      <h3 class="feature-title">
        <span class="en-content">Personalized Learning</span>
        <span class="zh-content">个性化学习</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">AI-powered curriculum tailored to your unique learning style and goals</span>
        <span class="zh-content">AI驱动的课程，根据您独特的学习风格和目标量身定制</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon">🏆</div>
      <h3 class="feature-title">
        <span class="en-content">Competition Excellence</span>
        <span class="zh-content">竞赛卓越</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Proven track record with 200+ competition winners and national champions</span>
        <span class="zh-content">200+竞赛获胜者和全国冠军的成功记录</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon">👨‍🏫</div>
      <h3 class="feature-title">
        <span class="en-content">Elite Instructors</span>
        <span class="zh-content">精英导师</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Learn from PhD holders, FAANG engineers, and competition gold medalists</span>
        <span class="zh-content">向博士、FAANG工程师和竞赛金牌得主学习</span>
      </p>
    </div>
  </div>
</section>

<!-- Course Categories -->
<section class="category-section">
  <div class="section-header">
    <h2 class="section-title">
      <span class="en-content">Our Premium Programs</span>
      <span class="zh-content">我们的高端课程</span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">World-class education for tomorrow's tech leaders</span>
      <span class="zh-content">为明天的科技领袖提供世界级教育</span>
    </p>
  </div>
  
  <div class="categories-grid">
    <div class="category-card category-1">
      <h3>
        <span class="en-content">💻 Programming Mastery</span>
        <span class="zh-content">💻 编程精通</span>
      </h3>
      <p>
        <span class="en-content">Python, Java, C++, Web Development</span>
        <span class="zh-content">Python, Java, C++, 网页开发</span>
      </p>
    </div>
    
    <div class="category-card category-2">
      <h3>
        <span class="en-content">🧮 Algorithms & Data</span>
        <span class="zh-content">🧮 算法与数据</span>
      </h3>
      <p>
        <span class="en-content">Advanced DS, Algorithms, Database Systems</span>
        <span class="zh-content">高级数据结构、算法、数据库系统</span>
      </p>
    </div>
    
    <div class="category-card category-3">
      <h3>
        <span class="en-content">🤖 AI & Machine Learning</span>
        <span class="zh-content">🤖 人工智能与机器学习</span>
      </h3>
      <p>
        <span class="en-content">Deep Learning, Computer Vision, NLP</span>
        <span class="zh-content">深度学习、计算机视觉、自然语言处理</span>
      </p>
    </div>
  </div>
</section>

<!-- Competition Section -->
<section class="competition-section">
  <div class="section-header">
    <h2 class="section-title">
      <span class="en-content">Competition Training Excellence</span>
      <span class="zh-content">竞赛培训卓越</span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Prepare for the world's most prestigious competitions</span>
      <span class="zh-content">为世界上最负盛名的竞赛做准备</span>
    </p>
  </div>
  
  <div class="competition-badges">
    <span class="badge badge-gold">
      <span class="en-content">🥇 USACO Platinum</span>
      <span class="zh-content">🥇 USACO 白金</span>
    </span>
    <span class="badge">USAAIO</span>
    <span class="badge">AMC 8/10/12</span>
    <span class="badge">AIME</span>
    <span class="badge">ACSL</span>
    <span class="badge">Kaggle</span>
    <span class="badge">Google Code Jam</span>
    <span class="badge">AP CSA (5)</span>
    <span class="badge">IOI Training</span>
  </div>
</section>

<!-- Stats Section -->
<section class="stats-section">
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">50+</div>
      <div class="stat-label">
        <span class="en-content">Students</span>
        <span class="zh-content">学生</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-number">90%</div>
      <div class="stat-label">
        <span class="en-content">Success Rate</span>
        <span class="zh-content">成功率</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-number">20+</div>
      <div class="stat-label">
        <span class="en-content">Awards Won</span>
        <span class="zh-content">获得奖项</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-number">5+</div>
      <div class="stat-label">
        <span class="en-content">Years Experience</span>
        <span class="zh-content">年经验</span>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-content">
    <h2 class="cta-title">
      <span class="en-content">Ready to Achieve Excellence?</span>
      <span class="zh-content">准备好追求卓越了吗？</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Join the elite community of future tech innovators and competition champions</span>
      <span class="zh-content">加入未来科技创新者和竞赛冠军的精英社区</span>
    </p>
    <div class="cta-buttons">
      <a href="./contact.html" class="cta-button">
        <span class="en-content">Get Started Today</span>
        <span class="zh-content">立即开始</span>
      </a>
      <a href="./course.html" class="cta-button cta-button-secondary">
        <span class="en-content">View All Courses</span>
        <span class="zh-content">查看所有课程</span>
      </a>
    </div>
  </div>
</section>
