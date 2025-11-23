---
layout: default
title: Data Structures Course
title_zh: 数据结构课程
description: Master Fundamental Data Structures for Programming Excellence
description_zh: 掌握基础数据结构，实现编程卓越
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
    content: '🗂️';
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
    color: white !important;
  }

  .course-hero p {
    font-size: 1.2rem;
    opacity: 0.95;
    position: relative;
    z-index: 1;
    color: white !important;
  }

  /* Course Overview */
  .course-overview {
    background: white;
    padding: 2.5rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    margin-bottom: 3rem;
  }

  /* Module Cards */
  .modules-container {
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
    border-left: 4px solid #06B6D4;
    transition: all 0.3s;
  }

  .module-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
  }

  .module-number {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    color: white;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 600;
    margin-bottom: 1rem;
  }

  .module-title {
    font-size: 1.3rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .module-content {
    color: #6B7280;
    line-height: 1.6;
    font-size: 0.95rem;
  }

  .module-topics {
    list-style: none;
    padding: 0;
    margin-top: 1rem;
  }

  .module-topics li {
    padding: 0.3rem 0;
    color: #4B5563;
    font-size: 0.9rem;
    display: flex;
    align-items: flex-start;
  }

  .module-topics li::before {
    content: '▸';
    color: #06B6D4;
    font-weight: bold;
    margin-right: 0.5rem;
    flex-shrink: 0;
  }

  /* Info Grid */
  .info-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin: 2rem 0;
    text-align: center;
  }

  .info-item {
    background: #F9FAFB;
    padding: 1.5rem;
    border-radius: 10px;
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

  /* Learning Outcomes */
  .outcomes-section {
    background: #F0FDF4;
    padding: 2.5rem;
    border-radius: 15px;
    margin: 3rem 0;
  }

  .outcomes-title {
    font-size: 1.8rem;
    font-weight: 600;
    color: #14532D;
    margin-bottom: 1.5rem;
    text-align: center;
  }

  .outcomes-list {
    list-style: none;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1rem;
  }

  .outcomes-list li {
    padding: 1rem;
    background: white;
    border-radius: 10px;
    display: flex;
    align-items: flex-start;
  }

  .outcomes-list li::before {
    content: '✓';
    color: #10B981;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 1.2rem;
    flex-shrink: 0;
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
    color: white !important;
  }

  .cta-button {
    background: white;
    color: #3B82F6;
    padding: 1rem 2rem;
    border-radius: 10px;
    text-decoration: none;
    display: inline-block;
    font-weight: 600;
    transition: all 0.3s;
    margin-top: 1rem;
  }

  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    color: #3B82F6;
  }

  /* Java API Section */
  .api-section {
    background: #FEF3C7;
    padding: 2rem;
    border-radius: 15px;
    margin: 2rem 0;
    border-left: 4px solid #F59E0B;
  }

  /* Responsive */
  @media (max-width: 768px) {
    .modules-container {
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
    <span class="en-content">Data Structures Mastery</span>
    <span class="zh-content">数据结构精通课程</span>
  </h1>
  <p>
    <span class="en-content">Build Strong Foundation for Advanced Programming</span>
    <span class="zh-content">为高级编程打下坚实基础</span>
  </p>
</div>

<!-- Course Overview -->
<div class="course-overview">
  <h2 style="color: #1F2937; border-bottom: 3px solid #06B6D4; padding-bottom: 0.5rem; margin-bottom: 1.5rem;">
    <span class="en-content">Course Overview</span>
    <span class="zh-content">课程概述</span>
  </h2>
  <p style="font-size: 1.1rem; color: #4B5563; line-height: 1.8;">
    <span class="en-content">
      Master the fundamental data structures that form the backbone of computer science and software engineering. 
      This comprehensive 40-hour course covers everything from basic linear structures to advanced trees and graphs, 
      preparing you for technical interviews, competitions, and real-world programming challenges.
    </span>
    <span class="zh-content">
      掌握构成计算机科学和软件工程支柱的基础数据结构。
      这门40小时的综合课程涵盖了从基本线性结构到高级树和图的所有内容，
      为您准备技术面试、竞赛和实际编程挑战。
    </span>
  </p>
</div>

<!-- Course Information -->
<div class="info-grid">
  <div class="info-item">
    <div class="info-icon">⏱️</div>
    <div class="info-label">
      <span class="en-content">Duration</span>
      <span class="zh-content">课程时长</span>
    </div>
    <div class="info-value">40 Hours</div>
  </div>
  
  <div class="info-item">
    <div class="info-icon">📊</div>
    <div class="info-label">
      <span class="en-content">Level</span>
      <span class="zh-content">级别</span>
    </div>
    <div class="info-value">
      <span class="en-content">Intermediate</span>
      <span class="zh-content">中级</span>
    </div>
  </div>
  
  <div class="info-item">
    <div class="info-icon">💻</div>
    <div class="info-label">
      <span class="en-content">Languages</span>
      <span class="zh-content">编程语言</span>
    </div>
    <div class="info-value">Java/Python</div>
  </div>
  
  <div class="info-item">
    <div class="info-icon">🎯</div>
    <div class="info-label">
      <span class="en-content">Prerequisites</span>
      <span class="zh-content">先修要求</span>
    </div>
    <div class="info-value">
      <span class="en-content">Basic Programming</span>
      <span class="zh-content">基础编程</span>
    </div>
  </div>
</div>

<!-- Detailed Curriculum -->
<h2 style="text-align: center; color: #1F2937; margin: 3rem 0 2rem;">
  <span class="en-content">Detailed Curriculum</span>
  <span class="zh-content">详细课程大纲</span>
</h2>

<div class="modules-container">
  <!-- Module 1 -->
  <div class="module-card">
    <div class="module-number">1</div>
    <h3 class="module-title">
      <span class="en-content">Complexity Analysis</span>
      <span class="zh-content">复杂度分析</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Understanding Time & Space Complexity</span>
      <span class="zh-content">理解时间与空间复杂度</span>
    </p>
    <ul class="module-topics">
      <li>Big O, Omega, and Theta Notation</li>
      <li>Best, Average, and Worst Case Analysis</li>
      <li>Amortized Analysis</li>
      <li>Space-Time Tradeoffs</li>
    </ul>
  </div>

  <!-- Module 2 -->
  <div class="module-card">
    <div class="module-number">2</div>
    <h3 class="module-title">
      <span class="en-content">Linked Lists</span>
      <span class="zh-content">链表</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Dynamic Linear Data Structures</span>
      <span class="zh-content">动态线性数据结构</span>
    </p>
    <ul class="module-topics">
      <li>Singly Linked Lists</li>
      <li>Doubly Linked Lists</li>
      <li>Circular Linked Lists</li>
      <li>Operations & Applications</li>
    </ul>
  </div>

  <!-- Module 3 -->
  <div class="module-card">
    <div class="module-number">3</div>
    <h3 class="module-title">
      <span class="en-content">Stacks</span>
      <span class="zh-content">栈</span>
    </h3>
    <p class="module-content">
      <span class="en-content">LIFO Data Structure</span>
      <span class="zh-content">后进先出数据结构</span>
    </p>
    <ul class="module-topics">
      <li>Array & Linked List Implementation</li>
      <li>Expression Evaluation</li>
      <li>Backtracking Applications</li>
      <li>Function Call Stack</li>
    </ul>
  </div>

  <!-- Module 4 -->
  <div class="module-card">
    <div class="module-number">4</div>
    <h3 class="module-title">
      <span class="en-content">Queues</span>
      <span class="zh-content">队列</span>
    </h3>
    <p class="module-content">
      <span class="en-content">FIFO Data Structure</span>
      <span class="zh-content">先进先出数据结构</span>
    </p>
    <ul class="module-topics">
      <li>Circular Queue</li>
      <li>Priority Queue</li>
      <li>Deque (Double-ended Queue)</li>
      <li>BFS Applications</li>
    </ul>
  </div>

  <!-- Module 5 -->
  <div class="module-card">
    <div class="module-number">5</div>
    <h3 class="module-title">
      <span class="en-content">Recursion</span>
      <span class="zh-content">递归</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Problem-solving Technique</span>
      <span class="zh-content">问题解决技术</span>
    </p>
    <ul class="module-topics">
      <li>Base Cases & Recursive Cases</li>
      <li>Tail Recursion</li>
      <li>Tree & Graph Traversals</li>
      <li>Dynamic Programming Intro</li>
    </ul>
  </div>

  <!-- Module 6 -->
  <div class="module-card">
    <div class="module-number">6</div>
    <h3 class="module-title">
      <span class="en-content">Binary Trees</span>
      <span class="zh-content">二叉树</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Hierarchical Data Structure</span>
      <span class="zh-content">层次数据结构</span>
    </p>
    <ul class="module-topics">
      <li>Tree Traversals (In, Pre, Post, Level)</li>
      <li>Binary Search Trees</li>
      <li>Tree Construction & Manipulation</li>
      <li>Applications in Searching</li>
    </ul>
  </div>

  <!-- Module 7 -->
  <div class="module-card">
    <div class="module-number">7</div>
    <h3 class="module-title">
      <span class="en-content">Balanced Trees</span>
      <span class="zh-content">平衡树</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Self-balancing Tree Structures</span>
      <span class="zh-content">自平衡树结构</span>
    </p>
    <ul class="module-topics">
      <li>AVL Trees</li>
      <li>Red-Black Trees</li>
      <li>B-Trees and B+ Trees</li>
      <li>Rotation Operations</li>
    </ul>
  </div>

  <!-- Module 8 -->
  <div class="module-card">
    <div class="module-number">8</div>
    <h3 class="module-title">
      <span class="en-content">Search & Hash Tables</span>
      <span class="zh-content">搜索与哈希表</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Efficient Data Retrieval</span>
      <span class="zh-content">高效数据检索</span>
    </p>
    <ul class="module-topics">
      <li>Linear & Binary Search</li>
      <li>Hash Functions</li>
      <li>Collision Resolution</li>
      <li>HashMaps & HashSets</li>
    </ul>
  </div>

  <!-- Module 9 -->
  <div class="module-card">
    <div class="module-number">9</div>
    <h3 class="module-title">
      <span class="en-content">Sorting Algorithms</span>
      <span class="zh-content">排序算法</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Ordering Data Efficiently</span>
      <span class="zh-content">高效数据排序</span>
    </p>
    <ul class="module-topics">
      <li>Bubble, Selection, Insertion Sort</li>
      <li>Merge Sort & Quick Sort</li>
      <li>Heap Sort & Radix Sort</li>
      <li>Stability & In-place Sorting</li>
    </ul>
  </div>

  <!-- Module 10 -->
  <div class="module-card">
    <div class="module-number">10</div>
    <h3 class="module-title">
      <span class="en-content">Graphs</span>
      <span class="zh-content">图</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Network Data Structures</span>
      <span class="zh-content">网络数据结构</span>
    </p>
    <ul class="module-topics">
      <li>Adjacency Matrix & List</li>
      <li>DFS & BFS Traversal</li>
      <li>Shortest Path Algorithms</li>
      <li>Minimum Spanning Trees</li>
    </ul>
  </div>

  <!-- Module 11 -->
  <div class="module-card">
    <div class="module-number">11</div>
    <h3 class="module-title">
      <span class="en-content">Java API Data Structures</span>
      <span class="zh-content">Java API 数据结构</span>
    </h3>
    <p class="module-content">
      <span class="en-content">Built-in Java Collections</span>
      <span class="zh-content">Java内置集合</span>
    </p>
    <ul class="module-topics">
      <li>ArrayList & LinkedList</li>
      <li>HashSet & TreeSet</li>
      <li>HashMap & TreeMap</li>
      <li>PriorityQueue & ArrayDeque</li>
    </ul>
  </div>
</div>

<!-- Learning Outcomes -->
<div class="outcomes-section">
  <h2 class="outcomes-title">
    <span class="en-content">🎯 Learning Outcomes</span>
    <span class="zh-content">🎯 学习成果</span>
  </h2>
  <ul class="outcomes-list">
    <li>
      <span class="en-content">Master fundamental data structures and their implementations</span>
      <span class="zh-content">掌握基础数据结构及其实现</span>
    </li>
    <li>
      <span class="en-content">Analyze time and space complexity of algorithms</span>
      <span class="zh-content">分析算法的时间和空间复杂度</span>
    </li>
    <li>
      <span class="en-content">Choose appropriate data structures for specific problems</span>
      <span class="zh-content">为特定问题选择合适的数据结构</span>
    </li>
    <li>
      <span class="en-content">Implement data structures from scratch in Java/Python</span>
      <span class="zh-content">在Java/Python中从零实现数据结构</span>
    </li>
    <li>
      <span class="en-content">Solve complex problems using advanced data structures</span>
      <span class="zh-content">使用高级数据结构解决复杂问题</span>
    </li>
    <li>
      <span class="en-content">Prepare for technical interviews and competitions</span>
      <span class="zh-content">为技术面试和竞赛做准备</span>
    </li>
  </ul>
</div>

<!-- Java API Section -->
<div class="api-section">
  <h3 style="color: #92400E; margin-bottom: 1rem;">
    <span class="en-content">💡 Special Focus: Java Collections Framework</span>
    <span class="zh-content">💡 特别关注：Java集合框架</span>
  </h3>
  <p style="color: #78350F; line-height: 1.6;">
    <span class="en-content">
      Learn how to effectively use Java's built-in data structures including ArrayList, LinkedList, HashMap, TreeMap, 
      HashSet, TreeSet, PriorityQueue, and more. Understand when to use each structure for optimal performance.
    </span>
    <span class="zh-content">
      学习如何有效使用Java的内置数据结构，包括ArrayList、LinkedList、HashMap、TreeMap、
      HashSet、TreeSet、PriorityQueue等。了解何时使用每种结构以获得最佳性能。
    </span>
  </p>
</div>

<!-- CTA Section -->
<div class="cta-section">
  <h2 class="cta-title">
    <span class="en-content">Master Data Structures Today!</span>
    <span class="zh-content">今天就掌握数据结构！</span>
  </h2>
  <p style="color: white;">
    <span class="en-content">Build a strong foundation for your programming career</span>
    <span class="zh-content">为您的编程生涯打下坚实基础</span>
  </p>
  <a href="../aicoding/contact.html" class="cta-button">
    <span class="en-content">Enroll Now</span>
    <span class="zh-content">立即报名</span>
  </a>
</div>
