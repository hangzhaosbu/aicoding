---
layout: default
title: Our Courses
title_zh: 我们的课程
description: Comprehensive Programming Curriculum for All Levels
description_zh: 全方位编程课程，适合各个水平
---

<style>
  /* Page Header */
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
    color: white !important;
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
    color: white !important;
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

  .new-badge {
    background: #10B981;
    color: white;
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  /* Learning Path Section */
  .learning-path {
    background: #F9FAFB;
    border-radius: 15px;
    padding: 2rem;
    margin: 3rem 0;
  }

  .path-title {
    font-size: 1.5rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 1.5rem;
    text-align: center;
  }

  .path-steps {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
  }

  .path-step {
    flex: 1;
    min-width: 150px;
    text-align: center;
    padding: 1rem;
    background: white;
    border-radius: 10px;
    position: relative;
  }

  .path-step::after {
    content: "→";
    position: absolute;
    right: -20px;
    top: 50%;
    transform: translateY(-50%);
    color: #9CA3AF;
    font-size: 1.5rem;
  }

  .path-step:last-child::after {
    display: none;
  }

  .step-number {
    background: #4F46E5;
    color: white;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 0.5rem;
    font-weight: 600;
  }

  .step-title {
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.25rem;
  }

  .step-description {
    font-size: 0.9rem;
    color: #6B7280;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .courses-grid {
      grid-template-columns: 1fr;
    }

    .path-steps {
      flex-direction: column;
    }

    .path-step::after {
      display: none;
    }
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

<!-- Learning Path -->
<div class="learning-path">
  <h2 class="path-title">
    <span class="en-content">🎯 Recommended Learning Path</span>
    <span class="zh-content">🎯 推荐学习路径</span>
  </h2>
  <div class="path-steps">
    <div class="path-step">
      <div class="step-number">1</div>
      <div class="step-title">
        <span class="en-content">Foundation</span>
        <span class="zh-content">基础</span>
      </div>
      <div class="step-description">
        <span class="en-content">Python/Java Basics</span>
        <span class="zh-content">Python/Java 基础</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">2</div>
      <div class="step-title">
        <span class="en-content">Core Concepts</span>
        <span class="zh-content">核心概念</span>
      </div>
      <div class="step-description">
        <span class="en-content">Data Structures</span>
        <span class="zh-content">数据结构</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">3</div>
      <div class="step-title">
        <span class="en-content">Advanced</span>
        <span class="zh-content">进阶</span>
      </div>
      <div class="step-description">
        <span class="en-content">Algorithms</span>
        <span class="zh-content">算法</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">4</div>
      <div class="step-title">
        <span class="en-content">Specialization</span>
        <span class="zh-content">专业化</span>
      </div>
      <div class="step-description">
        <span class="en-content">AI/ML or Competitions</span>
        <span class="zh-content">人工智能或竞赛</span>
      </div>
    </div>
  </div>
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

<!-- Computer Science Fundamentals -->
<div class="course-category">
  <h2 class="category-title">
    <span class="en-content">📚 Computer Science Core</span>
    <span class="zh-content">📚 计算机科学核心</span>
  </h2>
  
  <div class="courses-grid">
    <!-- Data Structures -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);">
        🗂️
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Data Structures</span>
          <span class="zh-content">数据结构</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Foundation of Efficient Programming</span>
          <span class="zh-content">高效编程的基础</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Arrays, Linked Lists, Stacks</span>
            <span class="zh-content">数组、链表、栈</span>
          </li>
          <li>
            <span class="en-content">Trees & Graphs</span>
            <span class="zh-content">树与图</span>
          </li>
          <li>
            <span class="en-content">Hash Tables & Heaps</span>
            <span class="zh-content">哈希表与堆</span>
          </li>
          <li>
            <span class="en-content">Time & Space Complexity</span>
            <span class="zh-content">时间与空间复杂度</span>
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
        <a href="./datastructure.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Algorithms -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);">
        🧮
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Algorithms</span>
          <span class="zh-content">算法</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Problem Solving & Optimization</span>
          <span class="zh-content">问题解决与优化</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Sorting & Searching</span>
            <span class="zh-content">排序与搜索</span>
          </li>
          <li>
            <span class="en-content">Dynamic Programming</span>
            <span class="zh-content">动态规划</span>
          </li>
          <li>
            <span class="en-content">Graph Algorithms</span>
            <span class="zh-content">图算法</span>
          </li>
          <li>
            <span class="en-content">Greedy & Divide-Conquer</span>
            <span class="zh-content">贪心与分治</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 13-18</span>
            <span class="zh-content">年龄: 13-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Advanced</span>
            <span class="zh-content">高级</span>
          </span>
        </div>
        <a href="./algorithm.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Machine Learning -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #F59E0B 0%, #EF4444 100%);">
        <div class="badge-container">
          <span class="new-badge">
            <span class="en-content">NEW</span>
            <span class="zh-content">新</span>
          </span>
        </div>
        🤖
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Machine Learning & AI</span>
          <span class="zh-content">机器学习与人工智能</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Future of Technology</span>
          <span class="zh-content">技术的未来</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Neural Networks</span>
            <span class="zh-content">神经网络</span>
          </li>
          <li>
            <span class="en-content">Deep Learning</span>
            <span class="zh-content">深度学习</span>
          </li>
          <li>
            <span class="en-content">Computer Vision</span>
            <span class="zh-content">计算机视觉</span>
          </li>
          <li>
            <span class="en-content">NLP & AI Projects</span>
            <span class="zh-content">自然语言处理与AI项目</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Advanced</span>
            <span class="zh-content">高级</span>
          </span>
        </div>
        <a href="./MachineLearning.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</div>

<!-- Competition & Exam Prep -->
<div class="course-category">
  <h2 class="category-title">
    <span class="en-content">🏆 Competition & Exam Preparation</span>
    <span class="zh-content">🏆 竞赛与考试准备</span>
  </h2>
  
  <div class="courses-grid">
    <!-- AP CSA -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #10B981 0%, #059669 100%);">
        📘
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">AP Computer Science A</span>
          <span class="zh-content">AP计算机科学A</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">College-Level Java Programming</span>
          <span class="zh-content">大学水平Java编程</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Complete AP CSA Curriculum</span>
            <span class="zh-content">完整的AP CSA课程</span>
          </li>
          <li>
            <span class="en-content">Practice Exams</span>
            <span class="zh-content">模拟考试</span>
          </li>
          <li>
            <span class="en-content">FRQ Training</span>
            <span class="zh-content">自由回答题训练</span>
          </li>
          <li>
            <span class="en-content">Score 5 Guarantee Program</span>
            <span class="zh-content">5分保证计划</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Intermediate</span>
            <span class="zh-content">中级</span>
          </span>
        </div>
        <a href="./APCSA.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- USACO -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">HOT</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        🥇
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">USA Computing Olympiad</span>
          <span class="zh-content">美国计算机奥林匹克</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Path to Gold & Platinum</span>
          <span class="zh-content">通往金牌与白金之路</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Bronze to Platinum Training</span>
            <span class="zh-content">从铜牌到白金培训</span>
          </li>
          <li>
            <span class="en-content">Contest Strategy</span>
            <span class="zh-content">竞赛策略</span>
          </li>
          <li>
            <span class="en-content">1000+ Practice Problems</span>
            <span class="zh-content">1000+练习题</span>
          </li>
          <li>
            <span class="en-content">Mock Competitions</span>
            <span class="zh-content">模拟竞赛</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">All Levels</span>
            <span class="zh-content">所有级别</span>
          </span>
        </div>
        <a href="./USACO.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- USAAIO -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);">
        <div class="badge-container">
          <span class="new-badge">
            <span class="en-content">NEW</span>
            <span class="zh-content">新</span>
          </span>
        </div>
        🧠
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">AI Olympiad Prep</span>
          <span class="zh-content">人工智能奥林匹克准备</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">USAAIO Competition Training</span>
          <span class="zh-content">USAAIO竞赛训练</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">AI & ML Fundamentals</span>
            <span class="zh-content">人工智能与机器学习基础</span>
          </li>
          <li>
            <span class="en-content">Model Building</span>
            <span class="zh-content">模型构建</span>
          </li>
          <li>
            <span class="en-content">Competition Projects</span>
            <span class="zh-content">竞赛项目</span>
          </li>
          <li>
            <span class="en-content">Research Paper Writing</span>
            <span class="zh-content">研究论文写作</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Advanced</span>
            <span class="zh-content">高级</span>
          </span>
        </div>
        <a href="#" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</div>

<!-- CTA Section -->
<div style="background: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%); border-radius: 20px; padding: 3rem; text-align: center; color: white; margin: 4rem 0;">
  <h2 style="font-size: 2rem; margin-bottom: 1rem; color: white;">
    <span class="en-content">Can't Find What You're Looking For?</span>
    <span class="zh-content">找不到您需要的课程？</span>
  </h2>
  <p style="font-size: 1.1rem; margin-bottom: 2rem; opacity: 0.95; color: white;">
    <span class="en-content">We offer customized courses tailored to your specific needs and goals</span>
    <span class="zh-content">我们提供根据您的具体需求和目标定制的课程</span>
  </p>
  <a href="./contact.html" style="background: white; color: #4F46E5; padding: 0.8rem 2rem; border-radius: 10px; text-decoration: none; font-weight: 600; display: inline-block;">
    <span class="en-content">Contact Us for Custom Programs</span>
    <span class="zh-content">联系我们定制课程</span>
  </a>
</div>
