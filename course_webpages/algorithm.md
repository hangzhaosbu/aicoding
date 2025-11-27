---
layout: default
title: Algorithm Course
title_zh: 算法课程
description: Master Algorithmic Thinking and Problem Solving
description_zh: 掌握算法思维和问题解决
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

  @keyframes slideIn {
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

  @keyframes algorithmFlow {
    0% { 
      transform: translateY(100%) rotate(0deg); 
      opacity: 0; 
    }
    10% { opacity: 0.15; }
    90% { opacity: 0.15; }
    100% { 
      transform: translateY(-100%) rotate(360deg); 
      opacity: 0; 
    }
  }

  @keyframes codeScroll {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 25%, #8B5CF6 50%, #A855F7 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🧮';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: float 8s ease-in-out infinite;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotateGlow 20s linear infinite;
  }

  /* Algorithm symbols floating */
  .algo-symbols {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .symbol {
    position: absolute;
    font-family: 'Courier New', monospace;
    color: rgba(255, 255, 255, 0.15);
    font-size: 1.5rem;
    animation: algorithmFlow 25s linear infinite;
  }

  .symbol:nth-child(1) { left: 10%; animation-delay: 0s; }
  .symbol:nth-child(2) { left: 25%; animation-delay: 5s; }
  .symbol:nth-child(3) { left: 40%; animation-delay: 10s; }
  .symbol:nth-child(4) { left: 55%; animation-delay: 15s; }
  .symbol:nth-child(5) { left: 70%; animation-delay: 20s; }
  .symbol:nth-child(6) { left: 85%; animation-delay: 25s; }

  .course-hero h1 {
    font-size: 4rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    position: relative;
    z-index: 1;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    animation: slideIn 1s ease-out;
    color: white !important;
  }

  .course-hero p {
    font-size: 1.5rem;
    opacity: 0.95;
    position: relative;
    z-index: 1;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    animation: slideIn 1s ease-out 0.2s backwards;
    color: white !important;
  }

  /* Course Container */
  .course-container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 2rem;
  }

  /* Course Content Section */
  .course-content-section {
    background: white;
    padding: 3.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.5);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out;
    margin-bottom: 3rem;
  }

  .course-content-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(6, 182, 212, 0.05), transparent);
    animation: shimmer 4s infinite;
  }

  .section-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 3px solid transparent;
    border-image: linear-gradient(90deg, #06B6D4, #3B82F6) 1;
    position: relative;
  }

  /* Info Bar - Premium */
  .info-bar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 3rem 0;
    background: linear-gradient(135deg, #EFF6FF 0%, #E0E7FF 100%);
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(59, 130, 246, 0.1);
  }

  @media (max-width: 968px) {
    .info-bar {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .info-bar {
      grid-template-columns: 1fr;
    }
  }

  .info-bar-item {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .info-bar-icon {
    font-size: 2.5rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .info-bar-content h4 {
    font-size: 0.9rem;
    color: #1E3A8A;
    margin-bottom: 0.3rem;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    font-weight: 600;
  }

  .info-bar-content p {
    font-size: 1.2rem;
    color: #1E293B;
    font-weight: 700;
  }

  /* Module Cards - Premium Grid */
  .modules-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem 0;
  }

  @media (max-width: 968px) {
    .modules-grid {
      grid-template-columns: 1fr;
    }
  }

  .module-card {
    background: white;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.08);
    border: 1px solid rgba(229, 231, 235, 0.5);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out backwards;
  }

  .module-card:nth-child(1) { animation-delay: 0.1s; }
  .module-card:nth-child(2) { animation-delay: 0.2s; }
  .module-card:nth-child(3) { animation-delay: 0.3s; }
  .module-card:nth-child(4) { animation-delay: 0.4s; }
  .module-card:nth-child(5) { animation-delay: 0.5s; }
  .module-card:nth-child(6) { animation-delay: 0.6s; }

  .module-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #06B6D4, #3B82F6, #8B5CF6);
    transform: scaleX(0);
    transition: transform 0.4s;
  }

  .module-card:hover::before {
    transform: scaleX(1);
  }

  .module-card::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(59, 130, 246, 0.05), transparent);
    transition: left 0.6s;
  }

  .module-card:hover::after {
    left: 100%;
  }

  .module-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 25px 50px rgba(59, 130, 246, 0.15);
    border-color: #3B82F6;
  }

  .module-icon {
    width: 70px;
    height: 70px;
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    margin-bottom: 2rem;
    box-shadow: 0 10px 25px rgba(59, 130, 246, 0.3);
    animation: codeScroll 4s ease-in-out infinite;
  }

  .module-card:nth-child(odd) .module-icon {
    animation-delay: 0s;
  }

  .module-card:nth-child(even) .module-icon {
    animation-delay: 2s;
  }

  .module-title {
    font-size: 1.8rem;
    font-weight: 700;
    color: #1E293B;
    margin-bottom: 1rem;
  }

  .module-description {
    color: #64748B;
    line-height: 1.6;
    margin-bottom: 2rem;
    font-size: 1.1rem;
  }

  .topics-list {
    list-style: none;
    padding: 0;
  }

  .topics-list li {
    padding: 0.7rem 0;
    color: #475569;
    font-size: 1rem;
    display: flex;
    align-items: flex-start;
    transition: all 0.3s ease;
    border-bottom: 1px solid rgba(229, 231, 235, 0.5);
  }

  .topics-list li:last-child {
    border-bottom: none;
  }

  .topics-list li:hover {
    padding-left: 0.5rem;
    color: #1E293B;
  }

  .topics-list li::before {
    content: '→';
    color: #3B82F6;
    font-weight: bold;
    margin-right: 0.8rem;
    flex-shrink: 0;
    transition: transform 0.3s;
  }

  .topics-list li:hover::before {
    transform: translateX(5px);
  }

  /* Prerequisites Section - Premium */
  .prereq-section {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
    border-left: 5px solid #F59E0B;
    padding: 3rem;
    border-radius: 25px;
    margin: 3rem 0;
    box-shadow: 0 15px 35px rgba(245, 158, 11, 0.15);
    position: relative;
    overflow: hidden;
  }

  .prereq-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(245, 158, 11, 0.1), transparent);
    animation: shimmer 4s infinite;
  }

  .prereq-title {
    font-size: 1.6rem;
    font-weight: 700;
    color: #92400E;
    margin-bottom: 1.5rem;
  }

  .prereq-list {
    list-style: none;
    padding: 0;
  }

  .prereq-list li {
    padding: 1rem 0;
    color: #78350F;
    display: flex;
    align-items: center;
    font-size: 1.05rem;
    transition: all 0.3s ease;
  }

  .prereq-list li:hover {
    padding-left: 0.5rem;
  }

  .prereq-list li::before {
    content: '✨';
    color: #F59E0B;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 1.2rem;
    animation: pulse 2s ease-in-out infinite;
  }

  /* Prerequisites and Enrollment Grid */
  .prereq-enroll-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    margin: 3rem 0;
  }

  @media (max-width: 968px) {
    .prereq-enroll-grid {
      grid-template-columns: 1fr;
    }
  }

  .prereq-box {
    background: white;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.5);
  }

  .enroll-box {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 25%, #8B5CF6 50%, #A855F7 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(59, 130, 246, 0.3);
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    overflow: hidden;
  }

  .enroll-box::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 60%);
    animation: rotateGlow 12s linear infinite;
  }

  .enroll-content {
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .enroll-title {
    font-size: 2.5rem;
    font-weight: 800;
    color: white;
    margin-bottom: 1.5rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  }

  .enroll-button {
    background: white;
    color: #3B82F6;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
  }

  .enroll-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(59, 130, 246, 0.2), transparent);
    transition: left 0.5s;
  }

  .enroll-button:hover::before {
    left: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #8B5CF6;
  }

  .enroll-subtitle {
    color: white;
    margin-top: 1.5rem;
    font-size: 1.1rem;
    opacity: 0.95;
  }

  /* Responsive */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2.5rem;
    }
    
    .course-hero p {
      font-size: 1.2rem;
    }

    .section-title {
      font-size: 1.8rem;
    }
  }
</style>

<div class="course-hero">
  <div class="algo-symbols">
    <span class="symbol">O(n)</span>
    <span class="symbol">∑</span>
    <span class="symbol">log n</span>
    <span class="symbol">DFS</span>
    <span class="symbol">DP</span>
    <span class="symbol">BFS</span>
  </div>
  <h1>
    <span class="en-content">Algorithm Mastery Course</span>
    <span class="zh-content">算法精通课程</span>
  </h1>
  <p>
    <span class="en-content">From Basic Algorithms to Advanced Problem Solving</span>
    <span class="zh-content">从基础算法到高级问题解决</span>
  </p>
</div>

<div class="course-container">
  <!-- Course Overview -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">🧮 Course Overview</span>
      <span class="zh-content">🧮 课程概述</span>
    </h2>
    <p style="color: #4B5563; line-height: 1.8; font-size: 1.1rem;">
      <span class="en-content">
        Master the art of algorithmic thinking and problem-solving in this comprehensive 60+ hour course. 
        From fundamental sorting algorithms to advanced dynamic programming and graph theory, you'll gain 
        the skills needed to excel in competitive programming (USACO, ACSL), technical interviews at top 
        tech companies, and real-world software development. Our systematic approach ensures deep understanding 
        of both theoretical concepts and practical implementations.
      </span>
      <span class="zh-content">
        在这个60多小时的综合课程中掌握算法思维和问题解决的艺术。从基础排序算法到高级动态规划和图论，
        您将获得在竞赛编程（USACO、ACSL）、顶级科技公司技术面试和实际软件开发中脱颖而出所需的技能。
        我们的系统化方法确保深入理解理论概念和实际实现。
      </span>
    </p>
  </div>

  <!-- Course Info Bar -->
  <div class="info-bar">
    <div class="info-bar-item">
      <div class="info-bar-icon">⏱️</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Duration</span><span class="zh-content">课程时长</span></h4>
        <p>60+ Hours</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">📊</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Level</span><span class="zh-content">级别</span></h4>
        <p>Inter to Advanced</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">👥</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Age Group</span><span class="zh-content">年龄组</span></h4>
        <p>13-18 Years</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">🏆</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Perfect For</span><span class="zh-content">适合</span></h4>
        <p>USACO, ACSL</p>
      </div>
    </div>
  </div>

  <!-- Course Modules -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">📚 Comprehensive Curriculum</span>
      <span class="zh-content">📚 完整课程大纲</span>
    </h2>
    
    <div class="modules-grid">
      <!-- Module 1: Basic Algorithms -->
      <div class="module-card">
        <div class="module-icon">📊</div>
        <h2 class="module-title">
          <span class="en-content">Basic Algorithms</span>
          <span class="zh-content">基础算法</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Master fundamental algorithmic techniques and concepts</span>
          <span class="zh-content">掌握基础算法技术和概念</span>
        </p>
        <ul class="topics-list">
          <li>Sorting Algorithms (Quick, Merge, Heap)</li>
          <li>Binary Search & Variations</li>
          <li>Two Pointer Technique</li>
          <li>Sliding Window Algorithm</li>
          <li>Bit Manipulation</li>
          <li>Prefix Sums & Differences</li>
          <li>Discretization</li>
          <li>Interval Merging</li>
        </ul>
      </div>

      <!-- Module 2: Data Structures -->
      <div class="module-card">
        <div class="module-icon">🗂️</div>
        <h2 class="module-title">
          <span class="en-content">Advanced Data Structures</span>
          <span class="zh-content">高级数据结构</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Essential data structures for efficient problem solving</span>
          <span class="zh-content">高效解决问题的基本数据结构</span>
        </p>
        <ul class="topics-list">
          <li>Linked Lists (Single & Double)</li>
          <li>Stacks & Queues</li>
          <li>Monotonic Stack & Queue</li>
          <li>String Algorithms (KMP, Z-Algorithm)</li>
          <li>Trie (Prefix Tree)</li>
          <li>Union-Find (Disjoint Set)</li>
          <li>Heaps & Priority Queues</li>
          <li>Hash Tables & Rolling Hash</li>
        </ul>
      </div>

      <!-- Module 3: Graph Theory -->
      <div class="module-card">
        <div class="module-icon">🕸️</div>
        <h2 class="module-title">
          <span class="en-content">Graph Theory</span>
          <span class="zh-content">图论</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Graph algorithms and network analysis</span>
          <span class="zh-content">图算法和网络分析</span>
        </p>
        <ul class="topics-list">
          <li>DFS & BFS Traversal</li>
          <li>Topological Sorting</li>
          <li>Shortest Path (Dijkstra, Bellman-Ford)</li>
          <li>SPFA Algorithm</li>
          <li>All-Pairs Shortest Path (Floyd-Warshall)</li>
          <li>MST (Prim & Kruskal)</li>
          <li>Bipartite Graph Detection & Matching</li>
          <li>Network Flow & Hungarian Algorithm</li>
        </ul>
      </div>

      <!-- Module 4: Mathematics -->
      <div class="module-card">
        <div class="module-icon">∑</div>
        <h2 class="module-title">
          <span class="en-content">Mathematical Foundations</span>
          <span class="zh-content">数学基础</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Mathematical concepts essential for algorithms</span>
          <span class="zh-content">算法必需的数学概念</span>
        </p>
        <ul class="topics-list">
          <li>Prime Numbers & Sieve of Eratosthenes</li>
          <li>GCD & Euler's Function</li>
          <li>Fast Exponentiation & Modular Arithmetic</li>
          <li>Extended Euclidean Algorithm</li>
          <li>Chinese Remainder Theorem</li>
          <li>Gaussian Elimination</li>
          <li>Combinatorics & Probability</li>
          <li>Inclusion-Exclusion Principle</li>
          <li>Game Theory & Nim</li>
        </ul>
      </div>

      <!-- Module 5: Dynamic Programming -->
      <div class="module-card">
        <div class="module-icon">🔄</div>
        <h2 class="module-title">
          <span class="en-content">Dynamic Programming</span>
          <span class="zh-content">动态规划</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Optimization through state-based problem solving</span>
          <span class="zh-content">通过状态优化问题解决</span>
        </p>
        <ul class="topics-list">
          <li>Knapsack Problems (0/1, Unbounded, Multiple)</li>
          <li>Linear DP & LIS/LCS</li>
          <li>Interval DP</li>
          <li>Counting DP</li>
          <li>Digit DP</li>
          <li>State Compression DP</li>
          <li>Tree DP</li>
          <li>DP Optimization (Convex Hull, Monotone Queue)</li>
        </ul>
      </div>

      <!-- Module 6: Greedy & Advanced -->
      <div class="module-card">
        <div class="module-icon">💎</div>
        <h2 class="module-title">
          <span class="en-content">Greedy & Advanced Topics</span>
          <span class="zh-content">贪心与高级主题</span>
        </h2>
        <p class="module-description">
          <span class="en-content">Optimal strategies and advanced techniques</span>
          <span class="zh-content">最优策略和高级技术</span>
        </p>
        <ul class="topics-list">
          <li>Interval Scheduling Problems</li>
          <li>Huffman Coding</li>
          <li>Activity Selection</li>
          <li>Fractional Knapsack</li>
          <li>Exchange Arguments</li>
          <li>Segment Trees & Fenwick Trees</li>
          <li>Heavy-Light Decomposition</li>
          <li>Persistent Data Structures</li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Prerequisites & Enrollment -->
  <div class="prereq-enroll-grid">
    <div class="prereq-box">
      <h2 class="section-title">
        <span class="en-content">📋 Prerequisites</span>
        <span class="zh-content">📋 先修要求</span>
      </h2>
      <ul class="prereq-list" style="list-style: none; padding: 0;">
        <li style="padding: 1rem 0; color: #475569; display: flex; align-items: center; font-size: 1.05rem;">
          <span style="content: '✨'; margin-right: 1rem; font-size: 1.2rem;">✨</span>
          <span class="en-content">Proficiency in Python, Java, or C++</span>
          <span class="zh-content">精通Python、Java或C++</span>
        </li>
        <li style="padding: 1rem 0; color: #475569; display: flex; align-items: center; font-size: 1.05rem;">
          <span style="content: '✨'; margin-right: 1rem; font-size: 1.2rem;">✨</span>
          <span class="en-content">Basic data structures knowledge</span>
          <span class="zh-content">基础数据结构知识</span>
        </li>
        <li style="padding: 1rem 0; color: #475569; display: flex; align-items: center; font-size: 1.05rem;">
          <span style="content: '✨'; margin-right: 1rem; font-size: 1.2rem;">✨</span>
          <span class="en-content">High school mathematics</span>
          <span class="zh-content">高中数学</span>
        </li>
        <li style="padding: 1rem 0; color: #475569; display: flex; align-items: center; font-size: 1.05rem;">
          <span style="content: '✨'; margin-right: 1rem; font-size: 1.2rem;">✨</span>
          <span class="en-content">Problem-solving mindset</span>
          <span class="zh-content">问题解决思维</span>
        </li>
      </ul>
    </div>

    <div class="enroll-box">
      <div class="enroll-content">
        <h2 class="enroll-title">
          <span class="en-content">Master Algorithms</span>
          <span class="zh-content">掌握算法</span>
        </h2>
        <a href="./contact.html" class="enroll-button">
          <span class="en-content">Start Learning</span>
          <span class="zh-content">开始学习</span>
        </a>
        <p class="enroll-subtitle">
          <span class="en-content">✨ Free consultation & assessment</span>
          <span class="zh-content">✨ 免费咨询和评估</span>
        </p>
      </div>
    </div>
  </div>
</div>
