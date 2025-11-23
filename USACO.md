---
layout: default
title: USACO Training
title_zh: USACO 培训
description: USA Computing Olympiad Competition Preparation
description_zh: 美国计算机奥林匹克竞赛准备
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

  .course-hero h1 {
    color: white !important;
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .course-hero p {
    color: white !important;
    font-size: 1.2rem;
    opacity: 0.95;
  }

  /* Level Cards Grid - 2x2 layout */
  .level-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    margin: 3rem auto;
    max-width: 1200px;
  }

  /* Responsive: 4 columns on large screens */
  @media (min-width: 1200px) {
    .level-cards {
      grid-template-columns: repeat(4, 1fr);
    }
  }

  /* Responsive: 1 column on mobile */
  @media (max-width: 768px) {
    .level-cards {
      grid-template-columns: 1fr;
    }
  }

  .level-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 2px solid #E5E7EB;
    transition: all 0.3s;
    display: flex;
    flex-direction: column;
  }

  .level-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
  }

  .bronze { 
    border-top: 5px solid #CD7F32;
    background: linear-gradient(to bottom, rgba(205, 127, 50, 0.05) 0%, white 30%);
  }
  
  .silver { 
    border-top: 5px solid #C0C0C0;
    background: linear-gradient(to bottom, rgba(192, 192, 192, 0.05) 0%, white 30%);
  }
  
  .gold { 
    border-top: 5px solid #FFD700;
    background: linear-gradient(to bottom, rgba(255, 215, 0, 0.05) 0%, white 30%);
  }
  
  .platinum { 
    border-top: 5px solid #E5E4E2;
    background: linear-gradient(to bottom, rgba(229, 228, 226, 0.08) 0%, white 30%);
  }

  .level-header {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .level-icon {
    font-size: 3rem;
    margin-bottom: 0.5rem;
  }

  .level-name {
    font-size: 1.4rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .level-subtitle {
    font-size: 0.9rem;
    font-weight: 500;
    color: #6B7280;
    margin-bottom: 1rem;
  }

  .level-topics {
    color: #6B7280;
    line-height: 1.6;
    flex-grow: 1;
  }

  .level-topics ul {
    padding-left: 1.2rem;
    margin: 0;
  }

  .level-topics li {
    margin: 0.3rem 0;
    font-size: 0.9rem;
  }

  /* Section headers */
  .section-header {
    text-align: center;
    color: #1F2937;
    margin: 3rem 0 2rem;
  }

  .section-header h2 {
    font-size: 2rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
  }

  .section-header p {
    color: #6B7280;
    font-size: 1.1rem;
  }

  /* Training Approach Section */
  .training-features {
    background: #F9FAFB;
    padding: 3rem;
    border-radius: 15px;
    margin: 3rem 0;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .feature-item {
    text-align: center;
    background: white;
    padding: 2rem;
    border-radius: 10px;
    transition: transform 0.3s;
  }

  .feature-item:hover {
    transform: translateY(-3px);
  }

  .feature-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .feature-title {
    color: #1F2937;
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
  }

  .feature-description {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.5;
  }

  /* Success Stories */
  .success-section {
    background: white;
    padding: 3rem;
    border-radius: 15px;
    margin: 3rem 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin: 2rem 0;
  }

  .stat-item {
    text-align: center;
  }

  .stat-number {
    font-size: 2.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .stat-label {
    color: #6B7280;
    font-size: 0.95rem;
    margin-top: 0.5rem;
  }

  /* Timeline */
  .timeline-section {
    padding: 3rem 0;
  }

  .timeline {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    max-width: 900px;
    margin: 2rem auto;
  }

  .timeline::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 0;
    right: 0;
    height: 2px;
    background: linear-gradient(to right, #CD7F32, #C0C0C0, #FFD700, #E5E4E2);
    z-index: 0;
  }

  .timeline-item {
    background: white;
    padding: 1rem;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    z-index: 1;
    position: relative;
    text-align: center;
    flex: 1;
    margin: 0 0.5rem;
  }

  .timeline-level {
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .timeline-duration {
    font-size: 0.85rem;
    color: #6B7280;
  }

  /* CTA Section */
  .cta-section {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    padding: 3rem;
    border-radius: 15px;
    text-align: center;
    color: white;
  }

  .cta-section h2 {
    color: white !important;
    font-size: 2rem;
    margin-bottom: 1rem;
  }

  .cta-section p {
    color: white !important;
    font-size: 1.1rem;
    margin: 1rem 0;
    opacity: 0.95;
  }

  .cta-button {
    background: white;
    color: #FFA500;
    padding: 1rem 2rem;
    border-radius: 10px;
    text-decoration: none;
    display: inline-block;
    font-weight: 600;
    margin-top: 1rem;
    transition: all 0.3s;
  }

  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    color: #FFA500;
  }
</style>

<div class="course-hero">
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
    <span class="en-content">Progressive training through all USACO divisions</span>
    <span class="zh-content">通过所有USACO级别的渐进式培训</span>
  </p>
</div>

<!-- Level Cards - 2x2 or 4x1 layout -->
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
        <span class="en-content">Getting Started</span>
        <span class="zh-content">入门基础</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Introduction to USACO</span>
          <span class="zh-content">USACO 简介</span>
        </li>
        <li>
          <span class="en-content">Input/Output handling</span>
          <span class="zh-content">输入输出处理</span>
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
          <span class="en-content">Simulation problems</span>
          <span class="zh-content">模拟题</span>
        </li>
        <li>
          <span class="en-content">Basic sorting</span>
          <span class="zh-content">基础排序</span>
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
          <span class="en-content">Graph Theory (DFS, BFS)</span>
          <span class="zh-content">图论（深搜、广搜）</span>
        </li>
        <li>
          <span class="en-content">Flood Fill</span>
          <span class="zh-content">洪水填充</span>
        </li>
        <li>
          <span class="en-content">Binary Search</span>
          <span class="zh-content">二分搜索</span>
        </li>
        <li>
          <span class="en-content">Two Pointers</span>
          <span class="zh-content">双指针</span>
        </li>
        <li>
          <span class="en-content">Prefix Sums</span>
          <span class="zh-content">前缀和</span>
        </li>
        <li>
          <span class="en-content">Custom Comparators</span>
          <span class="zh-content">自定义比较器</span>
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
          <span class="en-content">Shortest Paths (Dijkstra)</span>
          <span class="zh-content">最短路径（Dijkstra）</span>
        </li>
        <li>
          <span class="en-content">Minimum Spanning Trees</span>
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
          <span class="en-content">Euler Paths</span>
          <span class="zh-content">欧拉路径</span>
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
        <span class="en-content">Expert Level</span>
        <span class="zh-content">专家级别</span>
      </p>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Advanced DP</span>
          <span class="zh-content">高级动态规划</span>
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
          <span class="en-content">Advanced Data Structures</span>
          <span class="zh-content">高级数据结构</span>
        </li>
        <li>
          <span class="en-content">String Algorithms</span>
          <span class="zh-content">字符串算法</span>
        </li>
        <li>
          <span class="en-content">Number Theory</span>
          <span class="zh-content">数论</span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- Timeline Section -->
<div class="timeline-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Typical Progression Timeline</span>
      <span class="zh-content">典型进阶时间线</span>
    </h2>
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
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 2rem;">
    <span class="en-content">Our Training Approach</span>
    <span class="zh-content">我们的培训方法</span>
  </h2>
  
  <div class="features-grid">
    <div class="feature-item">
      <div class="feature-icon">📝</div>
      <h3 class="feature-title">
        <span class="en-content">1000+ Problems</span>
        <span class="zh-content">1000+ 题目</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Curated problem sets for each level</span>
        <span class="zh-content">为每个级别精心挑选的题目集</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">🎯</div>
      <h3 class="feature-title">
        <span class="en-content">Contest Strategy</span>
        <span class="zh-content">竞赛策略</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Time management and problem selection</span>
        <span class="zh-content">时间管理和题目选择技巧</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">💻</div>
      <h3 class="feature-title">
        <span class="en-content">Mock Contests</span>
        <span class="zh-content">模拟竞赛</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Regular practice competitions</span>
        <span class="zh-content">定期练习比赛</span>
      </p>
    </div>
    
    <div class="feature-item">
      <div class="feature-icon">📊</div>
      <h3 class="feature-title">
        <span class="en-content">Progress Tracking</span>
        <span class="zh-content">进度跟踪</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Personalized improvement plans</span>
        <span class="zh-content">个性化提升计划</span>
      </p>
    </div>

    <div class="feature-item">
      <div class="feature-icon">👨‍🏫</div>
      <h3 class="feature-title">
        <span class="en-content">Expert Instructors</span>
        <span class="zh-content">专家讲师</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Learn from USACO finalists</span>
        <span class="zh-content">向USACO决赛选手学习</span>
      </p>
    </div>

    <div class="feature-item">
      <div class="feature-icon">🤝</div>
      <h3 class="feature-title">
        <span class="en-content">Small Groups</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Maximum 4 students per class</span>
        <span class="zh-content">每班最多4名学生</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stories -->
<div class="success-section">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 2rem;">
    <span class="en-content">Our Track Record</span>
    <span class="zh-content">我们的成绩</span>
  </h2>
  
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">200+</div>
      <div class="stat-label">
        <span class="en-content">Students Trained</span>
        <span class="zh-content">培训学生</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">85%</div>
      <div class="stat-label">
        <span class="en-content">Promotion Rate</span>
        <span class="zh-content">晋级率</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">50+</div>
      <div class="stat-label">
        <span class="en-content">Gold & Above</span>
        <span class="zh-content">金牌及以上</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">12</div>
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
    <span class="zh-content">今天就开始您的USACO之旅！</span>
  </h2>
  <p>
    <span class="en-content">Join hundreds of students who have achieved Gold and Platinum</span>
    <span class="zh-content">加入数百名获得金牌和白金的学生行列</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Enroll Now</span>
    <span class="zh-content">立即报名</span>
  </a>
</div>
