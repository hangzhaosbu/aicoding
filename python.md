---
layout: default
title: Python Fundamental I & II
title_zh: Python 基础 I & II
description: Complete Python Programming Journey from Basics to Advanced
description_zh: 从基础到高级的完整Python编程之旅
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

  @keyframes pythonFloat {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  @keyframes codeTyping {
    from { width: 0; }
    to { width: 100%; }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🐍';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: pythonFloat 6s ease-in-out infinite;
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

  /* Code snippets floating */
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

  /* Course Info Grid - Premium Layout */
  .course-info-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 3rem;
    margin-bottom: 4rem;
    max-width: 1400px;
    margin-left: auto;
    margin-right: auto;
    padding: 0 2rem;
  }

  @media (max-width: 968px) {
    .course-info-grid {
      grid-template-columns: 1fr;
    }
  }

  /* Course Content Section - Enhanced */
  .course-content-section {
    background: white;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.5);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out;
    margin-bottom: 2rem;
  }

  .course-content-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.05), transparent);
    animation: shimmer 4s infinite;
  }

  .section-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 3px solid transparent;
    border-image: linear-gradient(90deg, #667eea, #764ba2) 1;
    position: relative;
  }

  /* Syllabus Modules - Premium Design */
  .syllabus-module {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 2rem;
    border-radius: 20px;
    margin-bottom: 1.5rem;
    border-left: 5px solid;
    border-image: linear-gradient(180deg, #667eea, #764ba2) 1;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .syllabus-module::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.1), transparent);
    transition: left 0.6s;
  }

  .syllabus-module:hover::before {
    left: 100%;
  }

  .syllabus-module:hover {
    transform: translateX(10px);
    box-shadow: 0 15px 30px rgba(102, 126, 234, 0.2);
    background: white;
  }

  .module-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .module-topics {
    list-style: none;
    margin-top: 1.5rem;
    padding-left: 0;
  }

  .module-topics li {
    padding: 0.8rem 0;
    color: #6B7280;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    position: relative;
  }

  .module-topics li:hover {
    color: #4B5563;
    padding-left: 0.5rem;
  }

  .module-topics li::before {
    content: '▶';
    color: #667eea;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 0.8rem;
    transition: transform 0.3s;
  }

  .module-topics li:hover::before {
    transform: translateX(5px);
  }

  /* Course Sidebar - Premium Style */
  .course-sidebar {
    position: sticky;
    top: 2rem;
    height: fit-content;
  }

  .info-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.5);
    margin-bottom: 2rem;
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out 0.2s backwards;
  }

  .info-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    animation: shimmer 3s infinite;
  }

  .info-card h3 {
    font-size: 1.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
  }

  .info-item {
    display: flex;
    align-items: center;
    margin-bottom: 1.5rem;
    padding: 1rem;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 15px;
    transition: all 0.3s ease;
  }

  .info-item:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.1);
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 100%);
  }

  .info-item:last-child {
    margin-bottom: 0;
  }

  .info-icon {
    font-size: 2rem;
    margin-right: 1rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .info-content h4 {
    font-size: 0.9rem;
    color: #6B7280;
    margin-bottom: 0.25rem;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .info-content p {
    font-size: 1.1rem;
    color: #1F2937;
    font-weight: 700;
  }

  /* Enroll Section - Premium CTA */
  .enroll-section {
    text-align: center;
    padding: 2.5rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    border-radius: 25px;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(102, 126, 234, 0.3);
  }

  .enroll-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 60%);
    animation: rotateGlow 12s linear infinite;
  }

  .price {
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .enroll-button {
    background: white;
    color: #667eea;
    padding: 1.2rem 2.5rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    width: 100%;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
    overflow: hidden;
  }

  .enroll-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.2), transparent);
    transition: left 0.5s;
  }

  .enroll-button:hover::before {
    left: 100%;
  }

  .enroll-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #764ba2;
  }

  /* Learning Outcomes - Premium Cards */
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
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    color: white;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
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
    box-shadow: 0 20px 40px rgba(102, 126, 234, 0.4);
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
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  /* Prerequisites - Premium List */
  .prereq-list {
    list-style: none;
    margin-top: 1.5rem;
    padding: 0;
  }

  .prereq-list li {
    padding: 1rem;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 15px;
    display: flex;
    align-items: center;
    transition: all 0.3s ease;
    border-left: 3px solid #667eea;
  }

  .prereq-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.1);
    background: white;
  }

  .prereq-list li::before {
    content: '✨';
    margin-right: 1rem;
    font-size: 1.2rem;
    animation: pulse 2s ease-in-out infinite;
  }

  /* Features Section - New Addition */
  .features-section {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
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
    background: radial-gradient(circle at 30% 70%, rgba(102, 126, 234, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(236, 72, 153, 0.05), transparent 50%);
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
    box-shadow: 0 15px 40px rgba(102, 126, 234, 0.2);
    border-color: #667eea;
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

  /* Responsive Adjustments */
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
  <div class="code-float">print("Hello World")</div>
  <div class="code-float">def learn():</div>
  <div class="code-float">for i in range(10):</div>
  <div class="code-float">class Python:</div>
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
      <p style="color: #4B5563; line-height: 1.8; font-size: 1.1rem;">
        <span class="en-content">
          This comprehensive Python programming course is designed to take students from absolute beginners to confident programmers. Through 40 hours of intensive learning, students will master Python fundamentals, data structures, object-oriented programming, and real-world applications. Our proven curriculum combines theoretical knowledge with hands-on practice, ensuring students build a solid foundation for advanced computer science topics and competitive programming.
        </span>
        <span class="zh-content">
          这门综合性的Python编程课程旨在将学生从零基础培养成自信的程序员。通过40小时的密集学习，学生将掌握Python基础知识、数据结构、面向对象编程和实际应用。我们经过验证的课程将理论知识与实践相结合，确保学生为高级计算机科学主题和竞赛编程打下坚实的基础。
        </span>
      </p>
    </div>

    <!-- Detailed Syllabus -->
    <div class="course-content-section">
      <h2 class="section-title">
        <span class="en-content">📚 Detailed Syllabus</span>
        <span class="zh-content">📚 详细课程大纲</span>
      </h2>
      
      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 1: Python Foundations (Hours 1-5)</span>
          <span class="zh-content">模块 1：Python 基础（第1-5小时）</span>
        </h3>
        <ul class="module-topics">
          <li>
            <span class="en-content">Installing Python & IDE Setup (PyCharm/VS Code)</span>
            <span class="zh-content">安装 Python 和 IDE 设置（PyCharm/VS Code）</span>
          </li>
          <li>
            <span class="en-content">Understanding Programming Logic & Computational Thinking</span>
            <span class="zh-content">理解编程逻辑与计算思维</span>
          </li>
          <li>
            <span class="en-content">Variables, Data Types, and Type Conversion</span>
            <span class="zh-content">变量、数据类型和类型转换</span>
          </li>
          <li>
            <span class="en-content">Input/Output Operations and String Formatting</span>
            <span class="zh-content">输入/输出操作和字符串格式化</span>
          </li>
          <li>
            <span class="en-content">Building Your First Interactive Programs</span>
            <span class="zh-content">构建您的第一个交互式程序</span>
          </li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 2: Control Structures (Hours 6-10)</span>
          <span class="zh-content">模块 2：控制结构（第6-10小时）</span>
        </h3>
        <ul class="module-topics">
          <li>
            <span class="en-content">Conditional Statements (if/elif/else)</span>
            <span class="zh-content">条件语句（if/elif/else）</span>
          </li>
          <li>
            <span class="en-content">Boolean Logic and Complex Conditions</span>
            <span class="zh-content">布尔逻辑和复杂条件</span>
          </li>
          <li>
            <span class="en-content">For Loops and Range Function</span>
            <span class="zh-content">For 循环和 Range 函数</span>
          </li>
          <li>
            <span class="en-content">While Loops and Loop Control</span>
            <span class="zh-content">While 循环和循环控制</span>
          </li>
          <li>
            <span class="en-content">Nested Loops and Pattern Problems</span>
            <span class="zh-content">嵌套循环和模式问题</span>
          </li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 3: Data Structures (Hours 11-20)</span>
          <span class="zh-content">模块 3：数据结构（第11-20小时）</span>
        </h3>
        <ul class="module-topics">
          <li>
            <span class="en-content">Strings: Methods, Slicing, and Manipulation</span>
            <span class="zh-content">字符串：方法、切片和操作</span>
          </li>
          <li>
            <span class="en-content">Lists: Operations, Methods, and List Comprehensions</span>
            <span class="zh-content">列表：操作、方法和列表推导式</span>
          </li>
          <li>
            <span class="en-content">Dictionaries: Key-Value Pairs and Applications</span>
            <span class="zh-content">字典：键值对和应用</span>
          </li>
          <li>
            <span class="en-content">Tuples and Sets: Immutable and Unique Collections</span>
            <span class="zh-content">元组和集合：不可变和唯一集合</span>
          </li>
          <li>
            <span class="en-content">2D Arrays and Matrix Operations</span>
            <span class="zh-content">二维数组和矩阵操作</span>
          </li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 4: Functions & OOP (Hours 21-30)</span>
          <span class="zh-content">模块 4：函数与面向对象（第21-30小时）</span>
        </h3>
        <ul class="module-topics">
          <li>
            <span class="en-content">Functions: Parameters, Return Values, and Scope</span>
            <span class="zh-content">函数：参数、返回值和作用域</span>
          </li>
          <li>
            <span class="en-content">Lambda Functions and Higher-Order Functions</span>
            <span class="zh-content">Lambda 函数和高阶函数</span>
          </li>
          <li>
            <span class="en-content">Classes and Objects: Creating Custom Types</span>
            <span class="zh-content">类和对象：创建自定义类型</span>
          </li>
          <li>
            <span class="en-content">Inheritance, Polymorphism, and Encapsulation</span>
            <span class="zh-content">继承、多态和封装</span>
          </li>
          <li>
            <span class="en-content">Special Methods and Operator Overloading</span>
            <span class="zh-content">特殊方法和运算符重载</span>
          </li>
        </ul>
      </div>

      <div class="syllabus-module">
        <h3 class="module-title">
          <span class="en-content">Module 5: Advanced Topics & Projects (Hours 31-40)</span>
          <span class="zh-content">模块 5：高级主题与项目（第31-40小时）</span>
        </h3>
        <ul class="module-topics">
          <li>
            <span class="en-content">File Handling: Reading, Writing, and CSV/JSON Processing</span>
            <span class="zh-content">文件处理：读取、写入和 CSV/JSON 处理</span>
          </li>
          <li>
            <span class="en-content">Error Handling and Debugging Techniques</span>
            <span class="zh-content">错误处理和调试技术</span>
          </li>
          <li>
            <span class="en-content">Regular Expressions for Pattern Matching</span>
            <span class="zh-content">正则表达式进行模式匹配</span>
          </li>
          <li>
            <span class="en-content">Introduction to Popular Libraries (NumPy, Pandas)</span>
            <span class="zh-content">流行库简介（NumPy、Pandas）</span>
          </li>
          <li>
            <span class="en-content">Building a Complete Python Application</span>
            <span class="zh-content">构建完整的 Python 应用程序</span>
          </li>
          <li>
            <span class="en-content">Final Project: Game or Data Analysis Tool</span>
            <span class="zh-content">最终项目：游戏或数据分析工具</span>
          </li>
        </ul>
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
          <div class="outcome-icon">💻</div>
          <div class="outcome-title">
            <span class="en-content">Professional Code</span>
            <span class="zh-content">专业代码</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🔧</div>
          <div class="outcome-title">
            <span class="en-content">Real Projects</span>
            <span class="zh-content">实际项目</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🧩</div>
          <div class="outcome-title">
            <span class="en-content">Problem Solving</span>
            <span class="zh-content">问题解决</span>
          </div>
        </div>
        
        <div class="outcome-card">
          <div class="outcome-icon">🚀</div>
          <div class="outcome-title">
            <span class="en-content">Competition Ready</span>
            <span class="zh-content">竞赛准备</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Sidebar -->
  <div class="course-sidebar">
    <!-- Course Info Card -->
    <div class="info-card">
      <h3>
        <span class="en-content">Course Information</span>
        <span class="zh-content">课程信息</span>
      </h3>
      
      <div class="info-item">
        <div class="info-icon">⏱️</div>
        <div class="info-content">
          <h4>
            <span class="en-content">Duration</span>
            <span class="zh-content">课程时长</span>
          </h4>
          <p>40 Hours</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">👥</div>
        <div class="info-content">
          <h4>
            <span class="en-content">Age Group</span>
            <span class="zh-content">年龄组</span>
          </h4>
          <p>10-18 Years</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">📊</div>
        <div class="info-content">
          <h4>
            <span class="en-content">Level</span>
            <span class="zh-content">级别</span>
          </h4>
          <p>Beginner to Intermediate</p>
        </div>
      </div>
      
      <div class="info-item">
        <div class="info-icon">🏫</div>
        <div class="info-content">
          <h4>
            <span class="en-content">Class Size</span>
            <span class="zh-content">班级规模</span>
          </h4>
          <p>1-on-1 or Max 4 Students</p>
        </div>
      </div>
    </div>

    <!-- Prerequisites -->
    <div class="info-card">
      <h3>
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
        <span class="en-content">Get Started Today</span>
        <span class="zh-content">立即开始</span>
      </div>
      <a href="./contact.html" class="enroll-button">
        <span class="en-content">Enroll Now</span>
        <span class="zh-content">立即报名</span>
      </a>
      <p style="margin-top: 1.5rem; font-size: 1rem; opacity: 0.95; position: relative; z-index: 1;">
        <span class="en-content">✨ Free consultation & assessment</span>
        <span class="zh-content">✨ 免费咨询和评估</span>
      </p>
    </div>
  </div>
</div>

<!-- Why Choose This Course -->
<div class="features-section">
  <h2 class="section-title" style="text-align: center; margin-bottom: 3rem;">
    <span class="en-content">Why Choose Our Python Course</span>
    <span class="zh-content">为什么选择我们的Python课程</span>
  </h2>
  
  <div class="features-grid">
    <div class="feature-box">
      <div class="feature-box-icon">🎓</div>
      <div class="feature-box-title">
        <span class="en-content">PhD Instructor</span>
        <span class="zh-content">博士讲师</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Learn from experts with industry experience</span>
        <span class="zh-content">向具有行业经验的专家学习</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">📝</div>
      <div class="feature-box-title">
        <span class="en-content">Hands-on Projects</span>
        <span class="zh-content">实践项目</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Build 10+ real-world applications</span>
        <span class="zh-content">构建10+个真实应用程序</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">🏆</div>
      <div class="feature-box-title">
        <span class="en-content">Competition Prep</span>
        <span class="zh-content">竞赛准备</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Foundation for USACO and coding contests</span>
        <span class="zh-content">为USACO和编程竞赛打基础</span>
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
        <span class="en-content">Access to 500+ practice problems</span>
        <span class="zh-content">访问500+练习题</span>
      </div>
    </div>
    
    <div class="feature-box">
      <div class="feature-box-icon">🔄</div>
      <div class="feature-box-title">
        <span class="en-content">Lifetime Support</span>
        <span class="zh-content">终身支持</span>
      </div>
      <div class="feature-box-desc">
        <span class="en-content">Continuous guidance after course completion</span>
        <span class="zh-content">课程结束后持续指导</span>
      </div>
    </div>
  </div>
</div>
