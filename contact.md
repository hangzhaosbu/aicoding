---
layout: default
title: Contact Us
title_zh: 联系我们
description: Get in Touch with AIcoding Academy
description_zh: 与 AIcoding 学院取得联系
---

<style>
  /* Advanced Animations */
  @keyframes gradientWave {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-10px) rotate(-2deg); }
    75% { transform: translateY(10px) rotate(2deg); }
  }

  @keyframes shimmer {
    0% { left: -100%; }
    100% { left: 100%; }
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

  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
  }

  @keyframes rotate {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes shimmerGlow {
    0%, 100% {
      opacity: 0.3;
      transform: translate(-50%, -50%) scale(0.8);
    }
    50% {
      opacity: 0.6;
      transform: translate(-50%, -50%) scale(1.2);
    }
  }

  @keyframes diagonalSweep1 {
    0% {
      left: -150%;
      top: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      left: 50%;
      top: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      left: 150%;
      top: 110%;
      opacity: 0;
    }
  }

  @keyframes diagonalSweep2 {
    0% {
      right: -150%;
      bottom: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      right: 50%;
      bottom: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      right: 150%;
      bottom: 110%;
      opacity: 0;
    }
  }

  /* Contact Hero - Ultra Premium */
  .contact-hero {
    min-height: 50vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
  }

  .contact-hero::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotate 15s linear infinite;
    pointer-events: none;
  }

  .contact-hero::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 30%;
    width: 500px;
    height: 500px;
    background: radial-gradient(circle at center, rgba(255,255,255,0.3) 0%, rgba(255,255,255,0.15) 20%, transparent 60%);
    transform: translate(-50%, -50%);
    filter: blur(40px);
    animation: shimmerGlow 4s ease-in-out infinite;
    pointer-events: none;
  }

  /* Diagonal shimmer effects */
  .contact-hero .diagonal-shimmer-1,
  .contact-hero .diagonal-shimmer-2 {
    position: absolute;
    width: 150%;
    height: 20px;
    background: linear-gradient(90deg, 
      transparent 0%, 
      rgba(255,255,255,0.1) 20%,
      rgba(255,255,255,0.3) 50%, 
      rgba(255,255,255,0.1) 80%,
      transparent 100%);
    filter: blur(20px);
    pointer-events: none;
  }

  .contact-hero .diagonal-shimmer-1 {
    top: -10px;
    left: -150%;
    transform: rotate(45deg);
    animation: diagonalSweep1 8s ease-in-out infinite;
  }

  .contact-hero .diagonal-shimmer-2 {
    bottom: -10px;
    right: -150%;
    transform: rotate(-45deg);
    animation: diagonalSweep2 8s ease-in-out infinite;
    animation-delay: 4s;
  }

  .contact-title {
    font-size: 4rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
    animation: float 6s ease-in-out infinite;
  }

  .contact-subtitle {
    font-size: 1.4rem;
    color: rgba(255, 255, 255, 0.95);
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: relative;
    z-index: 1;
  }

  /* Quick Contact Cards - Premium */
  .quick-contact-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 5rem 0;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1200px) {
    .quick-contact-cards {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .quick-contact-cards {
      grid-template-columns: 1fr;
    }
  }

  .quick-card {
    background: white;
    padding: 3rem 2rem;
    border-radius: 25px;
    text-align: center;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.6s ease-out;
    border: 1px solid rgba(229, 231, 235, 0.5);
  }

  .quick-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.1), transparent);
    animation: shimmer 3s infinite;
  }

  .quick-card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.3);
    border-color: #667eea;
  }

  .quick-card-icon {
    font-size: 3.5rem;
    margin-bottom: 1.5rem;
    display: inline-block;
    animation: pulse 3s ease-in-out infinite;
  }

  .quick-card-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .quick-card-content {
    color: #6B7280;
    line-height: 1.6;
    font-size: 1.05rem;
  }

  /* Main Contact Container */
  .contact-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 2rem;
  }

  @media (max-width: 968px) {
    .contact-container {
      grid-template-columns: 1fr;
    }
  }

  /* Contact Form - Premium */
  .contact-form-section {
    background: white;
    padding: 3.5rem;
    border-radius: 30px;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.3);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out;
  }

  .contact-form-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    animation: shimmer 3s infinite;
  }

  .form-title {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    text-align: center;
  }

  .form-group {
    margin-bottom: 2rem;
  }

  .form-label {
    display: block;
    margin-bottom: 0.75rem;
    color: #4B5563;
    font-weight: 600;
    font-size: 1.05rem;
  }

  .form-label .required {
    color: #EF4444;
  }

  .form-input, .form-textarea {
    width: 100%;
    padding: 1rem;
    border: 2px solid #E5E7EB;
    border-radius: 12px;
    font-size: 1rem;
    transition: all 0.3s ease;
    font-family: inherit;
    background: rgba(249, 250, 251, 0.5);
  }

  .form-input:focus, .form-textarea:focus {
    outline: none;
    border-color: #667eea;
    box-shadow: 0 0 0 4px rgba(102, 126, 234, 0.1);
    background: white;
  }

  .form-textarea {
    min-height: 150px;
    resize: vertical;
  }

  .form-select {
    width: 100%;
    padding: 1rem;
    border: 2px solid #E5E7EB;
    border-radius: 12px;
    font-size: 1rem;
    background: rgba(249, 250, 251, 0.5);
    cursor: pointer;
    transition: all 0.3s ease;
  }

  .form-select:focus {
    outline: none;
    border-color: #667eea;
    box-shadow: 0 0 0 4px rgba(102, 126, 234, 0.1);
    background: white;
  }

  .submit-btn {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 1.2rem 3rem;
    border: none;
    border-radius: 50px;
    font-size: 1.2rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    width: 100%;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
    position: relative;
    overflow: hidden;
  }

  .submit-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s;
  }

  .submit-btn:hover::before {
    left: 100%;
  }

  .submit-btn:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 40px rgba(102, 126, 234, 0.4);
  }

  .submit-btn:disabled {
    opacity: 0.7;
    cursor: not-allowed;
    transform: none;
  }

  /* Success/Error Messages */
  .message {
    padding: 1.2rem;
    border-radius: 12px;
    margin-bottom: 1.5rem;
    display: none;
    animation: slideIn 0.3s ease;
    font-weight: 500;
  }

  .message.success {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    border: 2px solid #10B981;
    color: #065F46;
  }

  .message.error {
    background: linear-gradient(135deg, #FEF2F2 0%, #FEE2E2 100%);
    border: 2px solid #EF4444;
    color: #991B1B;
  }

  .message.show {
    display: block;
  }

  /* Contact Info Section - Premium */
  .contact-info-section {
    background: white;
    padding: 3.5rem;
    border-radius: 30px;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(229, 231, 235, 0.3);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out;
    animation-delay: 0.2s;
  }

  .info-title {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
    text-align: center;
  }

  .contact-method {
    display: flex;
    align-items: center;
    margin-bottom: 2.5rem;
    padding: 2rem;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .contact-method::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.05), transparent);
    transition: left 0.5s;
  }

  .contact-method:hover::before {
    left: 100%;
  }

  .contact-method:hover {
    transform: translateX(10px) scale(1.02);
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.15);
    background: linear-gradient(135deg, white 0%, #EEF2FF 100%);
  }

  .contact-icon {
    width: 70px;
    height: 70px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    margin-right: 2rem;
    flex-shrink: 0;
    box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
    animation: float 6s ease-in-out infinite;
  }
  
  /* iOS-style Phone Icon */
  .contact-icon.phone-icon {
    background: linear-gradient(135deg, #4ade80 0%, #22c55e 100%);
    box-shadow: 0 10px 25px rgba(34, 197, 94, 0.3);
  }
  
  /* WeChat Icon */
  .contact-icon.wechat-icon {
    background: linear-gradient(135deg, #07c160 0%, #06ae56 100%);
    box-shadow: 0 10px 25px rgba(7, 193, 96, 0.3);
  }

  .contact-details h3 {
    color: #1F2937;
    margin-bottom: 0.5rem;
    font-size: 1.5rem;
    font-weight: 700;
  }

  .contact-details p {
    color: #6B7280;
    margin: 0;
    font-size: 1.2rem;
    font-weight: 500;
  }

  .contact-details .action-link {
    color: #667eea;
    text-decoration: none;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    margin-top: 0.75rem;
    font-size: 1.05rem;
    transition: all 0.3s ease;
  }

  .contact-details .action-link:hover {
    color: #764ba2;
    transform: translateX(5px);
  }

  /* Office Hours - Premium */
  .office-hours {
    background: linear-gradient(135deg, #EEF2FF 0%, #DDD6FE 100%);
    padding: 2.5rem;
    border-radius: 20px;
    margin-top: 2rem;
    border: 2px solid rgba(139, 92, 246, 0.2);
    position: relative;
    overflow: hidden;
  }

  .office-hours::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(139, 92, 246, 0.1), transparent);
    animation: shimmer 8s infinite;
  }

  .office-hours h3 {
    color: #4F46E5;
    margin-bottom: 1.5rem;
    font-size: 1.5rem;
    font-weight: 700;
    position: relative;
    z-index: 1;
  }

  .hours-list {
    list-style: none;
    position: relative;
    z-index: 1;
  }

  .hours-list li {
    display: flex;
    justify-content: space-between;
    padding: 1rem 0;
    color: #4B5563;
    font-size: 1.05rem;
    border-bottom: 1px solid rgba(139, 92, 246, 0.1);
    transition: all 0.3s ease;
  }

  .hours-list li:hover {
    padding-left: 1rem;
    color: #1F2937;
  }

  .hours-list li:last-child {
    border-bottom: none;
  }

  /* FAQ Section - Premium */
  .faq-section {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 5rem 3rem;
    border-radius: 30px;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
  }

  .faq-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(102, 126, 234, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(236, 72, 153, 0.05), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .faq-title {
    text-align: center;
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .faq-title::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 100px;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2);
    border-radius: 3px;
  }

  .faq-item {
    background: white;
    padding: 2.5rem;
    border-radius: 20px;
    margin-bottom: 1.5rem;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border-left: 4px solid #667eea;
  }

  .faq-item:hover {
    transform: translateX(10px);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.12);
  }

  .faq-question {
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    font-size: 1.3rem;
  }

  .faq-answer {
    color: #6B7280;
    line-height: 1.8;
    font-size: 1.05rem;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .contact-title {
      font-size: 2.5rem;
    }

    .quick-contact-cards {
      grid-template-columns: 1fr;
    }

    .contact-container {
      grid-template-columns: 1fr;
    }

    .faq-title {
      font-size: 2rem;
    }
  }
</style>

<!-- Contact Hero -->
<div class="contact-hero">
  <div class="diagonal-shimmer-1"></div>
  <div class="diagonal-shimmer-2"></div>
  <h1 class="contact-title">
    <span class="en-content">Let's Start Your Coding Journey</span>
    <span class="zh-content">开启您的编程之旅</span>
  </h1>
  <p class="contact-subtitle">
    <span class="en-content">We're here to answer your questions and help you succeed</span>
    <span class="zh-content">我们在这里回答您的问题并帮助您成功</span>
  </p>
</div>

<!-- Quick Contact Cards -->
<div class="quick-contact-cards">
  <div class="quick-card">
    <div class="quick-card-icon">⚡</div>
    <h3 class="quick-card-title">
      <span class="en-content">Quick Response</span>
      <span class="zh-content">快速响应</span>
    </h3>
    <p class="quick-card-content">
      <span class="en-content">We typically respond within 24 hours</span>
      <span class="zh-content">我们通常在24小时内回复</span>
    </p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">🌍</div>
    <h3 class="quick-card-title">
      <span class="en-content">Global Service</span>
      <span class="zh-content">全球服务</span>
    </h3>
    <p class="quick-card-content">
      <span class="en-content">Supporting students from US & China</span>
      <span class="zh-content">为美国和中国的学生提供支持</span>
    </p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">💬</div>
    <h3 class="quick-card-title">
      <span class="en-content">Bilingual Support</span>
      <span class="zh-content">双语支持</span>
    </h3>
    <p class="quick-card-content">
      <span class="en-content">English & Chinese communication available</span>
      <span class="zh-content">提供英文和中文沟通服务</span>
    </p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">📅</div>
    <h3 class="quick-card-title">
      <span class="en-content">Flexible Schedule</span>
      <span class="zh-content">灵活安排</span>
    </h3>
    <p class="quick-card-content">
      <span class="en-content">Classes available across time zones</span>
      <span class="zh-content">跨时区授课</span>
    </p>
  </div>
</div>

<!-- Main Contact Section -->
<div class="contact-container">
  <!-- Contact Form -->
  <div class="contact-form-section">
    <h2 class="form-title">
      <span class="en-content">Send Us a Message</span>
      <span class="zh-content">发送消息</span>
    </h2>
    
    <div id="successMessage" class="message success">
      <span class="en-content">✅ Thank you for your message! We'll get back to you soon.</span>
      <span class="zh-content">✅ 感谢您的消息！我们会尽快回复您。</span>
    </div>
    
    <div id="errorMessage" class="message error">
      <span class="en-content">❌ There was an error sending your message. Please try again.</span>
      <span class="zh-content">❌ 发送消息时出错。请重试。</span>
    </div>
    
    <form id="contactForm">
      <input type="hidden" name="_subject" value="New contact from AIcoding Academy">
      <div class="form-group">
        <label class="form-label" for="name">
          <span class="en-content">Full Name <span class="required">*</span></span>
          <span class="zh-content">姓名 <span class="required">*</span></span>
        </label>
        <input type="text" id="name" name="name" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="email">
          <span class="en-content">Email Address <span class="required">*</span></span>
          <span class="zh-content">电子邮箱 <span class="required">*</span></span>
        </label>
        <input type="email" id="email" name="email" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="phone">
          <span class="en-content">Phone Number</span>
          <span class="zh-content">电话号码</span>
        </label>
        <input type="tel" id="phone" name="phone" class="form-input">
      </div>
      
      <div class="form-group">
        <label class="form-label" for="course">
          <span class="en-content">Course Interest</span>
          <span class="zh-content">感兴趣的课程</span>
        </label>
        <select id="course" name="course" class="form-select">
          <option value="">
            <span class="en-content">Select a course...</span>
            <span class="zh-content">选择课程...</span>
          </option>
          <option value="python">
            <span class="en-content">Python Programming</span>
            <span class="zh-content">Python 编程</span>
          </option>
          <option value="java">
            <span class="en-content">Java Programming</span>
            <span class="zh-content">Java 编程</span>
          </option>
          <option value="cpp">
            <span class="en-content">C++ Programming</span>
            <span class="zh-content">C++ 编程</span>
          </option>
          <option value="usaco">
            <span class="en-content">USACO Prep</span>
            <span class="zh-content">USACO 准备</span>
          </option>
          <option value="apcsa">
            <span class="en-content">AP Computer Science A</span>
            <span class="zh-content">AP 计算机科学 A</span>
          </option>
          <option value="apcsp">
            <span class="en-content">AP Computer Science Principles</span>
            <span class="zh-content">AP 计算机科学原理</span>
          </option>
          <option value="ml">
            <span class="en-content">Machine Learning & AI</span>
            <span class="zh-content">机器学习与人工智能</span>
          </option>
          <option value="other">
            <span class="en-content">Other / Custom Program</span>
            <span class="zh-content">其他 / 定制课程</span>
          </option>
        </select>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="message">
          <span class="en-content">Message <span class="required">*</span></span>
          <span class="zh-content">留言 <span class="required">*</span></span>
        </label>
        <textarea id="message" name="message" class="form-textarea" required 
          placeholder="Tell us about your goals and how we can help..."
          data-placeholder-en="Tell us about your goals and how we can help..."
          data-placeholder-zh="请告诉我们您的目标以及我们如何帮助您..."></textarea>
      </div>
      
      <button type="submit" class="submit-btn" id="submitBtn">
        <span class="en-content">Send Message</span>
        <span class="zh-content">发送消息</span>
      </button>
    </form>
  </div>
  
  <!-- Contact Info -->
  <div class="contact-info-section">
    <h2 class="info-title">
      <span class="en-content">Get in Touch</span>
      <span class="zh-content">联系方式</span>
    </h2>
    
    <!-- Phone -->
    <div class="contact-method">
      <div class="contact-icon phone-icon">
        <svg width="30" height="30" viewBox="0 0 24 24" fill="white">
          <path d="M20.01 15.38c-1.23 0-2.42-.2-3.53-.56a.977.977 0 0 0-1.01.24l-1.57 1.97c-2.83-1.35-5.48-3.9-6.89-6.83l1.95-1.66c.27-.28.35-.67.24-1.02-.37-1.11-.56-2.3-.56-3.53 0-.54-.45-.99-.99-.99H4.19C3.65 3 3 3.24 3 3.99 3 13.28 10.73 21 20.01 21c.71 0 .99-.63.99-1.18v-3.45c0-.54-.45-.99-.99-.99z"/>
        </svg>
      </div>
      <div class="contact-details">
        <h3>
          <span class="en-content">Phone</span>
          <span class="zh-content">电话</span>
        </h3>
        <p>+1 (347) 379-6896</p>
        <a href="tel:+13473796896" class="action-link">
          <span class="en-content">Call Now →</span>
          <span class="zh-content">立即致电 →</span>
        </a>
      </div>
    </div>
    
    <!-- WeChat -->
    <div class="contact-method">
      <div class="contact-icon wechat-icon">
        <svg width="30" height="30" viewBox="0 0 24 24" fill="white">
          <path d="M15.85 8.14c.39 0 .77.03 1.14.08C16.31 5.25 13.19 3 9.44 3c-4.25 0-7.7 2.88-7.7 6.43 0 2.05 1.15 3.86 2.94 5.04L3.67 16.5l2.76-1.19c.59.21 1.21.38 1.87.47-.09-.39-.14-.79-.14-1.21-.01-3.77 3.69-6.43 7.69-6.43zM12 5.89c.57 0 1.04.46 1.04 1.04s-.46 1.04-1.04 1.04-1.04-.46-1.04-1.04.47-1.04 1.04-1.04zM6.63 7.96c-.57 0-1.04-.46-1.04-1.04s.46-1.04 1.04-1.04c.57 0 1.04.46 1.04 1.04s-.46 1.04-1.04 1.04z"/>
          <path d="M22.26 14.57c0-2.84-2.87-5.14-6.41-5.14s-6.41 2.3-6.41 5.14 2.87 5.14 6.41 5.14c.58 0 1.14-.08 1.67-.2L20.98 21l-1.2-2.4c1.5-.94 2.48-2.38 2.48-4.03zm-8.34-.51c-.41 0-.74-.33-.74-.74s.33-.74.74-.74.74.33.74.74-.33.74-.74.74zm3.85 0c-.41 0-.74-.33-.74-.74s.33-.74.74-.74.74.33.74.74-.32.74-.74.74z"/>
        </svg>
      </div>
      <div class="contact-details">
        <h3>
          <span class="en-content">WeChat</span>
          <span class="zh-content">微信</span>
        </h3>
        <p>SpiritedAway2023</p>
        <span class="action-link">
          <span class="en-content">Add on WeChat →</span>
          <span class="zh-content">添加微信 →</span>
        </span>
      </div>
    </div>
    
    <!-- Office Hours -->
    <div class="office-hours">
      <h3>
        <span class="en-content">🕐 Office Hours (PST)</span>
        <span class="zh-content">🕐 办公时间 (美西时间)</span>
      </h3>
      <ul class="hours-list">
        <li>
          <span>
            <span class="en-content">Monday - Friday</span>
            <span class="zh-content">周一至周五</span>
          </span>
          <span>9:00 AM - 9:00 PM</span>
        </li>
        <li>
          <span>
            <span class="en-content">Saturday - Sunday</span>
            <span class="zh-content">周六至周日</span>
          </span>
          <span>10:00 AM - 6:00 PM</span>
        </li>
        <li>
          <span>
            <span class="en-content">China Time Zone</span>
            <span class="zh-content">中国时区</span>
          </span>
          <span>
            <span class="en-content">Flexible Hours Available</span>
            <span class="zh-content">灵活安排时间</span>
          </span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- FAQ Section -->
<div class="faq-section">
  <h2 class="faq-title">
    <span class="en-content">Frequently Asked Questions</span>
    <span class="zh-content">常见问题</span>
  </h2>
  
  <div class="faq-item">
    <div class="faq-question">
      <span class="en-content">What age groups do you teach?</span>
      <span class="zh-content">你们教哪些年龄段的学生？</span>
    </div>
    <div class="faq-answer">
      <span class="en-content">We offer courses for students aged 10-18, as well as undergraduate and graduate students. Our curriculum is tailored to different skill levels and age-appropriate learning objectives.</span>
      <span class="zh-content">我们为10-18岁的学生以及本科生和研究生提供课程。我们的课程根据不同的技能水平和适合年龄的学习目标量身定制。</span>
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">
      <span class="en-content">Do you offer trial classes?</span>
      <span class="zh-content">你们提供试听课吗？</span>
    </div>
    <div class="faq-answer">
      <span class="en-content">Yes! We offer a free consultation session to assess your needs and recommend the best learning path. Contact us to schedule your trial class.</span>
      <span class="zh-content">是的！我们提供免费的咨询课程来评估您的需求并推荐最佳的学习路径。请联系我们安排试听课。</span>
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">
      <span class="en-content">What's the class format?</span>
      <span class="zh-content">课程形式是怎样的？</span>
    </div>
    <div class="faq-answer">
      <span class="en-content">We offer both one-on-one and small group classes (max 4 students) via online platforms. All classes are interactive with screen sharing, coding exercises, and real-time feedback.</span>
      <span class="zh-content">我们通过在线平台提供一对一和小班课程（最多4名学生）。所有课程都是互动式的，包括屏幕共享、编程练习和实时反馈。</span>
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">
      <span class="en-content">Can you help with competition preparation?</span>
      <span class="zh-content">你们能帮助准备竞赛吗？</span>
    </div>
    <div class="faq-answer">
      <span class="en-content">Absolutely! We specialize in USACO, USAAIO, AMC, ACSL, and other competitions. Our instructors have extensive experience and proven track records in competition coaching.</span>
      <span class="zh-content">当然可以！我们专门从事USACO、USAAIO、AMC、ACSL和其他竞赛的培训。我们的导师在竞赛辅导方面有丰富的经验和优秀的成绩记录。</span>
    </div>
  </div>
</div>

<!-- EmailJS SDK -->
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>

<script>
  // Initialize EmailJS with your public key
  (function(){
    // Your EmailJS public key
    emailjs.init("AoNX_tjdsa7y4pIhr"); 
  })();
  
  // Language switching functionality
  document.addEventListener('DOMContentLoaded', function() {
    // Function to update select options based on language
    function updateSelectOptions() {
      const selects = document.querySelectorAll('select');
      const isZh = localStorage.getItem('language') === 'zh';
      
      selects.forEach(select => {
        const options = select.querySelectorAll('option');
        options.forEach(option => {
          const enText = option.querySelector('.en-content')?.textContent;
          const zhText = option.querySelector('.zh-content')?.textContent;
          
          if (enText && zhText) {
            option.textContent = isZh ? zhText : enText;
          }
        });
      });
    }
    
    // Function to update placeholder based on language
    function updatePlaceholders() {
      const isZh = localStorage.getItem('language') === 'zh';
      const textarea = document.getElementById('message');
      
      if (textarea) {
        const enPlaceholder = textarea.getAttribute('data-placeholder-en');
        const zhPlaceholder = textarea.getAttribute('data-placeholder-zh');
        textarea.placeholder = isZh ? zhPlaceholder : enPlaceholder;
      }
    }
    
    // Initial setup
    updateSelectOptions();
    updatePlaceholders();
    
    // Listen for storage changes (language toggle)
    window.addEventListener('storage', function(e) {
      if (e.key === 'language') {
        updateSelectOptions();
        updatePlaceholders();
      }
    });
    
    // Also check periodically for language changes
    setInterval(function() {
      const currentLang = localStorage.getItem('language');
      const textarea = document.getElementById('message');
      if (textarea) {
        const isZh = currentLang === 'zh' || document.documentElement.lang === 'zh';
        const enPlaceholder = textarea.getAttribute('data-placeholder-en');
        const zhPlaceholder = textarea.getAttribute('data-placeholder-zh');
        const newPlaceholder = isZh ? zhPlaceholder : enPlaceholder;
        if (textarea.placeholder !== newPlaceholder) {
          textarea.placeholder = newPlaceholder;
          updateSelectOptions();
        }
      }
    }, 500);
  });
  
  // Form submission handler with EmailJS
  const form = document.getElementById('contactForm');
  const submitBtn = document.getElementById('submitBtn');
  const successMessage = document.getElementById('successMessage');
  const errorMessage = document.getElementById('errorMessage');
  
  form.addEventListener('submit', async function(e) {
    e.preventDefault();
    
    // Disable submit button
    submitBtn.disabled = true;
    submitBtn.innerHTML = '<span class="en-content">Sending...</span><span class="zh-content">发送中...</span>';
    
    // Prepare template params
    const templateParams = {
      from_name: form.name.value,
      from_email: form.email.value,
      phone: form.phone.value || 'Not provided',
      course: form.course.value || 'Not specified',
      message: form.message.value,
      to_email: 'hangzhao2021@gmail.com'
    };
    
    try {
      // Send email using EmailJS
      // REPLACE: "YOUR_SERVICE_ID" with "service_pgmmr85" (your Gmail service ID)
      // REPLACE: "YOUR_TEMPLATE_ID" with your actual template ID
      const response = await emailjs.send("service_pgmmr85", "template_iaomvs8", templateParams);
      
      if (response.status === 200) {
        // Show success message
        successMessage.classList.add('show');
        errorMessage.classList.remove('show');
        
        // Reset form
        form.reset();
        
        // Hide message after 5 seconds
        setTimeout(() => {
          successMessage.classList.remove('show');
        }, 5000);
      } else {
        throw new Error('Failed to send email');
      }
      
    } catch (error) {
      console.error('EmailJS Error:', error);
      
      // Fallback to mailto if EmailJS fails
      const subject = `New Contact from AIcoding Academy - ${form.name.value}`;
      const body = `
Name: ${form.name.value}
Email: ${form.email.value}
Phone: ${form.phone.value || 'Not provided'}
Course Interest: ${form.course.value || 'Not specified'}

Message:
${form.message.value}
      `;
      
      // Create mailto link as fallback
      const mailtoLink = `mailto:hangzhao2021@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
      window.location.href = mailtoLink;
      
      // Show error but explain fallback was used
      errorMessage.innerHTML = '<span class="en-content">⚠️ Direct send failed. Opening your email client instead.</span><span class="zh-content">⚠️ 直接发送失败。正在打开您的邮件客户端。</span>';
      errorMessage.classList.add('show');
      successMessage.classList.remove('show');
      
      setTimeout(() => {
        errorMessage.classList.remove('show');
      }, 5000);
    } finally {
      // Re-enable submit button
      submitBtn.disabled = false;
      submitBtn.innerHTML = '<span class="en-content">Send Message</span><span class="zh-content">发送消息</span>';
    }
  });
</script>
