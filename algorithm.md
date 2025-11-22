---
layout: default
title: Algorithm Course
description: Master Algorithmic Thinking and Problem Solving
---

<style>
  /* Course Hero Section */
  .course-hero {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    padding: 4rem 2rem;
    border-radius: 20px;
    color: white;
    text-align: center;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .course-hero::before {
    content: '🧮';
    position: absolute;
    font-size: 15rem;
    opacity: 0.1;
    right: -50px;
    top: -50px;
    transform: rotate(-15deg);
  }

  .course-hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .course-hero p {
    font-size: 1.2rem;
    opacity: 0.95;
    position: relative;
    z-index: 1;
  }

  /* Module Cards */
  .modules-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
  }

  .module-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 1px solid #E5E7EB;
    transition: all 0.3s;
  }

  .module-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
    border-color: #3B82F6;
  }

  .module-icon {
    width: 60px;
    height: 60px;
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
  }

  .module-title {
    font-size: 1.5rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .module-description {
    color: #6B7280;
    line-height: 1.6;
    margin-bottom: 1.5rem;
  }

  .topics-list {
    list-style: none;
    padding: 0;
  }

  .topics-list li {
    padding: 0.5rem 0;
    color: #4B5563;
    font-size: 0.9rem;
    display: flex;
    align-items: flex-start;
  }

  .topics-list li::before {
    content: '▸';
    color: #3B82F6;
    font-weight: bold;
    margin-right: 0.5rem;
    flex-shrink: 0;
  }

  /* Info Section */
  .info-section {
    background: #F9FAFB;
    padding: 3rem;
    border-radius: 15px;
    margin: 3rem 0;
  }

  .info-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    text-align: center;
  }

  .info-item {
    background: white;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
  }

  .info-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }

  .info-label {
    color: #6B7280;
    font-size: 0.9rem;
    margin-bottom: 0.5rem;
  }

  .info-value {
    font-size: 1.2rem;
    font-weight: 600;
    color: #1F2937;
  }

  /* Prerequisites */
  .prereq-section {
    background: #FEF3C7;
    border-left: 4px solid #F59E0B;
    padding: 1.5rem;
    border-radius: 10px;
    margin: 2rem 0;
  }

  .prereq-title {
    font-size: 1.2rem;
    font-weight: 600;
    color: #92400E;
    margin-bottom: 1rem;
  }

  .prereq-list {
    list-style: none;
    padding: 0;
  }

  .prereq-list li {
    padding: 0.5rem 0;
    color: #78350F;
    display: flex;
    align-items: center;
  }

  .prereq-list li::before {
    content: '✓';
    color: #F59E0B;
    font-weight: bold;
    margin-right: 0.5rem;
  }

  /* CTA Section */
  .cta-section {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    padding: 3rem;
    border-radius: 15px;
    text-align: center;
    color: white;
    margin: 3rem 0;
  }

  .cta-title {
    font-size: 2rem;
    margin-bottom: 1rem;
  }

  .cta-button {
    background: white;
    color: #3B82F6;
    padding: 1rem 2rem;
    border-radius: 10px;
    text-decoration: none;
    display: inline-block;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s;
    margin-top: 1rem;
  }

  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  }

  /* Responsive */
  @media (max-width: 768px) {
    .modules-grid {
      grid-template-columns: 1fr;
    }
    
    .course-hero h1 {
      font-size: 2rem;
    }
  }
</style>

<!-- Course Hero -->
<div class="course-hero">
  <h1>
    <span class="en-content">Algorithm Mastery Course</span>
    <span class="zh-content">算法精通课程</span>
  </h1>
  <p>
    <span class="en-content">From Basic Algorithms to Advanced Problem Solving</span>
    <span class="zh-content">从基础算法到高级问题解决</span>
  </p>
</div>

<!-- Course Modules -->
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
      <span class="en-content">Data Structures</span>
      <span class="zh-content">数据结构</span>
    </h2>
    <p class="module-description">
      <span class="en-content">Essential data structures for efficient problem solving</span>
      <span class="zh-content">高效解决问题的基本数据结构</span>
    </p>
    <ul class="topics-list">
      <li>Linked Lists (Single & Double)</li>
      <li>Stacks & Queues</li>
      <li>Monotonic Stack & Queue</li>
      <li>String Algorithms (KMP)</li>
      <li>Trie (Prefix Tree)</li>
      <li>Union-Find (Disjoint Set)</li>
      <li>Heaps & Priority Queues</li>
      <li>Hash Tables</li>
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
      <li>Bipartite Graph Detection</li>
      <li>Hungarian Algorithm</li>
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
      <li>Prime Numbers & Divisors</li>
      <li>Euler's Function</li>
      <li>Fast Exponentiation</li>
      <li>Extended Euclidean Algorithm</li>
      <li>Chinese Remainder Theorem</li>
      <li>Gaussian Elimination</li>
      <li>Combinatorics</li>
      <li>Inclusion-Exclusion Principle</li>
      <li>Game Theory</li>
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
      <li>Knapsack Problems</li>
      <li>Linear DP</li>
      <li>Interval DP</li>
      <li>Counting DP</li>
      <li>Digit DP</li>
      <li>State Compression DP</li>
      <li>Tree DP</li>
      <li>Memoization Techniques</li>
    </ul>
  </div>

  <!-- Module 6: Greedy Algorithms -->
  <div class="module-card">
    <div class="module-icon">💎</div>
    <h2 class="module-title">
      <span class="en-content">Greedy Algorithms</span>
      <span class="zh-content">贪心算法</span>
    </h2>
    <p class="module-description">
      <span class="en-content">Optimal local choices for global solutions</span>
      <span class="zh-content">局部最优到全局最优</span>
    </p>
    <ul class="topics-list">
      <li>Interval Scheduling Problems</li>
      <li>Huffman Coding</li>
      <li>Activity Selection</li>
      <li>Fractional Knapsack</li>
      <li>Ranking Inequalities</li>
      <li>Exchange Arguments</li>
      <li>Matroid Theory Basics</li>
    </ul>
  </div>
</div>

<!-- Course Information -->
<div class="info-section">
  <div class="info-grid">
    <div class="info-item">
      <div class="info-icon">⏱️</div>
      <div class="info-label">
        <span class="en-content">Duration</span>
        <span class="zh-content">课程时长</span>
      </div>
      <div class="info-value">60+ Hours</div>
    </div>
    
    <div class="info-item">
      <div class="info-icon">📊</div>
      <div class="info-label">
        <span class="en-content">Difficulty</span>
        <span class="zh-content">难度</span>
      </div>
      <div class="info-value">
        <span class="en-content">Intermediate to Advanced</span>
        <span class="zh-content">中级到高级</span>
      </div>
    </div>
    
    <div class="info-item">
      <div class="info-icon">👥</div>
      <div class="info-label">
        <span class="en-content">Age Group</span>
        <span class="zh-content">年龄组</span>
      </div>
      <div class="info-value">13-18</div>
    </div>
    
    <div class="info-item">
      <div class="info-icon">🏆</div>
      <div class="info-label">
        <span class="en-content">Perfect For</span>
        <span class="zh-content">适合</span>
      </div>
      <div class="info-value">USACO, ACSL</div>
    </div>
  </div>
</div>

<!-- Prerequisites -->
<div class="prereq-section">
  <h3 class="prereq-title">
    <span class="en-content">📚 Prerequisites</span>
    <span class="zh-content">📚 先修要求</span>
  </h3>
  <ul class="prereq-list">
    <li>
      <span class="en-content">Proficiency in at least one programming language (Python, Java, or C++)</span>
      <span class="zh-content">至少精通一门编程语言（Python、Java 或 C++）</span>
    </li>
    <li>
      <span class="en-content">Understanding of basic data structures (arrays, lists)</span>
      <span class="zh-content">理解基本数据结构（数组、列表）</span>
    </li>
    <li>
      <span class="en-content">High school mathematics background</span>
      <span class="zh-content">高中数学背景</span>
    </li>
    <li>
      <span class="en-content">Problem-solving mindset and patience</span>
      <span class="zh-content">解决问题的思维和耐心</span>
    </li>
  </ul>
</div>

<!-- CTA Section -->
<div class="cta-section">
  <h2 class="cta-title">
    <span class="en-content">Ready to Master Algorithms?</span>
    <span class="zh-content">准备掌握算法了吗？</span>
  </h2>
  <p>
    <span class="en-content">Join our comprehensive algorithm course and excel in competitions</span>
    <span class="zh-content">加入我们的综合算法课程，在竞赛中脱颖而出</span>
  </p>
  <a href="../aicoding/contact.html" class="cta-button">
    <span class="en-content">Start Learning Today</span>
    <span class="zh-content">立即开始学习</span>
  </a>
</div>
