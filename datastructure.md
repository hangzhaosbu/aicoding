---
layout: default
title: Data Structures Course
title_zh: 数据结构课程
description: Master Fundamental Data Structures for Programming Excellence
description_zh: 掌握基础数据结构，实现编程卓越
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

  @keyframes dataFlow {
    0% { transform: translateY(100%) rotate(-15deg); opacity: 0; }
    10% { opacity: 0.1; }
    90% { opacity: 0.1; }
    100% { transform: translateY(-100%) rotate(-10deg); opacity: 0; }
  }

  @keyframes nodeConnect {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 25%, #8B5CF6 50%, #EC4899 100%);
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
    content: '🗂️';
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

  /* Data structure nodes floating */
  .data-nodes {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .node {
    position: absolute;
    font-size: 1.5rem;
    opacity: 0.15;
    animation: dataFlow 20s linear infinite;
  }

  .node:nth-child(1) { left: 10%; animation-delay: 0s; }
  .node:nth-child(2) { left: 30%; animation-delay: 4s; }
  .node:nth-child(3) { left: 50%; animation-delay: 8s; }
  .node:nth-child(4) { left: 70%; animation-delay: 12s; }
  .node:nth-child(5) { left: 90%; animation-delay: 16s; }

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
    background: linear-gradient(135deg, #F0FDFA 0%, #E0F2FE 100%);
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(6, 182, 212, 0.1);
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
    color: #0E7490;
    margin-bottom: 0.3rem;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    font-weight: 600;
  }

  .info-bar-content p {
    font-size: 1.2rem;
    color: #0C4A6E;
    font-weight: 700;
  }

  /* Module Cards - Premium Grid */
  .modules-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin: 3rem 0;
  }

  @media (max-width: 1200px) {
    .modules-container {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .modules-container {
      grid-template-columns: 1fr;
    }
  }

  .module-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    border-left: 5px solid;
    border-image: linear-gradient(180deg, #06B6D4, #3B82F6) 1;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out backwards;
  }

  .module-card:nth-child(1) { animation-delay: 0.1s; }
  .module-card:nth-child(2) { animation-delay: 0.15s; }
  .module-card:nth-child(3) { animation-delay: 0.2s; }
  .module-card:nth-child(4) { animation-delay: 0.25s; }
  .module-card:nth-child(5) { animation-delay: 0.3s; }
  .module-card:nth-child(6) { animation-delay: 0.35s; }
  .module-card:nth-child(7) { animation-delay: 0.4s; }
  .module-card:nth-child(8) { animation-delay: 0.45s; }
  .module-card:nth-child(9) { animation-delay: 0.5s; }
  .module-card:nth-child(10) { animation-delay: 0.55s; }
  .module-card:nth-child(11) { animation-delay: 0.6s; }
  .module-card:nth-child(12) { animation-delay: 0.65s; }

  .module-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(6, 182, 212, 0.08), transparent);
    transition: left 0.6s;
  }

  .module-card:hover::before {
    left: 100%;
  }

  .module-card:hover {
    transform: translateY(-8px) scale(1.02);
    box-shadow: 0 20px 40px rgba(6, 182, 212, 0.15);
  }

  .module-number {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);
    color: white;
    width: 50px;
    height: 50px;
    border-radius: 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    font-size: 1.3rem;
    margin-bottom: 1.2rem;
    animation: nodeConnect 3s ease-in-out infinite;
    box-shadow: 0 5px 15px rgba(6, 182, 212, 0.3);
  }

  .module-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #0C4A6E;
    margin-bottom: 0.8rem;
  }

  .module-content {
    color: #64748B;
    line-height: 1.6;
    font-size: 1rem;
    margin-bottom: 1rem;
  }

  .module-topics {
    list-style: none;
    padding: 0;
    margin-top: 1rem;
  }

  .module-topics li {
    padding: 0.5rem 0;
    color: #475569;
    font-size: 0.9rem;
    display: flex;
    align-items: flex-start;
    transition: all 0.3s ease;
  }

  .module-topics li:hover {
    padding-left: 0.5rem;
    color: #0C4A6E;
  }

  .module-topics li::before {
    content: '→';
    color: #06B6D4;
    font-weight: bold;
    margin-right: 0.8rem;
    flex-shrink: 0;
  }

  /* Learning Outcomes - Premium */
  .outcomes-section {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(16, 185, 129, 0.1);
  }

  .outcomes-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(16, 185, 129, 0.08), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .outcomes-title {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .outcomes-list {
    list-style: none;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 768px) {
    .outcomes-list {
      grid-template-columns: 1fr;
    }
  }

  .outcomes-list li {
    padding: 1.5rem;
    background: white;
    border-radius: 15px;
    display: flex;
    align-items: flex-start;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease;
    border-left: 3px solid #10B981;
  }

  .outcomes-list li:hover {
    transform: translateX(10px);
    box-shadow: 0 10px 25px rgba(16, 185, 129, 0.15);
  }

  .outcomes-list li::before {
    content: '✨';
    color: #10B981;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 1.3rem;
    flex-shrink: 0;
    animation: pulse 2s ease-in-out infinite;
  }

  /* Java API Section - Premium */
  .api-section {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
    padding: 3rem;
    border-radius: 25px;
    margin: 3rem 0;
    border-left: 5px solid #F59E0B;
    box-shadow: 0 15px 35px rgba(245, 158, 11, 0.15);
    position: relative;
    overflow: hidden;
  }

  .api-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(245, 158, 11, 0.1), transparent);
    animation: shimmer 4s infinite;
  }

  .api-section h3 {
    color: #92400E;
    font-size: 1.6rem;
    font-weight: 700;
    margin-bottom: 1.2rem;
  }

  .api-section p {
    color: #78350F;
    line-height: 1.8;
    font-size: 1.05rem;
  }

  /* Prerequisites and Enrollment */
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

  .prereq-section {
    background: white;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.5);
  }

  .prereq-list {
    list-style: none;
    margin-top: 1.5rem;
    padding: 0;
  }

  .prereq-list li {
    padding: 1rem;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #F0FDFA 0%, #E0F2FE 100%);
    border-radius: 15px;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    border-left: 3px solid #06B6D4;
  }

  .prereq-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(6, 182, 212, 0.1);
    background: white;
  }

  .prereq-list li::before {
    content: '✨';
    margin-right: 1rem;
    font-size: 1.2rem;
    animation: pulse 2s ease-in-out infinite;
  }

  .enroll-box {
    background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 25%, #8B5CF6 50%, #EC4899 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(6, 182, 212, 0.3);
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
    color: #06B6D4;
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
    background: linear-gradient(90deg, transparent, rgba(6, 182, 212, 0.2), transparent);
    transition: left 0.5s;
  }

  .enroll-button:hover::before {
    left: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #3B82F6;
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
  <div class="data-nodes">
    <span class="node">[ ]→[ ]→[ ]</span>
    <span class="node">🌳</span>
    <span class="node">{ }</span>
    <span class="node">⟨⟩</span>
    <span class="node">▣</span>
  </div>
  <h1>
    <span class="en-content">Data Structures Mastery</span>
    <span class="zh-content">数据结构精通课程</span>
  </h1>
  <p>
    <span class="en-content">Build Strong Foundation for Advanced Programming</span>
    <span class="zh-content">为高级编程打下坚实基础</span>
  </p>
</div>

<div class="course-container">
  <!-- Course Overview -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">📊 Course Overview</span>
      <span class="zh-content">📊 课程概述</span>
    </h2>
    <p style="color: #4B5563; line-height: 1.8; font-size: 1.1rem;">
      <span class="en-content">
        Master the fundamental data structures that form the backbone of computer science and software engineering. 
        This comprehensive 40-hour course covers everything from basic linear structures to advanced trees and graphs, 
        preparing you for technical interviews at top tech companies, competitive programming contests like USACO, 
        and real-world software development challenges. Learn to analyze complexity, implement from scratch, and 
        choose the optimal data structure for any problem.
      </span>
      <span class="zh-content">
        掌握构成计算机科学和软件工程支柱的基础数据结构。这门40小时的综合课程涵盖了从基本线性结构到高级树和图的所有内容，
        为您准备顶级科技公司的技术面试、USACO等竞赛编程比赛，以及实际软件开发挑战。学习分析复杂度、从零实现，
        并为任何问题选择最优的数据结构。
      </span>
    </p>
  </div>

  <!-- Course Info Bar -->
  <div class="info-bar">
    <div class="info-bar-item">
      <div class="info-bar-icon">⏱️</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Duration</span><span class="zh-content">课程时长</span></h4>
        <p>40 Hours</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">📊</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Level</span><span class="zh-content">级别</span></h4>
        <p>Intermediate</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">💻</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Languages</span><span class="zh-content">编程语言</span></h4>
        <p>Java/Python</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">🏫</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Class Size</span><span class="zh-content">班级规模</span></h4>
        <p>1-on-1 or Max 4</p>
      </div>
    </div>
  </div>

  <!-- Detailed Curriculum -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">📚 Detailed Curriculum</span>
      <span class="zh-content">📚 详细课程大纲</span>
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
          <span class="en-content">Hash Tables</span>
          <span class="zh-content">哈希表</span>
        </h3>
        <p class="module-content">
          <span class="en-content">Efficient Data Retrieval</span>
          <span class="zh-content">高效数据检索</span>
        </p>
        <ul class="module-topics">
          <li>Hash Functions</li>
          <li>Collision Resolution</li>
          <li>HashMaps & HashSets</li>
          <li>Load Factor & Rehashing</li>
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
          <span class="en-content">Java Collections</span>
          <span class="zh-content">Java 集合框架</span>
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

      <!-- Module 12 -->
      <div class="module-card">
        <div class="module-number">12</div>
        <h3 class="module-title">
          <span class="en-content">Advanced Topics</span>
          <span class="zh-content">高级主题</span>
        </h3>
        <p class="module-content">
          <span class="en-content">Real-world Applications</span>
          <span class="zh-content">实际应用</span>
        </p>
        <ul class="module-topics">
          <li>Trie (Prefix Tree)</li>
          <li>Disjoint Set Union</li>
          <li>Segment Trees</li>
          <li>LRU Cache Design</li>
          <li>System Design Applications</li>
        </ul>
      </div>
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
    <h3>
      <span class="en-content">💡 Special Focus: Java Collections Framework</span>
      <span class="zh-content">💡 特别关注：Java集合框架</span>
    </h3>
    <p>
      <span class="en-content">
        Learn how to effectively use Java's built-in data structures including ArrayList, LinkedList, HashMap, TreeMap, 
        HashSet, TreeSet, PriorityQueue, and more. Understand when to use each structure for optimal performance 
        in real-world applications and competitive programming.
      </span>
      <span class="zh-content">
        学习如何有效使用Java的内置数据结构，包括ArrayList、LinkedList、HashMap、TreeMap、
        HashSet、TreeSet、PriorityQueue等。了解何时使用每种结构以在实际应用和竞赛编程中获得最佳性能。
      </span>
    </p>
  </div>

  <!-- Prerequisites & Enrollment -->
  <div class="prereq-enroll-grid">
    <div class="prereq-section">
      <h2 class="section-title">
        <span class="en-content">📋 Prerequisites</span>
        <span class="zh-content">📋 先修要求</span>
      </h2>
      <ul class="prereq-list">
        <li>
          <span class="en-content">Basic programming in Java or Python</span>
          <span class="zh-content">Java或Python基础编程</span>
        </li>
        <li>
          <span class="en-content">Understanding of loops and functions</span>
          <span class="zh-content">理解循环和函数</span>
        </li>
        <li>
          <span class="en-content">Basic math and logic skills</span>
          <span class="zh-content">基础数学和逻辑能力</span>
        </li>
      </ul>
    </div>

    <div class="enroll-box">
      <div class="enroll-content">
        <h2 class="enroll-title">
          <span class="en-content">Master Data Structures</span>
          <span class="zh-content">掌握数据结构</span>
        </h2>
        <a href="./contact.html" class="enroll-button">
          <span class="en-content">Enroll Now</span>
          <span class="zh-content">立即报名</span>
        </a>
        <p class="enroll-subtitle">
          <span class="en-content">✨ Free consultation & assessment</span>
          <span class="zh-content">✨ 免费咨询和评估</span>
        </p>
      </div>
    </div>
  </div>
</div>
