---
layout: default
title: Our Courses
description: Comprehensive Programming Curriculum for All Levels
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

  /* Course Cards Grid */
  .courses-container {
    margin: 3rem 0;
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
    object-fit: cover;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 4rem;
    color: white;
    position: relative;
    overflow: hidden;
  }

  .course-image::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.1);
    top: 0;
    left: 0;
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

  .course-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1rem;
    border-top: 1px solid #E5E7EB;
    margin-top: auto;
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

  .enroll-btn {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 0.5rem 1.5rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 500;
    transition: all 0.3s;
    display: inline-block;
  }

  .enroll-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
  }

  /* Special Badges */
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
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  .new-badge {
    background: #10B981;
    color: white;
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  /* Course Path Section */
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

    .page-title {
      font-size: 2rem;
    }
  }
</style>

<div class="page-header-custom">
  <h1 class="page-title">Our Course Catalog</h1>
  <p class="page-description">From Fundamentals to Advanced - Your Complete Learning Journey</p>
</div>

<!-- Learning Path -->
<div class="learning-path">
  <h2 class="path-title">🎯 Recommended Learning Path</h2>
  <div class="path-steps">
    <div class="path-step">
      <div class="step-number">1</div>
      <div class="step-title">Foundation</div>
      <div class="step-description">Python/Java Basics</div>
    </div>
    <div class="path-step">
      <div class="step-number">2</div>
      <div class="step-title">Core Concepts</div>
      <div class="step-description">Data Structures</div>
    </div>
    <div class="path-step">
      <div class="step-number">3</div>
      <div class="step-title">Advanced</div>
      <div class="step-description">Algorithms</div>
    </div>
    <div class="path-step">
      <div class="step-number">4</div>
      <div class="step-title">Specialization</div>
      <div class="step-description">AI/ML or Competitions</div>
    </div>
  </div>
</div>

<!-- Programming Languages -->
<div class="course-category">
  <h2 class="category-title">💻 Programming Languages</h2>
  
  <div class="courses-grid">
    <!-- Python Course -->
    <div class="course-card">
      <div class="course-image">
        <div class="badge-container">
          <span class="popular-badge">POPULAR</span>
        </div>
        🐍
      </div>
      <div class="course-content">
        <h3 class="course-title">Python Fundamental I & II</h3>
        <p class="course-subtitle">Complete Python Programming Journey</p>
        <ul class="course-features">
          <li>Variables, Data Types, Control Flow</li>
          <li>Functions, OOP Concepts</li>
          <li>File Handling & Libraries</li>
          <li>Real-world Projects</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 10-18</span>
          <span class="level-tag">Beginner</span>
        </div>
        <a href="./python.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- Java Course -->
    <div class="course-card">
      <div class="course-image">
        <div class="badge-container">
          <span class="popular-badge">POPULAR</span>
        </div>
        ☕
      </div>
      <div class="course-content">
        <h3 class="course-title">Java Fundamental I & II</h3>
        <p class="course-subtitle">Object-Oriented Programming Mastery</p>
        <ul class="course-features">
          <li>Java Syntax & Structure</li>
          <li>OOP Principles & Design</li>
          <li>Collections Framework</li>
          <li>GUI Development</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 10-18</span>
          <span class="level-tag">Beginner</span>
        </div>
        <a href="./java.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- C++ Course -->
    <div class="course-card">
      <div class="course-image">
        ⚙️
      </div>
      <div class="course-content">
        <h3 class="course-title">C++ Fundamental I & II</h3>
        <p class="course-subtitle">System Programming & Performance</p>
        <ul class="course-features">
          <li>Memory Management</li>
          <li>Pointers & References</li>
          <li>STL & Templates</li>
          <li>Competitive Programming</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 12-18</span>
          <span class="level-tag">Intermediate</span>
        </div>
        <a href="./cplusplus.html" class="enroll-btn">Learn More</a>
      </div>
    </div>
  </div>
</div>

<!-- Computer Science Fundamentals -->
<div class="course-category">
  <h2 class="category-title">📚 Computer Science Core</h2>
  
  <div class="courses-grid">
    <!-- Data Structures -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);">
        🗂️
      </div>
      <div class="course-content">
        <h3 class="course-title">Data Structures</h3>
        <p class="course-subtitle">Foundation of Efficient Programming</p>
        <ul class="course-features">
          <li>Arrays, Linked Lists, Stacks</li>
          <li>Trees & Graphs</li>
          <li>Hash Tables & Heaps</li>
          <li>Time & Space Complexity</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 12-18</span>
          <span class="level-tag">Intermediate</span>
        </div>
        <a href="./datastructure.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- Algorithms -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #06B6D4 0%, #3B82F6 100%);">
        🧮
      </div>
      <div class="course-content">
        <h3 class="course-title">Algorithms</h3>
        <p class="course-subtitle">Problem Solving & Optimization</p>
        <ul class="course-features">
          <li>Sorting & Searching</li>
          <li>Dynamic Programming</li>
          <li>Graph Algorithms</li>
          <li>Greedy & Divide-Conquer</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 13-18</span>
          <span class="level-tag">Advanced</span>
        </div>
        <a href="./algorithm.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- Machine Learning -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #F59E0B 0%, #EF4444 100%);">
        <div class="badge-container">
          <span class="new-badge">NEW</span>
        </div>
        🤖
      </div>
      <div class="course-content">
        <h3 class="course-title">Machine Learning & AI</h3>
        <p class="course-subtitle">Future of Technology</p>
        <ul class="course-features">
          <li>Neural Networks</li>
          <li>Deep Learning</li>
          <li>Computer Vision</li>
          <li>NLP & AI Projects</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 14-18</span>
          <span class="level-tag">Advanced</span>
        </div>
        <a href="./MachineLearning.html" class="enroll-btn">Learn More</a>
      </div>
    </div>
  </div>
</div>

<!-- Competition & Exam Prep -->
<div class="course-category">
  <h2 class="category-title">🏆 Competition & Exam Preparation</h2>
  
  <div class="courses-grid">
    <!-- AP CSA -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #10B981 0%, #059669 100%);">
        📘
      </div>
      <div class="course-content">
        <h3 class="course-title">AP Computer Science A</h3>
        <p class="course-subtitle">College-Level Java Programming</p>
        <ul class="course-features">
          <li>Complete AP CSA Curriculum</li>
          <li>Practice Exams</li>
          <li>FRQ Training</li>
          <li>Score 5 Guarantee Program</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 14-18</span>
          <span class="level-tag">Intermediate</span>
        </div>
        <a href="./APCSA.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- USACO -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);">
        <div class="badge-container">
          <span class="popular-badge">HOT</span>
        </div>
        🥇
      </div>
      <div class="course-content">
        <h3 class="course-title">USA Computing Olympiad</h3>
        <p class="course-subtitle">Path to Gold & Platinum</p>
        <ul class="course-features">
          <li>Bronze to Platinum Training</li>
          <li>Contest Strategy</li>
          <li>1000+ Practice Problems</li>
          <li>Mock Competitions</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 12-18</span>
          <span class="level-tag">All Levels</span>
        </div>
        <a href="./USACO.html" class="enroll-btn">Learn More</a>
      </div>
    </div>

    <!-- USAAIO -->
    <div class="course-card">
      <div class="course-image" style="background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);">
        <div class="badge-container">
          <span class="new-badge">NEW</span>
        </div>
        🧠
      </div>
      <div class="course-content">
        <h3 class="course-title">AI Olympiad Prep</h3>
        <p class="course-subtitle">USAAIO Competition Training</p>
        <ul class="course-features">
          <li>AI & ML Fundamentals</li>
          <li>Model Building</li>
          <li>Competition Projects</li>
          <li>Research Paper Writing</li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">Age: 14-18</span>
          <span class="level-tag">Advanced</span>
        </div>
        <a href="#" class="enroll-btn">Learn More</a>
      </div>
    </div>
  </div>
</div>

<!-- CTA Section -->
<div style="background: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%); border-radius: 20px; padding: 3rem; text-align: center; color: white; margin: 4rem 0;">
  <h2 style="font-size: 2rem; margin-bottom: 1rem;">Can't Find What You're Looking For?</h2>
  <p style="font-size: 1.1rem; margin-bottom: 2rem; opacity: 0.95;">
    We offer customized courses tailored to your specific needs and goals
  </p>
  <a href="./contact.html" style="background: white; color: #4F46E5; padding: 0.8rem 2rem; border-radius: 10px; text-decoration: none; font-weight: 600; display: inline-block; transition: transform 0.3s;">
    Contact Us for Custom Programs
  </a>
</div>
