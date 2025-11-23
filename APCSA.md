---
layout: default
title: AP Computer Science A
title_zh: AP计算机科学A
description: Excel in AP CSA Exam with Comprehensive Java Training
description_zh: 通过全面的Java培训在AP CSA考试中取得优异成绩
---

<style>
  /* AP CSA Specific Styling - Green/Teal Theme */
  .course-hero {
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    padding: 4rem 2rem;
    border-radius: 20px;
    color: white;
    text-align: center;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .course-hero::before {
    content: '📘';
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

  .ap-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    padding: 0.5rem 1rem;
    border-radius: 20px;
    margin-top: 1rem;
    font-weight: 600;
  }

  /* Overview Section */
  .overview-section {
    background: white;
    padding: 2.5rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    margin-bottom: 3rem;
    border-top: 3px solid #10B981;
  }

  /* Curriculum Cards */
  .curriculum-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
  }

  .unit-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    transition: all 0.3s;
    position: relative;
    overflow: hidden;
  }

  .unit-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #10B981 0%, #0891B2 100%);
  }

  .unit-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
  }

  .unit-number {
    display: inline-block;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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

  .unit-title {
    font-size: 1.3rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .unit-description {
    color: #6B7280;
    font-size: 0.95rem;
    margin-bottom: 1rem;
  }

  .topic-list {
    list-style: none;
    padding: 0;
  }

  .topic-list li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.9rem;
    display: flex;
    align-items: flex-start;
  }

  .topic-list li::before {
    content: '→';
    color: #10B981;
    font-weight: bold;
    margin-right: 0.5rem;
    flex-shrink: 0;
  }

  /* Exam Info Section */
  .exam-info {
    background: #F0FDF4;
    padding: 3rem;
    border-radius: 15px;
    margin: 3rem 0;
  }

  .exam-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin: 2rem 0;
  }

  .stat-card {
    background: white;
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
  }

  .stat-number {
    font-size: 2rem;
    font-weight: 700;
    color: #10B981;
    display: block;
  }

  .stat-label {
    color: #6B7280;
    font-size: 0.9rem;
    margin-top: 0.5rem;
  }

  /* Features Grid */
  .features-section {
    padding: 3rem 0;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
  }

  .feature-card {
    text-align: center;
    padding: 2rem;
    background: white;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    transition: transform 0.3s;
  }

  .feature-card:hover {
    transform: translateY(-3px);
  }

  .feature-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .feature-title {
    font-size: 1.2rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .feature-description {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.5;
  }

  /* Success Banner */
  .success-banner {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
    padding: 2rem;
    border-radius: 15px;
    margin: 3rem 0;
    text-align: center;
  }

  .success-title {
    font-size: 1.5rem;
    font-weight: 600;
    color: #92400E;
    margin-bottom: 1rem;
  }

  .score-badges {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
    margin-top: 1.5rem;
  }

  .score-badge {
    background: white;
    padding: 1rem 2rem;
    border-radius: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  .score-badge strong {
    color: #92400E;
    font-size: 1.2rem;
  }

  /* CTA Section */
  .cta-section {
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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
  }

  .cta-button {
    background: white;
    color: #10B981;
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
    color: #10B981;
  }

  /* Responsive */
  @media (max-width: 768px) {
    .curriculum-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="course-hero">
  <h1>
    <span class="en-content">AP Computer Science A</span>
    <span class="zh-content">AP计算机科学A</span>
  </h1>
  <p>
    <span class="en-content">Score 5 on Your AP Exam - Guaranteed!</span>
    <span class="zh-content">AP考试5分保证！</span>
  </p>
  <div class="ap-badge">
    <span class="en-content">⭐ Official AP Curriculum + Beyond</span>
    <span class="zh-content">⭐ 官方AP课程及扩展</span>
  </div>
</div>

<!-- Course Overview -->
<div class="overview-section">
  <h2 style="color: #1F2937; margin-bottom: 1.5rem;">
    <span class="en-content">AP CSA Exam Preparation Program</span>
    <span class="zh-content">AP CSA 考试准备计划</span>
  </h2>
  <p style="font-size: 1.1rem; color: #4B5563; line-height: 1.8;">
    <span class="en-content">
      Master the complete AP Computer Science A curriculum with our comprehensive 40-hour program. 
      Designed specifically for AP exam success, this course covers all College Board requirements 
      plus additional practice to ensure you achieve a score of 5. Our proven methodology combines 
      official AP content with extensive practice problems, mock exams, and personalized feedback.
    </span>
    <span class="zh-content">
      通过我们全面的40小时课程掌握完整的AP计算机科学A课程。
      专为AP考试成功而设计，本课程涵盖了所有大学理事会的要求，
      并提供额外的练习以确保您获得5分。我们经过验证的方法结合了
      官方AP内容与大量练习题、模拟考试和个性化反馈。
    </span>
  </p>
</div>

<!-- Exam Information -->
<div class="exam-info">
  <h2 style="text-align: center; color: #14532D; margin-bottom: 2rem;">
    <span class="en-content">2025 AP Exam Information</span>
    <span class="zh-content">2025年AP考试信息</span>
  </h2>
  
  <div class="exam-stats">
    <div class="stat-card">
      <span class="stat-number">
        <span class="en-content">May 7</span>
        <span class="zh-content">5月7日</span>
      </span>
      <div class="stat-label">
        <span class="en-content">2025 Exam Date</span>
        <span class="zh-content">2025考试日期</span>
      </div>
    </div>
    <div class="stat-card">
      <span class="stat-number">
        <span class="en-content">3 Hours</span>
        <span class="zh-content">3小时</span>
      </span>
      <div class="stat-label">
        <span class="en-content">Exam Duration</span>
        <span class="zh-content">考试时长</span>
      </div>
    </div>
    <div class="stat-card">
      <span class="stat-number">
        <span class="en-content">40 MCQ</span>
        <span class="zh-content">40道选择题</span>
      </span>
      <div class="stat-label">
        <span class="en-content">Multiple Choice</span>
        <span class="zh-content">选择题</span>
      </div>
    </div>
    <div class="stat-card">
      <span class="stat-number">
        <span class="en-content">4 FRQ</span>
        <span class="zh-content">4道问答题</span>
      </span>
      <div class="stat-label">
        <span class="en-content">Free Response</span>
        <span class="zh-content">自由回答题</span>
      </div>
    </div>
  </div>
</div>

<!-- AP Curriculum Units -->
<h2 style="text-align: center; color: #1F2937; margin: 3rem 0 2rem;">
  <span class="en-content">Official AP CSA Units</span>
  <span class="zh-content">官方AP CSA单元</span>
</h2>

<div class="curriculum-grid">
  <!-- Unit 1 -->
  <div class="unit-card">
    <div class="unit-number">1</div>
    <h3 class="unit-title">
      <span class="en-content">Primitive Types</span>
      <span class="zh-content">基本类型</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">2.5-5% of exam score</span>
      <span class="zh-content">占考试分数的2.5-5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Variables and Data Types</span>
        <span class="zh-content">变量和数据类型</span>
      </li>
      <li>
        <span class="en-content">Operations and Expressions</span>
        <span class="zh-content">运算和表达式</span>
      </li>
      <li>
        <span class="en-content">Type Casting</span>
        <span class="zh-content">类型转换</span>
      </li>
    </ul>
  </div>

  <!-- Unit 2 -->
  <div class="unit-card">
    <div class="unit-number">2</div>
    <h3 class="unit-title">
      <span class="en-content">Using Objects</span>
      <span class="zh-content">使用对象</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">5-7.5% of exam score</span>
      <span class="zh-content">占考试分数的5-7.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Object Instantiation</span>
        <span class="zh-content">对象实例化</span>
      </li>
      <li>
        <span class="en-content">Calling Methods</span>
        <span class="zh-content">调用方法</span>
      </li>
      <li>
        <span class="en-content">String Objects and Methods</span>
        <span class="zh-content">字符串对象和方法</span>
      </li>
      <li>
        <span class="en-content">Wrapper Classes</span>
        <span class="zh-content">包装类</span>
      </li>
    </ul>
  </div>

  <!-- Unit 3 -->
  <div class="unit-card">
    <div class="unit-number">3</div>
    <h3 class="unit-title">
      <span class="en-content">Boolean Expressions & if Statements</span>
      <span class="zh-content">布尔表达式与if语句</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">15-17.5% of exam score</span>
      <span class="zh-content">占考试分数的15-17.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Boolean Expressions</span>
        <span class="zh-content">布尔表达式</span>
      </li>
      <li>
        <span class="en-content">if, else if, else</span>
        <span class="zh-content">if, else if, else语句</span>
      </li>
      <li>
        <span class="en-content">Compound Boolean Expressions</span>
        <span class="zh-content">复合布尔表达式</span>
      </li>
      <li>
        <span class="en-content">De Morgan's Laws</span>
        <span class="zh-content">德摩根定律</span>
      </li>
    </ul>
  </div>

  <!-- Unit 4 -->
  <div class="unit-card">
    <div class="unit-number">4</div>
    <h3 class="unit-title">
      <span class="en-content">Iteration</span>
      <span class="zh-content">迭代</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">17.5-22.5% of exam score</span>
      <span class="zh-content">占考试分数的17.5-22.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">while Loops</span>
        <span class="zh-content">while循环</span>
      </li>
      <li>
        <span class="en-content">for Loops</span>
        <span class="zh-content">for循环</span>
      </li>
      <li>
        <span class="en-content">Enhanced for Loops</span>
        <span class="zh-content">增强for循环</span>
      </li>
      <li>
        <span class="en-content">Nested Loops</span>
        <span class="zh-content">嵌套循环</span>
      </li>
    </ul>
  </div>

  <!-- Unit 5 -->
  <div class="unit-card">
    <div class="unit-number">5</div>
    <h3 class="unit-title">
      <span class="en-content">Writing Classes</span>
      <span class="zh-content">编写类</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">5-7.5% of exam score</span>
      <span class="zh-content">占考试分数的5-7.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Class Anatomy</span>
        <span class="zh-content">类结构</span>
      </li>
      <li>
        <span class="en-content">Constructors</span>
        <span class="zh-content">构造函数</span>
      </li>
      <li>
        <span class="en-content">Instance Variables & Methods</span>
        <span class="zh-content">实例变量和方法</span>
      </li>
      <li>
        <span class="en-content">Static Variables & Methods</span>
        <span class="zh-content">静态变量和方法</span>
      </li>
      <li>
        <span class="en-content">Scope and Access</span>
        <span class="zh-content">作用域和访问控制</span>
      </li>
    </ul>
  </div>

  <!-- Unit 6 -->
  <div class="unit-card">
    <div class="unit-number">6</div>
    <h3 class="unit-title">
      <span class="en-content">Array</span>
      <span class="zh-content">数组</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">10-15% of exam score</span>
      <span class="zh-content">占考试分数的10-15%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Array Creation</span>
        <span class="zh-content">数组创建</span>
      </li>
      <li>
        <span class="en-content">Traversing Arrays</span>
        <span class="zh-content">遍历数组</span>
      </li>
      <li>
        <span class="en-content">Array Algorithms</span>
        <span class="zh-content">数组算法</span>
      </li>
      <li>
        <span class="en-content">Enhanced for Loop with Arrays</span>
        <span class="zh-content">数组的增强for循环</span>
      </li>
    </ul>
  </div>

  <!-- Unit 7 -->
  <div class="unit-card">
    <div class="unit-number">7</div>
    <h3 class="unit-title">
      <span class="en-content">ArrayList</span>
      <span class="zh-content">动态数组</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">2.5-7.5% of exam score</span>
      <span class="zh-content">占考试分数的2.5-7.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">ArrayList Methods</span>
        <span class="zh-content">ArrayList方法</span>
      </li>
      <li>
        <span class="en-content">Traversing ArrayLists</span>
        <span class="zh-content">遍历ArrayList</span>
      </li>
      <li>
        <span class="en-content">ArrayList Algorithms</span>
        <span class="zh-content">ArrayList算法</span>
      </li>
      <li>
        <span class="en-content">Searching and Sorting</span>
        <span class="zh-content">搜索和排序</span>
      </li>
    </ul>
  </div>

  <!-- Unit 8 -->
  <div class="unit-card">
    <div class="unit-number">8</div>
    <h3 class="unit-title">
      <span class="en-content">2D Array</span>
      <span class="zh-content">二维数组</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">7.5-10% of exam score</span>
      <span class="zh-content">占考试分数的7.5-10%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">2D Array Declaration</span>
        <span class="zh-content">二维数组声明</span>
      </li>
      <li>
        <span class="en-content">Nested Loops for 2D Arrays</span>
        <span class="zh-content">二维数组的嵌套循环</span>
      </li>
      <li>
        <span class="en-content">Row-Major vs Column-Major</span>
        <span class="zh-content">行优先vs列优先</span>
      </li>
    </ul>
  </div>

  <!-- Unit 9 -->
  <div class="unit-card">
    <div class="unit-number">9</div>
    <h3 class="unit-title">
      <span class="en-content">Inheritance</span>
      <span class="zh-content">继承</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">5-10% of exam score</span>
      <span class="zh-content">占考试分数的5-10%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Superclasses and Subclasses</span>
        <span class="zh-content">父类和子类</span>
      </li>
      <li>
        <span class="en-content">Method Overriding</span>
        <span class="zh-content">方法重写</span>
      </li>
      <li>
        <span class="en-content">super Keyword</span>
        <span class="zh-content">super关键字</span>
      </li>
      <li>
        <span class="en-content">Polymorphism</span>
        <span class="zh-content">多态性</span>
      </li>
      <li>
        <span class="en-content">Object Class</span>
        <span class="zh-content">Object类</span>
      </li>
    </ul>
  </div>

  <!-- Unit 10 -->
  <div class="unit-card">
    <div class="unit-number">10</div>
    <h3 class="unit-title">
      <span class="en-content">Recursion</span>
      <span class="zh-content">递归</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">5-7.5% of exam score</span>
      <span class="zh-content">占考试分数的5-7.5%</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Recursive Methods</span>
        <span class="zh-content">递归方法</span>
      </li>
      <li>
        <span class="en-content">Base Case & Recursive Call</span>
        <span class="zh-content">基本情况和递归调用</span>
      </li>
      <li>
        <span class="en-content">Binary Search</span>
        <span class="zh-content">二分搜索</span>
      </li>
      <li>
        <span class="en-content">Merge Sort</span>
        <span class="zh-content">归并排序</span>
      </li>
    </ul>
  </div>

  <!-- Unit 11 - Searching Algorithms -->
  <div class="unit-card">
    <div class="unit-number">11</div>
    <h3 class="unit-title">
      <span class="en-content">Searching Algorithms</span>
      <span class="zh-content">搜索算法</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">Essential for FRQs</span>
      <span class="zh-content">FRQ必备技能</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Linear/Sequential Search</span>
        <span class="zh-content">线性/顺序搜索</span>
      </li>
      <li>
        <span class="en-content">Binary Search Implementation</span>
        <span class="zh-content">二分搜索实现</span>
      </li>
      <li>
        <span class="en-content">Search in 2D Arrays</span>
        <span class="zh-content">二维数组搜索</span>
      </li>
      <li>
        <span class="en-content">Efficiency Analysis</span>
        <span class="zh-content">效率分析</span>
      </li>
      <li>
        <span class="en-content">Common FRQ Patterns</span>
        <span class="zh-content">常见FRQ模式</span>
      </li>
    </ul>
  </div>

  <!-- Unit 12 - Sorting Algorithms -->
  <div class="unit-card">
    <div class="unit-number">12</div>
    <h3 class="unit-title">
      <span class="en-content">Sorting Algorithms</span>
      <span class="zh-content">排序算法</span>
    </h3>
    <p class="unit-description">
      <span class="en-content">Critical for Success</span>
      <span class="zh-content">成功的关键</span>
    </p>
    <ul class="topic-list">
      <li>
        <span class="en-content">Selection Sort</span>
        <span class="zh-content">选择排序</span>
      </li>
      <li>
        <span class="en-content">Insertion Sort</span>
        <span class="zh-content">插入排序</span>
      </li>
      <li>
        <span class="en-content">Merge Sort (Recursive)</span>
        <span class="zh-content">归并排序（递归）</span>
      </li>
      <li>
        <span class="en-content">Quick Sort Concepts</span>
        <span class="zh-content">快速排序概念</span>
      </li>
      <li>
        <span class="en-content">Sorting Efficiency</span>
        <span class="zh-content">排序效率</span>
      </li>
    </ul>
  </div>
</div>

<!-- Features Section -->
<div class="features-section">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 2rem;">
    <span class="en-content">Why Choose Our AP CSA Program?</span>
    <span class="zh-content">为什么选择我们的AP CSA课程？</span>
  </h2>
  
  <div class="features-grid">
    <div class="feature-card">
      <div class="feature-icon">📚</div>
      <h3 class="feature-title">
        <span class="en-content">Complete Coverage</span>
        <span class="zh-content">完整覆盖</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">All 10 AP units covered in detail</span>
        <span class="zh-content">详细涵盖所有10个AP单元</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon">✍️</div>
      <h3 class="feature-title">
        <span class="en-content">FRQ Mastery</span>
        <span class="zh-content">FRQ精通</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Intensive free-response practice</span>
        <span class="zh-content">密集的自由回答练习</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon">🎯</div>
      <h3 class="feature-title">
        <span class="en-content">Practice Tests</span>
        <span class="zh-content">模拟考试</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">5+ full-length mock exams</span>
        <span class="zh-content">5次以上完整模拟考试</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon">📊</div>
      <h3 class="feature-title">
        <span class="en-content">Score Tracking</span>
        <span class="zh-content">分数跟踪</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Monitor progress to exam</span>
        <span class="zh-content">监控考试进度</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stories -->
<div class="success-banner">
  <h2 class="success-title">
    <span class="en-content">🏆 Our Students' AP Scores</span>
    <span class="zh-content">🏆 我们学生的AP成绩</span>
  </h2>
  <div class="score-badges">
    <div class="score-badge">
      <strong>92%</strong> 
      <span class="en-content">Score 5</span>
      <span class="zh-content">获得5分</span>
    </div>
    <div class="score-badge">
      <strong>8%</strong> 
      <span class="en-content">Score 4</span>
      <span class="zh-content">获得4分</span>
    </div>
    <div class="score-badge">
      <strong>100%</strong> 
      <span class="en-content">Pass Rate</span>
      <span class="zh-content">通过率</span>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Ace Your AP CSA Exam!</span>
    <span class="zh-content">在AP CSA考试中取得优异成绩！</span>
  </h2>
  <p>
    <span class="en-content">Join our proven AP preparation program and secure your score of 5</span>
    <span class="zh-content">加入我们经过验证的AP准备课程，确保获得5分</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Start Preparing Now</span>
    <span class="zh-content">立即开始准备</span>
  </a>
</div>
