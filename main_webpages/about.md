---
layout: default
title: About AIcoding
title_zh: 关于 AIcoding
description: Elite Programming Education by PhD Computer Scientists
description_zh: 由计算机科学博士提供的精英编程教育
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

  @keyframes borderGlow {
    0%, 100% { opacity: 0.5; }
    50% { opacity: 1; }
  }

  @keyframes expand {
    from { transform: scaleX(0); }
    to { transform: scaleX(1); }
  }

  @keyframes countUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes imageFloat {
    0%, 100% { transform: rotate(-2deg) translateY(0px); }
    50% { transform: rotate(-2deg) translateY(-15px); }
  }

  @keyframes morphShape {
    0%, 100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
    20% { border-radius: 50% 50% 50% 50% / 60% 40% 60% 40%; }
    40% { border-radius: 70% 30% 50% 50% / 50% 60% 40% 60%; }
    60% { border-radius: 40% 60% 30% 70% / 70% 50% 50% 30%; }
    80% { border-radius: 60% 40% 60% 40% / 40% 70% 30% 60%; }
  }

  @keyframes windMorph {
    0%, 100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; transform: scale(1) rotate(0deg); }
    25% { border-radius: 60% 40% 50% 50% / 40% 60% 40% 60%; transform: scale(1.02) rotate(5deg); }
    50% { border-radius: 50% 50% 30% 70% / 60% 40% 60% 40%; transform: scale(1) rotate(-5deg); }
    75% { border-radius: 40% 60% 60% 40% / 50% 50% 50% 50%; transform: scale(1.02) rotate(3deg); }
  }

  @keyframes sealRotate {
    0%, 100% { transform: rotate(15deg) scale(1); }
    25% { transform: rotate(10deg) scale(1.05); }
    50% { transform: rotate(20deg) scale(1); }
    75% { transform: rotate(12deg) scale(1.05); }
  }

  @keyframes cornerGlow {
    0%, 100% { opacity: 0.7; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.1); }
  }

  /* ========================================
     About Hero - Ultra Premium Cosmic
  ======================================== */
  .about-hero {
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
    max-width: 700px;
    margin: 0 auto;
    line-height: 1.7;
  }

  /* ========================================
     Mission Section - Premium Glass
  ======================================== */
  .mission-section {
    background: white;
    padding: 4.5rem 3.5rem;
    border-radius: 32px;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.02);
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out;
    border: 1px solid rgba(0, 0, 0, 0.04);
  }

  .mission-section::before {
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

  .mission-section::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(99, 102, 241, 0.05), transparent);
    animation: shimmer 4s infinite;
    pointer-events: none;
  }

  .section-header {
    text-align: center;
    margin-bottom: 2.5rem;
  }

  .section-eyebrow {
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

  .section-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 0.5rem;
    position: relative;
    display: inline-block;
    letter-spacing: -1px;
  }

  .section-title::after {
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

  .mission-text {
    font-size: 1.25rem;
    line-height: 1.9;
    color: #4B5563;
    text-align: center;
    max-width: 900px;
    margin: 2rem auto 0;
    position: relative;
    z-index: 1;
  }

  /* ========================================
     Instructor Section - Premium Design
  ======================================== */
  .instructor-section {
    background: white;
    padding: 5rem 3.5rem;
    border-radius: 32px;
    margin: 5rem 0;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.02);
    position: relative;
    overflow: hidden;
    border: 1px solid rgba(0, 0, 0, 0.04);
  }

  .instructor-section::before {
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

  .instructor-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 3rem;
    gap: 3rem;
  }

  .instructor-image-container {
    position: relative;
    width: 100%;
    display: flex;
    justify-content: center;
    animation: slideInUp 1s ease-out;
  }

  .instructor-image-wrapper {
    position: relative;
    width: 300px;
    height: 300px;
  }

  .instructor-image-frame {
    width: 100%;
    height: 100%;
    position: relative;
    padding: 15px;
    background: linear-gradient(135deg, rgba(245,242,235,0.9), white);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    box-shadow: 
      0 20px 60px rgba(0, 0, 0, 0.15),
      inset 0 0 40px rgba(0, 0, 0, 0.05);
    transform: rotate(-2deg);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    animation: morphShape 15s ease-in-out infinite, imageFloat 6s ease-in-out infinite;
  }

  .instructor-image-frame::before {
    content: '';
    position: absolute;
    top: -6px;
    left: -6px;
    right: -6px;
    bottom: -6px;
    background: linear-gradient(45deg, 
      #6366f1 0%,
      #8b5cf6 25%,
      #ec4899 50%,
      #f59e0b 75%,
      #6366f1 100%);
    background-size: 400% 400%;
    border-radius: inherit;
    z-index: -1;
    opacity: 0.8;
    animation: gradientFlow 8s ease infinite, morphShape 15s ease-in-out infinite;
  }

  .wind-effect {
    position: absolute;
    top: -12px;
    left: -12px;
    right: -12px;
    bottom: -12px;
    border: 2px solid rgba(99, 102, 241, 0.3);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    opacity: 0.4;
    animation: windMorph 12s ease-in-out infinite;
    z-index: -2;
  }

  .wind-effect-2 {
    position: absolute;
    top: -18px;
    left: -18px;
    right: -18px;
    bottom: -18px;
    border: 1px solid rgba(236, 72, 153, 0.2);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    opacity: 0.3;
    animation: windMorph 10s ease-in-out infinite reverse;
    animation-delay: -2s;
    z-index: -3;
  }

  .instructor-image-frame:hover {
    animation-play-state: paused;
    transform: rotate(0deg) scale(1.05);
    box-shadow: 
      0 30px 80px rgba(99, 102, 241, 0.25),
      inset 0 0 40px rgba(0, 0, 0, 0.05);
  }

  .instructor-image-frame:hover::before {
    animation-duration: 3s;
    opacity: 1;
  }

  .instructor-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: sepia(5%) contrast(1.05);
    border: 4px solid white;
    border-radius: inherit;
    position: relative;
    z-index: 1;
  }

  /* Decorative Corner Elements */
  .image-corner {
    position: absolute;
    width: 25px;
    height: 25px;
    border: 2px solid rgba(99, 102, 241, 0.6);
    z-index: 2;
    animation: cornerGlow 4s ease-in-out infinite;
    opacity: 0.7;
  }

  .image-corner.top-left {
    top: 10px;
    left: 10px;
    border-right: none;
    border-bottom: none;
    border-radius: 30% 0 0 0;
  }

  .image-corner.top-right {
    top: 10px;
    right: 10px;
    border-left: none;
    border-bottom: none;
    border-radius: 0 30% 0 0;
    animation-delay: 1s;
  }

  .image-corner.bottom-left {
    bottom: 10px;
    left: 10px;
    border-right: none;
    border-top: none;
    border-radius: 0 0 0 30%;
    animation-delay: 2s;
  }

  .image-corner.bottom-right {
    bottom: 10px;
    right: 10px;
    border-left: none;
    border-top: none;
    border-radius: 0 0 30% 0;
    animation-delay: 3s;
  }

  .image-seal {
    position: absolute;
    bottom: 25px;
    right: 25px;
    width: 55px;
    height: 55px;
    background: linear-gradient(135deg, #6366f1, #8b5cf6);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-family: 'Noto Serif SC', serif;
    font-weight: 700;
    font-size: 1.2rem;
    box-shadow: 0 8px 25px rgba(99, 102, 241, 0.4);
    transform: rotate(15deg);
    animation: sealRotate 10s ease-in-out infinite;
    z-index: 3;
  }

  .instructor-info {
    padding: 0 2rem;
    text-align: center;
    max-width: 900px;
    margin: 0 auto;
    animation: slideInUp 1s ease-out 0.3s backwards;
  }

  .instructor-name {
    font-size: 2.8rem;
    font-weight: 900;
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.8rem;
    text-align: center;
  }

  .instructor-title {
    font-size: 1.3rem;
    color: #6B7280;
    margin-bottom: 2rem;
    font-weight: 600;
    text-align: center;
  }

  .instructor-bio {
    color: #4B5563;
    line-height: 1.9;
    font-size: 1.1rem;
    margin-bottom: 1.5rem;
    text-align: left;
  }

  .instructor-highlights {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 2.5rem;
    justify-content: center;
  }

  .highlight-badge {
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
    color: #4F46E5;
    padding: 0.6rem 1.3rem;
    border-radius: 50px;
    font-size: 0.9rem;
    font-weight: 700;
    border: 1px solid rgba(99, 102, 241, 0.2);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .highlight-badge:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 10px 25px rgba(99, 102, 241, 0.2);
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.15), rgba(139, 92, 246, 0.15));
  }

  /* ========================================
     Values Section - Premium Cards
  ======================================== */
  .values-section {
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

  .values-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    position: relative;
    z-index: 1;
    margin-top: 3rem;
  }

  .value-card {
    background: white;
    padding: 2.5rem 2rem;
    border-radius: 24px;
    box-shadow: 
      0 15px 40px rgba(0, 0, 0, 0.06),
      0 1px 3px rgba(0, 0, 0, 0.02);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .value-card:nth-child(1) { animation-delay: 0.1s; }
  .value-card:nth-child(2) { animation-delay: 0.2s; }
  .value-card:nth-child(3) { animation-delay: 0.3s; }
  .value-card:nth-child(4) { animation-delay: 0.4s; }
  .value-card:nth-child(5) { animation-delay: 0.5s; }
  .value-card:nth-child(6) { animation-delay: 0.6s; }

  .value-card::before {
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

  .value-card:hover::before {
    transform: scaleX(1);
  }

  .value-card::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(99, 102, 241, 0.05), transparent);
    transition: none;
    z-index: 0;
  }

  .value-card:hover::after {
    animation: shimmer 0.8s ease forwards;
  }

  .value-card:hover {
    transform: translateY(-12px) scale(1.02);
    box-shadow: 
      0 30px 60px rgba(99, 102, 241, 0.15),
      0 0 0 2px rgba(99, 102, 241, 0.1);
  }

  .value-icon {
    font-size: 3.5rem;
    margin-bottom: 1.2rem;
    text-align: center;
    animation: float 5s ease-in-out infinite;
    position: relative;
    z-index: 1;
  }

  .value-title {
    font-size: 1.4rem;
    font-weight: 800;
    color: #1F2937;
    text-align: center;
    margin-bottom: 0.8rem;
    position: relative;
    z-index: 1;
  }

  .value-description {
    color: #6B7280;
    text-align: center;
    line-height: 1.7;
    font-size: 0.95rem;
    position: relative;
    z-index: 1;
  }

  /* ========================================
     Stats Section - Cosmic Theme
  ======================================== */
  .stats-section {
    background: linear-gradient(135deg, 
      #0f0c29 0%, 
      #302b63 25%, 
      #24243e 50%,
      #1a1a2e 75%,
      #0f0c29 100%);
    background-size: 400% 400%;
    animation: gradientFlow 20s ease infinite;
    border-radius: 40px;
    padding: 5rem 3rem;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 50px 100px rgba(0, 0, 0, 0.4),
      inset 0 0 100px rgba(99, 102, 241, 0.1);
  }

  .stats-section::before {
    content: '';
    position: absolute;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
    background: conic-gradient(
      from 0deg at 50% 50%,
      transparent 0deg,
      rgba(99, 102, 241, 0.08) 60deg,
      transparent 120deg,
      rgba(139, 92, 246, 0.06) 180deg,
      transparent 240deg,
      rgba(236, 72, 153, 0.04) 300deg,
      transparent 360deg
    );
    animation: rotateGlow 30s linear infinite;
    pointer-events: none;
  }

  .stats-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.3;
    animation: morphBlob 20s ease-in-out infinite;
    pointer-events: none;
  }

  .stats-orb-1 {
    width: 350px;
    height: 350px;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.5), rgba(139, 92, 246, 0.3));
    top: -100px;
    left: -80px;
  }

  .stats-orb-2 {
    width: 250px;
    height: 250px;
    background: linear-gradient(135deg, rgba(236, 72, 153, 0.4), rgba(239, 68, 68, 0.2));
    bottom: -80px;
    right: -50px;
    animation-delay: -10s;
  }

  .stats-content {
    position: relative;
    z-index: 10;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2.5rem;
    margin-top: 3rem;
  }

  .stat-item {
    text-align: center;
    animation: countUp 1s ease-out backwards;
    padding: 1.5rem;
    background: rgba(255, 255, 255, 0.03);
    border-radius: 20px;
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.05);
    transition: all 0.4s ease;
  }

  .stat-item:nth-child(1) { animation-delay: 0.1s; }
  .stat-item:nth-child(2) { animation-delay: 0.2s; }
  .stat-item:nth-child(3) { animation-delay: 0.3s; }
  .stat-item:nth-child(4) { animation-delay: 0.4s; }

  .stat-item:hover {
    background: rgba(255, 255, 255, 0.06);
    transform: translateY(-5px);
  }

  .stat-number {
    font-size: 4rem;
    font-weight: 900;
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 50%, #ddd6fe 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.5rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: rgba(255, 255, 255, 0.7);
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-weight: 600;
  }

  /* ========================================
     Philosophy Section - Premium Glass
  ======================================== */
  .philosophy-section {
    background: linear-gradient(135deg, 
      rgba(245, 158, 11, 0.08) 0%, 
      rgba(251, 191, 36, 0.05) 50%, 
      rgba(245, 158, 11, 0.03) 100%);
    backdrop-filter: blur(10px);
    padding: 4.5rem 3.5rem;
    border-radius: 32px;
    margin: 5rem 0;
    border-left: 6px solid;
    border-image: linear-gradient(180deg, #f59e0b, #fbbf24, #f59e0b) 1;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 60px rgba(245, 158, 11, 0.1);
  }

  .philosophy-section::before {
    content: '';
    position: absolute;
    top: 50%;
    right: 5%;
    width: 350px;
    height: 350px;
    background: radial-gradient(circle, rgba(245, 158, 11, 0.1) 0%, transparent 70%);
    animation: pulse 5s ease-in-out infinite;
    pointer-events: none;
  }

  .philosophy-title {
    font-size: 2.5rem;
    font-weight: 800;
    color: #92400E;
    margin-bottom: 2.5rem;
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .philosophy-list {
    list-style: none;
    padding: 0;
    position: relative;
    z-index: 1;
    max-width: 900px;
    margin: 0 auto;
  }

  .philosophy-item {
    padding: 1.5rem 2rem;
    color: #78350F;
    display: flex;
    align-items: flex-start;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    background: rgba(255, 255, 255, 0.5);
    border-radius: 16px;
    margin-bottom: 1rem;
    border: 1px solid rgba(245, 158, 11, 0.2);
  }

  .philosophy-item:hover {
    transform: translateX(15px);
    background: rgba(255, 255, 255, 0.8);
    box-shadow: 0 10px 30px rgba(245, 158, 11, 0.1);
  }

  .philosophy-check {
    color: #F59E0B;
    font-weight: bold;
    margin-right: 1.5rem;
    font-size: 1.5rem;
    flex-shrink: 0;
    width: 40px;
    height: 40px;
    background: linear-gradient(135deg, rgba(245, 158, 11, 0.2), rgba(251, 191, 36, 0.2));
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .philosophy-item strong {
    color: #92400E;
    font-weight: 700;
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
    margin-bottom: 2.5rem;
    color: rgba(255, 255, 255, 0.85);
    max-width: 550px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.7;
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
  @media (max-width: 1200px) {
    .values-grid {
      grid-template-columns: repeat(2, 1fr);
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 2.5rem;
    }

    .section-title {
      font-size: 2rem;
    }

    .values-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
    }

    .stats-grid {
      grid-template-columns: 1fr 1fr;
      gap: 1.5rem;
    }

    .stat-number {
      font-size: 3rem;
    }

    .cta-title {
      font-size: 2rem;
    }

    .about-hero {
      border-radius: 24px;
      min-height: 45vh;
    }

    .mission-section,
    .instructor-section {
      padding: 3rem 1.5rem;
      border-radius: 24px;
    }

    .values-section,
    .stats-section,
    .cta-section {
      padding: 3rem 1.5rem;
      border-radius: 24px;
    }

    .philosophy-section {
      padding: 3rem 1.5rem;
      border-radius: 24px;
    }

    .hero-icons {
      display: none;
    }

    .instructor-image-wrapper {
      width: 250px;
      height: 250px;
    }
  }

  @media (max-width: 480px) {
    .hero-title {
      font-size: 2rem;
    }

    .stats-grid {
      grid-template-columns: 1fr;
    }

    .cta-button {
      padding: 1rem 2.5rem;
      font-size: 1rem;
    }

    .philosophy-item {
      padding: 1rem 1.2rem;
    }
  }
</style>

<!-- About Hero -->
<section class="about-hero">
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
    <span class="hero-floating-icon">🎓</span>
    <span class="hero-floating-icon">💻</span>
    <span class="hero-floating-icon">🏆</span>
    <span class="hero-floating-icon">🚀</span>
  </div>
  
  <div class="hero-content">
    <div class="hero-icon">🌟</div>
    <h1 class="hero-title">
      <span class="en-content">About AIcoding Edu</span>
      <span class="zh-content">关于 AIcoding 学院</span>
    </h1>
    <p class="hero-subtitle">
      <span class="en-content">An educational brand created by Ph.D. computer science majors dedicated to excellence</span>
      <span class="zh-content">由计算机科学博士创立的致力于卓越的教育品牌</span>
    </p>
  </div>
</section>

<!-- Mission Statement -->
<section class="mission-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Who We Are</span>
      <span class="zh-content">关于我们</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Our Mission</span>
      <span class="zh-content">我们的使命</span>
    </h2>
  </div>
  <p class="mission-text">
    <span class="en-content">AIcoding is an educational brand created by a group of Ph.D. computer science majors to provide premium tutoring and background improvement services to K-12 students. We bridge the gap between academic excellence and practical programming skills, preparing the next generation of tech innovators.</span>
    <span class="zh-content">AIcoding 是由一群计算机科学博士创立的教育品牌，为K-12学生提供优质的辅导和背景提升服务。我们在学术卓越与实践编程技能之间架起桥梁，培养下一代科技创新者。</span>
  </p>
</section>

<!-- Instructor Introduction -->
<section class="instructor-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Expert Guidance</span>
      <span class="zh-content">专业指导</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">Meet Our Lead Instructor</span>
      <span class="zh-content">认识我们的首席讲师</span>
    </h2>
  </div>
  
  <div class="instructor-content">
    <div class="instructor-image-container">
      <div class="instructor-image-wrapper">
        <div class="instructor-image-frame">
          <div class="wind-effect"></div>
          <div class="wind-effect-2"></div>
          <div class="image-corner top-left"></div>
          <div class="image-corner top-right"></div>
          <div class="image-corner bottom-left"></div>
          <div class="image-corner bottom-right"></div>
          <img src="{{ site.baseurl }}/images/h.png" alt="H Teacher" class="instructor-image">
          <div class="image-seal">H</div>
        </div>
      </div>
    </div>
    
    <div class="instructor-info">
      <h3 class="instructor-name">
        <span class="en-content">Dr. H</span>
        <span class="zh-content">H 老师</span>
      </h3>
      <p class="instructor-title">
        <span class="en-content">Machine Learning Engineer & Research Scientist</span>
        <span class="zh-content">机器学习工程师与科研研究员</span>
      </p>
      <p class="instructor-bio">
        <span class="en-content">H is a machine learning engineer and research scientist with a Ph.D. in Computer Science. He was a research assistant in the Human-Computer Interaction Lab and has served as a teaching assistant for graduate-level computer science courses twice at Stony Brook University. His research interests include machine learning, deep learning, medical diagnosis through artificial intelligence, and Large Language Models. He has published academic papers eight times in top-tier conferences in the fields of machine learning and human-computer interaction (CHI, UIST, Ubicomp, etc.) and has won the best paper award twice. He has been invited multiple times to serve as a paper reviewer for CHI and UIST.</span>
        <span class="zh-content">H老师是机器学习工程师和科研研究员，拥有美国计算机博士学位，曾任人机交互实验室研究助理。他两次任职石溪大学计算机研究生课助教。他的研究方向包括机器学习、深度学习、人工智能医学诊断和大语言模型。八次在计算机机器学习和人机交互顶会 (CHI, UIST, UBICOMP等) 发表学术论文并两次获得最佳论文奖。他曾多次被邀请作为CHI和UIST论文审稿人。</span>
      </p>
      <p class="instructor-bio">
        <span class="en-content">With years of experience in both 1-on-1 and group instruction entirely in English, he is proficient in Python, Java, C++, AP Computer Science A, AP Computer Science Principles, object-oriented programming, data structures, algorithms, machine learning, artificial intelligence, and competition preparation for USACO, AMC/AIME, and USAAIO.</span>
        <span class="zh-content">他有多年的1v1和1v多全英文教学经验，擅长Python、Java、C++、APCSA、APCSP、面向对象编程、数据结构、算法、机器学习、人工智能，以及USACO竞赛、AMC/AIME竞赛和USAAIO竞赛的培训。</span>
      </p>
      
      <div class="instructor-highlights">
        <span class="highlight-badge">Ph.D. Computer Science</span>
        <span class="highlight-badge">8x Published Author</span>
        <span class="highlight-badge">2x Best Paper Award</span>
        <span class="highlight-badge">CHI & UIST Reviewer</span>
        <span class="highlight-badge">ML/AI Expert</span>
        <span class="highlight-badge">Competition Coach</span>
      </div>
    </div>
  </div>
</section>

<!-- Our Values -->
<section class="values-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Why Choose Us</span>
      <span class="zh-content">为什么选择我们</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">What Sets Us Apart</span>
      <span class="zh-content">我们的独特之处</span>
    </h2>
  </div>
  
  <div class="values-grid">
    <div class="value-card">
      <div class="value-icon">🎓</div>
      <h3 class="value-title">
        <span class="en-content">PhD-Level Expertise</span>
        <span class="zh-content">博士级专业知识</span>
      </h3>
      <p class="value-description">
        <span class="en-content">Our instructors are PhD holders from top computer science programs, bringing cutting-edge knowledge to every lesson.</span>
        <span class="zh-content">我们的导师是来自顶尖计算机科学项目的博士，为每堂课带来前沿知识。</span>
      </p>
    </div>
    
    <div class="value-card">
      <div class="value-icon">🏆</div>
      <h3 class="value-title">
        <span class="en-content">Competition Success</span>
        <span class="zh-content">竞赛成就</span>
      </h3>
      <p class="value-description">
        <span class="en-content">Proven track record in USACO, USAAIO, AMC, and other prestigious competitions with multiple students reaching Gold and Platinum levels.</span>
        <span class="zh-content">在USACO、USAAIO、AMC和其他知名竞赛中有着卓越的成绩，多名学生达到金牌和白金级别。</span>
      </p>
    </div>
    
    <div class="value-card">
      <div class="value-icon">🎯</div>
      <h3 class="value-title">
        <span class="en-content">Personalized Learning</span>
        <span class="zh-content">个性化学习</span>
      </h3>
      <p class="value-description">
        <span class="en-content">Customized curriculum tailored to each student's goals, whether it's competition prep, college applications, or skill development.</span>
        <span class="zh-content">根据每个学生的目标定制课程，无论是竞赛准备、大学申请还是技能发展。</span>
      </p>
    </div>
    
    <div class="value-card">
      <div class="value-icon">🌍</div>
      <h3 class="value-title">
        <span class="en-content">Global Reach</span>
        <span class="zh-content">全球服务</span>
      </h3>
      <p class="value-description">
        <span class="en-content">Supporting students from both the US and China with bilingual instruction and flexible scheduling across time zones.</span>
        <span class="zh-content">为美国和中国的学生提供双语教学和跨时区的灵活安排。</span>
      </p>
    </div>
    
    <div class="value-card">
      <div class="value-icon">💼</div>
      <h3 class="value-title">
        <span class="en-content">Industry Connection</span>
        <span class="zh-content">行业联系</span>
      </h3>
      <p class="value-description">
        <span class="en-content">Our instructors work at leading tech companies, bringing real-world experience and industry best practices to education.</span>
        <span class="zh-content">我们的导师在领先的科技公司工作，将实际经验和行业最佳实践带入教育。</span>
      </p>
    </div>
    
    <div class="value-card">
      <div class="value-icon">📈</div>
      <h3 class="value-title">
        <span class="en-content">Proven Results</span>
        <span class="zh-content">成果验证</span>
      </h3>
      <p class="value-description">
        <span class="en-content">95% success rate in competition advancement and AP exam scores, with many students receiving college recommendation letters.</span>
        <span class="zh-content">95%的竞赛晋级和AP考试成功率，许多学生获得大学推荐信。</span>
      </p>
    </div>
  </div>
</section>

<!-- Student Success Stats -->
<section class="stats-section">
  <div class="stats-orb stats-orb-1"></div>
  <div class="stats-orb stats-orb-2"></div>
  
  <div class="stats-content">
    <div class="section-header">
      <h2 class="section-title" style="color: white; -webkit-text-fill-color: white;">
        <span class="en-content">Student Success Stories</span>
        <span class="zh-content">学生成功故事</span>
      </h2>
    </div>
    
    <div class="stats-grid">
      <div class="stat-item">
        <div class="stat-number">50+</div>
        <div class="stat-label">
          <span class="en-content">Students Taught</span>
          <span class="zh-content">教授学生</span>
        </div>
      </div>
      
      <div class="stat-item">
        <div class="stat-number">20+</div>
        <div class="stat-label">
          <span class="en-content">Competition Winners</span>
          <span class="zh-content">竞赛获奖者</span>
        </div>
      </div>
      
      <div class="stat-item">
        <div class="stat-number">90%</div>
        <div class="stat-label">
          <span class="en-content">AP Score 5 Rate</span>
          <span class="zh-content">AP 5分率</span>
        </div>
      </div>
      
      <div class="stat-item">
        <div class="stat-number">100%</div>
        <div class="stat-label">
          <span class="en-content">College Acceptance</span>
          <span class="zh-content">大学录取率</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Educational Philosophy -->
<section class="philosophy-section">
  <h2 class="philosophy-title">
    <span class="en-content">📚 Our Educational Philosophy</span>
    <span class="zh-content">📚 我们的教育理念</span>
  </h2>
  
  <ul class="philosophy-list">
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Learning by Doing: </strong>
        <strong class="zh-content">实践学习：</strong>
        <span class="en-content">Hands-on coding from day one with real projects and practical applications</span>
        <span class="zh-content">从第一天起就通过真实项目和实际应用进行编程实践</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Conceptual Understanding: </strong>
        <strong class="zh-content">概念理解：</strong>
        <span class="en-content">Deep comprehension of algorithms and data structures, not just memorization</span>
        <span class="zh-content">深入理解算法和数据结构，而不仅仅是死记硬背</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Competitive Edge: </strong>
        <strong class="zh-content">竞争优势：</strong>
        <span class="en-content">Training students to excel in competitions and stand out in college applications</span>
        <span class="zh-content">培训学生在竞赛中脱颖而出，在大学申请中崭露头角</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Lifelong Skills: </strong>
        <strong class="zh-content">终身技能：</strong>
        <span class="en-content">Building problem-solving abilities that extend beyond programming</span>
        <span class="zh-content">培养超越编程的问题解决能力</span>
      </span>
    </li>
  </ul>
</section>

<!-- CTA Section -->
<section class="cta-section">
  <div class="cta-orb cta-orb-1"></div>
  <div class="cta-orb cta-orb-2"></div>
  
  <div class="cta-content">
    <div class="cta-icon">🚀</div>
    <h2 class="cta-title">
      <span class="en-content">Join the AIcoding Family</span>
      <span class="zh-content">加入 AIcoding 大家庭</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Experience the difference that expert instruction makes. Start your journey to coding excellence today.</span>
      <span class="zh-content">体验专家指导的不同之处。今天就开始您的编程卓越之旅。</span>
    </p>
    <a href="{{ site.baseurl }}/contact.html" class="cta-button">
      <span class="en-content">Get Started Today →</span>
      <span class="zh-content">立即开始 →</span>
    </a>
  </div>
</section>
