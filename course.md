---
layout: default
title: Our Courses
title_zh: 我们的课程
description: Comprehensive Programming Curriculum for All Levels
description_zh: 全方位编程课程，适合各个水平
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

  @keyframes ripple {
    0% { transform: scale(0.8); opacity: 1; }
    100% { transform: scale(2.5); opacity: 0; }
  }

  @keyframes textGradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes glowPulse {
    0%, 100% { filter: drop-shadow(0 0 10px currentColor); }
    50% { filter: drop-shadow(0 0 25px currentColor); }
  }

  /* ========================================
     Page Header - Ultra Premium
  ======================================== */
  .page-header-premium {
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
  .header-aurora {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .header-aurora::before,
  .header-aurora::after {
    content: '';
    position: absolute;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
  }

  .header-aurora::before {
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

  .header-aurora::after {
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
  .header-orbs {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
    overflow: hidden;
  }

  .header-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.4;
    animation: morphBlob 20s ease-in-out infinite, float 15s ease-in-out infinite;
  }

  .header-orb:nth-child(1) {
    width: 450px;
    height: 450px;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.6), rgba(139, 92, 246, 0.4));
    top: -150px;
    left: -100px;
  }

  .header-orb:nth-child(2) {
    width: 350px;
    height: 350px;
    background: linear-gradient(135deg, rgba(236, 72, 153, 0.5), rgba(239, 68, 68, 0.3));
    bottom: -100px;
    right: -80px;
    animation-delay: -5s;
  }

  .header-orb:nth-child(3) {
    width: 280px;
    height: 280px;
    background: linear-gradient(135deg, rgba(6, 182, 212, 0.4), rgba(16, 185, 129, 0.3));
    top: 50%;
    left: 60%;
    animation-delay: -10s;
  }

  /* Twinkling Stars */
  .header-stars {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
  }

  .header-star {
    position: absolute;
    width: 3px;
    height: 3px;
    background: white;
    border-radius: 50%;
    animation: starTwinkle 4s ease-in-out infinite;
    box-shadow: 0 0 10px 2px rgba(255, 255, 255, 0.5);
  }

  .header-star:nth-child(1) { left: 8%; top: 15%; animation-delay: 0s; }
  .header-star:nth-child(2) { left: 18%; top: 45%; animation-delay: 0.7s; }
  .header-star:nth-child(3) { left: 28%; top: 75%; animation-delay: 1.4s; }
  .header-star:nth-child(4) { left: 42%; top: 20%; animation-delay: 2.1s; }
  .header-star:nth-child(5) { left: 58%; top: 65%; animation-delay: 0.3s; }
  .header-star:nth-child(6) { left: 72%; top: 30%; animation-delay: 1s; }
  .header-star:nth-child(7) { left: 88%; top: 55%; animation-delay: 1.7s; }
  .header-star:nth-child(8) { left: 95%; top: 25%; animation-delay: 2.4s; }

  /* Floating Particles */
  .header-particles {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    pointer-events: none;
  }

  .header-particle {
    position: absolute;
    width: 6px;
    height: 6px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.2));
    border-radius: 50%;
    animation: particleFloat 10s ease-in-out infinite;
  }

  .header-particle:nth-child(1) { left: 15%; bottom: 20%; animation-delay: 0s; }
  .header-particle:nth-child(2) { left: 35%; bottom: 30%; animation-delay: 2s; }
  .header-particle:nth-child(3) { left: 55%; bottom: 15%; animation-delay: 4s; }
  .header-particle:nth-child(4) { left: 75%; bottom: 25%; animation-delay: 1s; }
  .header-particle:nth-child(5) { left: 90%; bottom: 35%; animation-delay: 3s; }

  /* Floating Icons */
  .header-icons {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 1;
    pointer-events: none;
  }

  .header-floating-icon {
    position: absolute;
    font-size: 2.5rem;
    opacity: 0.12;
    filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.3));
  }

  .header-floating-icon:nth-child(1) { top: 15%; left: 8%; animation: float 10s infinite ease-in-out; }
  .header-floating-icon:nth-child(2) { top: 20%; right: 10%; animation: floatReverse 12s infinite ease-in-out 1s; }
  .header-floating-icon:nth-child(3) { bottom: 20%; left: 12%; animation: float 9s infinite ease-in-out 2s; }
  .header-floating-icon:nth-child(4) { bottom: 25%; right: 15%; animation: floatReverse 11s infinite ease-in-out 0.5s; }

  .header-content {
    position: relative;
    z-index: 10;
    text-align: center;
    animation: slideInUp 1.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .page-icon {
    font-size: 4rem;
    margin-bottom: 1.5rem;
    animation: iconBounce 3s ease-in-out infinite;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.3));
  }

  .page-title {
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

  .page-description {
    font-size: 1.4rem;
    color: rgba(255, 255, 255, 0.9);
    text-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.7;
  }

  /* ========================================
     Learning Path - Premium Glass Design
  ======================================== */
  .learning-path {
    background: linear-gradient(135deg, 
      rgba(99, 102, 241, 0.08) 0%, 
      rgba(139, 92, 246, 0.05) 50%, 
      rgba(236, 72, 153, 0.03) 100%);
    backdrop-filter: blur(20px);
    border-radius: 40px;
    padding: 5rem 3rem;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.1),
      inset 0 1px 0 rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(99, 102, 241, 0.15);
  }

  .learning-path::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899, #f59e0b);
    background-size: 300% 100%;
    animation: gradientFlow 5s linear infinite;
  }

  .path-title {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 3rem;
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .path-steps {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    position: relative;
    z-index: 1;
  }

  /* Connecting Line */
  .path-steps::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 10%;
    right: 10%;
    height: 4px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899, #10b981);
    border-radius: 2px;
    z-index: -1;
    opacity: 0.3;
  }

  .path-step {
    background: white;
    padding: 2.5rem 2rem;
    border-radius: 24px;
    text-align: center;
    border: 2px solid rgba(99, 102, 241, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
  }

  .path-step::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6);
    transform: scaleX(0);
    transition: transform 0.4s ease;
  }

  .path-step:hover::before {
    transform: scaleX(1);
  }

  .path-step:hover {
    transform: translateY(-12px) scale(1.03);
    border-color: #6366f1;
    box-shadow: 
      0 25px 60px rgba(99, 102, 241, 0.2),
      0 0 0 1px rgba(99, 102, 241, 0.1);
  }

  .step-number {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
    color: white;
    width: 70px;
    height: 70px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 1.2rem;
    font-weight: 800;
    font-size: 1.6rem;
    box-shadow: 
      0 15px 35px rgba(99, 102, 241, 0.4),
      inset 0 -3px 0 rgba(0, 0, 0, 0.1);
    position: relative;
  }

  .step-number::after {
    content: '';
    position: absolute;
    inset: -4px;
    border-radius: 50%;
    border: 2px solid rgba(99, 102, 241, 0.3);
    animation: pulse 2s ease-in-out infinite;
  }

  .step-title {
    font-weight: 700;
    color: #1F2937;
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
  }

  .step-description {
    font-size: 1rem;
    color: #6B7280;
    font-weight: 500;
  }

  /* ========================================
     Section Headers
  ======================================== */
  .course-category {
    margin-bottom: 6rem;
  }

  .category-header {
    text-align: center;
    margin-bottom: 4rem;
  }

  .category-eyebrow {
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

  .category-title {
    font-size: 3.2rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    position: relative;
    display: inline-block;
    letter-spacing: -1px;
  }

  .category-title::after {
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

  .category-subtitle {
    color: #6B7280;
    font-size: 1.25rem;
    margin-top: 1.5rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
  }

  /* ========================================
     Course Cards - Ultra Premium
  ======================================== */
  .courses-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin-top: 3rem;
  }

  .course-card {
    background: white;
    border-radius: 28px;
    overflow: hidden;
    box-shadow: 
      0 20px 50px rgba(0, 0, 0, 0.08),
      0 1px 3px rgba(0, 0, 0, 0.03);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 1px solid rgba(0, 0, 0, 0.04);
    display: flex;
    flex-direction: column;
    position: relative;
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .course-card:nth-child(1) { animation-delay: 0.1s; }
  .course-card:nth-child(2) { animation-delay: 0.2s; }
  .course-card:nth-child(3) { animation-delay: 0.3s; }
  .course-card:nth-child(4) { animation-delay: 0.4s; }
  .course-card:nth-child(5) { animation-delay: 0.5s; }
  .course-card:nth-child(6) { animation-delay: 0.6s; }

  .course-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
    transition: none;
    z-index: 10;
    pointer-events: none;
  }

  .course-card:hover::before {
    animation: shimmer 0.8s ease forwards;
  }

  .course-card:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 
      0 40px 80px rgba(0, 0, 0, 0.15),
      0 0 0 1px rgba(99, 102, 241, 0.1);
  }

  /* Course Image - Premium Gradients */
  .course-image {
    width: 100%;
    height: 220px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 5rem;
    color: white;
    position: relative;
    background-size: 300% 300%;
    animation: gradientFlow 12s ease infinite;
    overflow: hidden;
  }

  .course-image::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, transparent 0%, rgba(0, 0, 0, 0.1) 100%);
  }

  .course-image::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.15) 0%, transparent 60%);
    animation: rotateGlow 20s linear infinite;
    pointer-events: none;
  }

  .course-image-icon {
    position: relative;
    z-index: 2;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.3));
    animation: float 5s ease-in-out infinite;
  }

  /* Gradient Themes */
  .gradient-python {
    background: linear-gradient(135deg, #FF6B6B 0%, #FF8E53 30%, #FED330 60%, #FF6B6B 100%);
  }

  .gradient-java {
    background: linear-gradient(135deg, #00C9FF 0%, #92FE9D 30%, #00C9FF 60%, #2196F3 100%);
  }

  .gradient-cpp {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 30%, #8B5CF6 60%, #667eea 100%);
  }

  .gradient-ds {
    background: linear-gradient(135deg, #3BF0E4 0%, #BCA1F7 30%, #00D9FF 60%, #3BF0E4 100%);
  }

  .gradient-algo {
    background: linear-gradient(135deg, #F093FB 0%, #F5576C 30%, #FF6B6B 60%, #F093FB 100%);
  }

  .gradient-ml {
    background: linear-gradient(135deg, #00FFF0 0%, #7B2FF7 30%, #F107A3 60%, #00FFF0 100%);
  }

  .gradient-apcsa {
    background: linear-gradient(135deg, #10B981 0%, #34D399 30%, #6EE7B7 60%, #10B981 100%);
  }

  .gradient-apcsp {
    background: linear-gradient(135deg, #EC4899 0%, #F472B6 30%, #FB7185 60%, #EC4899 100%);
  }

  .gradient-webdev {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 30%, #a855f7 60%, #6366f1 100%);
  }

  /* Badge Styles */
  .badge-container {
    position: absolute;
    top: 1rem;
    right: 1rem;
    z-index: 5;
  }

  .course-badge {
    padding: 0.5rem 1.2rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 1px;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    animation: pulse 2s ease-in-out infinite;
  }

  .badge-popular {
    background: linear-gradient(135deg, #EF4444 0%, #DC2626 100%);
    color: white;
  }

  .badge-new {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
  }

  .badge-hot {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
  }

  .badge-trending {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    color: white;
  }

  /* Course Content */
  .course-content {
    padding: 2rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .course-title {
    font-size: 1.5rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 0.5rem;
    letter-spacing: -0.5px;
  }

  .course-subtitle {
    color: #6B7280;
    font-size: 1rem;
    margin-bottom: 1.5rem;
    line-height: 1.6;
  }

  .course-features {
    list-style: none;
    margin: 0;
    padding: 0;
    flex-grow: 1;
  }

  .course-features li {
    padding: 0.7rem 0;
    color: #4B5563;
    display: flex;
    align-items: center;
    font-size: 0.95rem;
    transition: all 0.3s ease;
    border-bottom: 1px solid #F3F4F6;
  }

  .course-features li:last-child {
    border-bottom: none;
  }

  .course-features li:hover {
    transform: translateX(8px);
    color: #6366f1;
  }

  .course-features li::before {
    content: "✓";
    color: #10B981;
    font-weight: 700;
    margin-right: 1rem;
    font-size: 1rem;
    width: 24px;
    height: 24px;
    background: rgba(16, 185, 129, 0.1);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
  }

  .course-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1.5rem;
    border-top: 1px solid #E5E7EB;
    margin-top: auto;
    margin-bottom: 1.5rem;
  }

  .course-tag {
    padding: 0.5rem 1rem;
    border-radius: 50px;
    font-size: 0.85rem;
    font-weight: 600;
  }

  .age-tag {
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
    color: #6366f1;
  }

  .level-tag {
    background: linear-gradient(135deg, rgba(16, 185, 129, 0.1), rgba(5, 150, 105, 0.1));
    color: #10B981;
  }

  .enroll-btn {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
    color: white !important;
    padding: 1rem 2rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 700;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    text-align: center;
    box-shadow: 0 10px 30px rgba(99, 102, 241, 0.3);
    position: relative;
    overflow: hidden;
  }

  .enroll-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s ease;
  }

  .enroll-btn:hover::before {
    left: 100%;
  }

  .enroll-btn:hover {
    transform: translateY(-4px) scale(1.02);
    box-shadow: 0 20px 50px rgba(99, 102, 241, 0.4);
    color: white !important;
  }

  /* ========================================
     Competition Grid - Premium
  ======================================== */
  .competition-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-top: 3rem;
  }

  .competition-card {
    background: white;
    border-radius: 24px;
    padding: 2.5rem 2rem;
    text-align: center;
    box-shadow: 
      0 15px 40px rgba(0, 0, 0, 0.06),
      0 1px 3px rgba(0, 0, 0, 0.02);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
    min-height: 300px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .competition-card:nth-child(1) { animation-delay: 0.1s; }
  .competition-card:nth-child(2) { animation-delay: 0.15s; }
  .competition-card:nth-child(3) { animation-delay: 0.2s; }
  .competition-card:nth-child(4) { animation-delay: 0.25s; }
  .competition-card:nth-child(5) { animation-delay: 0.3s; }
  .competition-card:nth-child(6) { animation-delay: 0.35s; }
  .competition-card:nth-child(7) { animation-delay: 0.4s; }
  .competition-card:nth-child(8) { animation-delay: 0.45s; }
  .competition-card:nth-child(9) { animation-delay: 0.5s; }

  .competition-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899);
    transform: scaleX(0);
    transition: transform 0.4s ease;
  }

  .competition-card:hover::before {
    transform: scaleX(1);
  }

  .competition-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 
      0 30px 60px rgba(0, 0, 0, 0.12),
      0 0 0 2px #6366f1;
    border-color: transparent;
  }

  .competition-icon {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    display: block;
    animation: float 5s ease-in-out infinite;
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .kaggle-logo {
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Arial Black', sans-serif;
    font-weight: 900;
    font-size: 3.5rem;
    color: #20BEFF;
    text-shadow: 0 4px 15px rgba(32, 190, 255, 0.4);
    margin-bottom: 1rem;
    animation: float 5s ease-in-out infinite;
    height: 70px;
  }

  .competition-name {
    font-size: 1.4rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 0.6rem;
  }

  .competition-desc {
    color: #6B7280;
    font-size: 1rem;
    line-height: 1.6;
    flex-grow: 1;
    margin-bottom: 1.5rem;
  }

  .competition-btn {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
    color: white !important;
    padding: 0.9rem 1.8rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 700;
    font-size: 0.95rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    box-shadow: 0 8px 25px rgba(99, 102, 241, 0.3);
  }

  .competition-btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 15px 40px rgba(99, 102, 241, 0.4);
    color: white !important;
  }

  /* ========================================
     CTA Section - Ultimate Premium
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
    padding: 6rem 4rem;
    text-align: center;
    color: white;
    margin: 6rem 0;
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
    font-size: 5rem;
    margin-bottom: 2rem;
    animation: float 5s ease-in-out infinite;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.3));
  }

  .cta-title {
    font-size: 3.5rem;
    font-weight: 900;
    margin-bottom: 1.2rem;
    color: white !important;
    text-shadow: 0 4px 40px rgba(0, 0, 0, 0.3);
    letter-spacing: -1px;
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 50%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 8s ease infinite;
  }

  .cta-description {
    font-size: 1.3rem;
    margin-bottom: 2.5rem;
    color: rgba(255, 255, 255, 0.85) !important;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.8;
  }

  .cta-button {
    background: linear-gradient(135deg, #ffffff, #f0f0f0);
    color: #4338ca;
    padding: 1.3rem 3.5rem;
    border-radius: 60px;
    text-decoration: none;
    font-weight: 800;
    font-size: 1.15rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    box-shadow: 
      0 15px 40px rgba(0, 0, 0, 0.3),
      0 0 0 1px rgba(255, 255, 255, 0.1);
    position: relative;
    overflow: hidden;
  }

  .cta-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(99, 102, 241, 0.2), transparent);
    transition: left 0.5s ease;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-6px) scale(1.02);
    box-shadow: 
      0 25px 60px rgba(0, 0, 0, 0.4),
      0 0 60px rgba(99, 102, 241, 0.2);
    color: #4338ca;
  }

  /* ========================================
     Responsive Design
  ======================================== */
  @media (max-width: 1400px) {
    .courses-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 1200px) {
    .path-steps {
      grid-template-columns: repeat(2, 1fr);
    }

    .path-steps::before {
      display: none;
    }

    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 900px) {
    .page-title {
      font-size: 3rem;
    }

    .category-title {
      font-size: 2.4rem;
    }

    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .page-title {
      font-size: 2.5rem;
    }

    .courses-grid {
      grid-template-columns: 1fr;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .path-steps {
      grid-template-columns: 1fr;
      max-width: 350px;
      margin-left: auto;
      margin-right: auto;
    }

    .competition-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
    }

    .category-title {
      font-size: 2rem;
    }

    .cta-title {
      font-size: 2rem;
    }

    .header-icons {
      display: none;
    }

    .page-header-premium {
      border-radius: 24px;
    }

    .learning-path {
      border-radius: 24px;
      padding: 3rem 1.5rem;
    }

    .cta-section {
      border-radius: 24px;
      padding: 4rem 2rem;
    }
  }

  @media (max-width: 480px) {
    .page-title {
      font-size: 2rem;
    }

    .course-image {
      height: 180px;
    }

    .cta-button {
      padding: 1rem 2.5rem;
      font-size: 1rem;
    }
  }
</style>

<!-- Page Header -->
<section class="page-header-premium">
  <div class="header-aurora"></div>
  
  <div class="header-orbs">
    <div class="header-orb"></div>
    <div class="header-orb"></div>
    <div class="header-orb"></div>
  </div>
  
  <div class="header-stars">
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
    <div class="header-star"></div>
  </div>

  <div class="header-particles">
    <div class="header-particle"></div>
    <div class="header-particle"></div>
    <div class="header-particle"></div>
    <div class="header-particle"></div>
    <div class="header-particle"></div>
  </div>
  
  <div class="header-icons">
    <span class="header-floating-icon">💻</span>
    <span class="header-floating-icon">🚀</span>
    <span class="header-floating-icon">🏆</span>
    <span class="header-floating-icon">🧠</span>
  </div>
  
  <div class="header-content">
    <div class="page-icon">📚</div>
    <h1 class="page-title">
      <span class="en-content">Course Catalog</span>
      <span class="zh-content">课程目录</span>
    </h1>
    <p class="page-description">
      <span class="en-content">World-Class Programming Education for Future Innovators</span>
      <span class="zh-content">为未来创新者提供世界级编程教育</span>
    </p>
  </div>
</section>

<!-- Learning Path -->
<section class="learning-path">
  <h2 class="path-title">
    <span class="en-content">🚀 Your Learning Journey</span>
    <span class="zh-content">🚀 您的学习之旅</span>
  </h2>
  <div class="path-steps">
    <div class="path-step">
      <div class="step-number">1</div>
      <div class="step-title">
        <span class="en-content">Foundation</span>
        <span class="zh-content">基础</span>
      </div>
      <div class="step-description">
        <span class="en-content">Python / Java Basics</span>
        <span class="zh-content">Python / Java 基础</span>
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
</section>

<!-- Programming Languages -->
<section class="course-category">
  <div class="category-header">
    <span class="category-eyebrow">
      <span class="en-content">Start Here</span>
      <span class="zh-content">从这里开始</span>
    </span>
    <h2 class="category-title">
      <span class="en-content">💻 Programming Languages</span>
      <span class="zh-content">💻 编程语言</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Master the world's most powerful programming languages</span>
      <span class="zh-content">掌握世界上最强大的编程语言</span>
    </p>
  </div>
  
  <div class="courses-grid">
    <!-- Python -->
    <div class="course-card">
      <div class="course-image gradient-python">
        <div class="badge-container">
          <span class="course-badge badge-popular">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        <span class="course-image-icon">🐍</span>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="course-tag level-tag">
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

    <!-- Java -->
    <div class="course-card">
      <div class="course-image gradient-java">
        <div class="badge-container">
          <span class="course-badge badge-popular">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        <span class="course-image-icon">☕</span>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="course-tag level-tag">
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

    <!-- C++ -->
    <div class="course-card">
      <div class="course-image gradient-cpp">
        <span class="course-image-icon">⚙️</span>
      </div>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="course-tag level-tag">
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
</section>

<!-- Computer Science Core -->
<section class="course-category">
  <div class="category-header">
    <span class="category-eyebrow">
      <span class="en-content">Level Up</span>
      <span class="zh-content">进阶提升</span>
    </span>
    <h2 class="category-title">
      <span class="en-content">📚 Computer Science Core</span>
      <span class="zh-content">📚 计算机科学核心</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Essential foundations for every programmer</span>
      <span class="zh-content">每个程序员的必备基础</span>
    </p>
  </div>
  
  <div class="courses-grid">
    <!-- Data Structures -->
    <div class="course-card">
      <div class="course-image gradient-ds">
        <span class="course-image-icon">🗂️</span>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="course-tag level-tag">
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
      <div class="course-image gradient-algo">
        <span class="course-image-icon">🧮</span>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 13-18</span>
            <span class="zh-content">年龄: 13-18</span>
          </span>
          <span class="course-tag level-tag">
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
      <div class="course-image gradient-ml">
        <div class="badge-container">
          <span class="course-badge badge-hot">
            <span class="en-content">HOT</span>
            <span class="zh-content">火爆</span>
          </span>
        </div>
        <span class="course-image-icon">🤖</span>
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
          <span class="course-tag age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="course-tag level-tag">
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

    <!-- AP CSA -->
    <div class="course-card">
      <div class="course-image gradient-apcsa">
        <span class="course-image-icon">📘</span>
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
            <span class="en-content">Score 5 Guarantee</span>
            <span class="zh-content">5分保证</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="course-tag age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="course-tag level-tag">
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

    <!-- AP CSP -->
    <div class="course-card">
      <div class="course-image gradient-apcsp">
        <div class="badge-container">
          <span class="course-badge badge-new">
            <span class="en-content">NEW</span>
            <span class="zh-content">新</span>
          </span>
        </div>
        <span class="course-image-icon">💡</span>
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">AP Computer Science Principles</span>
          <span class="zh-content">AP计算机科学原理</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Computational Thinking & Creativity</span>
          <span class="zh-content">计算思维与创造力</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Computational Thinking</span>
            <span class="zh-content">计算思维</span>
          </li>
          <li>
            <span class="en-content">Data & Information</span>
            <span class="zh-content">数据与信息</span>
          </li>
          <li>
            <span class="en-content">Internet & Computing</span>
            <span class="zh-content">互联网与计算</span>
          </li>
          <li>
            <span class="en-content">Creative Performance Task</span>
            <span class="zh-content">创意表现任务</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="course-tag age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="course-tag level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./APCSP.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Web Development -->
    <div class="course-card">
      <div class="course-image gradient-webdev">
        <div class="badge-container">
          <span class="course-badge badge-trending">
            <span class="en-content">TRENDING</span>
            <span class="zh-content">趋势</span>
          </span>
        </div>
        <span class="course-image-icon">🌐</span>
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Full-Stack Web Development</span>
          <span class="zh-content">全栈网页开发</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Build Modern Web Applications</span>
          <span class="zh-content">构建现代网页应用</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">HTML5, CSS3, JavaScript</span>
            <span class="zh-content">HTML5, CSS3, JavaScript</span>
          </li>
          <li>
            <span class="en-content">React, Vue, Angular</span>
            <span class="zh-content">React, Vue, Angular</span>
          </li>
          <li>
            <span class="en-content">Node.js & Database Design</span>
            <span class="zh-content">Node.js与数据库设计</span>
          </li>
          <li>
            <span class="en-content">Deploy Real Applications</span>
            <span class="zh-content">部署真实应用</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="course-tag age-tag">
            <span class="en-content">Age: 13-18</span>
            <span class="zh-content">年龄: 13-18</span>
          </span>
          <span class="course-tag level-tag">
            <span class="en-content">All Levels</span>
            <span class="zh-content">所有级别</span>
          </span>
        </div>
        <a href="./webdev.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Competition Training -->
<section class="course-category">
  <div class="category-header">
    <span class="category-eyebrow">
      <span class="en-content">Excel & Compete</span>
      <span class="zh-content">卓越竞争</span>
    </span>
    <h2 class="category-title">
      <span class="en-content">🏆 Competition Training</span>
      <span class="zh-content">🏆 竞赛培训</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Excel in world-renowned competitions</span>
      <span class="zh-content">在世界知名竞赛中脱颖而出</span>
    </p>
  </div>
  
  <div class="competition-grid">
    <!-- USACO -->
    <div class="competition-card">
      <span class="competition-icon">🥇</span>
      <h3 class="competition-name">USACO</h3>
      <p class="competition-desc">
        <span class="en-content">USA Computing Olympiad</span>
        <span class="zh-content">美国计算机奥林匹克</span>
      </p>
      <a href="./USACO.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- USAAIO -->
    <div class="competition-card">
      <span class="competition-icon">🤖</span>
      <h3 class="competition-name">USAAIO</h3>
      <p class="competition-desc">
        <span class="en-content">USA AI Olympiad</span>
        <span class="zh-content">美国人工智能奥林匹克</span>
      </p>
      <a href="./USAAIO.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- Kaggle -->
    <div class="competition-card">
      <span class="kaggle-logo">K</span>
      <h3 class="competition-name">Kaggle</h3>
      <p class="competition-desc">
        <span class="en-content">Data Science Competitions</span>
        <span class="zh-content">数据科学竞赛</span>
      </p>
      <a href="./kaggle.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- AMC -->
    <div class="competition-card">
      <span class="competition-icon">🔢</span>
      <h3 class="competition-name">AMC 8/10/12</h3>
      <p class="competition-desc">
        <span class="en-content">American Mathematics Competitions</span>
        <span class="zh-content">美国数学竞赛</span>
      </p>
      <a href="./amc.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- AIME -->
    <div class="competition-card">
      <span class="competition-icon">📐</span>
      <h3 class="competition-name">AIME</h3>
      <p class="competition-desc">
        <span class="en-content">American Invitational Math Exam</span>
        <span class="zh-content">美国数学邀请赛</span>
      </p>
      <a href="./aime.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- USAMO -->
    <div class="competition-card">
      <span class="competition-icon">🎯</span>
      <h3 class="competition-name">USAMO</h3>
      <p class="competition-desc">
        <span class="en-content">USA Mathematical Olympiad</span>
        <span class="zh-content">美国数学奥林匹克</span>
      </p>
      <a href="./USAMO.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- ACSL -->
    <div class="competition-card">
      <span class="competition-icon">💻</span>
      <h3 class="competition-name">ACSL</h3>
      <p class="competition-desc">
        <span class="en-content">Computer Science League</span>
        <span class="zh-content">计算机科学联赛</span>
      </p>
      <a href="./ACSL.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- WorldQuant -->
    <div class="competition-card">
      <span class="competition-icon">📈</span>
      <h3 class="competition-name">WorldQuant</h3>
      <p class="competition-desc">
        <span class="en-content">Quantitative Finance Challenge</span>
        <span class="zh-content">量化金融挑战赛</span>
      </p>
      <a href="./WorldQuant.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- HiMCM -->
    <div class="competition-card">
      <span class="competition-icon">📋</span>
      <h3 class="competition-name">HiMCM</h3>
      <p class="competition-desc">
        <span class="en-content">Mathematical Modeling Contest</span>
        <span class="zh-content">数学建模竞赛</span>
      </p>
      <a href="./HiMCM.html" class="competition-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
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
      <span class="en-content">Ready to Excel?</span>
      <span class="zh-content">准备好卓越了吗？</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Customized learning paths for every student's unique journey. Start your transformation today.</span>
      <span class="zh-content">为每个学生的独特旅程定制学习路径。今天开始您的蜕变。</span>
    </p>
    <a href="./contact.html" class="cta-button">
      <span class="en-content">Start Your Journey Today</span>
      <span class="zh-content">今天开始您的旅程</span>
    </a>
  </div>
</section>
