---
layout: default
title: AIcoding Academy
title_zh: AIcoding 学院
description: Elite Programming Education for Future Tech Leaders
description_zh: 为未来科技领袖提供的精英编程教育
---

<style>
  /* ========================================
     Advanced Animations
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

  @keyframes shimmer {
    0% { background-position: -1000px 0; }
    100% { background-position: 1000px 0; }
  }

  @keyframes slideInUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes slideInLeft {
    from { opacity: 0; transform: translateX(-40px); }
    to { opacity: 1; transform: translateX(0); }
  }

  @keyframes slideInRight {
    from { opacity: 0; transform: translateX(40px); }
    to { opacity: 1; transform: translateX(0); }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 0.8; }
    50% { transform: scale(1.05); opacity: 1; }
  }

  @keyframes pulseGlow {
    0%, 100% { box-shadow: 0 0 20px rgba(102, 126, 234, 0.4); }
    50% { box-shadow: 0 0 40px rgba(102, 126, 234, 0.8); }
  }

  @keyframes rotate {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes rotateReverse {
    0% { transform: rotate(360deg); }
    100% { transform: rotate(0deg); }
  }

  @keyframes morphBlob {
    0%, 100% { border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; }
    25% { border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%; }
    50% { border-radius: 50% 60% 30% 60% / 30% 60% 70% 40%; }
    75% { border-radius: 60% 40% 60% 30% / 70% 30% 50% 60%; }
  }

  @keyframes starTwinkle {
    0%, 100% { opacity: 0.3; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.3); }
  }

  @keyframes typewriter {
    from { width: 0; }
    to { width: 100%; }
  }

  @keyframes blink {
    50% { border-color: transparent; }
  }

  @keyframes countUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes ripple {
    0% { transform: scale(1); opacity: 0.5; }
    100% { transform: scale(2.5); opacity: 0; }
  }

  @keyframes borderGlow {
    0%, 100% { border-color: rgba(102, 126, 234, 0.5); }
    50% { border-color: rgba(168, 85, 247, 0.8); }
  }

  @keyframes textGradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes bounceIn {
    0% { transform: scale(0.3); opacity: 0; }
    50% { transform: scale(1.05); }
    70% { transform: scale(0.9); }
    100% { transform: scale(1); opacity: 1; }
  }

  @keyframes waveMove {
    0% { transform: translateX(0) translateY(0); }
    50% { transform: translateX(-25px) translateY(10px); }
    100% { transform: translateX(0) translateY(0); }
  }

  /* ========================================
     Hero Section - Ultra Premium
  ======================================== */
  .hero-section {
    min-height: 95vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, 
      #667eea 0%, 
      #764ba2 20%, 
      #6366F1 40%, 
      #8B5CF6 60%, 
      #A855F7 80%, 
      #667eea 100%);
    background-size: 400% 400%;
    animation: gradientFlow 12s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 30px 80px rgba(102, 126, 234, 0.4),
      0 0 120px rgba(139, 92, 246, 0.2);
  }

  /* Aurora effect */
  .hero-aurora {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .hero-aurora::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: linear-gradient(
      45deg,
      transparent 30%,
      rgba(120, 119, 198, 0.15) 40%,
      rgba(167, 139, 250, 0.2) 50%,
      rgba(120, 119, 198, 0.15) 60%,
      transparent 70%
    );
    animation: rotate 20s linear infinite;
  }

  .hero-aurora::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: linear-gradient(
      -45deg,
      transparent 30%,
      rgba(236, 72, 153, 0.1) 40%,
      rgba(245, 158, 11, 0.1) 50%,
      rgba(236, 72, 153, 0.1) 60%,
      transparent 70%
    );
    animation: rotateReverse 25s linear infinite;
  }

  /* Floating orbs */
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
    filter: blur(60px);
    opacity: 0.4;
    animation: morphBlob 15s ease-in-out infinite, float 12s ease-in-out infinite;
  }

  .hero-orb:nth-child(1) {
    width: 400px;
    height: 400px;
    background: rgba(167, 139, 250, 0.6);
    top: -150px;
    left: -100px;
    animation-delay: 0s;
  }

  .hero-orb:nth-child(2) {
    width: 350px;
    height: 350px;
    background: rgba(236, 72, 153, 0.5);
    top: 60%;
    right: -100px;
    animation-delay: -5s;
    animation-direction: reverse;
  }

  .hero-orb:nth-child(3) {
    width: 300px;
    height: 300px;
    background: rgba(245, 158, 11, 0.4);
    bottom: -100px;
    left: 30%;
    animation-delay: -3s;
  }

  /* Twinkling stars */
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
    width: 4px;
    height: 4px;
    background: white;
    border-radius: 50%;
    animation: starTwinkle 3s ease-in-out infinite;
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
  }

  .hero-star:nth-child(1) { left: 5%; top: 10%; animation-delay: 0s; }
  .hero-star:nth-child(2) { left: 15%; top: 40%; animation-delay: 0.5s; }
  .hero-star:nth-child(3) { left: 25%; top: 70%; animation-delay: 1s; }
  .hero-star:nth-child(4) { left: 40%; top: 15%; animation-delay: 1.5s; }
  .hero-star:nth-child(5) { left: 55%; top: 80%; animation-delay: 0.3s; }
  .hero-star:nth-child(6) { left: 70%; top: 35%; animation-delay: 0.8s; }
  .hero-star:nth-child(7) { left: 85%; top: 60%; animation-delay: 1.2s; }
  .hero-star:nth-child(8) { left: 95%; top: 20%; animation-delay: 0.6s; }
  .hero-star:nth-child(9) { left: 30%; top: 5%; animation-delay: 1.8s; }
  .hero-star:nth-child(10) { left: 75%; top: 85%; animation-delay: 2s; }
  .hero-star:nth-child(11) { left: 60%; top: 50%; animation-delay: 0.2s; }
  .hero-star:nth-child(12) { left: 10%; top: 85%; animation-delay: 1.3s; }

  /* Floating icons */
  .floating-icons {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 0;
  }

  .floating-icon {
    position: absolute;
    font-size: 3.5rem;
    opacity: 0.15;
    color: white;
    filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.3));
  }

  .floating-icon:nth-child(1) { top: 8%; left: 8%; animation: float 8s infinite ease-in-out; }
  .floating-icon:nth-child(2) { top: 15%; right: 12%; animation: floatReverse 9s infinite ease-in-out 1s; }
  .floating-icon:nth-child(3) { bottom: 25%; left: 12%; animation: float 7s infinite ease-in-out 2s; }
  .floating-icon:nth-child(4) { bottom: 15%; right: 15%; animation: floatReverse 10s infinite ease-in-out 0.5s; }
  .floating-icon:nth-child(5) { top: 45%; left: 5%; animation: float 8.5s infinite ease-in-out 1.5s; }
  .floating-icon:nth-child(6) { top: 35%; right: 5%; animation: floatReverse 7.5s infinite ease-in-out 2.5s; }
  .floating-icon:nth-child(7) { bottom: 40%; left: 45%; animation: float 9.5s infinite ease-in-out 3s; }

  .hero-content {
    position: relative;
    z-index: 2;
    text-align: center;
    animation: slideInUp 1s ease-out;
  }

  /* Animated badge */
  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    padding: 0.6rem 1.5rem;
    border-radius: 50px;
    margin-bottom: 2rem;
    border: 1px solid rgba(255, 255, 255, 0.3);
    animation: bounceIn 1s ease-out 0.3s backwards;
  }

  .hero-badge-dot {
    width: 8px;
    height: 8px;
    background: #10B981;
    border-radius: 50%;
    animation: pulse 2s ease-in-out infinite;
    box-shadow: 0 0 10px #10B981;
  }

  .hero-badge-text {
    color: white;
    font-size: 0.9rem;
    font-weight: 600;
    letter-spacing: 0.5px;
  }

  .hero-title {
    font-size: 5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 50px rgba(0, 0, 0, 0.3);
    margin-bottom: 1.5rem;
    letter-spacing: -3px;
    line-height: 1.1;
  }

  .hero-title-gradient {
    background: linear-gradient(135deg, #ffffff 0%, #E0E7FF 50%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 5s ease infinite;
  }

  .hero-subtitle {
    font-size: 1.6rem;
    color: rgba(255, 255, 255, 0.95);
    margin-bottom: 1rem;
    font-weight: 400;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
    text-shadow: 0 2px 15px rgba(0, 0, 0, 0.2);
    animation: slideInUp 1s ease-out 0.2s backwards;
  }

  .hero-description {
    font-size: 1.15rem;
    color: rgba(255, 255, 255, 0.85);
    margin-bottom: 3rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
    animation: slideInUp 1s ease-out 0.4s backwards;
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
    animation: slideInUp 1s ease-out 0.6s backwards;
  }

  .hero-btn {
    padding: 1.2rem 3rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.1rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    position: relative;
    overflow: hidden;
  }

  .hero-btn-primary {
    background: white;
    color: #667eea;
    box-shadow: 
      0 10px 40px rgba(0, 0, 0, 0.2),
      0 0 30px rgba(255, 255, 255, 0.2);
  }

  .hero-btn-primary::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.2), transparent);
    transition: left 0.5s;
  }

  .hero-btn-primary:hover::before {
    left: 100%;
  }

  .hero-btn-primary:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 
      0 20px 50px rgba(0, 0, 0, 0.3),
      0 0 50px rgba(255, 255, 255, 0.3);
    color: #667eea;
  }

  .hero-btn-secondary {
    background: rgba(255, 255, 255, 0.12);
    backdrop-filter: blur(10px);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.4);
  }

  .hero-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.25);
    transform: translateY(-5px);
    color: white;
    border-color: rgba(255, 255, 255, 0.6);
  }

  /* Hero stats row */
  .hero-stats {
    display: flex;
    gap: 3rem;
    justify-content: center;
    margin-top: 4rem;
    animation: slideInUp 1s ease-out 0.8s backwards;
  }

  .hero-stat {
    text-align: center;
    position: relative;
  }

  .hero-stat::after {
    content: '';
    position: absolute;
    right: -1.5rem;
    top: 50%;
    transform: translateY(-50%);
    width: 1px;
    height: 40px;
    background: rgba(255, 255, 255, 0.3);
  }

  .hero-stat:last-child::after {
    display: none;
  }

  .hero-stat-number {
    font-size: 2.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 0 30px rgba(255, 255, 255, 0.5);
  }

  .hero-stat-label {
    font-size: 0.9rem;
    color: rgba(255, 255, 255, 0.8);
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: 500;
  }

  /* ========================================
     Trusted By / Social Proof Section
  ======================================== */
  .trusted-section {
    padding: 3rem 0;
    text-align: center;
    margin-bottom: 3rem;
  }

  .trusted-label {
    font-size: 0.9rem;
    color: #9CA3AF;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-bottom: 2rem;
    font-weight: 600;
  }

  .trusted-logos {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 3rem;
    flex-wrap: wrap;
    opacity: 0.6;
    filter: grayscale(100%);
    transition: all 0.5s ease;
  }

  .trusted-logos:hover {
    opacity: 1;
    filter: grayscale(0%);
  }

  .trusted-logo {
    font-size: 1.5rem;
    font-weight: 700;
    color: #6B7280;
    padding: 1rem 2rem;
    background: #F3F4F6;
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .trusted-logo:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  }

  /* ========================================
     Features Grid - Premium Cards
  ======================================== */
  .features-section {
    margin: 6rem 0;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin: 3rem 0;
  }

  .feature-card {
    background: white;
    border-radius: 25px;
    padding: 3rem 2.5rem;
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 1px solid rgba(229, 231, 235, 0.5);
    position: relative;
    overflow: hidden;
  }

  .feature-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #EC4899);
    transform: scaleX(0);
    transition: transform 0.5s ease;
    transform-origin: left;
  }

  .feature-card:hover::before {
    transform: scaleX(1);
  }

  .feature-card:hover {
    transform: translateY(-12px);
    box-shadow: 0 35px 70px rgba(0, 0, 0, 0.12);
  }

  .feature-icon-wrapper {
    position: relative;
    width: 85px;
    height: 85px;
    margin: 0 auto 2rem;
  }

  .feature-icon {
    width: 85px;
    height: 85px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.8rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 22px;
    color: white;
    box-shadow: 0 15px 35px rgba(102, 126, 234, 0.35);
    position: relative;
    z-index: 1;
    transition: all 0.4s ease;
  }

  .feature-card:hover .feature-icon {
    transform: scale(1.08) rotate(-3deg);
    box-shadow: 0 20px 45px rgba(102, 126, 234, 0.45);
  }

  .feature-icon-glow {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, #667eea, #764ba2);
    border-radius: 22px;
    filter: blur(20px);
    opacity: 0.4;
    z-index: 0;
    animation: pulseGlow 3s ease-in-out infinite;
  }

  .feature-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    text-align: center;
  }

  .feature-description {
    color: #6B7280;
    line-height: 1.8;
    text-align: center;
    font-size: 1.05rem;
  }

  /* ========================================
     Courses Showcase Section
  ======================================== */
  .courses-section {
    margin: 6rem 0;
    padding: 5rem 0;
    background: linear-gradient(180deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 40px;
    position: relative;
    overflow: hidden;
  }

  .courses-section::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: 
      radial-gradient(ellipse at 20% 0%, rgba(102, 126, 234, 0.08) 0%, transparent 50%),
      radial-gradient(ellipse at 80% 100%, rgba(236, 72, 153, 0.06) 0%, transparent 50%);
    pointer-events: none;
  }

  .section-header {
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    z-index: 1;
  }

  .section-eyebrow {
    display: inline-block;
    font-size: 0.85rem;
    font-weight: 700;
    color: #667eea;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin-bottom: 1rem;
    padding: 0.5rem 1.5rem;
    background: rgba(102, 126, 234, 0.1);
    border-radius: 50px;
  }

  .section-title {
    font-size: 3.2rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    position: relative;
    display: inline-block;
  }

  .section-title-underline {
    position: absolute;
    bottom: -8px;
    left: 50%;
    transform: translateX(-50%);
    width: 80px;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #EC4899);
    border-radius: 3px;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.3rem;
    font-weight: 400;
    max-width: 600px;
    margin: 1.5rem auto 0;
    line-height: 1.6;
  }

  /* Course categories tabs */
  .course-tabs {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 3rem;
    flex-wrap: wrap;
    padding: 0 2rem;
  }

  .course-tab {
    padding: 0.8rem 2rem;
    background: white;
    border: 2px solid #E5E7EB;
    border-radius: 50px;
    font-weight: 600;
    color: #6B7280;
    cursor: pointer;
    transition: all 0.3s ease;
    font-size: 0.95rem;
  }

  .course-tab:hover,
  .course-tab.active {
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    border-color: transparent;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
    transform: translateY(-2px);
  }

  /* Course cards grid */
  .courses-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    padding: 0 2rem;
    position: relative;
    z-index: 1;
  }

  .course-card {
    background: white;
    border-radius: 24px;
    overflow: hidden;
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 1px solid rgba(229, 231, 235, 0.5);
  }

  .course-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
  }

  .course-card-header {
    height: 160px;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  .course-card-header::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.15) 0%, transparent 60%);
    animation: rotate 15s linear infinite;
  }

  .course-card-icon {
    font-size: 4rem;
    filter: drop-shadow(0 10px 20px rgba(0, 0, 0, 0.2));
    position: relative;
    z-index: 1;
    animation: float 5s ease-in-out infinite;
  }

  .course-card-badge {
    position: absolute;
    top: 1rem;
    right: 1rem;
    padding: 0.4rem 1rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    z-index: 2;
  }

  .badge-popular {
    background: #EF4444;
    color: white;
  }

  .badge-new {
    background: #10B981;
    color: white;
  }

  .badge-hot {
    background: #F59E0B;
    color: white;
  }

  .course-card-body {
    padding: 2rem;
  }

  .course-card-title {
    font-size: 1.35rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .course-card-subtitle {
    font-size: 0.95rem;
    color: #9CA3AF;
    margin-bottom: 1.5rem;
  }

  .course-card-features {
    list-style: none;
    padding: 0;
    margin: 0 0 1.5rem 0;
  }

  .course-card-features li {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    color: #4B5563;
    font-size: 0.95rem;
    margin-bottom: 0.6rem;
  }

  .course-card-features li::before {
    content: '→';
    color: #10B981;
    font-weight: 700;
  }

  .course-card-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1.5rem;
    border-top: 1px solid #F3F4F6;
  }

  .course-card-tags {
    display: flex;
    gap: 0.5rem;
  }

  .course-tag {
    padding: 0.3rem 0.8rem;
    background: #F3F4F6;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 600;
    color: #6B7280;
  }

  .course-tag.age {
    background: rgba(102, 126, 234, 0.1);
    color: #667eea;
  }

  .course-tag.level {
    background: rgba(16, 185, 129, 0.1);
    color: #10B981;
  }

  .course-card-btn {
    padding: 0.7rem 1.5rem;
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    border-radius: 50px;
    font-weight: 600;
    font-size: 0.9rem;
    text-decoration: none;
    transition: all 0.3s ease;
  }

  .course-card-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 25px rgba(102, 126, 234, 0.4);
    color: white;
  }

  /* Course gradient backgrounds */
  .course-gradient-python { background: linear-gradient(135deg, #F472B6, #EC4899); }
  .course-gradient-java { background: linear-gradient(135deg, #60A5FA, #3B82F6); }
  .course-gradient-cpp { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .course-gradient-apcsa { background: linear-gradient(135deg, #34D399, #10B981); }
  .course-gradient-apcsp { background: linear-gradient(135deg, #FBBF24, #F59E0B); }
  .course-gradient-webdev { background: linear-gradient(135deg, #A78BFA, #8B5CF6); }
  .course-gradient-ds { background: linear-gradient(135deg, #38BDF8, #0EA5E9); }
  .course-gradient-algo { background: linear-gradient(135deg, #FB923C, #F97316); }
  .course-gradient-ml { background: linear-gradient(135deg, #E879F9, #D946EF); }

  /* ========================================
     Competition Training Section
  ======================================== */
  .competition-section {
    margin: 6rem 0;
    padding: 5rem;
    background: linear-gradient(135deg, #1F2937 0%, #111827 100%);
    border-radius: 40px;
    position: relative;
    overflow: hidden;
  }

  .competition-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #667eea, #EC4899, #F59E0B, #10B981, #667eea);
    background-size: 300% 100%;
    animation: gradientFlow 6s ease infinite;
  }

  .competition-section::after {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: 
      radial-gradient(ellipse at 10% 20%, rgba(102, 126, 234, 0.15) 0%, transparent 50%),
      radial-gradient(ellipse at 90% 80%, rgba(236, 72, 153, 0.1) 0%, transparent 50%);
    pointer-events: none;
  }

  .competition-content {
    position: relative;
    z-index: 1;
  }

  .competition-section .section-header {
    margin-bottom: 3rem;
  }

  .competition-section .section-eyebrow {
    background: rgba(102, 126, 234, 0.2);
    color: #A5B4FC;
  }

  .competition-section .section-title {
    color: white;
  }

  .competition-section .section-subtitle {
    color: #9CA3AF;
  }

  /* Competition grid */
  .competition-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-bottom: 3rem;
  }

  .competition-card {
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 20px;
    padding: 2rem;
    text-align: center;
    transition: all 0.4s ease;
    position: relative;
    overflow: hidden;
  }

  .competition-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: linear-gradient(90deg, var(--comp-color-1), var(--comp-color-2));
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .competition-card:hover::before {
    opacity: 1;
  }

  .competition-card:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-8px);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
  }

  .competition-card-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    filter: drop-shadow(0 5px 15px rgba(0, 0, 0, 0.3));
  }

  .competition-card-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: white;
    margin-bottom: 0.5rem;
  }

  .competition-card-subtitle {
    font-size: 0.9rem;
    color: #9CA3AF;
    margin-bottom: 1rem;
  }

  .competition-card-link {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    color: #A5B4FC;
    font-weight: 600;
    font-size: 0.9rem;
    text-decoration: none;
    transition: all 0.3s ease;
  }

  .competition-card-link:hover {
    color: white;
    gap: 0.8rem;
  }

  /* Competition colors */
  .comp-usaco { --comp-color-1: #FFD700; --comp-color-2: #FFA500; }
  .comp-usaaio { --comp-color-1: #667eea; --comp-color-2: #764ba2; }
  .comp-kaggle { --comp-color-1: #20BEFF; --comp-color-2: #0097A7; }
  .comp-amc { --comp-color-1: #10B981; --comp-color-2: #059669; }
  .comp-aime { --comp-color-1: #3B82F6; --comp-color-2: #1D4ED8; }
  .comp-usamo { --comp-color-1: #EF4444; --comp-color-2: #DC2626; }
  .comp-acsl { --comp-color-1: #8B5CF6; --comp-color-2: #7C3AED; }
  .comp-wq { --comp-color-1: #1E3A5F; --comp-color-2: #C9A227; }
  .comp-himcm { --comp-color-1: #14B8A6; --comp-color-2: #0F766E; }

  /* Featured competition highlight */
  .competition-featured {
    grid-column: span 3;
    background: linear-gradient(135deg, rgba(255, 215, 0, 0.15), rgba(255, 165, 0, 0.1));
    border-color: rgba(255, 215, 0, 0.3);
    display: flex;
    align-items: center;
    gap: 3rem;
    padding: 3rem;
    text-align: left;
  }

  .competition-featured-icon {
    font-size: 5rem;
    animation: float 4s ease-in-out infinite;
  }

  .competition-featured-content {
    flex: 1;
  }

  .competition-featured-badge {
    display: inline-block;
    background: linear-gradient(135deg, #FFD700, #FFA500);
    color: #1F2937;
    padding: 0.4rem 1rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 1rem;
  }

  .competition-featured-title {
    font-size: 2rem;
    font-weight: 800;
    color: white;
    margin-bottom: 0.5rem;
  }

  .competition-featured-subtitle {
    color: #D1D5DB;
    font-size: 1.1rem;
    margin-bottom: 1rem;
  }

  .competition-featured-stats {
    display: flex;
    gap: 2rem;
  }

  .competition-featured-stat {
    text-align: left;
  }

  .competition-featured-stat-number {
    font-size: 1.5rem;
    font-weight: 800;
    color: #FFD700;
  }

  .competition-featured-stat-label {
    font-size: 0.85rem;
    color: #9CA3AF;
  }

  /* ========================================
     Learning Path Section
  ======================================== */
  .path-section {
    margin: 6rem 0;
    padding: 5rem 2rem;
  }

  .path-timeline {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    position: relative;
    max-width: 1100px;
    margin: 4rem auto 0;
  }

  .path-timeline::before {
    content: '';
    position: absolute;
    top: 40px;
    left: 60px;
    right: 60px;
    height: 4px;
    background: linear-gradient(90deg, #667eea, #764ba2, #EC4899, #F59E0B, #10B981);
    border-radius: 2px;
  }

  .path-step {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    width: 180px;
    position: relative;
    z-index: 1;
  }

  .path-step-icon {
    width: 80px;
    height: 80px;
    background: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.2rem;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.15);
    margin-bottom: 1.5rem;
    border: 4px solid;
    transition: all 0.4s ease;
  }

  .path-step:hover .path-step-icon {
    transform: scale(1.1);
    box-shadow: 0 15px 50px rgba(0, 0, 0, 0.2);
  }

  .path-step:nth-child(1) .path-step-icon { border-color: #667eea; }
  .path-step:nth-child(2) .path-step-icon { border-color: #764ba2; }
  .path-step:nth-child(3) .path-step-icon { border-color: #EC4899; }
  .path-step:nth-child(4) .path-step-icon { border-color: #F59E0B; }
  .path-step:nth-child(5) .path-step-icon { border-color: #10B981; }

  .path-step-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .path-step-description {
    font-size: 0.9rem;
    color: #6B7280;
    line-height: 1.5;
  }

  /* ========================================
     Stats Section
  ======================================== */
  .stats-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #EC4899 100%);
    background-size: 200% 200%;
    animation: gradientFlow 10s ease infinite;
    border-radius: 40px;
    padding: 5rem 3rem;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
  }

  .stats-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.1) 0%, transparent 60%);
    animation: rotate 30s linear infinite;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 3rem;
    position: relative;
    z-index: 1;
  }

  .stat-item {
    text-align: center;
  }

  .stat-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    filter: drop-shadow(0 5px 15px rgba(0, 0, 0, 0.2));
  }

  .stat-number {
    font-size: 4rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    margin-bottom: 0.5rem;
    line-height: 1;
  }

  .stat-label {
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
  }

  /* ========================================
     Testimonials Section
  ======================================== */
  .testimonials-section {
    margin: 6rem 0;
    padding: 5rem 0;
  }

  .testimonials-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-top: 3rem;
  }

  .testimonial-card {
    background: white;
    border-radius: 24px;
    padding: 2.5rem;
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    transition: all 0.4s ease;
    border: 1px solid #F3F4F6;
  }

  .testimonial-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 60px rgba(0, 0, 0, 0.12);
  }

  .testimonial-card::before {
    content: '"';
    position: absolute;
    top: 1.5rem;
    left: 2rem;
    font-size: 5rem;
    font-family: Georgia, serif;
    color: #E5E7EB;
    line-height: 1;
  }

  .testimonial-content {
    position: relative;
    z-index: 1;
    margin-bottom: 2rem;
  }

  .testimonial-text {
    font-size: 1.05rem;
    color: #4B5563;
    line-height: 1.8;
    font-style: italic;
  }

  .testimonial-author {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .testimonial-avatar {
    width: 55px;
    height: 55px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    font-weight: 700;
    color: white;
  }

  .testimonial-avatar.gradient-1 { background: linear-gradient(135deg, #667eea, #764ba2); }
  .testimonial-avatar.gradient-2 { background: linear-gradient(135deg, #EC4899, #F472B6); }
  .testimonial-avatar.gradient-3 { background: linear-gradient(135deg, #10B981, #34D399); }

  .testimonial-info h4 {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.2rem;
  }

  .testimonial-info p {
    font-size: 0.9rem;
    color: #9CA3AF;
  }

  .testimonial-badge {
    position: absolute;
    top: 1.5rem;
    right: 1.5rem;
    padding: 0.4rem 1rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 700;
  }

  .badge-usaco-gold { background: linear-gradient(135deg, #FFD700, #FFA500); color: #1F2937; }
  .badge-ap5 { background: linear-gradient(135deg, #10B981, #059669); color: white; }
  .badge-finalist { background: linear-gradient(135deg, #3B82F6, #1D4ED8); color: white; }

  /* ========================================
     CTA Section
  ======================================== */
  .cta-section {
    background: linear-gradient(135deg, #1F2937 0%, #111827 100%);
    border-radius: 40px;
    padding: 6rem 3rem;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(ellipse at 20% 50%, rgba(102, 126, 234, 0.2) 0%, transparent 50%),
      radial-gradient(ellipse at 80% 50%, rgba(236, 72, 153, 0.15) 0%, transparent 50%);
    pointer-events: none;
  }

  .cta-section::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.03) 0%, transparent 50%);
    animation: rotate 40s linear infinite;
  }

  .cta-content {
    position: relative;
    z-index: 1;
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
  }

  .cta-icon {
    font-size: 4rem;
    margin-bottom: 2rem;
    animation: float 4s ease-in-out infinite;
  }

  .cta-title {
    font-size: 3.5rem;
    font-weight: 800;
    color: white;
    margin-bottom: 1.5rem;
    line-height: 1.2;
  }

  .cta-title-gradient {
    background: linear-gradient(135deg, #667eea, #EC4899, #F59E0B);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 5s ease infinite;
  }

  .cta-description {
    font-size: 1.3rem;
    color: #9CA3AF;
    margin-bottom: 3rem;
    line-height: 1.7;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
    margin-bottom: 3rem;
  }

  .cta-button {
    padding: 1.2rem 3rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.1rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }

  .cta-button-primary {
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    box-shadow: 0 10px 40px rgba(102, 126, 234, 0.4);
  }

  .cta-button-primary:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 20px 50px rgba(102, 126, 234, 0.5);
    color: white;
  }

  .cta-button-secondary {
    background: transparent;
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .cta-button-secondary:hover {
    background: rgba(255, 255, 255, 0.1);
    border-color: rgba(255, 255, 255, 0.5);
    transform: translateY(-5px);
    color: white;
  }

  .cta-contact {
    display: flex;
    justify-content: center;
    gap: 3rem;
    padding-top: 2rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
  }

  .cta-contact-item {
    display: flex;
    align-items: center;
    gap: 0.8rem;
    color: #9CA3AF;
    font-size: 1rem;
  }

  .cta-contact-icon {
    font-size: 1.3rem;
  }

  /* ========================================
     Responsive Design
  ======================================== */
  @media (max-width: 1200px) {
    .courses-grid,
    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }

    .competition-featured {
      grid-column: span 2;
    }
  }

  @media (max-width: 900px) {
    .features-grid,
    .testimonials-grid {
      grid-template-columns: repeat(2, 1fr);
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
    }

    .path-timeline {
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
    }

    .path-timeline::before {
      display: none;
    }

    .path-step {
      width: 45%;
    }
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 3rem;
      letter-spacing: -1px;
    }

    .hero-subtitle {
      font-size: 1.2rem;
    }

    .hero-stats {
      flex-direction: column;
      gap: 1.5rem;
    }

    .hero-stat::after {
      display: none;
    }

    .features-grid,
    .courses-grid,
    .competition-grid,
    .testimonials-grid {
      grid-template-columns: 1fr;
    }

    .competition-featured {
      grid-column: span 1;
      flex-direction: column;
      text-align: center;
    }

    .competition-featured-stats {
      justify-content: center;
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }

    .section-title {
      font-size: 2.2rem;
    }

    .cta-title {
      font-size: 2.2rem;
    }

    .path-step {
      width: 100%;
    }

    .cta-contact {
      flex-direction: column;
      align-items: center;
      gap: 1.5rem;
    }

    .floating-icons {
      display: none;
    }

    .hero-orbs {
      opacity: 0.5;
    }
  }

  @media (max-width: 480px) {
    .hero-btn {
      padding: 1rem 2rem;
      font-size: 1rem;
    }

    .hero-buttons {
      flex-direction: column;
      align-items: center;
    }

    .stats-grid {
      grid-template-columns: 1fr;
    }

    .stat-number {
      font-size: 3rem;
    }
  }
</style>

<!-- Hero Section -->
<section class="hero-section">
  <!-- Aurora effect -->
  <div class="hero-aurora"></div>
  
  <!-- Floating orbs -->
  <div class="hero-orbs">
    <div class="hero-orb"></div>
    <div class="hero-orb"></div>
    <div class="hero-orb"></div>
  </div>
  
  <!-- Twinkling stars -->
  <div class="hero-stars">
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
    <div class="hero-star"></div>
  </div>
  
  <!-- Floating icons -->
  <div class="floating-icons">
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🚀</span>
    <span class="floating-icon">🎯</span>
    <span class="floating-icon">🏆</span>
    <span class="floating-icon">⚡</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">✨</span>
  </div>
  
  <div class="hero-content">
    <div class="hero-badge">
      <span class="hero-badge-dot"></span>
      <span class="hero-badge-text">
        <span class="en-content">Now Enrolling for 2025</span>
        <span class="zh-content">2025年招生进行中</span>
      </span>
    </div>
    
    <h1 class="hero-title">
      <span class="en-content"><span class="hero-title-gradient">AIcoding</span> Academy</span>
      <span class="zh-content"><span class="hero-title-gradient">AIcoding</span> 学院</span>
    </h1>
    
    <p class="hero-subtitle">
      <span class="en-content">Transforming Students into Tech Innovators</span>
      <span class="zh-content">将学生培养成科技创新者</span>
    </p>
    
    <p class="hero-description">
      <span class="en-content">Elite programming education, competition training, and personalized mentorship for future tech leaders aged 10-18.</span>
      <span class="zh-content">为10-18岁的未来科技领袖提供精英编程教育、竞赛培训和个性化指导。</span>
    </p>
    
    <div class="hero-buttons">
      <a href="./contact.html" class="hero-btn hero-btn-primary">
        <span class="en-content">🚀 Start Your Journey</span>
        <span class="zh-content">🚀 开始您的旅程</span>
      </a>
      <a href="./course.html" class="hero-btn hero-btn-secondary">
        <span class="en-content">📚 Explore Courses</span>
        <span class="zh-content">📚 探索课程</span>
      </a>
    </div>
    
    <div class="hero-stats">
      <div class="hero-stat">
        <div class="hero-stat-number">9+</div>
        <div class="hero-stat-label">
          <span class="en-content">Courses</span>
          <span class="zh-content">课程</span>
        </div>
      </div>
      <div class="hero-stat">
        <div class="hero-stat-number">9+</div>
        <div class="hero-stat-label">
          <span class="en-content">Competitions</span>
          <span class="zh-content">竞赛</span>
        </div>
      </div>
      <div class="hero-stat">
        <div class="hero-stat-number">90%</div>
        <div class="hero-stat-label">
          <span class="en-content">Success Rate</span>
          <span class="zh-content">成功率</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Features Section -->
<section class="features-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Why Choose Us</span>
      <span class="zh-content">为什么选择我们</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">The AIcoding Advantage</span>
      <span class="zh-content">AIcoding 的优势</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">World-class education designed to unlock your full potential</span>
      <span class="zh-content">世界级教育，旨在释放您的全部潜力</span>
    </p>
  </div>
  
  <div class="features-grid">
    <div class="feature-card">
      <div class="feature-icon-wrapper">
        <div class="feature-icon">🎯</div>
        <div class="feature-icon-glow"></div>
      </div>
      <h3 class="feature-title">
        <span class="en-content">Personalized Learning</span>
        <span class="zh-content">个性化学习</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">AI-powered curriculum tailored to your unique learning style, pace, and goals. Small class sizes ensure individual attention.</span>
        <span class="zh-content">AI驱动的课程，根据您独特的学习风格、节奏和目标量身定制。小班教学确保个性化关注。</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon-wrapper">
        <div class="feature-icon">🏆</div>
        <div class="feature-icon-glow"></div>
      </div>
      <h3 class="feature-title">
        <span class="en-content">Competition Excellence</span>
        <span class="zh-content">竞赛卓越</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Proven track record with USACO Platinum, AMC qualifiers, and Kaggle winners. Strategic preparation for 9+ major competitions.</span>
        <span class="zh-content">USACO白金、AMC晋级者和Kaggle获奖者的成功记录。为9+项主要竞赛提供战略性备考。</span>
      </p>
    </div>
    
    <div class="feature-card">
      <div class="feature-icon-wrapper">
        <div class="feature-icon">👨‍🏫</div>
        <div class="feature-icon-glow"></div>
      </div>
      <h3 class="feature-title">
        <span class="en-content">Elite Instructors</span>
        <span class="zh-content">精英导师</span>
      </h3>
      <p class="feature-description">
        <span class="en-content">Learn from PhD holders, FAANG engineers, and competition gold medalists with 5+ years of teaching experience.</span>
        <span class="zh-content">向拥有5年以上教学经验的博士、FAANG工程师和竞赛金牌得主学习。</span>
      </p>
    </div>
  </div>
</section>

<!-- Courses Showcase Section -->
<section class="courses-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Our Curriculum</span>
      <span class="zh-content">我们的课程</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Premium Courses</span>
      <span class="zh-content">高端课程</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">From fundamentals to advanced topics, we cover the complete programming journey</span>
      <span class="zh-content">从基础到高级，我们涵盖完整的编程学习之旅</span>
    </p>
  </div>
  
  <div class="courses-grid">
    <!-- Python -->
    <div class="course-card">
      <div class="course-card-header course-gradient-python">
        <span class="course-card-badge badge-popular">POPULAR</span>
        <span class="course-card-icon">🐍</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Python Fundamental I & II</span>
          <span class="zh-content">Python基础 I & II</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Complete Python Programming Journey</span>
          <span class="zh-content">完整的Python编程之旅</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Variables, Data Types, Control Flow</span><span class="zh-content">变量、数据类型、控制流</span></li>
          <li><span class="en-content">Functions & OOP Concepts</span><span class="zh-content">函数和面向对象概念</span></li>
          <li><span class="en-content">File Handling & Libraries</span><span class="zh-content">文件处理和库</span></li>
          <li><span class="en-content">Real-world Projects</span><span class="zh-content">实际项目</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 10-18</span>
            <span class="course-tag level">Beginner</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- Java -->
    <div class="course-card">
      <div class="course-card-header course-gradient-java">
        <span class="course-card-badge badge-popular">POPULAR</span>
        <span class="course-card-icon">☕</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Java Fundamental I & II</span>
          <span class="zh-content">Java基础 I & II</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Object-Oriented Programming Mastery</span>
          <span class="zh-content">面向对象编程精通</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Java Syntax & Structure</span><span class="zh-content">Java语法和结构</span></li>
          <li><span class="en-content">OOP Principles & Design</span><span class="zh-content">OOP原则和设计</span></li>
          <li><span class="en-content">Collections Framework</span><span class="zh-content">集合框架</span></li>
          <li><span class="en-content">GUI Development</span><span class="zh-content">GUI开发</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 10-18</span>
            <span class="course-tag level">Beginner</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- C++ -->
    <div class="course-card">
      <div class="course-card-header course-gradient-cpp">
        <span class="course-card-icon">⚙️</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">C++ Fundamental I & II</span>
          <span class="zh-content">C++基础 I & II</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">System Programming & Performance</span>
          <span class="zh-content">系统编程与性能</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Memory Management</span><span class="zh-content">内存管理</span></li>
          <li><span class="en-content">Pointers & References</span><span class="zh-content">指针和引用</span></li>
          <li><span class="en-content">STL & Templates</span><span class="zh-content">STL和模板</span></li>
          <li><span class="en-content">Competitive Programming</span><span class="zh-content">竞赛编程</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 12-18</span>
            <span class="course-tag level">Intermediate</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- AP CSA -->
    <div class="course-card">
      <div class="course-card-header course-gradient-apcsa">
        <span class="course-card-icon">📘</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">AP Computer Science A</span>
          <span class="zh-content">AP计算机科学A</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">College-Level Java Programming</span>
          <span class="zh-content">大学水平Java编程</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Complete AP CSA Curriculum</span><span class="zh-content">完整AP CSA课程</span></li>
          <li><span class="en-content">Practice Exams</span><span class="zh-content">模拟考试</span></li>
          <li><span class="en-content">FRQ Training</span><span class="zh-content">FRQ培训</span></li>
          <li><span class="en-content">Score 5 Guarantee</span><span class="zh-content">5分保障</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 14-18</span>
            <span class="course-tag level">Intermediate</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- AP CSP -->
    <div class="course-card">
      <div class="course-card-header course-gradient-apcsp">
        <span class="course-card-badge badge-new">NEW</span>
        <span class="course-card-icon">💡</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">AP Computer Science Principles</span>
          <span class="zh-content">AP计算机科学原理</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Computational Thinking & Creativity</span>
          <span class="zh-content">计算思维与创造力</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Computational Thinking</span><span class="zh-content">计算思维</span></li>
          <li><span class="en-content">Data & Information</span><span class="zh-content">数据与信息</span></li>
          <li><span class="en-content">Internet & Computing</span><span class="zh-content">互联网与计算</span></li>
          <li><span class="en-content">Creative Performance Task</span><span class="zh-content">创意绩效任务</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 14-18</span>
            <span class="course-tag level">Beginner</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- Full-Stack Web Development -->
    <div class="course-card">
      <div class="course-card-header course-gradient-webdev">
        <span class="course-card-badge badge-hot">TRENDING</span>
        <span class="course-card-icon">🌐</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Full-Stack Web Development</span>
          <span class="zh-content">全栈网站开发</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Build Modern Web Applications</span>
          <span class="zh-content">构建现代Web应用</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">HTML5, CSS3, JavaScript</span><span class="zh-content">HTML5, CSS3, JavaScript</span></li>
          <li><span class="en-content">React, Vue, Angular</span><span class="zh-content">React, Vue, Angular</span></li>
          <li><span class="en-content">Node.js & Database Design</span><span class="zh-content">Node.js与数据库设计</span></li>
          <li><span class="en-content">Deploy Real Applications</span><span class="zh-content">部署真实应用</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 13-18</span>
            <span class="course-tag level">All Levels</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- Data Structures -->
    <div class="course-card">
      <div class="course-card-header course-gradient-ds">
        <span class="course-card-icon">📦</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Data Structures</span>
          <span class="zh-content">数据结构</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Foundation of Efficient Programming</span>
          <span class="zh-content">高效编程的基础</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Arrays, Linked Lists, Stacks</span><span class="zh-content">数组、链表、栈</span></li>
          <li><span class="en-content">Trees & Graphs</span><span class="zh-content">树和图</span></li>
          <li><span class="en-content">Hash Tables & Heaps</span><span class="zh-content">哈希表和堆</span></li>
          <li><span class="en-content">Time & Space Complexity</span><span class="zh-content">时间和空间复杂度</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 12-18</span>
            <span class="course-tag level">Intermediate</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- Algorithms -->
    <div class="course-card">
      <div class="course-card-header course-gradient-algo">
        <span class="course-card-icon">🧮</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Algorithms</span>
          <span class="zh-content">算法</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Problem Solving & Optimization</span>
          <span class="zh-content">问题解决与优化</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Sorting & Searching</span><span class="zh-content">排序和搜索</span></li>
          <li><span class="en-content">Dynamic Programming</span><span class="zh-content">动态规划</span></li>
          <li><span class="en-content">Graph Algorithms</span><span class="zh-content">图算法</span></li>
          <li><span class="en-content">Greedy & Divide-Conquer</span><span class="zh-content">贪心和分治</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 13-18</span>
            <span class="course-tag level">Advanced</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
    
    <!-- Machine Learning & AI -->
    <div class="course-card">
      <div class="course-card-header course-gradient-ml">
        <span class="course-card-badge badge-hot">HOT</span>
        <span class="course-card-icon">🤖</span>
      </div>
      <div class="course-card-body">
        <h3 class="course-card-title">
          <span class="en-content">Machine Learning & AI</span>
          <span class="zh-content">机器学习与人工智能</span>
        </h3>
        <p class="course-card-subtitle">
          <span class="en-content">Future of Technology</span>
          <span class="zh-content">技术的未来</span>
        </p>
        <ul class="course-card-features">
          <li><span class="en-content">Neural Networks</span><span class="zh-content">神经网络</span></li>
          <li><span class="en-content">Deep Learning</span><span class="zh-content">深度学习</span></li>
          <li><span class="en-content">Computer Vision</span><span class="zh-content">计算机视觉</span></li>
          <li><span class="en-content">NLP & AI Projects</span><span class="zh-content">NLP和AI项目</span></li>
        </ul>
        <div class="course-card-footer">
          <div class="course-card-tags">
            <span class="course-tag age">Age: 14-18</span>
            <span class="course-tag level">Advanced</span>
          </div>
          <a href="./course.html" class="course-card-btn">
            <span class="en-content">Learn More</span>
            <span class="zh-content">了解更多</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Competition Training Section -->
<section class="competition-section">
  <div class="competition-content">
    <div class="section-header">
      <span class="section-eyebrow">
        <span class="en-content">Competition Training</span>
        <span class="zh-content">竞赛培训</span>
      </span>
      <h2 class="section-title">
        <span class="en-content">Prepare for Excellence</span>
        <span class="zh-content">备战卓越</span>
        <span class="section-title-underline"></span>
      </h2>
      <p class="section-subtitle">
        <span class="en-content">Strategic preparation for the world's most prestigious competitions</span>
        <span class="zh-content">为世界上最负盛名的竞赛提供战略性备考</span>
      </p>
    </div>
    
    <div class="competition-grid">
      <!-- Featured: USACO -->
      <div class="competition-card competition-featured comp-usaco">
        <span class="competition-featured-icon">🥇</span>
        <div class="competition-featured-content">
          <span class="competition-featured-badge">FLAGSHIP PROGRAM</span>
          <h3 class="competition-featured-title">USACO</h3>
          <p class="competition-featured-subtitle">
            <span class="en-content">USA Computing Olympiad - The gold standard in competitive programming</span>
            <span class="zh-content">美国计算机奥林匹克 - 竞赛编程的黄金标准</span>
          </p>
          <div class="competition-featured-stats">
            <div class="competition-featured-stat">
              <div class="competition-featured-stat-number">10+</div>
              <div class="competition-featured-stat-label">
                <span class="en-content">Platinum Qualifiers</span>
                <span class="zh-content">白金晋级者</span>
              </div>
            </div>
            <div class="competition-featured-stat">
              <div class="competition-featured-stat-number">95%</div>
              <div class="competition-featured-stat-label">
                <span class="en-content">Promotion Rate</span>
                <span class="zh-content">晋级率</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      
      <!-- USAAIO -->
      <div class="competition-card comp-usaaio">
        <span class="competition-card-icon">🤖</span>
        <h4 class="competition-card-title">USAAIO</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">USA AI Olympiad</span>
          <span class="zh-content">美国AI奥林匹克</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- Kaggle -->
      <div class="competition-card comp-kaggle">
        <span class="competition-card-icon">📊</span>
        <h4 class="competition-card-title">Kaggle</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">Data Science Competitions</span>
          <span class="zh-content">数据科学竞赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- AMC -->
      <div class="competition-card comp-amc">
        <span class="competition-card-icon">🔢</span>
        <h4 class="competition-card-title">AMC 8/10/12</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">American Mathematics Competitions</span>
          <span class="zh-content">美国数学竞赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- AIME -->
      <div class="competition-card comp-aime">
        <span class="competition-card-icon">📐</span>
        <h4 class="competition-card-title">AIME</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">American Invitational Math Exam</span>
          <span class="zh-content">美国数学邀请赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- USAMO -->
      <div class="competition-card comp-usamo">
        <span class="competition-card-icon">🎯</span>
        <h4 class="competition-card-title">USAMO</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">USA Mathematical Olympiad</span>
          <span class="zh-content">美国数学奥林匹克</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- ACSL -->
      <div class="competition-card comp-acsl">
        <span class="competition-card-icon">💻</span>
        <h4 class="competition-card-title">ACSL</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">Computer Science League</span>
          <span class="zh-content">计算机科学联赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- WorldQuant -->
      <div class="competition-card comp-wq">
        <span class="competition-card-icon">📈</span>
        <h4 class="competition-card-title">WorldQuant</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">Quantitative Finance Challenge</span>
          <span class="zh-content">量化金融挑战赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
      
      <!-- HiMCM -->
      <div class="competition-card comp-himcm">
        <span class="competition-card-icon">📋</span>
        <h4 class="competition-card-title">HiMCM</h4>
        <p class="competition-card-subtitle">
          <span class="en-content">Mathematical Modeling Contest</span>
          <span class="zh-content">数学建模竞赛</span>
        </p>
        <a href="./course.html" class="competition-card-link">
          <span class="en-content">Learn More →</span>
          <span class="zh-content">了解更多 →</span>
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Learning Path Section -->
<section class="path-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Your Journey</span>
      <span class="zh-content">您的旅程</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Learning Path</span>
      <span class="zh-content">学习路径</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">A structured roadmap from beginner to expert</span>
      <span class="zh-content">从入门到专家的结构化路线图</span>
    </p>
  </div>
  
  <div class="path-timeline">
    <div class="path-step">
      <div class="path-step-icon">🌱</div>
      <h4 class="path-step-title">
        <span class="en-content">Fundamentals</span>
        <span class="zh-content">基础</span>
      </h4>
      <p class="path-step-description">
        <span class="en-content">Python, Java, or C++ basics</span>
        <span class="zh-content">Python、Java或C++基础</span>
      </p>
    </div>
    
    <div class="path-step">
      <div class="path-step-icon">📚</div>
      <h4 class="path-step-title">
        <span class="en-content">Data Structures</span>
        <span class="zh-content">数据结构</span>
      </h4>
      <p class="path-step-description">
        <span class="en-content">Arrays, Trees, Graphs</span>
        <span class="zh-content">数组、树、图</span>
      </p>
    </div>
    
    <div class="path-step">
      <div class="path-step-icon">⚡</div>
      <h4 class="path-step-title">
        <span class="en-content">Algorithms</span>
        <span class="zh-content">算法</span>
      </h4>
      <p class="path-step-description">
        <span class="en-content">DP, Graph, Optimization</span>
        <span class="zh-content">动态规划、图、优化</span>
      </p>
    </div>
    
    <div class="path-step">
      <div class="path-step-icon">🏆</div>
      <h4 class="path-step-title">
        <span class="en-content">Competitions</span>
        <span class="zh-content">竞赛</span>
      </h4>
      <p class="path-step-description">
        <span class="en-content">USACO, AMC, ACSL</span>
        <span class="zh-content">USACO、AMC、ACSL</span>
      </p>
    </div>
    
    <div class="path-step">
      <div class="path-step-icon">🚀</div>
      <h4 class="path-step-title">
        <span class="en-content">Advanced</span>
        <span class="zh-content">高级</span>
      </h4>
      <p class="path-step-description">
        <span class="en-content">AI, ML, Research</span>
        <span class="zh-content">AI、机器学习、研究</span>
      </p>
    </div>
  </div>
</section>

<!-- Stats Section -->
<section class="stats-section">
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-icon">👨‍🎓</div>
      <div class="stat-number">50+</div>
      <div class="stat-label">
        <span class="en-content">Students</span>
        <span class="zh-content">学生</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">🏆</div>
      <div class="stat-number">20+</div>
      <div class="stat-label">
        <span class="en-content">Awards Won</span>
        <span class="zh-content">获得奖项</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">📈</div>
      <div class="stat-number">90%</div>
      <div class="stat-label">
        <span class="en-content">Success Rate</span>
        <span class="zh-content">成功率</span>
      </div>
    </div>
    
    <div class="stat-item">
      <div class="stat-icon">⭐</div>
      <div class="stat-number">5+</div>
      <div class="stat-label">
        <span class="en-content">Years Experience</span>
        <span class="zh-content">年经验</span>
      </div>
    </div>
  </div>
</section>

<!-- Testimonials Section -->
<section class="testimonials-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Success Stories</span>
      <span class="zh-content">成功故事</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Student Testimonials</span>
      <span class="zh-content">学生评价</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Hear from our accomplished students</span>
      <span class="zh-content">听听我们优秀学生的声音</span>
    </p>
  </div>
  
  <div class="testimonials-grid">
    <div class="testimonial-card">
      <span class="testimonial-badge badge-usaco-gold">USACO Gold</span>
      <div class="testimonial-content">
        <p class="testimonial-text">
          <span class="en-content">"The structured USACO training helped me advance from Bronze to Gold in just 8 months. The problem-solving strategies I learned here are invaluable."</span>
          <span class="zh-content">"结构化的USACO培训帮助我在短短8个月内从铜级晋升到金级。我在这里学到的问题解决策略非常宝贵。"</span>
        </p>
      </div>
      <div class="testimonial-author">
        <div class="testimonial-avatar gradient-1">A</div>
        <div class="testimonial-info">
          <h4>Alex Chen</h4>
          <p>
            <span class="en-content">High School Junior</span>
            <span class="zh-content">高中二年级</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-ap5">AP Score: 5</span>
      <div class="testimonial-content">
        <p class="testimonial-text">
          <span class="en-content">"The AP CSA course was incredibly well-structured. The practice exams and FRQ training prepared me perfectly. Got a 5 with confidence!"</span>
          <span class="zh-content">"AP CSA课程结构非常完善。模拟考试和FRQ培训让我准备得很充分。自信地拿到了5分！"</span>
        </p>
      </div>
      <div class="testimonial-author">
        <div class="testimonial-avatar gradient-2">S</div>
        <div class="testimonial-info">
          <h4>Sarah Wang</h4>
          <p>
            <span class="en-content">High School Senior</span>
            <span class="zh-content">高中三年级</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-finalist">HiMCM Finalist</span>
      <div class="testimonial-content">
        <p class="testimonial-text">
          <span class="en-content">"The mathematical modeling training was exceptional. Our team reached Finalist status in HiMCM, and I learned skills that will last a lifetime."</span>
          <span class="zh-content">"数学建模培训非常出色。我们的团队在HiMCM中获得了Finalist称号，我学到了终身受用的技能。"</span>
        </p>
      </div>
      <div class="testimonial-author">
        <div class="testimonial-avatar gradient-3">M</div>
        <div class="testimonial-info">
          <h4>Michael Liu</h4>
          <p>
            <span class="en-content">High School Junior</span>
            <span class="zh-content">高中二年级</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-content">
    <div class="cta-icon">🚀</div>
    <h2 class="cta-title">
      <span class="en-content">Ready to <span class="cta-title-gradient">Transform</span> Your Future?</span>
      <span class="zh-content">准备好<span class="cta-title-gradient">改变</span>您的未来了吗？</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Join the elite community of future tech innovators. Start your journey with a free consultation today.</span>
      <span class="zh-content">加入未来科技创新者的精英社区。立即通过免费咨询开始您的旅程。</span>
    </p>
    <div class="cta-buttons">
      <a href="./contact.html" class="cta-button cta-button-primary">
        <span class="en-content">🎯 Schedule Free Consultation</span>
        <span class="zh-content">🎯 预约免费咨询</span>
      </a>
      <a href="./course.html" class="cta-button cta-button-secondary">
        <span class="en-content">📚 Browse All Courses</span>
        <span class="zh-content">📚 浏览所有课程</span>
      </a>
    </div>
    <div class="cta-contact">
      <div class="cta-contact-item">
        <span class="cta-contact-icon">📞</span>
        <span>+1 (347) 379-6896</span>
      </div>
      <div class="cta-contact-item">
        <span class="cta-contact-icon">💬</span>
        <span>WeChat: SpiritedAway2023</span>
      </div>
    </div>
  </div>
</section>
