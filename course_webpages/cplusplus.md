---
layout: default
title: C++ Fundamental I & II
title_zh: C++ 基础 I & II
description: Master System Programming with C++
description_zh: 掌握C++系统编程
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

  @keyframes gearRotate {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(15deg); }
  }

  @keyframes binaryFlow {
    0% { transform: translateY(100%); opacity: 0; }
    10% { opacity: 1; }
    90% { opacity: 1; }
    100% { transform: translateY(-100%); opacity: 0; }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #0EA5E9 0%, #2563EB 25%, #3B82F6 50%, #60A5FA 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(14, 165, 233, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '⚙️';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: gearRotate 8s ease-in-out infinite;
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

  /* C++ code snippets floating */
  .code-float {
    position: absolute;
    font-family: 'Courier New', monospace;
    color: rgba(255, 255, 255, 0.15);
    font-size: 0.9rem;
    animation: float 10s ease-in-out infinite;
  }

  .code-float:nth-child(1) { left: 10%; top: 20%; animation-delay: 0s; }
  .code-float:nth-child(2) { right: 10%; top: 30%; animation-delay: 2s; }
  .code-float:nth-child(3) { left: 15%; bottom: 30%; animation-delay: 4s; }
  .code-float:nth-child(4) { right: 15%; bottom: 20%; animation-delay: 6s; }

  /* Binary numbers flowing */
  .binary-bg {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .binary {
    position: absolute;
    font-family: 'Courier New', monospace;
    color: rgba(255, 255, 255, 0.1);
    font-size: 1.2rem;
    animation: binaryFlow 15s linear infinite;
  }

  .binary:nth-child(1) { left: 5%; animation-delay: 0s; }
  .binary:nth-child(2) { left: 25%; animation-delay: 3s; }
  .binary:nth-child(3) { left: 45%; animation-delay: 6s; }
  .binary:nth-child(4) { left: 65%; animation-delay: 9s; }
  .binary:nth-child(5) { left: 85%; animation-delay: 12s; }

  .course-hero h1 {
    font-size: 4rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    position: relative;
    z-index: 1;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    animation: slideIn 1s ease-out;
  }

  .course-hero p {
    font-size: 1.5rem;
    opacity: 0.95;
    position: relative;
    z-index: 1;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    animation: slideIn 1s ease-out 0.2s backwards;
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
    background: linear-gradient(90deg, transparent, rgba(14, 165, 233, 0.05), transparent);
    animation: shimmer 4s infinite;
  }

  .section-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0EA5E9 0%, #2563EB 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 3px solid transparent;
    border-image: linear-gradient(90deg, #0EA5E9, #2563EB) 1;
    position: relative;
  }

  /* Info Bar */
  .info-bar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 3rem 0;
    background: linear-gradient(135deg, #EFF6FF 0%, #DBEAFE 100%);
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(14, 165, 233, 0.1);
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

  /* Curriculum Cards */
  .curriculum-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin-top: 2rem;
  }

  @media (max-width: 968px) {
    .curriculum-grid {
      grid-template-columns: 1fr;
    }
  }

  .curriculum-card {
    background: white;
    padding: 2.5rem;
    border-radius: 20px;
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border-top: 4px solid;
  }

  .fundamentals-card {
    border-top-color: #0EA5E9;
  }

  .advanced-card {
    border-top-color: #2563EB;
  }

  .curriculum-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(14, 165, 233, 0.08), transparent);
    transition: left 0.6s;
  }

  .curriculum-card:hover::before {
    left: 100%;
  }

  .curriculum-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 50px rgba(14, 165, 233, 0.2);
  }

  .card-title {
    font-size: 1.6rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .fundamentals-card .card-title {
    color: #0EA5E9;
  }

  .advanced-card .card-title {
    color: #2563EB;
  }

  .topic-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .topic-item {
    padding: 1.2rem;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    border-radius: 12px;
    border-left: 3px solid #0EA5E9;
    transition: all 0.3s ease;
  }

  .topic-item:hover {
    transform: translateX(8px);
    box-shadow: 0 5px 15px rgba(14, 165, 233, 0.1);
    background: linear-gradient(135deg, #EFF6FF 0%, #DBEAFE 100%);
  }

  .topic-title {
    font-weight: 700;
    color: #1E293B;
    margin-bottom: 0.3rem;
    font-size: 1.1rem;
  }

  .topic-desc {
    color: #64748B;
    font-size: 0.9rem;
  }

  /* Why C++ Section */
  .why-section {
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .why-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(14, 165, 233, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(37, 99, 235, 0.05), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .why-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1200px) {
    .why-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .why-grid {
      grid-template-columns: 1fr;
    }
  }

  .why-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
    position: relative;
    overflow: hidden;
  }

  .why-card::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(14, 165, 233, 0.1) 0%, transparent 60%);
    opacity: 0;
    transition: opacity 0.4s;
  }

  .why-card:hover::after {
    opacity: 1;
    animation: rotateGlow 4s linear infinite;
  }

  .why-card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 20px 40px rgba(14, 165, 233, 0.2);
    border-color: #0EA5E9;
  }

  .why-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    display: inline-block;
    animation: float 6s ease-in-out infinite;
  }

  .why-card:nth-child(1) .why-icon { animation-delay: 0s; }
  .why-card:nth-child(2) .why-icon { animation-delay: 1s; }
  .why-card:nth-child(3) .why-icon { animation-delay: 2s; }
  .why-card:nth-child(4) .why-icon { animation-delay: 3s; }

  .why-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1E293B;
    margin-bottom: 0.5rem;
  }

  .why-desc {
    color: #64748B;
    font-size: 0.95rem;
    line-height: 1.5;
  }

  /* Learning Outcomes */
  .outcomes-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 1200px) {
    .outcomes-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .outcomes-grid {
      grid-template-columns: 1fr;
    }
  }

  .outcome-card {
    background: linear-gradient(135deg, #0EA5E9 0%, #2563EB 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    color: white;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(14, 165, 233, 0.3);
  }

  .outcome-card::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 60%);
    opacity: 0;
    transition: opacity 0.4s;
  }

  .outcome-card:hover::before {
    opacity: 1;
    animation: rotateGlow 4s linear infinite;
  }

  .outcome-card:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 20px 40px rgba(14, 165, 233, 0.4);
  }

  .outcome-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    animation: float 6s ease-in-out infinite;
  }

  .outcome-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: white !important;
    margin-bottom: 0.5rem;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  .outcome-desc {
    font-size: 0.95rem;
    color: rgba(255, 255, 255, 0.9);
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
    background: linear-gradient(135deg, #EFF6FF 0%, #DBEAFE 100%);
    border-radius: 15px;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    border-left: 3px solid #0EA5E9;
  }

  .prereq-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(14, 165, 233, 0.1);
    background: white;
  }

  .prereq-list li::before {
    content: '✨';
    margin-right: 1rem;
    font-size: 1.2rem;
    animation: pulse 2s ease-in-out infinite;
  }

  .enroll-box {
    background: linear-gradient(135deg, #0EA5E9 0%, #2563EB 25%, #3B82F6 50%, #60A5FA 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(14, 165, 233, 0.3);
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
    color: #0EA5E9;
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
    background: linear-gradient(90deg, transparent, rgba(14, 165, 233, 0.2), transparent);
    transition: left 0.5s;
  }

  .enroll-button:hover::before {
    left: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #2563EB;
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
  <div class="binary-bg">
    <span class="binary">101010</span>
    <span class="binary">110011</span>
    <span class="binary">100101</span>
    <span class="binary">111000</span>
    <span class="binary">010110</span>
  </div>
  <div class="code-float">#include &lt;iostream&gt;</div>
  <div class="code-float">using namespace std;</div>
  <div class="code-float">int main() {</div>
  <div class="code-float">vector&lt;int&gt; nums;</div>
  <h1>
    <span class="en-content">C++ Fundamental I & II</span>
    <span class="zh-content">C++ 基础 I & II</span>
  </h1>
  <p>
    <span class="en-content">System Programming & High Performance Computing</span>
    <span class="zh-content">系统编程与高性能计算</span>
  </p>
</div>

<div class="course-container">
  <!-- Course Overview -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">⚙️ Program Overview</span>
      <span class="zh-content">⚙️ 课程概述</span>
    </h2>
    <p style="color: #4B5563; line-height: 1.8; font-size: 1.1rem;">
      <span class="en-content">
        Master C++ programming for competitive programming and system-level development. This 40-hour intensive course covers everything from basic syntax to advanced STL usage, preparing students for USACO Gold/Platinum competitions, game development, and high-performance computing. Learn the language that powers operating systems, game engines, and performance-critical applications.
      </span>
      <span class="zh-content">
        掌握C++编程，用于竞赛编程和系统级开发。这个40小时的密集课程涵盖从基本语法到高级STL使用的所有内容，为学生准备USACO金牌/白金竞赛、游戏开发和高性能计算。学习驱动操作系统、游戏引擎和性能关键应用程序的语言。
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
      <div class="info-bar-icon">👥</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Age Group</span><span class="zh-content">年龄组</span></h4>
        <p>12-18 Years</p>
      </div>
    </div>
    
    <div class="info-bar-item">
      <div class="info-bar-icon">📊</div>
      <div class="info-bar-content">
        <h4><span class="en-content">Level</span><span class="zh-content">级别</span></h4>
        <p>Beginner to Advanced</p>
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

  <!-- Comprehensive Curriculum -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">📚 Comprehensive Curriculum</span>
      <span class="zh-content">📚 完整课程大纲</span>
    </h2>
    
    <div class="curriculum-grid">
      <!-- Core Fundamentals -->
      <div class="curriculum-card fundamentals-card">
        <h3 class="card-title">
          <span>📘</span>
          <span class="en-content">Core Fundamentals</span>
          <span class="zh-content">核心基础</span>
        </h3>
        <ul class="topic-list">
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">1. Variables & I/O</span>
                <span class="zh-content">1. 变量与输入输出</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Input/output streams, sequential programming</span>
                <span class="zh-content">输入输出流，顺序编程</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">2. Control Flow</span>
                <span class="zh-content">2. 控制流</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">If statements and conditional logic</span>
                <span class="zh-content">If语句和条件逻辑</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">3. Iterations</span>
                <span class="zh-content">3. 迭代</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Loops and iteration patterns</span>
                <span class="zh-content">循环和迭代模式</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">4. Arrays & Strings</span>
                <span class="zh-content">4. 数组与字符串</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Data storage and manipulation</span>
                <span class="zh-content">数据存储和操作</span>
              </div>
            </div>
          </li>
        </ul>
      </div>
      
      <!-- Advanced Topics -->
      <div class="curriculum-card advanced-card">
        <h3 class="card-title">
          <span>🚀</span>
          <span class="en-content">Advanced Topics</span>
          <span class="zh-content">高级主题</span>
        </h3>
        <ul class="topic-list">
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">5. Functions</span>
                <span class="zh-content">5. 函数</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Modular programming and recursion</span>
                <span class="zh-content">模块化编程和递归</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">6. OOP Concepts</span>
                <span class="zh-content">6. 面向对象概念</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Structs, classes, and objects</span>
                <span class="zh-content">结构体、类和对象</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">7. Pointers & References</span>
                <span class="zh-content">7. 指针与引用</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Memory management and optimization</span>
                <span class="zh-content">内存管理和优化</span>
              </div>
            </div>
          </li>
          <li class="topic-item">
            <div>
              <div class="topic-title">
                <span class="en-content">8. STL & Algorithms</span>
                <span class="zh-content">8. STL与算法</span>
              </div>
              <div class="topic-desc">
                <span class="en-content">Containers, iterators, algorithms</span>
                <span class="zh-content">容器、迭代器、算法</span>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Learning Outcomes -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">🎯 Learning Outcomes</span>
      <span class="zh-content">🎯 学习成果</span>
    </h2>
    
    <div class="outcomes-grid">
      <div class="outcome-card">
        <div class="outcome-icon">⚡</div>
        <div class="outcome-title">
          <span class="en-content">Performance Master</span>
          <span class="zh-content">性能大师</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Write optimized code</span>
          <span class="zh-content">编写优化代码</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">🏆</div>
        <div class="outcome-title">
          <span class="en-content">USACO Ready</span>
          <span class="zh-content">USACO 准备</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Gold/Platinum level</span>
          <span class="zh-content">金牌/白金级别</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">🎮</div>
        <div class="outcome-title">
          <span class="en-content">Game Dev Skills</span>
          <span class="zh-content">游戏开发技能</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Engine programming basics</span>
          <span class="zh-content">引擎编程基础</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">💻</div>
        <div class="outcome-title">
          <span class="en-content">System Programming</span>
          <span class="zh-content">系统编程</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Low-level development</span>
          <span class="zh-content">底层开发</span>
        </div>
      </div>
    </div>
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
          <span class="en-content">Basic programming concepts</span>
          <span class="zh-content">基本编程概念</span>
        </li>
        <li>
          <span class="en-content">Strong math foundation</span>
          <span class="zh-content">扎实的数学基础</span>
        </li>
        <li>
          <span class="en-content">Problem-solving skills</span>
          <span class="zh-content">问题解决能力</span>
        </li>
      </ul>
    </div>

    <div class="enroll-box">
      <div class="enroll-content">
        <h2 class="enroll-title">
          <span class="en-content">Master C++ Today</span>
          <span class="zh-content">今天掌握C++</span>
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

<!-- Why Learn C++ -->
<div class="why-section">
  <h2 class="section-title" style="text-align: center; margin-bottom: 3rem;">
    <span class="en-content">Why Learn C++?</span>
    <span class="zh-content">为什么学习C++？</span>
  </h2>
  
  <div class="why-grid">
    <div class="why-card">
      <div class="why-icon">⚡</div>
      <h4 class="why-title">
        <span class="en-content">High Performance</span>
        <span class="zh-content">高性能</span>
      </h4>
      <p class="why-desc">
        <span class="en-content">Fastest execution for competitive programming</span>
        <span class="zh-content">竞赛编程中最快的执行速度</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">🎮</div>
      <h4 class="why-title">
        <span class="en-content">Game Development</span>
        <span class="zh-content">游戏开发</span>
      </h4>
      <p class="why-desc">
        <span class="en-content">Industry standard for AAA game engines</span>
        <span class="zh-content">3A游戏引擎的行业标准</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">🏆</div>
      <h4 class="why-title">
        <span class="en-content">USACO Excellence</span>
        <span class="zh-content">USACO 卓越</span>
      </h4>
      <p class="why-desc">
        <span class="en-content">Preferred language for Gold/Platinum levels</span>
        <span class="zh-content">金牌/白金级别的首选语言</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">💻</div>
      <h4 class="why-title">
        <span class="en-content">System Programming</span>
        <span class="zh-content">系统编程</span>
      </h4>
      <p class="why-desc">
        <span class="en-content">Operating systems and embedded systems</span>
        <span class="zh-content">操作系统和嵌入式系统</span>
      </p>
    </div>
  </div>
</div>
