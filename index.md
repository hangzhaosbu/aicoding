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

  @keyframes slideInUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
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

  @keyframes bounceIn {
    0% { transform: scale(0.3); opacity: 0; }
    50% { transform: scale(1.05); }
    70% { transform: scale(0.9); }
    100% { transform: scale(1); opacity: 1; }
  }

  @keyframes textGradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes drawLine {
    from { stroke-dashoffset: 1000; }
    to { stroke-dashoffset: 0; }
  }

  @keyframes fadeInScale {
    from { opacity: 0; transform: scale(0.8); }
    to { opacity: 1; transform: scale(1); }
  }

  /* ========================================
     Hero Section
  ======================================== */
  .hero-section {
    min-height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, 
      #1e1b4b 0%, 
      #312e81 25%, 
      #4338ca 50%, 
      #6366f1 75%, 
      #4338ca 100%);
    background-size: 400% 400%;
    animation: gradientFlow 15s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 80px rgba(67, 56, 202, 0.4);
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
      rgba(99, 102, 241, 0.15) 40%,
      rgba(139, 92, 246, 0.2) 50%,
      rgba(99, 102, 241, 0.15) 60%,
      transparent 70%
    );
    animation: rotate 25s linear infinite;
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
    filter: blur(80px);
    opacity: 0.3;
    animation: morphBlob 15s ease-in-out infinite, float 12s ease-in-out infinite;
  }

  .hero-orb:nth-child(1) {
    width: 400px;
    height: 400px;
    background: rgba(139, 92, 246, 0.5);
    top: -150px;
    left: -100px;
  }

  .hero-orb:nth-child(2) {
    width: 350px;
    height: 350px;
    background: rgba(59, 130, 246, 0.4);
    top: 60%;
    right: -100px;
    animation-delay: -5s;
  }

  .hero-orb:nth-child(3) {
    width: 300px;
    height: 300px;
    background: rgba(16, 185, 129, 0.3);
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
    font-size: 3rem;
    opacity: 0.12;
    color: white;
    filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.3));
  }

  .floating-icon:nth-child(1) { top: 8%; left: 8%; animation: float 8s infinite ease-in-out; }
  .floating-icon:nth-child(2) { top: 15%; right: 12%; animation: floatReverse 9s infinite ease-in-out 1s; }
  .floating-icon:nth-child(3) { bottom: 25%; left: 12%; animation: float 7s infinite ease-in-out 2s; }
  .floating-icon:nth-child(4) { bottom: 15%; right: 15%; animation: floatReverse 10s infinite ease-in-out 0.5s; }
  .floating-icon:nth-child(5) { top: 45%; left: 5%; animation: float 8.5s infinite ease-in-out 1.5s; }

  .hero-content {
    position: relative;
    z-index: 2;
    text-align: center;
    animation: slideInUp 1s ease-out;
  }

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
    font-size: 4.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 4px 30px rgba(0, 0, 0, 0.4);
    margin-bottom: 1.5rem;
    letter-spacing: -2px;
    line-height: 1.1;
  }

  .hero-title-gradient {
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 50%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: textGradient 5s ease infinite;
  }

  .hero-subtitle {
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.95);
    margin-bottom: 1rem;
    font-weight: 400;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
  }

  .hero-description {
    font-size: 1.1rem;
    color: rgba(255, 255, 255, 0.85);
    margin-bottom: 2.5rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .hero-btn {
    padding: 1.1rem 2.5rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.05rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }

  .hero-btn-primary {
    background: white;
    color: #4338ca;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.25);
  }

  .hero-btn-primary:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    color: #4338ca;
  }

  .hero-btn-secondary {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.4);
  }

  .hero-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.25);
    transform: translateY(-5px);
    color: white;
  }

  /* ========================================
     Section Styles
  ======================================== */
  .section-header {
    text-align: center;
    margin-bottom: 4rem;
  }

  .section-eyebrow {
    display: inline-block;
    font-size: 0.85rem;
    font-weight: 700;
    color: #6366f1;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin-bottom: 1rem;
    padding: 0.5rem 1.5rem;
    background: rgba(99, 102, 241, 0.1);
    border-radius: 50px;
  }

  .section-title {
    font-size: 3rem;
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
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #a855f7);
    border-radius: 3px;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.2rem;
    font-weight: 400;
    max-width: 650px;
    margin: 1.5rem auto 0;
    line-height: 1.7;
  }

  /* ========================================
     What We Offer Section
  ======================================== */
  .offer-section {
    margin: 6rem 0;
  }

  .offer-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin-top: 3rem;
  }

  .offer-card {
    background: white;
    border-radius: 24px;
    padding: 2.5rem;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.06);
    border: 1px solid #F3F4F6;
    transition: all 0.4s ease;
    text-align: center;
  }

  .offer-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 25px 60px rgba(0, 0, 0, 0.1);
  }

  .offer-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.5rem;
    border-radius: 20px;
    position: relative;
  }

  .offer-icon-programming {
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.15), rgba(139, 92, 246, 0.15));
  }

  .offer-icon-competition {
    background: linear-gradient(135deg, rgba(245, 158, 11, 0.15), rgba(239, 68, 68, 0.15));
  }

  .offer-icon-research {
    background: linear-gradient(135deg, rgba(16, 185, 129, 0.15), rgba(6, 182, 212, 0.15));
  }

  .offer-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.8rem;
  }

  .offer-description {
    color: #6B7280;
    font-size: 1rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
  }

  .offer-list {
    list-style: none;
    padding: 0;
    margin: 0;
    text-align: left;
  }

  .offer-list li {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    padding: 0.5rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    border-bottom: 1px solid #F3F4F6;
  }

  .offer-list li:last-child {
    border-bottom: none;
  }

  .offer-list li::before {
    content: '✓';
    color: #10B981;
    font-weight: 700;
  }

  /* ========================================
     Learning Paths Section - ENHANCED
  ======================================== */
  .paths-section {
    margin: 6rem 0;
    padding: 5rem 2rem;
    background: linear-gradient(180deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 40px;
    position: relative;
    overflow: hidden;
  }

  .paths-section::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: 
      radial-gradient(ellipse at 0% 0%, rgba(99, 102, 241, 0.08) 0%, transparent 50%),
      radial-gradient(ellipse at 100% 100%, rgba(16, 185, 129, 0.06) 0%, transparent 50%);
    pointer-events: none;
  }

  .paths-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    margin-top: 3rem;
    position: relative;
    z-index: 1;
  }

  .path-card {
    background: white;
    border-radius: 24px;
    overflow: hidden;
    box-shadow: 0 15px 50px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
  }

  .path-card:hover {
    transform: translateY(-12px);
    box-shadow: 0 30px 70px rgba(0, 0, 0, 0.12);
  }

  .path-card-header {
    padding: 2.5rem 2rem 2rem;
    position: relative;
    overflow: hidden;
  }

  .path-card-header::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    opacity: 0.1;
  }

  .path-header-algo {
    background: linear-gradient(135deg, #6366f1, #8b5cf6);
  }

  .path-header-ml {
    background: linear-gradient(135deg, #10B981, #06B6D4);
  }

  .path-header-research {
    background: linear-gradient(135deg, #F59E0B, #EF4444);
  }

  .path-icon {
    width: 70px;
    height: 70px;
    background: white;
    border-radius: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.2rem;
    margin-bottom: 1.5rem;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
  }

  .path-title {
    font-size: 1.5rem;
    font-weight: 800;
    color: white;
    margin-bottom: 0.5rem;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  .path-tagline {
    color: rgba(255, 255, 255, 0.9);
    font-size: 0.95rem;
    font-weight: 500;
  }

  .path-card-body {
    padding: 2rem;
  }

  .path-description {
    color: #4B5563;
    font-size: 1rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
  }

  .path-stages {
    margin-bottom: 1.5rem;
  }

  .path-stage {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    padding: 1rem 0;
    border-bottom: 1px solid #F3F4F6;
  }

  .path-stage:last-child {
    border-bottom: none;
  }

  .path-stage-number {
    width: 28px;
    height: 28px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.8rem;
    font-weight: 700;
    color: white;
    flex-shrink: 0;
  }

  .path-stage-algo .path-stage-number { background: linear-gradient(135deg, #6366f1, #8b5cf6); }
  .path-stage-ml .path-stage-number { background: linear-gradient(135deg, #10B981, #06B6D4); }
  .path-stage-research .path-stage-number { background: linear-gradient(135deg, #F59E0B, #EF4444); }

  .path-stage-content h4 {
    font-size: 1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .path-stage-content p {
    font-size: 0.9rem;
    color: #6B7280;
    line-height: 1.5;
  }

  .path-target {
    background: #F9FAFB;
    border-radius: 12px;
    padding: 1rem 1.2rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
  }

  .path-target-icon {
    font-size: 1.3rem;
  }

  .path-target-text {
    font-size: 0.9rem;
    color: #4B5563;
    font-weight: 600;
  }

  .path-target-text span {
    font-weight: 700;
  }

  .path-target-algo span { color: #6366f1; }
  .path-target-ml span { color: #10B981; }
  .path-target-research span { color: #F59E0B; }

  /* ========================================
     Why Choose Us Section
  ======================================== */
  .why-section {
    margin: 6rem 0;
  }

  .why-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 3rem;
  }

  .why-card {
    background: white;
    border-radius: 20px;
    padding: 2rem;
    text-align: center;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.05);
    border: 1px solid #F3F4F6;
    transition: all 0.4s ease;
  }

  .why-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.1);
  }

  .why-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .why-title {
    font-size: 1.15rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .why-description {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* ========================================
     Stats Section
  ======================================== */
  .stats-section {
    background: linear-gradient(135deg, #1e1b4b 0%, #312e81 50%, #4338ca 100%);
    border-radius: 30px;
    padding: 4rem 3rem;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
  }

  .stats-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(ellipse at 20% 50%, rgba(99, 102, 241, 0.3) 0%, transparent 50%),
      radial-gradient(ellipse at 80% 50%, rgba(139, 92, 246, 0.2) 0%, transparent 50%);
    pointer-events: none;
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
    font-size: 2.5rem;
    margin-bottom: 0.8rem;
    filter: drop-shadow(0 5px 15px rgba(0, 0, 0, 0.3));
  }

  .stat-number {
    font-size: 3.5rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
    margin-bottom: 0.3rem;
    line-height: 1;
  }

  .stat-label {
    color: rgba(255, 255, 255, 0.85);
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
  }

  /* ========================================
     Testimonials Section
  ======================================== */
  .testimonials-section {
    margin: 6rem 0;
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
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.06);
    position: relative;
    border: 1px solid #F3F4F6;
    transition: all 0.4s ease;
  }

  .testimonial-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 60px rgba(0, 0, 0, 0.1);
  }

  .testimonial-quote {
    font-size: 3rem;
    color: #E5E7EB;
    font-family: Georgia, serif;
    line-height: 1;
    margin-bottom: 1rem;
  }

  .testimonial-text {
    font-size: 1.05rem;
    color: #4B5563;
    line-height: 1.8;
    font-style: italic;
    margin-bottom: 1.5rem;
  }

  .testimonial-author {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .testimonial-avatar {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    font-weight: 700;
    color: white;
  }

  .avatar-purple { background: linear-gradient(135deg, #6366f1, #8b5cf6); }
  .avatar-green { background: linear-gradient(135deg, #10B981, #06B6D4); }
  .avatar-orange { background: linear-gradient(135deg, #F59E0B, #EF4444); }

  .testimonial-info h4 {
    font-size: 1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.2rem;
  }

  .testimonial-info p {
    font-size: 0.85rem;
    color: #9CA3AF;
  }

  .testimonial-badge {
    position: absolute;
    top: 1.5rem;
    right: 1.5rem;
    padding: 0.4rem 0.8rem;
    border-radius: 50px;
    font-size: 0.7rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .badge-gold { 
    background: linear-gradient(135deg, #FFD700, #FFA500); 
    color: #1F2937; 
  }
  .badge-green { 
    background: linear-gradient(135deg, #10B981, #059669); 
    color: white; 
  }
  .badge-blue { 
    background: linear-gradient(135deg, #3B82F6, #1D4ED8); 
    color: white; 
  }

  /* ========================================
     CTA Section
  ======================================== */
  .cta-section {
    background: white;
    border-radius: 30px;
    padding: 5rem 3rem;
    margin: 6rem 0;
    text-align: center;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.08);
    border: 1px solid #F3F4F6;
    position: relative;
    overflow: hidden;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #a855f7, #ec4899);
  }

  .cta-icon {
    font-size: 4rem;
    margin-bottom: 1.5rem;
    animation: float 4s ease-in-out infinite;
  }

  .cta-title {
    font-size: 2.8rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    line-height: 1.2;
  }

  .cta-description {
    font-size: 1.2rem;
    color: #6B7280;
    margin-bottom: 2.5rem;
    max-width: 600px;
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
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.05rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }

  .cta-btn-primary {
    background: linear-gradient(135deg, #6366f1, #8b5cf6);
    color: white;
    box-shadow: 0 10px 40px rgba(99, 102, 241, 0.4);
  }

  .cta-btn-primary:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 50px rgba(99, 102, 241, 0.5);
    color: white;
  }

  .cta-btn-secondary {
    background: #F3F4F6;
    color: #4B5563;
  }

  .cta-btn-secondary:hover {
    background: #E5E7EB;
    transform: translateY(-5px);
    color: #1F2937;
  }

  /* ========================================
     Responsive Design
  ======================================== */
  @media (max-width: 1100px) {
    .paths-grid {
      grid-template-columns: 1fr;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .why-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 900px) {
    .offer-grid,
    .testimonials-grid {
      grid-template-columns: 1fr;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
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

    .section-title {
      font-size: 2.2rem;
    }

    .why-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
    }

    .floating-icons {
      display: none;
    }

    .cta-title {
      font-size: 2rem;
    }
  }

  @media (max-width: 480px) {
    .hero-buttons {
      flex-direction: column;
      align-items: center;
    }

    .hero-btn {
      width: 100%;
      max-width: 280px;
      justify-content: center;
    }

    .stats-grid {
      grid-template-columns: 1fr;
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
  }
</style>

<!-- Hero Section -->
<section class="hero-section">
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
  
  <div class="floating-icons">
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🚀</span>
    <span class="floating-icon">🎯</span>
    <span class="floating-icon">🏆</span>
    <span class="floating-icon">🧠</span>
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
      <span class="en-content">Empowering Future Tech Leaders</span>
      <span class="zh-content">培养未来科技领袖</span>
    </p>
    
    <p class="hero-description">
      <span class="en-content">Elite programming education, competition training, and research mentorship for students aged 10-18. Choose your path to excellence.</span>
      <span class="zh-content">为10-18岁学生提供精英编程教育、竞赛培训和研究指导。选择您的卓越之路。</span>
    </p>
    
    <div class="hero-buttons">
      <a href="./course.html" class="hero-btn hero-btn-primary">
        <span class="en-content">🚀 Explore Programs</span>
        <span class="zh-content">🚀 探索课程</span>
      </a>
      <a href="./contact.html" class="hero-btn hero-btn-secondary">
        <span class="en-content">📞 Free Consultation</span>
        <span class="zh-content">📞 免费咨询</span>
      </a>
    </div>
  </div>
</section>

<!-- What We Offer Section -->
<section class="offer-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">What We Offer</span>
      <span class="zh-content">我们提供</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Three Pillars of Excellence</span>
      <span class="zh-content">卓越的三大支柱</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Comprehensive education designed to prepare students for any tech career path</span>
      <span class="zh-content">全面的教育，旨在为学生的任何科技职业道路做好准备</span>
    </p>
  </div>
  
  <div class="offer-grid">
    <div class="offer-card">
      <div class="offer-icon offer-icon-programming">💻</div>
      <h3 class="offer-title">
        <span class="en-content">Programming Courses</span>
        <span class="zh-content">编程课程</span>
      </h3>
      <p class="offer-description">
        <span class="en-content">From fundamentals to advanced topics, master the languages and skills that power modern technology.</span>
        <span class="zh-content">从基础到高级，掌握驱动现代技术的语言和技能。</span>
      </p>
      <ul class="offer-list">
        <li><span class="en-content">Python, Java, C++ Fundamentals</span><span class="zh-content">Python、Java、C++ 基础</span></li>
        <li><span class="en-content">AP Computer Science A & Principles</span><span class="zh-content">AP计算机科学A和原理</span></li>
        <li><span class="en-content">Data Structures & Algorithms</span><span class="zh-content">数据结构与算法</span></li>
        <li><span class="en-content">Full-Stack Web Development</span><span class="zh-content">全栈网站开发</span></li>
      </ul>
    </div>
    
    <div class="offer-card">
      <div class="offer-icon offer-icon-competition">🏆</div>
      <h3 class="offer-title">
        <span class="en-content">Competition Training</span>
        <span class="zh-content">竞赛培训</span>
      </h3>
      <p class="offer-description">
        <span class="en-content">Strategic preparation for prestigious competitions that stand out on college applications.</span>
        <span class="zh-content">为在大学申请中脱颖而出的著名竞赛提供战略性准备。</span>
      </p>
      <ul class="offer-list">
        <li><span class="en-content">USACO (Bronze → Platinum)</span><span class="zh-content">USACO（铜→白金）</span></li>
        <li><span class="en-content">AMC 8/10/12, AIME, USAMO</span><span class="zh-content">AMC 8/10/12、AIME、USAMO</span></li>
        <li><span class="en-content">USAAIO, Kaggle, ACSL</span><span class="zh-content">USAAIO、Kaggle、ACSL</span></li>
        <li><span class="en-content">HiMCM, WorldQuant</span><span class="zh-content">HiMCM、WorldQuant</span></li>
      </ul>
    </div>
    
    <div class="offer-card">
      <div class="offer-icon offer-icon-research">🔬</div>
      <h3 class="offer-title">
        <span class="en-content">Research & AI</span>
        <span class="zh-content">研究与人工智能</span>
      </h3>
      <p class="offer-description">
        <span class="en-content">Cutting-edge AI/ML training and research mentorship for future innovators.</span>
        <span class="zh-content">为未来创新者提供前沿AI/ML培训和研究指导。</span>
      </p>
      <ul class="offer-list">
        <li><span class="en-content">Machine Learning Fundamentals</span><span class="zh-content">机器学习基础</span></li>
        <li><span class="en-content">Deep Learning & Neural Networks</span><span class="zh-content">深度学习与神经网络</span></li>
        <li><span class="en-content">Computer Vision & NLP</span><span class="zh-content">计算机视觉与NLP</span></li>
        <li><span class="en-content">Research Project Mentorship</span><span class="zh-content">研究项目指导</span></li>
      </ul>
    </div>
  </div>
</section>

<!-- Learning Paths Section -->
<section class="paths-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Choose Your Path</span>
      <span class="zh-content">选择您的路径</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Learning Paths</span>
      <span class="zh-content">学习路径</span>
      <span class="section-title-underline"></span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Three distinct tracks to match your interests and goals. Each path leads to excellence.</span>
      <span class="zh-content">三条不同的路线，匹配您的兴趣和目标。每条路径都通向卓越。</span>
    </p>
  </div>
  
  <div class="paths-grid">
    <!-- Algorithm Competition Path -->
    <div class="path-card">
      <div class="path-card-header path-header-algo">
        <div class="path-icon">⚡</div>
        <h3 class="path-title">
          <span class="en-content">Algorithm Track</span>
          <span class="zh-content">算法竞赛路线</span>
        </h3>
        <p class="path-tagline">
          <span class="en-content">Competitive Programming Excellence</span>
          <span class="zh-content">竞赛编程卓越</span>
        </p>
      </div>
      <div class="path-card-body">
        <p class="path-description">
          <span class="en-content">Master algorithmic problem-solving and compete in prestigious olympiads. Perfect for students who love logical challenges.</span>
          <span class="zh-content">掌握算法问题解决并参加著名奥赛。适合热爱逻辑挑战的学生。</span>
        </p>
        
        <div class="path-stages">
          <div class="path-stage path-stage-algo">
            <span class="path-stage-number">1</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Foundation</span><span class="zh-content">基础</span></h4>
              <p><span class="en-content">C++/Python basics, intro algorithms</span><span class="zh-content">C++/Python基础，算法入门</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-algo">
            <span class="path-stage-number">2</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></h4>
              <p><span class="en-content">Trees, graphs, hash tables, heaps</span><span class="zh-content">树、图、哈希表、堆</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-algo">
            <span class="path-stage-number">3</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Advanced Algorithms</span><span class="zh-content">高级算法</span></h4>
              <p><span class="en-content">DP, graph algorithms, number theory</span><span class="zh-content">动态规划、图算法、数论</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-algo">
            <span class="path-stage-number">4</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Competition Prep</span><span class="zh-content">竞赛备战</span></h4>
              <p><span class="en-content">USACO Silver → Gold → Platinum</span><span class="zh-content">USACO 银→金→白金</span></p>
            </div>
          </div>
        </div>
        
        <div class="path-target path-target-algo">
          <span class="path-target-icon">🎯</span>
          <span class="path-target-text">
            <span class="en-content">Target: <span>USACO Platinum, ACSL, AMC/AIME</span></span>
            <span class="zh-content">目标：<span>USACO白金、ACSL、AMC/AIME</span></span>
          </span>
        </div>
      </div>
    </div>
    
    <!-- Machine Learning Path -->
    <div class="path-card">
      <div class="path-card-header path-header-ml">
        <div class="path-icon">🤖</div>
        <h3 class="path-title">
          <span class="en-content">AI/ML Track</span>
          <span class="zh-content">人工智能路线</span>
        </h3>
        <p class="path-tagline">
          <span class="en-content">Data Science & Machine Learning</span>
          <span class="zh-content">数据科学与机器学习</span>
        </p>
      </div>
      <div class="path-card-body">
        <p class="path-description">
          <span class="en-content">Learn AI/ML from fundamentals to advanced applications. Build real-world projects and compete in data science challenges.</span>
          <span class="zh-content">从基础到高级应用学习AI/ML。构建真实项目并参加数据科学挑战。</span>
        </p>
        
        <div class="path-stages">
          <div class="path-stage path-stage-ml">
            <span class="path-stage-number">1</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Python & Data</span><span class="zh-content">Python与数据</span></h4>
              <p><span class="en-content">Python, NumPy, Pandas, visualization</span><span class="zh-content">Python、NumPy、Pandas、可视化</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-ml">
            <span class="path-stage-number">2</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Machine Learning</span><span class="zh-content">机器学习</span></h4>
              <p><span class="en-content">Supervised/unsupervised learning</span><span class="zh-content">监督/无监督学习</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-ml">
            <span class="path-stage-number">3</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Deep Learning</span><span class="zh-content">深度学习</span></h4>
              <p><span class="en-content">Neural networks, CNN, RNN, transformers</span><span class="zh-content">神经网络、CNN、RNN、Transformer</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-ml">
            <span class="path-stage-number">4</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Applications</span><span class="zh-content">应用</span></h4>
              <p><span class="en-content">CV, NLP, competition projects</span><span class="zh-content">计算机视觉、NLP、竞赛项目</span></p>
            </div>
          </div>
        </div>
        
        <div class="path-target path-target-ml">
          <span class="path-target-icon">🎯</span>
          <span class="path-target-text">
            <span class="en-content">Target: <span>USAAIO, Kaggle Medals, HiMCM</span></span>
            <span class="zh-content">目标：<span>USAAIO、Kaggle奖牌、HiMCM</span></span>
          </span>
        </div>
      </div>
    </div>
    
    <!-- Research Path -->
    <div class="path-card">
      <div class="path-card-header path-header-research">
        <div class="path-icon">🔬</div>
        <h3 class="path-title">
          <span class="en-content">Research Track</span>
          <span class="zh-content">科研路线</span>
        </h3>
        <p class="path-tagline">
          <span class="en-content">Academic Research & Publications</span>
          <span class="zh-content">学术研究与发表</span>
        </p>
      </div>
      <div class="path-card-body">
        <p class="path-description">
          <span class="en-content">Conduct original research under mentorship. Develop projects worthy of science fairs and academic publications.</span>
          <span class="zh-content">在导师指导下进行原创研究。开发值得参加科学展览和学术发表的项目。</span>
        </p>
        
        <div class="path-stages">
          <div class="path-stage path-stage-research">
            <span class="path-stage-number">1</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Programming Skills</span><span class="zh-content">编程技能</span></h4>
              <p><span class="en-content">Python, data analysis, web development</span><span class="zh-content">Python、数据分析、网站开发</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-research">
            <span class="path-stage-number">2</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Research Methods</span><span class="zh-content">研究方法</span></h4>
              <p><span class="en-content">Literature review, methodology design</span><span class="zh-content">文献综述、方法论设计</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-research">
            <span class="path-stage-number">3</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Project Development</span><span class="zh-content">项目开发</span></h4>
              <p><span class="en-content">Build original research project</span><span class="zh-content">构建原创研究项目</span></p>
            </div>
          </div>
          <div class="path-stage path-stage-research">
            <span class="path-stage-number">4</span>
            <div class="path-stage-content">
              <h4><span class="en-content">Publication</span><span class="zh-content">发表</span></h4>
              <p><span class="en-content">Paper writing, submission, presentation</span><span class="zh-content">论文撰写、投稿、演示</span></p>
            </div>
          </div>
        </div>
        
        <div class="path-target path-target-research">
          <span class="path-target-icon">🎯</span>
          <span class="path-target-text">
            <span class="en-content">Target: <span>Science Fairs, Publications, Patents</span></span>
            <span class="zh-content">目标：<span>科学展览、论文发表、专利</span></span>
          </span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Why Choose Us Section -->
<section class="why-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Why AIcoding</span>
      <span class="zh-content">为什么选择AIcoding</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">The AIcoding Difference</span>
      <span class="zh-content">AIcoding的独特优势</span>
      <span class="section-title-underline"></span>
    </h2>
  </div>
  
  <div class="why-grid">
    <div class="why-card">
      <div class="why-icon">👨‍🏫</div>
      <h4 class="why-title">
        <span class="en-content">Expert Instructors</span>
        <span class="zh-content">专家导师</span>
      </h4>
      <p class="why-description">
        <span class="en-content">PhD holders, FAANG engineers, and competition gold medalists</span>
        <span class="zh-content">博士、FAANG工程师和竞赛金牌得主</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">👥</div>
      <h4 class="why-title">
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h4>
      <p class="why-description">
        <span class="en-content">Maximum 8 students per class for personalized attention</span>
        <span class="zh-content">每班最多8名学生，确保个性化关注</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">📈</div>
      <h4 class="why-title">
        <span class="en-content">Proven Results</span>
        <span class="zh-content">成果显著</span>
      </h4>
      <p class="why-description">
        <span class="en-content">90% success rate in competitions and AP exams</span>
        <span class="zh-content">竞赛和AP考试90%成功率</span>
      </p>
    </div>
    
    <div class="why-card">
      <div class="why-icon">🎯</div>
      <h4 class="why-title">
        <span class="en-content">Flexible Learning</span>
        <span class="zh-content">灵活学习</span>
      </h4>
      <p class="why-description">
        <span class="en-content">Online and in-person options to fit your schedule</span>
        <span class="zh-content">线上和线下选项，适合您的时间安排</span>
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
        <span class="en-content">Awards</span>
        <span class="zh-content">奖项</span>
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
        <span class="en-content">Years</span>
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
      <span class="en-content">What Students Say</span>
      <span class="zh-content">学生评价</span>
      <span class="section-title-underline"></span>
    </h2>
  </div>
  
  <div class="testimonials-grid">
    <div class="testimonial-card">
      <span class="testimonial-badge badge-gold">USACO Gold</span>
      <div class="testimonial-quote">"</div>
      <p class="testimonial-text">
        <span class="en-content">The structured training helped me advance from Bronze to Gold in 8 months. The problem-solving strategies are invaluable.</span>
        <span class="zh-content">结构化培训帮助我在8个月内从铜级晋升到金级。问题解决策略非常宝贵。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar avatar-purple">A</div>
        <div class="testimonial-info">
          <h4>Alex C.</h4>
          <p><span class="en-content">Algorithm Track</span><span class="zh-content">算法竞赛路线</span></p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-green">AP Score: 5</span>
      <div class="testimonial-quote">"</div>
      <p class="testimonial-text">
        <span class="en-content">The AP CSA course was incredibly well-structured. Practice exams and FRQ training prepared me perfectly. Got a 5!</span>
        <span class="zh-content">AP CSA课程结构非常完善。模拟考试和FRQ培训让我准备充分。拿到了5分！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar avatar-green">S</div>
        <div class="testimonial-info">
          <h4>Sarah W.</h4>
          <p><span class="en-content">AP Track</span><span class="zh-content">AP课程</span></p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-blue">Research Published</span>
      <div class="testimonial-quote">"</div>
      <p class="testimonial-text">
        <span class="en-content">My mentor guided me through my first research project. We published a paper and I won at the regional science fair!</span>
        <span class="zh-content">导师指导我完成了第一个研究项目。我们发表了论文，我还在地区科学展览中获奖！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar avatar-orange">M</div>
        <div class="testimonial-info">
          <h4>Michael L.</h4>
          <p><span class="en-content">Research Track</span><span class="zh-content">科研路线</span></p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-icon">🚀</div>
  <h2 class="cta-title">
    <span class="en-content">Ready to Start Your Journey?</span>
    <span class="zh-content">准备好开始您的旅程了吗？</span>
  </h2>
  <p class="cta-description">
    <span class="en-content">Join AIcoding Academy and unlock your full potential. Schedule a free consultation to find the perfect learning path for you.</span>
    <span class="zh-content">加入AIcoding学院，释放您的全部潜力。预约免费咨询，找到最适合您的学习路径。</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-btn cta-btn-primary">
      <span class="en-content">📞 Free Consultation</span>
      <span class="zh-content">📞 免费咨询</span>
    </a>
    <a href="./course.html" class="cta-btn cta-btn-secondary">
      <span class="en-content">📚 View All Courses</span>
      <span class="zh-content">📚 查看所有课程</span>
    </a>
  </div>
</section>
