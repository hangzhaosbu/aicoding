---
layout: default
title: Java Fundamental I & II
title_zh: Java 基础 I & II
description: Master Object-Oriented Programming with Java
description_zh: 掌握Java面向对象编程
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

  @keyframes coffeeFloat {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  @keyframes codeTyping {
    from { width: 0; }
    to { width: 100%; }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #EA580C 0%, #DC2626 25%, #F97316 50%, #FB923C 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(234, 88, 12, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '☕';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: coffeeFloat 6s ease-in-out infinite;
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

  /* Java code snippets floating */
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
    background: linear-gradient(90deg, transparent, rgba(234, 88, 12, 0.05), transparent);
    animation: shimmer 4s infinite;
  }

  .section-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #EA580C 0%, #DC2626 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 3px solid transparent;
    border-image: linear-gradient(90deg, #EA580C, #DC2626) 1;
    position: relative;
  }

  /* Info Bar */
  .info-bar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 3rem 0;
    background: linear-gradient(135deg, #FFF7ED 0%, #FED7AA 100%);
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(234, 88, 12, 0.1);
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
    color: #92400E;
    margin-bottom: 0.3rem;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    font-weight: 600;
  }

  .info-bar-content p {
    font-size: 1.2rem;
    color: #451A03;
    font-weight: 700;
  }

  /* Curriculum Modules */
  .curriculum-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 968px) {
    .curriculum-grid {
      grid-template-columns: 1fr;
    }
  }

  .curriculum-part {
    background: linear-gradient(135deg, #FFF7ED 0%, #FED7AA 100%);
    padding: 2.5rem;
    border-radius: 20px;
    border-left: 5px solid;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .part-1 {
    border-left-color: #EA580C;
  }

  .part-2 {
    border-left-color: #DC2626;
  }

  .curriculum-part::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(234, 88, 12, 0.1), transparent);
    transition: left 0.6s;
  }

  .curriculum-part:hover::before {
    left: 100%;
  }

  .curriculum-part:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 40px rgba(234, 88, 12, 0.15);
    background: white;
  }

  .part-title {
    font-size: 1.5rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
  }

  .part-1 .part-title {
    color: #EA580C;
  }

  .part-2 .part-title {
    color: #DC2626;
  }

  .curriculum-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .curriculum-list li {
    padding: 0.8rem 0;
    color: #6B7280;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    position: relative;
    font-size: 1.05rem;
  }

  .curriculum-list li:hover {
    color: #4B5563;
    padding-left: 0.5rem;
  }

  .curriculum-list li::before {
    content: '→';
    color: #EA580C;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 1rem;
    transition: transform 0.3s;
  }

  .curriculum-list li:hover::before {
    transform: translateX(5px);
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
    background: linear-gradient(135deg, #EA580C 0%, #DC2626 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    color: white;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(234, 88, 12, 0.3);
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
    box-shadow: 0 20px 40px rgba(234, 88, 12, 0.4);
  }

  .outcome-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    animation: float 6s ease-in-out infinite;
  }

  .outcome-card:nth-child(1) .outcome-icon { animation-delay: 0s; }
  .outcome-card:nth-child(2) .outcome-icon { animation-delay: 1s; }
  .outcome-card:nth-child(3) .outcome-icon { animation-delay: 2s; }
  .outcome-card:nth-child(4) .outcome-icon { animation-delay: 3s; }

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
    background: linear-gradient(135deg, #FFF7ED 0%, #FED7AA 100%);
    border-radius: 15px;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    border-left: 3px solid #EA580C;
  }

  .prereq-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(234, 88, 12, 0.1);
    background: white;
  }

  .prereq-list li::before {
    content: '✨';
    margin-right: 1rem;
    font-size: 1.2rem;
    animation: pulse 2s ease-in-out infinite;
  }

  .enroll-box {
    background: linear-gradient(135deg, #EA580C 0%, #DC2626 25%, #F97316 50%, #FB923C 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(234, 88, 12, 0.3);
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
    color: #EA580C;
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
    background: linear-gradient(90deg, transparent, rgba(234, 88, 12, 0.2), transparent);
    transition: left 0.5s;
  }

  .enroll-button:hover::before {
    left: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #DC2626;
  }

  .enroll-subtitle {
    color: white;
    margin-top: 1.5rem;
    font-size: 1.1rem;
    opacity: 0.95;
  }

  /* Features Section */
  .features-section {
    background: linear-gradient(135deg, #FFF7ED 0%, #FED7AA 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem auto;
    max-width: 1400px;
    position: relative;
    overflow: hidden;
  }

  .features-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(234, 88, 12, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(220, 38, 38, 0.05), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin-top: 2rem;
    position: relative;
    z-index: 1;
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

  .feature-box {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
  }

  .feature-box:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 40px rgba(234, 88, 12, 0.2);
    border-color: #EA580C;
  }

  .feature-box-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    display: inline-block;
    animation: float 6s ease-in-out infinite;
  }

  .feature-box-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .feature-box-desc {
    color: #6B7280;
    font-size: 0.95rem;
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
  <div class="code-float">public class Main {</div>
  <div class="code-float">System.out.println();</div>
  <div class="code-float">for(int i=0; i<10; i++)</div>
  <div class="code-float">class Student extends</div>
  <h1>
    <span class="en-content">Java Fundamental I & II</span>
    <span class="zh-content">Java 基础 I & II</span>
  </h1>
  <p>
    <span class="en-content">Master Object-Oriented Programming from Zero to Hero</span>
    <span class="zh-content">从零开始掌握面向对象编程</span>
  </p>
</div>

<div class="course-container">
  <!-- Course Overview -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">☕ Program Overview</span>
      <span class="zh-content">☕ 课程概述</span>
    </h2>
    <p style="color: #4B5563; line-height: 1.8; font-size: 1.1rem;">
      <span class="en-content">
        Master Java programming from fundamentals to advanced concepts in this comprehensive 40-hour course. Designed to take students from complete beginners to confident Java developers, this program covers everything from basic syntax to object-oriented programming, preparing students for AP Computer Science A, USACO competitions, and real-world application development. Our curriculum emphasizes hands-on practice with industry-standard tools and best practices.
      </span>
      <span class="zh-content">
        在这个全面的40小时课程中，从基础到高级概念掌握Java编程。本课程旨在将学生从完全的初学者培养成自信的Java开发者，涵盖从基本语法到面向对象编程的所有内容，为学生准备AP计算机科学A、USACO竞赛和实际应用程序开发。我们的课程强调使用行业标准工具和最佳实践进行实践练习。
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
        <p>11-18 Years</p>
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

  <!-- Complete Curriculum -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">📚 Complete Curriculum</span>
      <span class="zh-content">📚 完整课程大纲</span>
    </h2>
    
    <div class="curriculum-grid">
      <!-- Part I -->
      <div class="curriculum-part part-1">
        <h3 class="part-title">
          <span class="en-content">Part I: Java Foundations (Hours 1-20)</span>
          <span class="zh-content">第一部分：Java 基础（1-20小时）</span>
        </h3>
        <ul class="curriculum-list">
          <li>
            <span class="en-content">Installing Java & IDE Setup (IntelliJ/Eclipse)</span>
            <span class="zh-content">安装Java和IDE设置（IntelliJ/Eclipse）</span>
          </li>
          <li>
            <span class="en-content">Introduction to Programming Logic</span>
            <span class="zh-content">编程逻辑介绍</span>
          </li>
          <li>
            <span class="en-content">Primitive Types & Variables</span>
            <span class="zh-content">原始类型和变量</span>
          </li>
          <li>
            <span class="en-content">Using Objects & Methods</span>
            <span class="zh-content">使用对象和方法</span>
          </li>
          <li>
            <span class="en-content">Boolean Expressions & Conditionals</span>
            <span class="zh-content">布尔表达式和条件语句</span>
          </li>
          <li>
            <span class="en-content">Loops and Iterations</span>
            <span class="zh-content">循环和迭代</span>
          </li>
          <li>
            <span class="en-content">String Manipulation & Processing</span>
            <span class="zh-content">字符串操作和处理</span>
          </li>
          <li>
            <span class="en-content">Methods & Parameters</span>
            <span class="zh-content">方法和参数</span>
          </li>
        </ul>
      </div>
      
      <!-- Part II -->
      <div class="curriculum-part part-2">
        <h3 class="part-title">
          <span class="en-content">Part II: Advanced Concepts (Hours 21-40)</span>
          <span class="zh-content">第二部分：高级概念（21-40小时）</span>
        </h3>
        <ul class="curriculum-list">
          <li>
            <span class="en-content">Writing Classes & Constructors</span>
            <span class="zh-content">编写类和构造函数</span>
          </li>
          <li>
            <span class="en-content">Arrays & Array Operations</span>
            <span class="zh-content">数组和数组操作</span>
          </li>
          <li>
            <span class="en-content">ArrayList & Collections Framework</span>
            <span class="zh-content">ArrayList和集合框架</span>
          </li>
          <li>
            <span class="en-content">2D Arrays & Matrix Operations</span>
            <span class="zh-content">二维数组和矩阵操作</span>
          </li>
          <li>
            <span class="en-content">Inheritance & Polymorphism</span>
            <span class="zh-content">继承和多态</span>
          </li>
          <li>
            <span class="en-content">Abstract Classes & Interfaces</span>
            <span class="zh-content">抽象类和接口</span>
          </li>
          <li>
            <span class="en-content">Recursion & Recursive Algorithms</span>
            <span class="zh-content">递归和递归算法</span>
          </li>
          <li>
            <span class="en-content">Sorting & Searching Algorithms</span>
            <span class="zh-content">排序和搜索算法</span>
          </li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Learning Outcomes -->
  <div class="course-content-section">
    <h2 class="section-title">
      <span class="en-content">🎯 What You'll Achieve</span>
      <span class="zh-content">🎯 学习成果</span>
    </h2>
    
    <div class="outcomes-grid">
      <div class="outcome-card">
        <div class="outcome-icon">🎓</div>
        <div class="outcome-title">
          <span class="en-content">AP Ready</span>
          <span class="zh-content">AP 准备</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Fully prepared for AP CSA exam</span>
          <span class="zh-content">完全准备好AP CSA考试</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">💼</div>
        <div class="outcome-title">
          <span class="en-content">Real Projects</span>
          <span class="zh-content">实际项目</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Build portfolio-worthy apps</span>
          <span class="zh-content">构建作品集级应用</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">🏆</div>
        <div class="outcome-title">
          <span class="en-content">Competition Ready</span>
          <span class="zh-content">竞赛准备</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Prepared for USACO Bronze/Silver</span>
          <span class="zh-content">为USACO铜/银牌准备</span>
        </div>
      </div>
      
      <div class="outcome-card">
        <div class="outcome-icon">🚀</div>
        <div class="outcome-title">
          <span class="en-content">Industry Skills</span>
          <span class="zh-content">行业技能</span>
        </div>
        <div class="outcome-desc">
          <span class="en-content">Professional coding practices</span>
          <span class="zh-content">专业编码实践</span>
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
          <span class="en-content">Basic computer skills</span>
          <span class="zh-content">基本计算机技能</span>
        </li>
        <li>
          <span class="en-content">Algebra fundamentals</span>
          <span class="zh-content">代数基础</span>
        </li>
        <li>
          <span class="en-content">Problem-solving mindset</span>
          <span class="zh-content">问题解决思维</span>
        </li>
      </ul>
    </div>

    <div class="enroll-box">
      <div class="enroll-content">
        <h2 class="enroll-title">
          <span class="en-content">Start Your Java Journey</span>
          <span class="zh-content">开始您的Java之旅</span>
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

<!-- Why Choose This Course -->
<div class="features-section">
  <h2 class="section-title" style="text-align: center; margin-bottom: 3rem;">
    <span class="en-content">Why Choose Our Java Course</span>
    <span class="zh-content">为什么选择我们的Java课程</span>
  </h2>
  
  <div class="features-grid">
    <div class="feature-box">
      <div class="feature-box-icon">🎓</div>
      <div class="feature-box-title">
        <span class="en-content">AP CSA Focus</span>
        <span class="zh-content">AP CSA 重点</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Complete AP exam preparation included</span>
        <span class="zh-content">包含完整的AP考试准备</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">💻</div>
      <div class="feature-box-title">
        <span class="en-content">Project-Based</span>
        <span class="zh-content">项目驱动</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Build 10+ real Java applications</span>
        <span class="zh-content">构建10+个真实Java应用</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">🏆</div>
      <div class="feature-box-title">
        <span class="en-content">Competition Prep</span>
        <span class="zh-content">竞赛准备</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">USACO Bronze/Silver level training</span>
        <span class="zh-content">USACO铜牌/银牌级培训</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">🌟</div>
      <div class="feature-box-title">
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Maximum 4 students per class</span>
        <span class="zh-content">每班最多4名学生</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">📚</div>
      <div class="feature-box-title">
        <span class="en-content">Rich Resources</span>
        <span class="zh-content">丰富资源</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">600+ practice problems & solutions</span>
        <span class="zh-content">600+练习题和解答</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">🔄</div>
      <div class="feature-box-title">
        <span class="en-content">Ongoing Support</span>
        <span class="zh-content">持续支持</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Continuous mentorship after course</span>
        <span class="zh-content">课程结束后持续指导</span>
      </div>
    </div>
  </div>
</div>
