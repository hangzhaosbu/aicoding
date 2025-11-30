---
layout: default
title: Contact Us
title_zh: 联系我们
description: Get in Touch with AIcoding Edu
description_zh: 与 AIcoding 学院取得联系
---

<style>
  /* ========================================
     Premium Animation Library
  ======================================== */
  @keyframes gradientFlow {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-15px) rotate(-2deg); }
    75% { transform: translateY(15px) rotate(2deg); }
  }

  @keyframes floatReverse {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(15px) rotate(2deg); }
    75% { transform: translateY(-15px) rotate(-2deg); }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50% { transform: scale(1.08); opacity: 0.9; }
  }

  @keyframes shimmer {
    0% { left: -100%; opacity: 0; }
    50% { opacity: 1; }
    100% { left: 100%; opacity: 0; }
  }

  @keyframes slideInUp {
    from { opacity: 0; transform: translateY(50px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes slideInLeft {
    from { opacity: 0; transform: translateX(-50px); }
    to { opacity: 1; transform: translateX(0); }
  }

  @keyframes slideInRight {
    from { opacity: 0; transform: translateX(50px); }
    to { opacity: 1; transform: translateX(0); }
  }

  @keyframes rotateGlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes morphBlob {
    0%, 100% { border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; }
    25% { border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%; }
    50% { border-radius: 50% 60% 30% 60% / 30% 60% 70% 40%; }
    75% { border-radius: 60% 40% 60% 30% / 70% 30% 50% 60%; }
  }

  @keyframes starTwinkle {
    0%, 100% { opacity: 0.2; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.5); }
  }

  @keyframes particleFloat {
    0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.6; }
    25% { transform: translate(15px, -25px) scale(1.2); opacity: 1; }
    50% { transform: translate(-10px, -50px) scale(0.8); opacity: 0.8; }
    75% { transform: translate(-20px, -25px) scale(1.1); opacity: 0.9; }
  }

  @keyframes borderGlow {
    0%, 100% { box-shadow: 0 0 20px rgba(99, 102, 241, 0.3); }
    50% { box-shadow: 0 0 40px rgba(99, 102, 241, 0.6); }
  }

  @keyframes cardEntrance {
    from { opacity: 0; transform: translateY(40px) scale(0.95); }
    to { opacity: 1; transform: translateY(0) scale(1); }
  }

  @keyframes iconBounce {
    0%, 100% { transform: translateY(0) scale(1); }
    50% { transform: translateY(-10px) scale(1.1); }
  }

  @keyframes textGradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes inputFocus {
    0% { box-shadow: 0 0 0 0 rgba(99, 102, 241, 0.4); }
    100% { box-shadow: 0 0 0 8px rgba(99, 102, 241, 0); }
  }

  @keyframes successPop {
    0% { transform: scale(0.8); opacity: 0; }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); opacity: 1; }
  }

  @keyframes typing {
    from { width: 0; }
    to { width: 100%; }
  }

  @keyframes blink {
    50% { border-color: transparent; }
  }

  @keyframes ripple {
    0% { transform: scale(0.8); opacity: 1; }
    100% { transform: scale(2.5); opacity: 0; }
  }

  @keyframes glowPulse {
    0%, 100% { filter: drop-shadow(0 0 10px currentColor); }
    50% { filter: drop-shadow(0 0 25px currentColor); }
  }

  @keyframes shake {
    0%, 100% { transform: translateX(0); }
    10%, 30%, 50%, 70%, 90% { transform: translateX(-5px); }
    20%, 40%, 60%, 80% { transform: translateX(5px); }
  }

  /* ========================================
     Contact Hero - Ultra Premium
  ======================================== */
  .contact-hero {
    min-height: 55vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, 
      #0f0c29 0%, 
      #302b63 25%, 
      #24243e 50%,
      #1a1a2e 75%,
      #0f0c29 100%);
    background-size: 400% 400%;
    animation: gradientFlow 20s ease infinite;
    border-radius: 40px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 50px 100px rgba(0, 0, 0, 0.5),
      inset 0 0 100px rgba(99, 102, 241, 0.1);
  }

  /* Aurora Effect */
  .hero-aurora {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .hero-aurora::before,
  .hero-aurora::after {
    content: '';
    position: absolute;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
  }

  .hero-aurora::before {
    background: conic-gradient(
      from 0deg at 50% 50%,
      transparent 0deg,
      rgba(99, 102, 241, 0.15) 60deg,
      transparent 120deg,
      rgba(139, 92, 246, 0.1) 180deg,
      transparent 240deg,
      rgba(236, 72, 153, 0.08) 300deg,
      transparent 360deg
    );
    animation: rotateGlow 30s linear infinite;
  }

  .hero-aurora::after {
    background: conic-gradient(
      from 180deg at 50% 50%,
      transparent 0deg,
      rgba(6, 182, 212, 0.1) 90deg,
      transparent 180deg,
      rgba(16, 185, 129, 0.08) 270deg,
      transparent 360deg
    );
    animation: rotateGlow 25s linear infinite reverse;
  }

  /* Morphing Orbs */
  .hero-orbs {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
    overflow: hidden;
  }

  .hero-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.4;
    animation: morphBlob 20s ease-in-out infinite, float 15s ease-in-out infinite;
  }

  .hero-orb:nth-child(1) {
    width: 450px;
    height: 450px;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.6), rgba(139, 92, 246, 0.4));
    top: -150px;
    left: -100px;
  }

  .hero-orb:nth-child(2) {
    width: 350px;
    height: 350px;
    background: linear-gradient(135deg, rgba(236, 72, 153, 0.5), rgba(239, 68, 68, 0.3));
    bottom: -100px;
    right: -80px;
    animation-delay: -5s;
  }

  .hero-orb:nth-child(3) {
    width: 280px;
    height: 280px;
    background: linear-gradient(135deg, rgba(6, 182, 212, 0.4), rgba(16, 185, 129, 0.3));
    top: 50%;
    left: 60%;
    animation-delay: -10s;
  }

  /* Twinkling Stars */
  .hero-stars {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
  }

  .hero-star {
    position: absolute;
    width: 3px;
    height: 3px;
    background: white;
    border-radius: 50%;
    animation: starTwinkle 4s ease-in-out infinite;
    box-shadow: 0 0 10px 2px rgba(255, 255, 255, 0.5);
  }

  .hero-star:nth-child(1) { left: 8%; top: 15%; animation-delay: 0s; }
  .hero-star:nth-child(2) { left: 18%; top: 45%; animation-delay: 0.7s; }
  .hero-star:nth-child(3) { left: 28%; top: 75%; animation-delay: 1.4s; }
  .hero-star:nth-child(4) { left: 42%; top: 20%; animation-delay: 2.1s; }
  .hero-star:nth-child(5) { left: 58%; top: 65%; animation-delay: 0.3s; }
  .hero-star:nth-child(6) { left: 72%; top: 30%; animation-delay: 1s; }
  .hero-star:nth-child(7) { left: 88%; top: 55%; animation-delay: 1.7s; }
  .hero-star:nth-child(8) { left: 95%; top: 25%; animation-delay: 2.4s; }

  /* Floating Particles */
  .hero-particles {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    pointer-events: none;
  }

  .hero-particle {
    position: absolute;
    width: 6px;
    height: 6px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.2));
    border-radius: 50%;
    animation: particleFloat 10s ease-in-out infinite;
  }

  .hero-particle:nth-child(1) { left: 15%; bottom: 20%; animation-delay: 0s; }
  .hero-particle:nth-child(2) { left: 35%; bottom: 30%; animation-delay: 2s; }
  .hero-particle:nth-child(3) { left: 55%; bottom: 15%; animation-delay: 4s; }
  .hero-particle:nth-child(4) { left: 75%; bottom: 25%; animation-delay: 1s; }
  .hero-particle:nth-child(5) { left: 90%; bottom: 35%; animation-delay: 3s; }

  /* Floating Icons */
  .hero-icons {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 1;
    pointer-events: none;
  }

  .hero-floating-icon {
    position: absolute;
    font-size: 2.5rem;
    opacity: 0.12;
    filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.3));
  }

  .hero-floating-icon:nth-child(1) { top: 15%; left: 8%; animation: float 10s infinite ease-in-out; }
  .hero-floating-icon:nth-child(2) { top: 20%; right: 10%; animation: floatReverse 12s infinite ease-in-out 1s; }
  .hero-floating-icon:nth-child(3) { bottom: 20%; left: 12%; animation: float 9s infinite ease-in-out 2s; }
  .hero-floating-icon:nth-child(4) { bottom: 25%; right: 15%; animation: floatReverse 11s infinite ease-in-out 0.5s; }

  .hero-content {
    position: relative;
    z-index: 10;
    text-align: center;
    animation: slideInUp 1.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .hero-icon {
    font-size: 4rem;
    margin-bottom: 1.5rem;
    animation: iconBounce 3s ease-in-out infinite;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.3));
  }

  .hero-title {
    font-size: 4.5rem;
    font-weight: 900;
    color: white;
    text-shadow: 0 4px 60px rgba(0, 0, 0, 0.5);
    margin-bottom: 1rem;
    letter-spacing: -2px;
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 30%, #ffffff 50%, #ddd6fe 70%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 8s ease infinite;
  }

  .hero-subtitle {
    font-size: 1.4rem;
    color: rgba(255, 255, 255, 0.9);
    text-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.7;
  }

  /* ========================================
     Quick Contact Cards - Premium
  ======================================== */
  .quick-contact-section {
    margin: 5rem 0;
  }

  .quick-contact-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    position: relative;
    z-index: 1;
  }

  .quick-card {
    background: white;
    padding: 2.5rem 2rem;
    border-radius: 28px;
    text-align: center;
    box-shadow: 
      0 20px 50px rgba(0, 0, 0, 0.08),
      0 1px 3px rgba(0, 0, 0, 0.03);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 1px solid rgba(0, 0, 0, 0.04);
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .quick-card:nth-child(1) { animation-delay: 0.1s; }
  .quick-card:nth-child(2) { animation-delay: 0.2s; }
  .quick-card:nth-child(3) { animation-delay: 0.3s; }
  .quick-card:nth-child(4) { animation-delay: 0.4s; }

  .quick-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899);
    transform: scaleX(0);
    transition: transform 0.4s ease;
  }

  .quick-card:hover::before {
    transform: scaleX(1);
  }

  .quick-card::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(99, 102, 241, 0.08), transparent);
    transition: none;
    z-index: 0;
  }

  .quick-card:hover::after {
    animation: shimmer 0.8s ease forwards;
  }

  .quick-card:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 
      0 30px 60px rgba(99, 102, 241, 0.2),
      0 0 0 1px rgba(99, 102, 241, 0.1);
  }

  .quick-card-icon {
    font-size: 3.5rem;
    margin-bottom: 1.5rem;
    display: inline-block;
    animation: float 5s ease-in-out infinite;
    position: relative;
    z-index: 1;
  }

  .quick-card-title {
    font-size: 1.4rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 0.8rem;
    position: relative;
    z-index: 1;
  }

  .quick-card-content {
    color: #6B7280;
    line-height: 1.6;
    font-size: 1rem;
    position: relative;
    z-index: 1;
  }

  /* ========================================
     Main Contact Container
  ======================================== */
  .contact-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 2rem;
  }

  /* ========================================
     Contact Form - Ultra Premium
  ======================================== */
  .contact-form-section {
    background: white;
    padding: 3.5rem;
    border-radius: 32px;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.02);
    border: 1px solid rgba(0, 0, 0, 0.04);
    position: relative;
    overflow: hidden;
    animation: slideInLeft 1s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .contact-form-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899, #f59e0b);
    background-size: 300% 100%;
    animation: gradientFlow 5s linear infinite;
  }

  .form-header {
    text-align: center;
    margin-bottom: 2.5rem;
  }

  .form-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    animation: iconBounce 3s ease-in-out infinite;
  }

  .form-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.5rem;
  }

  .form-subtitle {
    color: #6B7280;
    font-size: 1rem;
  }

  .form-group {
    margin-bottom: 1.8rem;
    position: relative;
  }

  .form-label {
    display: block;
    margin-bottom: 0.6rem;
    color: #374151;
    font-weight: 700;
    font-size: 0.95rem;
    transition: color 0.3s ease;
  }

  .form-label .required {
    color: #EF4444;
    margin-left: 2px;
  }

  .form-input,
  .form-textarea,
  .form-select {
    width: 100%;
    padding: 1rem 1.2rem;
    border: 2px solid #E5E7EB;
    border-radius: 14px;
    font-size: 1rem;
    font-family: inherit;
    background: rgba(249, 250, 251, 0.5);
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  }

  .form-input:hover,
  .form-textarea:hover,
  .form-select:hover {
    border-color: #C7D2FE;
  }

  .form-input:focus,
  .form-textarea:focus,
  .form-select:focus {
    outline: none;
    border-color: #6366f1;
    background: white;
    box-shadow: 
      0 0 0 4px rgba(99, 102, 241, 0.1),
      0 10px 30px rgba(99, 102, 241, 0.1);
    animation: inputFocus 0.3s ease;
  }

  .form-input:focus + .input-highlight,
  .form-textarea:focus + .input-highlight {
    opacity: 1;
    transform: scaleX(1);
  }

  .input-highlight {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 2px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6);
    transform: scaleX(0);
    opacity: 0;
    transition: all 0.3s ease;
  }

  .form-textarea {
    min-height: 140px;
    resize: vertical;
    line-height: 1.6;
  }

  .form-select {
    cursor: pointer;
    appearance: none;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 24 24' stroke='%236B7280'%3E%3Cpath stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M19 9l-7 7-7-7'%3E%3C/path%3E%3C/svg%3E");
    background-repeat: no-repeat;
    background-position: right 1rem center;
    background-size: 1.2rem;
    padding-right: 3rem;
  }

  .submit-btn {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
    color: white;
    padding: 1.2rem 3rem;
    border: none;
    border-radius: 60px;
    font-size: 1.15rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    width: 100%;
    box-shadow: 0 15px 40px rgba(99, 102, 241, 0.3);
    position: relative;
    overflow: hidden;
    margin-top: 1rem;
  }

  .submit-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s ease;
  }

  .submit-btn:hover::before {
    left: 100%;
  }

  .submit-btn:hover {
    transform: translateY(-4px) scale(1.02);
    box-shadow: 0 20px 50px rgba(99, 102, 241, 0.4);
  }

  .submit-btn:active {
    transform: translateY(-2px) scale(1.01);
  }

  .submit-btn:disabled {
    opacity: 0.7;
    cursor: not-allowed;
    transform: none;
  }

  .submit-btn .btn-text {
    position: relative;
    z-index: 1;
  }

  .submit-btn .btn-loader {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 24px;
    height: 24px;
    border: 3px solid rgba(255, 255, 255, 0.3);
    border-top-color: white;
    border-radius: 50%;
    animation: rotateGlow 0.8s linear infinite;
    display: none;
  }

  .submit-btn.loading .btn-text {
    opacity: 0;
  }

  .submit-btn.loading .btn-loader {
    display: block;
  }

  /* Success/Error Messages */
  .message {
    padding: 1.2rem 1.5rem;
    border-radius: 14px;
    margin-bottom: 1.5rem;
    display: none;
    font-weight: 600;
    align-items: center;
    gap: 0.8rem;
  }

  .message.show {
    display: flex;
    animation: successPop 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
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

  .message-icon {
    font-size: 1.5rem;
    flex-shrink: 0;
  }

  /* ========================================
     Contact Info Section - Premium
  ======================================== */
  .contact-info-section {
    background: white;
    padding: 3.5rem;
    border-radius: 32px;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.02);
    border: 1px solid rgba(0, 0, 0, 0.04);
    position: relative;
    overflow: hidden;
    animation: slideInRight 1s cubic-bezier(0.16, 1, 0.3, 1);
    animation-delay: 0.2s;
    animation-fill-mode: backwards;
  }

  .info-header {
    text-align: center;
    margin-bottom: 2.5rem;
  }

  .info-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    animation: iconBounce 3s ease-in-out infinite;
    animation-delay: 0.5s;
  }

  .info-title {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.5rem;
  }

  .info-subtitle {
    color: #6B7280;
    font-size: 1rem;
  }

  .contact-method {
    display: flex;
    align-items: center;
    margin-bottom: 1.8rem;
    padding: 1.8rem;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
  }

  .contact-method::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(99, 102, 241, 0.05), transparent);
    transition: left 0.5s ease;
  }

  .contact-method:hover::before {
    left: 100%;
  }

  .contact-method:hover {
    transform: translateX(10px) scale(1.02);
    box-shadow: 0 15px 40px rgba(99, 102, 241, 0.12);
    background: linear-gradient(135deg, white 0%, #EEF2FF 100%);
    border-color: rgba(99, 102, 241, 0.2);
  }

  .contact-icon {
    width: 65px;
    height: 65px;
    border-radius: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-right: 1.5rem;
    flex-shrink: 0;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
    animation: float 6s ease-in-out infinite;
    position: relative;
    z-index: 1;
  }

  .contact-icon.phone-icon {
    background: linear-gradient(135deg, #4ade80 0%, #22c55e 100%);
  }

  .contact-icon.wechat-icon {
    background: linear-gradient(135deg, #07c160 0%, #06ae56 100%);
  }

  .contact-icon.email-icon {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
  }

  .contact-icon svg {
    width: 28px;
    height: 28px;
    fill: white;
  }

  .contact-details {
    flex: 1;
    position: relative;
    z-index: 1;
  }

  .contact-details h3 {
    color: #1F2937;
    margin-bottom: 0.4rem;
    font-size: 1.3rem;
    font-weight: 800;
  }

  .contact-details p {
    color: #6B7280;
    margin: 0;
    font-size: 1.1rem;
    font-weight: 600;
  }

  .contact-details .action-link {
    color: #6366f1;
    text-decoration: none;
    font-weight: 700;
    display: inline-flex;
    align-items: center;
    margin-top: 0.6rem;
    font-size: 0.95rem;
    transition: all 0.3s ease;
  }

  .contact-details .action-link:hover {
    color: #8b5cf6;
    transform: translateX(5px);
  }

  /* Office Hours - Premium Glass */
  .office-hours {
    background: linear-gradient(135deg, 
      rgba(99, 102, 241, 0.08) 0%, 
      rgba(139, 92, 246, 0.05) 50%, 
      rgba(236, 72, 153, 0.03) 100%);
    backdrop-filter: blur(10px);
    padding: 2rem;
    border-radius: 20px;
    margin-top: 1.5rem;
    border: 1px solid rgba(99, 102, 241, 0.15);
    position: relative;
    overflow: hidden;
  }

  .office-hours::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899);
    border-radius: 3px 3px 0 0;
  }

  .office-hours h3 {
    color: #4338ca;
    margin-bottom: 1.2rem;
    font-size: 1.3rem;
    font-weight: 800;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .hours-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .hours-list li {
    display: flex;
    justify-content: space-between;
    padding: 0.9rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    font-weight: 500;
    border-bottom: 1px solid rgba(99, 102, 241, 0.1);
    transition: all 0.3s ease;
  }

  .hours-list li:hover {
    padding-left: 0.8rem;
    color: #1F2937;
    background: rgba(99, 102, 241, 0.03);
    border-radius: 8px;
  }

  .hours-list li:last-child {
    border-bottom: none;
  }

  .hours-list li span:last-child {
    font-weight: 700;
    color: #6366f1;
  }

  /* ========================================
     FAQ Section - Premium Accordion
  ======================================== */
  .faq-section {
    background: linear-gradient(135deg, 
      rgba(99, 102, 241, 0.03) 0%, 
      rgba(139, 92, 246, 0.02) 50%, 
      rgba(236, 72, 153, 0.01) 100%);
    padding: 5rem 3rem;
    border-radius: 40px;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
    border: 1px solid rgba(99, 102, 241, 0.08);
  }

  .faq-header {
    text-align: center;
    margin-bottom: 4rem;
  }

  .faq-eyebrow {
    display: inline-block;
    font-size: 0.85rem;
    font-weight: 700;
    color: #6366f1;
    text-transform: uppercase;
    letter-spacing: 4px;
    margin-bottom: 1rem;
    padding: 0.6rem 1.8rem;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
    border-radius: 50px;
    border: 1px solid rgba(99, 102, 241, 0.2);
  }

  .faq-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    position: relative;
    display: inline-block;
    letter-spacing: -1px;
  }

  .faq-title::after {
    content: '';
    position: absolute;
    bottom: -12px;
    left: 50%;
    transform: translateX(-50%);
    width: 100px;
    height: 5px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899);
    border-radius: 3px;
  }

  .faq-subtitle {
    color: #6B7280;
    font-size: 1.15rem;
    margin-top: 1.5rem;
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
  }

  .faq-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    max-width: 1200px;
    margin: 0 auto;
  }

  .faq-item {
    background: white;
    padding: 2rem 2.5rem;
    border-radius: 24px;
    box-shadow: 
      0 10px 40px rgba(0, 0, 0, 0.06),
      0 1px 3px rgba(0, 0, 0, 0.02);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .faq-item:nth-child(1) { animation-delay: 0.1s; }
  .faq-item:nth-child(2) { animation-delay: 0.2s; }
  .faq-item:nth-child(3) { animation-delay: 0.3s; }
  .faq-item:nth-child(4) { animation-delay: 0.4s; }

  .faq-item::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 5px;
    height: 100%;
    background: linear-gradient(180deg, #6366f1, #8b5cf6, #ec4899);
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .faq-item:hover::before {
    opacity: 1;
  }

  .faq-item:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 
      0 25px 60px rgba(99, 102, 241, 0.12),
      0 0 0 2px rgba(99, 102, 241, 0.1);
  }

  .faq-question {
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    font-size: 1.2rem;
    display: flex;
    align-items: flex-start;
    gap: 0.8rem;
    line-height: 1.4;
  }

  .faq-question-icon {
    color: #6366f1;
    font-size: 1.3rem;
    flex-shrink: 0;
    margin-top: 2px;
  }

  .faq-answer {
    color: #6B7280;
    line-height: 1.8;
    font-size: 1rem;
    padding-left: 2.1rem;
  }

  /* ========================================
     CTA Section - Ultra Premium
  ======================================== */
  .cta-section {
    background: linear-gradient(135deg, 
      #0f0c29 0%, 
      #302b63 25%, 
      #24243e 50%,
      #1a1a2e 75%,
      #0f0c29 100%);
    background-size: 400% 400%;
    animation: gradientFlow 20s ease infinite;
    border-radius: 40px;
    padding: 5rem 4rem;
    text-align: center;
    color: white;
    margin: 5rem 0 0 0;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 50px 100px rgba(0, 0, 0, 0.4),
      inset 0 0 100px rgba(99, 102, 241, 0.1);
  }

  .cta-section::before {
    content: '';
    position: absolute;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
    background: conic-gradient(
      from 0deg at 50% 50%,
      transparent 0deg,
      rgba(99, 102, 241, 0.1) 60deg,
      transparent 120deg,
      rgba(139, 92, 246, 0.08) 180deg,
      transparent 240deg,
      rgba(236, 72, 153, 0.05) 300deg,
      transparent 360deg
    );
    animation: rotateGlow 30s linear infinite;
    pointer-events: none;
  }

  .cta-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.3;
    animation: morphBlob 20s ease-in-out infinite;
    pointer-events: none;
  }

  .cta-orb-1 {
    width: 400px;
    height: 400px;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.6), rgba(139, 92, 246, 0.4));
    top: -150px;
    left: -100px;
  }

  .cta-orb-2 {
    width: 300px;
    height: 300px;
    background: linear-gradient(135deg, rgba(236, 72, 153, 0.5), rgba(239, 68, 68, 0.3));
    bottom: -100px;
    right: -50px;
    animation-delay: -10s;
  }

  .cta-content {
    position: relative;
    z-index: 10;
  }

  .cta-icon {
    font-size: 4rem;
    margin-bottom: 1.5rem;
    animation: float 5s ease-in-out infinite;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.3));
  }

  .cta-title {
    font-size: 3rem;
    font-weight: 900;
    margin-bottom: 1rem;
    letter-spacing: -1px;
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 50%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 8s ease infinite;
  }

  .cta-description {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    color: rgba(255, 255, 255, 0.85);
    max-width: 550px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-btn {
    padding: 1.1rem 2.5rem;
    border-radius: 60px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }

  .cta-btn-primary {
    background: linear-gradient(135deg, #ffffff, #f0f0f0);
    color: #4338ca;
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
  }

  .cta-btn-primary:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 25px 60px rgba(0, 0, 0, 0.4);
    color: #4338ca;
  }

  .cta-btn-secondary {
    background: rgba(255, 255, 255, 0.1);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.3);
    backdrop-filter: blur(10px);
  }

  .cta-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.2);
    border-color: rgba(255, 255, 255, 0.5);
    transform: translateY(-5px);
    color: white;
  }

  /* ========================================
     Responsive Design
  ======================================== */
  @media (max-width: 1200px) {
    .quick-contact-cards {
      grid-template-columns: repeat(2, 1fr);
    }

    .faq-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 968px) {
    .contact-container {
      grid-template-columns: 1fr;
    }

    .hero-title {
      font-size: 3.5rem;
    }
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 2.5rem;
    }

    .quick-contact-cards {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
    }

    .contact-hero {
      border-radius: 24px;
      min-height: 45vh;
    }

    .contact-form-section,
    .contact-info-section {
      padding: 2.5rem 1.5rem;
      border-radius: 24px;
    }

    .faq-section {
      padding: 3rem 1.5rem;
      border-radius: 24px;
    }

    .faq-title {
      font-size: 2rem;
    }

    .cta-section {
      padding: 3rem 1.5rem;
      border-radius: 24px;
    }

    .cta-title {
      font-size: 2rem;
    }

    .cta-buttons {
      flex-direction: column;
      align-items: center;
    }

    .cta-btn {
      width: 100%;
      max-width: 280px;
      justify-content: center;
    }

    .hero-icons {
      display: none;
    }
  }

  @media (max-width: 480px) {
    .hero-title {
      font-size: 2rem;
    }

    .form-title,
    .info-title {
      font-size: 1.8rem;
    }

    .contact-method {
      flex-direction: column;
      text-align: center;
    }

    .contact-icon {
      margin-right: 0;
      margin-bottom: 1rem;
    }
  }
</style>

<!-- Contact Hero -->
<section class="contact-hero">
  <div class="hero-aurora"></div>
  
  <div class="hero-orbs">
    <div class="hero-orb"></div>
    <div class="hero-orb"></div>
    <div class="hero-orb"></div>
  </div>
  
  <div class="hero-stars">
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
  </div>

  <div class="hero-particles">
    <div class="hero-particle"></div>
    <div class="hero-particle"></div>
    <div class="hero-particle"></div>
    <div class="hero-particle"></div>
    <div class="hero-particle"></div>
  </div>
  
  <div class="hero-icons">
    <span class="hero-floating-icon">📧</span>
    <span class="hero-floating-icon">💬</span>
    <span class="hero-floating-icon">🌍</span>
    <span class="hero-floating-icon">📞</span>
  </div>
  
  <div class="hero-content">
    <div class="hero-icon">✉️</div>
    <h1 class="hero-title">
      <span class="en-content">Let's Connect</span>
      <span class="zh-content">与我们联系</span>
    </h1>
    <p class="hero-subtitle">
      <span class="en-content">We're here to answer your questions and help you succeed on your coding journey</span>
      <span class="zh-content">我们随时为您解答问题，帮助您在编程之路上取得成功</span>
    </p>
  </div>
</section>

<!-- Quick Contact Cards -->
<section class="quick-contact-section">
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
        <span class="en-content">Supporting students from US, Canada & China</span>
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
        <span class="en-content">English & Chinese communication</span>
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
</section>

<!-- Main Contact Section -->
<div class="contact-container">
  <!-- Contact Form -->
  <div class="contact-form-section">
    <div class="form-header">
      <div class="form-icon">📝</div>
      <h2 class="form-title">
        <span class="en-content">Send Us a Message</span>
        <span class="zh-content">发送消息</span>
      </h2>
      <p class="form-subtitle">
        <span class="en-content">Fill out the form and we'll get back to you soon</span>
        <span class="zh-content">填写表格，我们会尽快回复您</span>
      </p>
    </div>
    
    <div id="successMessage" class="message success">
      <span class="message-icon">✅</span>
      <span>
        <span class="en-content">Thank you for your message! We'll get back to you soon.</span>
        <span class="zh-content">感谢您的消息！我们会尽快回复您。</span>
      </span>
    </div>
    
    <div id="errorMessage" class="message error">
      <span class="message-icon">❌</span>
      <span>
        <span class="en-content">There was an error sending your message. Please try again.</span>
        <span class="zh-content">发送消息时出错。请重试。</span>
      </span>
    </div>
    
    <form id="contactForm">
      <input type="hidden" name="_subject" value="New contact from AIcoding Edu">
      
      <div class="form-group">
        <label class="form-label" for="name">
          <span class="en-content">Full Name <span class="required">*</span></span>
          <span class="zh-content">姓名 <span class="required">*</span></span>
        </label>
        <input type="text" id="name" name="name" class="form-input" required>
        <div class="input-highlight"></div>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="email">
          <span class="en-content">Email Address <span class="required">*</span></span>
          <span class="zh-content">电子邮箱 <span class="required">*</span></span>
        </label>
        <input type="email" id="email" name="email" class="form-input" required>
        <div class="input-highlight"></div>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="phone">
          <span class="en-content">Phone Number</span>
          <span class="zh-content">电话号码</span>
        </label>
        <input type="tel" id="phone" name="phone" class="form-input">
        <div class="input-highlight"></div>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="course">
          <span class="en-content">Course Interest</span>
          <span class="zh-content">感兴趣的课程</span>
        </label>
        <select id="course" name="course" class="form-select">
          <option value="">Select a course... / 选择课程...</option>
          <option value="python">Python Programming / Python 编程</option>
          <option value="java">Java Programming / Java 编程</option>
          <option value="cpp">C++ Programming / C++ 编程</option>
          <option value="usaco">USACO Prep / USACO 准备</option>
          <option value="apcsa">AP Computer Science A</option>
          <option value="apcsp">AP Computer Science Principles</option>
          <option value="ml">Machine Learning & AI / 机器学习与AI</option>
          <option value="other">Other / Custom Program / 其他</option>
        </select>
      </div>
      
      <div class="form-group">
        <label class="form-label" for="message">
          <span class="en-content">Message <span class="required">*</span></span>
          <span class="zh-content">留言 <span class="required">*</span></span>
        </label>
        <textarea id="message" name="message" class="form-textarea" required 
          placeholder="Tell us about your goals and how we can help... / 请告诉我们您的目标以及我们如何帮助您..."></textarea>
        <div class="input-highlight"></div>
      </div>
      
      <button type="submit" class="submit-btn" id="submitBtn">
        <span class="btn-text">
          <span class="en-content">Send Message →</span>
          <span class="zh-content">发送消息 →</span>
        </span>
        <span class="btn-loader"></span>
      </button>
    </form>
  </div>
  
  <!-- Contact Info -->
  <div class="contact-info-section">
    <div class="info-header">
      <div class="info-icon">📱</div>
      <h2 class="info-title">
        <span class="en-content">Get in Touch</span>
        <span class="zh-content">联系方式</span>
      </h2>
      <p class="info-subtitle">
        <span class="en-content">Reach out to us directly</span>
        <span class="zh-content">直接与我们联系</span>
      </p>
    </div>
    
    <!-- Phone -->
    <div class="contact-method">
      <div class="contact-icon phone-icon">
        <svg viewBox="0 0 24 24">
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
        <svg viewBox="0 0 24 24">
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
    
    <!-- Email - Contact via Form -->
    <div class="contact-method">
      <div class="contact-icon email-icon">
        <svg viewBox="0 0 24 24">
          <path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
        </svg>
      </div>
      <div class="contact-details">
        <h3>
          <span class="en-content">Email</span>
          <span class="zh-content">邮箱</span>
        </h3>
        <p>
          <span class="en-content">Use the contact form</span>
          <span class="zh-content">请使用联系表单</span>
        </p>
        <span class="action-link" style="cursor: pointer;" onclick="document.getElementById('name').focus();">
          <span class="en-content">Send Message →</span>
          <span class="zh-content">发送消息 →</span>
        </span>
      </div>
    </div>
    
    <!-- Office Hours -->
    <div class="office-hours">
      <h3>
        <span>🕐</span>
        <span class="en-content">Office Hours (PST)</span>
        <span class="zh-content">办公时间 (美西时间)</span>
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
            <span class="en-content">Flexible</span>
            <span class="zh-content">灵活安排</span>
          </span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- FAQ Section -->
<section class="faq-section">
  <div class="faq-header">
    <span class="faq-eyebrow">
      <span class="en-content">Have Questions?</span>
      <span class="zh-content">有疑问？</span>
    </span>
    <h2 class="faq-title">
      <span class="en-content">Frequently Asked Questions</span>
      <span class="zh-content">常见问题</span>
    </h2>
    <p class="faq-subtitle">
      <span class="en-content">Find answers to common questions about our programs</span>
      <span class="zh-content">查找有关我们课程的常见问题解答</span>
    </p>
  </div>
  
  <div class="faq-grid">
    <div class="faq-item">
      <div class="faq-question">
        <span class="faq-question-icon">❓</span>
        <span>
          <span class="en-content">What age groups do you teach?</span>
          <span class="zh-content">你们教哪些年龄段的学生？</span>
        </span>
      </div>
      <div class="faq-answer">
        <span class="en-content">We offer courses for students aged 10-18, as well as undergraduate and graduate students. Our curriculum is tailored to different skill levels and age-appropriate learning objectives.</span>
        <span class="zh-content">我们为10-18岁的学生以及本科生和研究生提供课程。我们的课程根据不同的技能水平和适合年龄的学习目标量身定制。</span>
      </div>
    </div>
    
    <div class="faq-item">
      <div class="faq-question">
        <span class="faq-question-icon">❓</span>
        <span>
          <span class="en-content">Do you offer trial classes?</span>
          <span class="zh-content">你们提供试听课吗？</span>
        </span>
      </div>
      <div class="faq-answer">
        <span class="en-content">Yes! We offer a free consultation session to assess your needs and recommend the best learning path. Contact us to schedule your trial class.</span>
        <span class="zh-content">是的！我们提供免费的咨询课程来评估您的需求并推荐最佳的学习路径。请联系我们安排试听课。</span>
      </div>
    </div>
    
    <div class="faq-item">
      <div class="faq-question">
        <span class="faq-question-icon">❓</span>
        <span>
          <span class="en-content">What's the class format?</span>
          <span class="zh-content">课程形式是怎样的？</span>
        </span>
      </div>
      <div class="faq-answer">
        <span class="en-content">We offer both one-on-one and small group classes (max 4 students) via online platforms. All classes are interactive with screen sharing, coding exercises, and real-time feedback.</span>
        <span class="zh-content">我们通过在线平台提供一对一和小班课程（最多4名学生）。所有课程都是互动式的，包括屏幕共享、编程练习和实时反馈。</span>
      </div>
    </div>
    
    <div class="faq-item">
      <div class="faq-question">
        <span class="faq-question-icon">❓</span>
        <span>
          <span class="en-content">Can you help with competition preparation?</span>
          <span class="zh-content">你们能帮助准备竞赛吗？</span>
        </span>
      </div>
      <div class="faq-answer">
        <span class="en-content">Absolutely! We specialize in USACO, USAAIO, AMC, ACSL, and other competitions. Our instructors have extensive experience and proven track records in competition coaching.</span>
        <span class="zh-content">当然可以！我们专门从事USACO、USAAIO、AMC、ACSL和其他竞赛的培训。我们的导师在竞赛辅导方面有丰富的经验和优秀的成绩记录。</span>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-orb cta-orb-1"></div>
  <div class="cta-orb cta-orb-2"></div>
  
  <div class="cta-content">
    <div class="cta-icon">🚀</div>
    <h2 class="cta-title">
      <span class="en-content">Ready to Start Learning?</span>
      <span class="zh-content">准备好开始学习了吗？</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Book a free consultation today and discover how we can help you achieve your programming goals.</span>
      <span class="zh-content">立即预约免费咨询，了解我们如何帮助您实现编程目标。</span>
    </p>
    <div class="cta-buttons">
      <a href="./course.html" class="cta-btn cta-btn-primary">
        <span class="en-content">📚 View All Courses</span>
        <span class="zh-content">📚 查看所有课程</span>
      </a>
      <a href="tel:+13473796896" class="cta-btn cta-btn-secondary">
        <span class="en-content">📞 Call Us Now</span>
        <span class="zh-content">📞 立即致电</span>
      </a>
    </div>
  </div>
</section>

<!-- EmailJS SDK -->
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<script>
  // Initialize EmailJS
  (function(){
    emailjs.init("AoNX_tjdsa7y4pIhr"); 
  })();
  
  // Form submission handler
  const form = document.getElementById('contactForm');
  const submitBtn = document.getElementById('submitBtn');
  const successMessage = document.getElementById('successMessage');
  const errorMessage = document.getElementById('errorMessage');
  
  form.addEventListener('submit', async function(e) {
    e.preventDefault();
    
    // Add loading state
    submitBtn.classList.add('loading');
    submitBtn.disabled = true;
    
    // Prepare template params
    const templateParams = {
      from_name: form.name.value,
      from_email: form.email.value,
      phone: form.phone.value || 'Not provided',
      course: form.course.value || 'Not specified',
      message: form.message.value
    };
    
    try {
      const response = await emailjs.send("service_pgmmr85", "template_iaomvs8", templateParams);
      
      if (response.status === 200) {
        successMessage.classList.add('show');
        errorMessage.classList.remove('show');
        form.reset();
        
        setTimeout(() => {
          successMessage.classList.remove('show');
        }, 5000);
      } else {
        throw new Error('Failed to send email');
      }
      
    } catch (error) {
      console.error('EmailJS Error:', error);
      
      // Show error message - form submission failed
      errorMessage.innerHTML = '<span class="message-icon">⚠️</span><span><span class="en-content">Message failed to send. Please try again or contact us by phone/WeChat.</span><span class="zh-content">消息发送失败。请重试或通过电话/微信联系我们。</span></span>';
      errorMessage.classList.add('show');
      successMessage.classList.remove('show');
      
      setTimeout(() => {
        errorMessage.classList.remove('show');
      }, 5000);
    } finally {
      submitBtn.classList.remove('loading');
      submitBtn.disabled = false;
    }
  });
  
  // Add ripple effect to buttons
  document.querySelectorAll('.submit-btn, .cta-btn').forEach(btn => {
    btn.addEventListener('click', function(e) {
      const ripple = document.createElement('span');
      const rect = this.getBoundingClientRect();
      ripple.style.cssText = `
        position: absolute;
        background: rgba(255,255,255,0.3);
        border-radius: 50%;
        width: 100px;
        height: 100px;
        left: ${e.clientX - rect.left - 50}px;
        top: ${e.clientY - rect.top - 50}px;
        animation: ripple 0.6s ease-out;
        pointer-events: none;
      `;
      this.appendChild(ripple);
      setTimeout(() => ripple.remove(), 600);
    });
  });
</script>

