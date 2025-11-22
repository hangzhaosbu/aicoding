---
layout: default
title: Contact Us
description: Get in Touch with AIcoding Academy
---

<style>
  /* Contact Page Styles */
  .contact-hero {
    text-align: center;
    padding: 3rem 0;
    margin-bottom: 3rem;
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    border-radius: 20px;
  }

  .contact-title {
    font-size: 2.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 1rem;
  }

  .contact-subtitle {
    font-size: 1.2rem;
    color: #6B7280;
  }

  .contact-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    max-width: 1200px;
    margin: 0 auto;
  }

  /* Contact Form */
  .contact-form-section {
    background: white;
    padding: 2.5rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 1px solid #E5E7EB;
  }

  .form-title {
    font-size: 1.8rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 1.5rem;
  }

  .form-group {
    margin-bottom: 1.5rem;
  }

  .form-label {
    display: block;
    margin-bottom: 0.5rem;
    color: #4B5563;
    font-weight: 500;
  }

  .form-input, .form-textarea {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #D1D5DB;
    border-radius: 8px;
    font-size: 1rem;
    transition: all 0.3s;
    font-family: inherit;
  }

  .form-input:focus, .form-textarea:focus {
    outline: none;
    border-color: #4F46E5;
    box-shadow: 0 0 0 3px rgba(79, 70, 229, 0.1);
  }

  .form-textarea {
    min-height: 120px;
    resize: vertical;
  }

  .form-select {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #D1D5DB;
    border-radius: 8px;
    font-size: 1rem;
    background: white;
    cursor: pointer;
  }

  .submit-btn {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 0.75rem 2rem;
    border: none;
    border-radius: 8px;
    font-size: 1.1rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s;
    width: 100%;
  }

  .submit-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(102, 126, 234, 0.3);
  }

  /* Contact Info Section */
  .contact-info-section {
    background: white;
    padding: 2.5rem;
    border-radius: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
    border: 1px solid #E5E7EB;
  }

  .info-title {
    font-size: 1.8rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 1.5rem;
  }

  .contact-method {
    display: flex;
    align-items: center;
    margin-bottom: 2rem;
    padding: 1.5rem;
    background: #F9FAFB;
    border-radius: 12px;
    transition: all 0.3s;
  }

  .contact-method:hover {
    background: #F3F4F6;
    transform: translateX(5px);
  }

  .contact-icon {
    width: 50px;
    height: 50px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    margin-right: 1.5rem;
    flex-shrink: 0;
  }

  .contact-details h3 {
    color: #1F2937;
    margin-bottom: 0.5rem;
    font-size: 1.2rem;
  }

  .contact-details p {
    color: #6B7280;
    margin: 0;
    font-size: 1.1rem;
  }

  .contact-details .action-link {
    color: #4F46E5;
    text-decoration: none;
    font-weight: 500;
    display: inline-flex;
    align-items: center;
    margin-top: 0.5rem;
  }

  .contact-details .action-link:hover {
    text-decoration: underline;
  }

  /* Quick Contact Cards */
  .quick-contact-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin: 3rem 0;
  }

  .quick-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    text-align: center;
    border: 2px solid #E5E7EB;
    transition: all 0.3s;
  }

  .quick-card:hover {
    border-color: #4F46E5;
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .quick-card-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .quick-card-title {
    font-size: 1.2rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .quick-card-content {
    color: #6B7280;
    line-height: 1.6;
  }

  /* FAQ Section */
  .faq-section {
    background: #F9FAFB;
    padding: 3rem;
    border-radius: 15px;
    margin: 3rem 0;
  }

  .faq-title {
    text-align: center;
    font-size: 2rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 2rem;
  }

  .faq-item {
    background: white;
    padding: 1.5rem;
    border-radius: 10px;
    margin-bottom: 1rem;
    border: 1px solid #E5E7EB;
  }

  .faq-question {
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
    font-size: 1.1rem;
  }

  .faq-answer {
    color: #6B7280;
    line-height: 1.6;
  }

  /* Response Message */
  .response-message {
    background: #ECFDF5;
    border: 1px solid #10B981;
    color: #065F46;
    padding: 1rem;
    border-radius: 8px;
    margin-bottom: 1rem;
    display: none;
  }

  .response-message.show {
    display: block;
    animation: slideIn 0.3s ease;
  }

  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateY(-10px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  /* Office Hours */
  .office-hours {
    background: #EEF2FF;
    padding: 1.5rem;
    border-radius: 10px;
    margin-top: 1.5rem;
  }

  .office-hours h3 {
    color: #4F46E5;
    margin-bottom: 1rem;
    font-size: 1.2rem;
  }

  .hours-list {
    list-style: none;
  }

  .hours-list li {
    display: flex;
    justify-content: space-between;
    padding: 0.5rem 0;
    color: #4B5563;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .contact-container {
      grid-template-columns: 1fr;
    }

    .contact-title {
      font-size: 2rem;
    }

    .quick-contact-cards {
      grid-template-columns: 1fr;
    }
  }
</style>

<!-- Contact Hero -->
<div class="contact-hero">
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
    
    <div id="responseMessage" class="response-message">
      <span class="en-content">Thank you for your message! We'll get back to you soon.</span>
      <span class="zh-content">感谢您的消息！我们会尽快回复您。</span>
    </div>
    
    <form id="contactForm">
      <div class="form-group">
        <label class="form-label" for="name">
          <span class="en-content">Full Name *</span>
          <span class="zh-content">姓名 *</span>
        </label>
        <input type="text" id="name" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="email">
          <span class="en-content">Email Address *</span>
          <span class="zh-content">电子邮箱 *</span>
        </label>
        <input type="email" id="email" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="phone">
          <span class="en-content">Phone Number</span>
          <span class="zh-content">电话号码</span>
        </label>
        <input type="tel" id="phone" class="form-input">
      </div>
      
      <div class="form-group">
        <label class="form-label" for="course">
          <span class="en-content">Course Interest</span>
          <span class="zh-content">感兴趣的课程</span>
        </label>
        <select id="course" class="form-select">
          <option value="">
            <span class="en-content">Select a course...</span>
            <span class="zh-content">选择课程...</span>
          </option>
          <option value="python">
            <span class="en-content">Python Programming</span>
            <span class="zh-content">Python编程</span>
          </option>
          <option value="java">
            <span class="en-content">Java Programming</span>
            <span class="zh-content">Java编程</span>
          </option>
          <option value="cpp">
            <span class="en-content">C++ Programming</span>
            <span class="zh-content">C++编程</span>
          </option>
          <option value="usaco">
            <span class="en-content">USACO Prep</span>
            <span class="zh-content">USACO准备</span>
          </option>
          <option value="apcsa">AP Computer Science A</option>
          <option value="ml">
            <span class="en-content">Machine Learning & AI</span>
            <span class="zh-content">机器学习与人工智能</span>
          </option>
          <option value="other">
            <span class="en-content">Other / Custom Program</span>
            <span class="zh-content">其他/定制课程</span>
          </option>
        </select>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="message">
          <span class="en-content">Message *</span>
          <span class="zh-content">留言 *</span>
        </label>
        <textarea id="message" class="form-textarea" required 
          placeholder="Tell us about your goals and how we can help..."></textarea>
      </div>
      
      <button type="submit" class="submit-btn">
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
      <div class="contact-icon">📱</div>
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
      <div class="contact-icon">💬</div>
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
    
    <!-- Email -->
    <div class="contact-method">
      <div class="contact-icon">✉️</div>
      <div class="contact-details">
        <h3>
          <span class="en-content">Email</span>
          <span class="zh-content">邮箱</span>
        </h3>
        <p>hangzhao2021@gmail.com</p>
        <a href="mailto:hangzhao2021@gmail.com" class="action-link">
          <span class="en-content">Send Email →</span>
          <span class="zh-content">发送邮件 →</span>
        </a>
      </div>
    </div>
    
    <!-- Office Hours -->
    <div class="office-hours">
      <h3>
        <span class="en-content">🕐 Office Hours (EST)</span>
        <span class="zh-content">🕐 办公时间 (美东时间)</span>
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

<script>
  // Form submission handler
  document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();
    
    // Show success message
    const message = document.getElementById('responseMessage');
    message.classList.add('show');
    
    // Reset form
    this.reset();
    
    // Hide message after 5 seconds
    setTimeout(() => {
      message.classList.remove('show');
    }, 5000);
  });
</script>

