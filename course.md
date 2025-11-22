---
layout: default
title: Our Courses
title_zh: 我们的课程
description: Comprehensive Programming Curriculum for All Levels
description_zh: 全方位编程课程，适合各个水平
---

<style>
  /* 保留您原有的所有样式 */
  .page-header-custom {
    text-align: center;
    margin-bottom: 3rem;
    padding: 2rem 0;
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    border-radius: 15px;
  }

  .page-title {
    font-size: 2.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 1rem;
  }

  .page-description {
    font-size: 1.2rem;
    color: #6B7280;
  }

  .course-category {
    margin-bottom: 4rem;
  }

  .category-title {
    font-size: 1.8rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 2rem;
    padding-bottom: 0.5rem;
    border-bottom: 3px solid #4F46E5;
    display: inline-block;
  }

  .courses-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2.5rem;
    margin-top: 2rem;
  }

  .course-card {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    transition: all 0.3s ease;
    border: 1px solid #E5E7EB;
    display: flex;
    flex-direction: column;
  }

  .course-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
  }

  .course-image {
    width: 100%;
    height: 220px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 4rem;
    color: white;
    position: relative;
  }

  .course-content {
    padding: 1.5rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .course-title {
    font-size: 1.4rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .course-subtitle {
    color: #6B7280;
    font-size: 0.95rem;
    margin-bottom: 1rem;
  }

  .course-features {
    list-style: none;
    margin: 1rem 0;
    flex-grow: 1;
  }

  .course-features li {
    padding: 0.5rem 0;
    color: #4B5563;
    display: flex;
    align-items: center;
  }

  .course-features li::before {
    content: "✓";
    color: #10B981;
    font-weight: bold;
    margin-right: 0.5rem;
  }

  .enroll-btn {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 0.5rem 1.5rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 500;
    transition: all 0.3s;
    display: inline-block;
    text-align: center;
  }

  .enroll-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
  }

  .age-tag {
    background: #EEF2FF;
    color: #4F46E5;
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 500;
  }

  .level-tag {
    background: #ECFDF5;
    color: #10B981;
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 500;
  }

  .course-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1rem;
    border-top: 1px solid #E5E7EB;
    margin-top: auto;
  }

  .badge-container {
    position: absolute;
    top: 1rem;
    right: 1rem;
    z-index: 1;
  }

  .popular-badge {
    background: #EF4444;
    color: white;
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
  }
</style>

<div class="page-header-custom">
  <h1 class="page-title">
    <span class="en-content">Our Course Catalog</span>
    <span class="zh-content">课程目录</span>
  </h1>
  <p class="page-description">
    <span class="en-content">From Fundamentals to Advanced - Your Complete Learning Journey</span>
    <span class="zh-content">从基础到高级 - 您的完整学习之旅</span>
  </p>
</div>

<!-- Programming Languages -->
<div class="course-category">
  <h2 class="category-title">
    <span class="en-content">💻 Programming Languages</span>
    <span class="zh-content">💻 编程语言</span>
  </h2>
  
  <div class="courses-grid">
    <!-- Python Course -->
    <div class="course-card">
      <div class="course-image">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        🐍
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Python Fundamental I & II</span>
          <span class="zh-content">Python 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Complete Python Programming Journey</span>
          <span class="zh-content">完整的Python编程之旅</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Variables, Data Types, Control Flow</span>
            <span class="zh-content">变量、数据类型、控制流</span>
          </li>
          <li>
            <span class="en-content">Functions, OOP Concepts</span>
            <span class="zh-content">函数、面向对象概念</span>
          </li>
          <li>
            <span class="en-content">File Handling & Libraries</span>
            <span class="zh-content">文件处理与库</span>
          </li>
          <li>
            <span class="en-content">Real-world Projects</span>
            <span class="zh-content">实际项目</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./python.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Java Course -->
    <div class="course-card">
      <div class="course-image">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        ☕
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Java Fundamental I & II</span>
          <span class="zh-content">Java 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Object-Oriented Programming Mastery</span>
          <span class="zh-content">面向对象编程精通</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Java Syntax & Structure</span>
            <span class="zh-content">Java语法与结构</span>
          </li>
          <li>
            <span class="en-content">OOP Principles & Design</span>
            <span class="zh-content">面向对象原则与设计</span>
          </li>
          <li>
            <span class="en-content">Collections Framework</span>
            <span class="zh-content">集合框架</span>
          </li>
          <li>
            <span class="en-content">GUI Development</span>
            <span class="zh-content">GUI开发</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./java.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- C++ Course -->
    <div class="course-card">
      <div class="course-image">⚙️</div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">C++ Fundamental I & II</span>
          <span class="zh-content">C++ 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">System Programming & Performance</span>
          <span class="zh-content">系统编程与性能</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Memory Management</span>
            <span class="zh-content">内存管理</span>
          </li>
          <li>
            <span class="en-content">Pointers & References</span>
            <span class="zh-content">指针与引用</span>
          </li>
          <li>
            <span class="en-content">STL & Templates</span>
            <span class="zh-content">STL与模板</span>
          </li>
          <li>
            <span class="en-content">Competitive Programming</span>
            <span class="zh-content">竞赛编程</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Intermediate</span>
            <span class="zh-content">中级</span>
          </span>
        </div>
        <a href="./cplusplus.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</div>

<!-- More categories can be added with the same pattern... -->

<!-- CTA Section -->
<div style="background: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%); border-radius: 20px; padding: 3rem; text-align: center; color: white; margin: 4rem 0;">
  <h2 style="font-size: 2rem; margin-bottom: 1rem;">
    <span class="en-content">Can't Find What You're Looking For?</span>
    <span class="zh-content">找不到您需要的课程？</span>
  </h2>
  <p style="font-size: 1.1rem; margin-bottom: 2rem; opacity: 0.95;">
    <span class="en-content">We offer customized courses tailored to your specific needs and goals</span>
    <span class="zh-content">我们提供根据您的具体需求和目标定制的课程</span>
  </p>
  <a href="./contact.html" style="background: white; color: #4F46E5; padding: 0.8rem 2rem; border-radius: 10px; text-decoration: none; font-weight: 600; display: inline-block;">
    <span class="en-content">Contact Us for Custom Programs</span>
    <span class="zh-content">联系我们定制课程</span>
  </a>
</div>
