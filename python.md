---
layout: default
title: Python Fundamental I & II
description: Complete Python Programming Journey from Basics to Advanced
---

<style>
  /* Course Hero Section */
  .course-hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    padding: 4rem 2rem;
    border-radius: 20px;
    color: white;
    text-align: center;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .course-hero::before {
    content: '🐍';
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

  /* Course Info Grid */
  .course-info-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 2rem;
    margin-bottom: 3rem;
  }

  /* Course Content Section */
  .course-content-section {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 1px solid #E5E7EB;
  }

  .section-title {
    font-size: 1.8rem;
    color: #1F2937;
    margin-bottom: 1.5rem;
    padding-bottom: 0.5rem;
    border-bottom: 3px solid #4F46E5;
  }

  /* Syllabus */
  .syllabus-module {
    background: #F9FAFB;
    padding: 1.5rem;
    border-radius: 10px;
    margin-bottom: 1rem;
    border-left: 4px solid #4F46E5;
  }

  .module-title {
    font-size: 1.2rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .module-topics {
    list-style: none;
    margin-top: 1rem;
  }

  .module-topics li {
    padding: 0.5rem 0;
    color: #6B7280;
    display: flex;
    align-items: center;
  }

  .module-topics li::before {
    content: '•';
    color: #4F46E5;
    font-weight: bold;
    margin-right: 0.75rem;
    font-size: 1.2rem;
  }

  /* Course Info Sidebar */
  .course-sidebar {
    position: sticky;
    top: 2rem;
    height: fit-content;
  }

  .info-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 1px solid #E5E7EB;
    margin-bottom: 1.5rem;
  }

  .info-item {
    display: flex;
    align-items: center;
    margin-bottom: 1rem;
    padding: 0.75rem;
    background: #F9FAFB;
    border-radius: 8px;
  }

  .info-item:last-child {
    margin-bottom: 0;
  }

  .info-icon {
    font-size: 1.5rem;
    margin-right: 1rem;
  }

  .info-content h4 {
    font-size: 0.9rem;
    color: #6B7280;
    margin-bottom: 0.25rem;
  }

  .info-content p {
    font-size: 1rem;
    color: #1F2937;
    font-weight: 600;
  }

  /* Enroll Button */
  .enroll-section {
    text-align: center;
    padding: 1.5rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 15px;
    color: white;
  }

  .price {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }

  .enroll-button {
    background: white;
    color: #4F46E5;
    padding: 1rem 2rem;
    border-radius: 10px;
    text-decoration: none;
    display: inline-block;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s;
    width: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  }

  /* Learning Outcomes */
  .outcomes-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin-top: 1.5rem;
  }

  .outcome-card {
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
  }

  .outcome-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .outcome-title {
    font-size: 1.1rem;
    font-weight: 600;
    color: #1F2937;
  }

  /* Prerequisites */
  .prereq-list {
    list-style: none;
    margin-top: 1rem;
  }

  .prereq-list li {
    padding: 0.75rem;
    margin-bottom: 0.5rem;
    background: #F9FAFB;
    border-radius: 8px;
    display: flex;
    align-items: center;
  }

  .prereq-list li::before {
    content: '✅';
    margin-right: 0.75rem;
  }

  /* Responsive */
  @media (max-width: 768px) {
    .course-info-grid {
      grid-template-columns: 1fr;
    }
    
    .course-hero h1 {
      font-size: 2rem;
    }
  }
</style>

<div class="course-hero">
  <h1>
    <span class="en-content">Python Fundamental I & II</span>
    <span class="zh-content">Python 基础 I & II</span>
  </h1>
  <p>
    <span class="en-content">Master Python Programming from Zero to Hero</span>
    <span class="zh-content">从零开始掌握 Python 编程</span>
  </p>
</div>

<div class="course-info-grid">
  <!-- Main Content -->
  <div>
    <!-- Course Overview -->
    <div class="course-content-section">
      <h2 class="section-title">
        <span class="en-content">📘 Course Overview</span>
        <span class="zh-content">📘 课程概述</span>
      </h2>
      <p style="color: #4B5563; line-height: 1.8;">
        <span class="en-content">
          This comprehensive Python programming course is designed to take students from absolute beginners to confident programmers. Through 40 hours of intensive learning, students will master Python fundamentals, data structures, object-oriented programming, and real-world applications.
        </span>
        <span class="zh-content">
          这门综合性的Python编程课程旨在将学生从零基础培养成自信的程序员。通过40小时的密集学习，学生将掌握Python基础知识、数据结构、面向对象编程和实际应用。
        </span>
      </p>
    </div>

    <!-- Detailed Syllabus -->
    <div class="course-content-section" style="margin-top: 2rem;">
      <h2 class="section-title">
        <span class="en-content">📚 Detailed Syllabus</span>
        <span class="zh-content">📚 详细课程大纲</span>
      </h2>
      
      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 1: Getting Started (Hours 1-5)</span>
          <span class="zh-content">模块 1：入门基础（第1-5小时）</span>
        </h3>
        <ul class="module-topics">
          <li>Installing Python and Setting Up Development Environment</li>
          <li>Why Program? Understanding Programming Logic</li>
          <li>Variables, Expressions, and Statements</li>
          <li>Basic Input/Output Operations</li>
          <li>First Python Programs</li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 2: Control Flow (Hours 6-10)</span>
          <span class="zh-content">模块 2：控制流（第6-10小时）</span>
        </h3>
        <ul class="module-topics">
          <li>Conditional Execution (if/elif/else)</li>
          <li>Boolean Expressions and Logic</li>
          <li>Loops and Iterations (for/while)</li>
          <li>Break, Continue, and Pass Statements</li>
          <li>Practice Problems and Exercises</li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 3: Data Structures (Hours 11-20)</span>
          <span class="zh-content">模块 3：数据结构（第11-20小时）</span>
        </h3>
        <ul class="module-topics">
          <li>Strings and String Manipulation</li>
          <li>Lists and List Operations</li>
          <li>Dictionaries and Key-Value Pairs</li>
          <li>Tuples and Sets</li>
          <li>Data Structure Applications</li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 4: Functions & OOP (Hours 21-30)</span>
          <span class="zh-content">模块 4：函数与面向对象（第21-30小时）</span>
        </h3>
        <ul class="module-topics">
          <li>Functions and Parameters</li>
          <li>Return Values and Scope</li>
          <li>Object-Oriented Programming Concepts</li>
          <li>Classes and Objects</li>
          <li>Inheritance and Polymorphism</li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 5: Advanced Topics (Hours 31-40)</span>
          <span class="zh-content">模块 5：高级主题（第31-40小时）</span>
        </h3>
        <ul class="module-topics">
          <li>File Handling and I/O Operations</li>
          <li>Regular Expressions</li>
          <li>Network Programming Basics</li>
          <li>Database Operations</li>
          <li>Data Visualization</li>
          <li>Final Project Development</li>
        </ul>
      </div>
    </div>

    <!-- Learning Outcomes -->
    <div class="course-content-section" style="margin-top: 2rem;">
      <h2 class="section-title">
        <span class="en-content">🎯 Learning Outcomes</span>
        <span class="zh-content">🎯 学习成果</span>
      </h2>
      
      <div class="outcomes-grid">
        <div class="outcome-card">
          <div class="outcome-icon">💻</div>
          <div class="outcome-title">
            <span class="en-content">Write Clean Code</span>
            <span class="zh-content">编写整洁代码</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🔧</div>
          <div class="outcome-title">
            <span class="en-content">Build Real Projects</span>
            <span class="zh-content">构建实际项目</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🧩</div>
          <div class="outcome-title">
            <span class="en-content">Solve Complex Problems</span>
            <span class="zh-content">解决复杂问题</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🚀</div>
          <div class="outcome-title">
            <span class="en-content">Ready for Advanced Topics</span>
            <span class="zh-content">为进阶做准备</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Sidebar -->
  <div class="course-sidebar">
    <!-- Course Info Card -->
    <div class="info-card">
      <h3 style="color: #1F2937; margin-bottom: 1.5rem;">
        <span class="en-content">Course Information</span>
        <span class="zh-content">课程信息</span>
      </h3>
      
      <div class="info-item">
        <div class="info-icon">⏱️</div>
        <div class="info-content">
          <h4>Duration</h4>
          <p>40 Hours</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">👥</div>
        <div class="info-content">
          <h4>Age Group</h4>
          <p>10-18 Years</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">📊</div>
        <div class="info-content">
          <h4>Level</h4>
          <p>Beginner to Intermediate</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">🏫</div>
        <div class="info-content">
          <h4>Class Size</h4>
          <p>1-on-1 or Small Group</p>
        </div>
      </div>
    </div>

    <!-- Prerequisites -->
    <div class="info-card">
      <h3 style="color: #1F2937; margin-bottom: 1rem;">
        <span class="en-content">Prerequisites</span>
        <span class="zh-content">先修要求</span>
      </h3>
      <ul class="prereq-list">
        <li>
          <span class="en-content">Basic computer skills</span>
          <span class="zh-content">基本计算机技能</span>
        </li>
        <li>
          <span class="en-content">Elementary math knowledge</span>
          <span class="zh-content">基础数学知识</span>
        </li>
        <li>
          <span class="en-content">Enthusiasm to learn!</span>
          <span class="zh-content">学习热情！</span>
        </li>
      </ul>
    </div>

    <!-- Enroll Section -->
    <div class="enroll-section">
      <div class="price">
        <span class="en-content">Contact for Pricing</span>
        <span class="zh-content">联系咨询价格</span>
      </div>
      <a href="../aicoding/contact.html" class="enroll-button">
        <span class="en-content">Enroll Now</span>
        <span class="zh-content">立即报名</span>
      </a>
      <p style="margin-top: 1rem; font-size: 0.9rem;">
        <span class="en-content">Free consultation available</span>
        <span class="zh-content">提供免费咨询</span>
      </p>
    </div>
  </div>
</div>
