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
  <h1 class="contact-title">Let's Start Your Coding Journey</h1>
  <p class="contact-subtitle">We're here to answer your questions and help you succeed</p>
</div>

<!-- Quick Contact Cards -->
<div class="quick-contact-cards">
  <div class="quick-card">
    <div class="quick-card-icon">⚡</div>
    <h3 class="quick-card-title">Quick Response</h3>
    <p class="quick-card-content">We typically respond within 24 hours</p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">🌍</div>
    <h3 class="quick-card-title">Global Service</h3>
    <p class="quick-card-content">Supporting students from US & China</p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">💬</div>
    <h3 class="quick-card-title">Bilingual Support</h3>
    <p class="quick-card-content">English & Chinese communication available</p>
  </div>
  
  <div class="quick-card">
    <div class="quick-card-icon">📅</div>
    <h3 class="quick-card-title">Flexible Schedule</h3>
    <p class="quick-card-content">Classes available across time zones</p>
  </div>
</div>

<!-- Main Contact Section -->
<div class="contact-container">
  <!-- Contact Form -->
  <div class="contact-form-section">
    <h2 class="form-title">Send Us a Message</h2>
    
    <div id="responseMessage" class="response-message">
      Thank you for your message! We'll get back to you soon.
    </div>
    
    <form id="contactForm">
      <div class="form-group">
        <label class="form-label" for="name">Full Name *</label>
        <input type="text" id="name" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="email">Email Address *</label>
        <input type="email" id="email" class="form-input" required>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="phone">Phone Number</label>
        <input type="tel" id="phone" class="form-input">
      </div>
      
      <div class="form-group">
        <label class="form-label" for="course">Course Interest</label>
        <select id="course" class="form-select">
          <option value="">Select a course...</option>
          <option value="python">Python Programming</option>
          <option value="java">Java Programming</option>
          <option value="cpp">C++ Programming</option>
          <option value="usaco">USACO Prep</option>
          <option value="apcsa">AP Computer Science A</option>
          <option value="ml">Machine Learning & AI</option>
          <option value="other">Other / Custom Program</option>
        </select>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="message">Message *</label>
        <textarea id="message" class="form-textarea" required placeholder="Tell us about your goals and how we can help..."></textarea>
      </div>
      
      <button type="submit" class="submit-btn">Send Message</button>
    </form>
  </div>
  
  <!-- Contact Info -->
  <div class="contact-info-section">
    <h2 class="info-title">Get in Touch</h2>
    
    <!-- Phone -->
    <div class="contact-method">
      <div class="contact-icon">📱</div>
      <div class="contact-details">
        <h3>Phone</h3>
        <p>+1 (347) 379-6896</p>
        <a href="tel:+13473796896" class="action-link">Call Now →</a>
      </div>
    </div>
    
    <!-- WeChat -->
    <div class="contact-method">
      <div class="contact-icon">💬</div>
      <div class="contact-details">
        <h3>WeChat</h3>
        <p>SpiritedAway2023</p>
        <span class="action-link">Add on WeChat →</span>
      </div>
    </div>
    
    <!-- Email -->
    <div class="contact-method">
      <div class="contact-icon">✉️</div>
      <div class="contact-details">
        <h3>Email</h3>
        <p>contact@aicodingacademy.com</p>
        <a href="mailto:contact@aicodingacademy.com" class="action-link">Send Email →</a>
      </div>
    </div>
    
    <!-- Office Hours -->
    <div class="office-hours">
      <h3>🕐 Office Hours (EST)</h3>
      <ul class="hours-list">
        <li>
          <span>Monday - Friday</span>
          <span>9:00 AM - 9:00 PM</span>
        </li>
        <li>
          <span>Saturday - Sunday</span>
          <span>10:00 AM - 6:00 PM</span>
        </li>
        <li>
          <span>China Time Zone</span>
          <span>Flexible Hours Available</span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- FAQ Section -->
<div class="faq-section">
  <h2 class="faq-title">Frequently Asked Questions</h2>
  
  <div class="faq-item">
    <div class="faq-question">What age groups do you teach?</div>
    <div class="faq-answer">
      We offer courses for students aged 10-18, as well as undergraduate and graduate students. Our curriculum is tailored to different skill levels and age-appropriate learning objectives.
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">Do you offer trial classes?</div>
    <div class="faq-answer">
      Yes! We offer a free consultation session to assess your needs and recommend the best learning path. Contact us to schedule your trial class.
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">What's the class format?</div>
    <div class="faq-answer">
      We offer both one-on-one and small group classes (max 4 students) via online platforms. All classes are interactive with screen sharing, coding exercises, and real-time feedback.
    </div>
  </div>
  
  <div class="faq-item">
    <div class="faq-question">Can you help with competition preparation?</div>
    <div class="faq-answer">
      Absolutely! We specialize in USACO, USAAIO, AMC, ACSL, and other competitions. Our instructors have extensive experience and proven track records in competition coaching.
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
