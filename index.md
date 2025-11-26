---
layout: default
title: AIcoding Academy
title_zh: AIcoding 学院
description: Elite Programming Education for Future Tech Leaders
description_zh: 为未来科技领袖提供的精英编程教育
---

<style>
  /* ========================================
     Premium Animations Library
  ======================================== */
  @keyframes gradientFlow {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-20px) rotate(-3deg); }
    75% { transform: translateY(20px) rotate(3deg); }
  }

  @keyframes floatReverse {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(20px) rotate(3deg); }
    75% { transform: translateY(-20px) rotate(-3deg); }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 0.8; }
    50% { transform: scale(1.08); opacity: 1; }
  }

  @keyframes slideInUp {
    from { opacity: 0; transform: translateY(60px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes slideInLeft {
    from { opacity: 0; transform: translateX(-40px); }
    to { opacity: 1; transform: translateX(0); }
  }

  @keyframes starTwinkle {
    0%, 100% { opacity: 0.2; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.5); }
  }

  @keyframes arrowFlow {
    0% { transform: translateX(-3px); opacity: 0.4; }
    50% { transform: translateX(8px); opacity: 1; }
    100% { transform: translateX(-3px); opacity: 0.4; }
  }

  @keyframes shimmer {
    0% { background-position: -200% 0; }
    100% { background-position: 200% 0; }
  }

  @keyframes borderGlow {
    0%, 100% { box-shadow: 0 0 5px currentColor, 0 0 10px currentColor; }
    50% { box-shadow: 0 0 20px currentColor, 0 0 30px currentColor; }
  }

  @keyframes morphBlob {
    0%, 100% { border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; }
    25% { border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%; }
    50% { border-radius: 50% 60% 30% 60% / 30% 60% 70% 40%; }
    75% { border-radius: 60% 40% 60% 30% / 70% 30% 50% 60%; }
  }

  @keyframes rotateGlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes particleFloat {
    0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.6; }
    25% { transform: translate(10px, -20px) scale(1.2); opacity: 1; }
    50% { transform: translate(-5px, -40px) scale(0.8); opacity: 0.8; }
    75% { transform: translate(-15px, -20px) scale(1.1); opacity: 0.9; }
  }

  @keyframes textReveal {
    from { clip-path: inset(0 100% 0 0); }
    to { clip-path: inset(0 0 0 0); }
  }

  @keyframes bounceIn {
    0% { transform: scale(0.3); opacity: 0; }
    50% { transform: scale(1.05); }
    70% { transform: scale(0.9); }
    100% { transform: scale(1); opacity: 1; }
  }

  @keyframes ripple {
    0% { transform: scale(0.8); opacity: 1; }
    100% { transform: scale(2.5); opacity: 0; }
  }

  @keyframes cardEntrance {
    from { opacity: 0; transform: translateY(30px) scale(0.95); }
    to { opacity: 1; transform: translateY(0) scale(1); }
  }

  /* ========================================
     Hero Section - Premium Design
  ======================================== */
  .hero-section {
    min-height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5rem 2rem;
    background: linear-gradient(135deg, 
      #0f0c29 0%, 
      #302b63 30%, 
      #24243e 60%,
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

  /* Aurora Background Effect */
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
    width: 500px;
    height: 500px;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.6), rgba(139, 92, 246, 0.4));
    top: -200px;
    left: -150px;
  }

  .hero-orb:nth-child(2) {
    width: 400px;
    height: 400px;
    background: linear-gradient(135deg, rgba(236, 72, 153, 0.5), rgba(239, 68, 68, 0.3));
    bottom: -150px;
    right: -100px;
    animation-delay: -5s;
  }

  .hero-orb:nth-child(3) {
    width: 300px;
    height: 300px;
    background: linear-gradient(135deg, rgba(6, 182, 212, 0.4), rgba(16, 185, 129, 0.3));
    bottom: 20%;
    left: 10%;
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

  .hero-star:nth-child(1) { left: 5%; top: 10%; animation-delay: 0s; }
  .hero-star:nth-child(2) { left: 12%; top: 35%; animation-delay: 0.7s; }
  .hero-star:nth-child(3) { left: 20%; top: 65%; animation-delay: 1.4s; }
  .hero-star:nth-child(4) { left: 35%; top: 15%; animation-delay: 2.1s; }
  .hero-star:nth-child(5) { left: 50%; top: 80%; animation-delay: 0.3s; }
  .hero-star:nth-child(6) { left: 65%; top: 25%; animation-delay: 1s; }
  .hero-star:nth-child(7) { left: 75%; top: 55%; animation-delay: 1.7s; }
  .hero-star:nth-child(8) { left: 85%; top: 75%; animation-delay: 2.4s; }
  .hero-star:nth-child(9) { left: 92%; top: 20%; animation-delay: 0.5s; }
  .hero-star:nth-child(10) { left: 45%; top: 45%; animation-delay: 1.2s; }

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
    animation: particleFloat 8s ease-in-out infinite;
  }

  .hero-particle:nth-child(1) { left: 10%; bottom: 20%; animation-delay: 0s; }
  .hero-particle:nth-child(2) { left: 30%; bottom: 30%; animation-delay: 2s; }
  .hero-particle:nth-child(3) { left: 50%; bottom: 15%; animation-delay: 4s; }
  .hero-particle:nth-child(4) { left: 70%; bottom: 25%; animation-delay: 1s; }
  .hero-particle:nth-child(5) { left: 90%; bottom: 35%; animation-delay: 3s; }

  /* Floating Emoji Icons */
  .floating-icons {
    position: absolute;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 1;
    pointer-events: none;
  }

  .floating-icon {
    position: absolute;
    font-size: 2.5rem;
    opacity: 0.15;
    filter: drop-shadow(0 0 20px rgba(255, 255, 255, 0.3));
  }

  .floating-icon:nth-child(1) { top: 12%; left: 8%; animation: float 10s infinite ease-in-out; }
  .floating-icon:nth-child(2) { top: 18%; right: 10%; animation: floatReverse 12s infinite ease-in-out 1s; }
  .floating-icon:nth-child(3) { bottom: 25%; left: 10%; animation: float 9s infinite ease-in-out 2s; }
  .floating-icon:nth-child(4) { bottom: 20%; right: 12%; animation: floatReverse 11s infinite ease-in-out 0.5s; }
  .floating-icon:nth-child(5) { top: 50%; left: 5%; animation: float 13s infinite ease-in-out 1.5s; }
  .floating-icon:nth-child(6) { top: 40%; right: 5%; animation: floatReverse 10s infinite ease-in-out 2.5s; }

  .hero-content {
    position: relative;
    z-index: 10;
    text-align: center;
    animation: slideInUp 1.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.6rem;
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    padding: 0.7rem 1.8rem;
    border-radius: 50px;
    margin-bottom: 2rem;
    border: 1px solid rgba(255, 255, 255, 0.2);
    animation: bounceIn 1s ease-out 0.3s backwards;
    box-shadow: 
      0 8px 32px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(255, 255, 255, 0.1);
  }

  .hero-badge-dot {
    width: 10px;
    height: 10px;
    background: #10B981;
    border-radius: 50%;
    animation: pulse 2s ease-in-out infinite;
    box-shadow: 0 0 20px #10B981, 0 0 40px #10B981;
  }

  .hero-badge-text {
    color: white;
    font-size: 0.95rem;
    font-weight: 600;
    letter-spacing: 0.5px;
  }

  .hero-title {
    font-size: 5rem;
    font-weight: 900;
    color: white;
    text-shadow: 0 4px 60px rgba(0, 0, 0, 0.5);
    margin-bottom: 1.5rem;
    letter-spacing: -3px;
    line-height: 1.1;
    background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 30%, #ffffff 50%, #ddd6fe 70%, #ffffff 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: gradientFlow 8s ease infinite;
  }

  .hero-subtitle {
    font-size: 1.6rem;
    color: rgba(255, 255, 255, 0.95);
    margin-bottom: 1rem;
    font-weight: 500;
    text-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
    letter-spacing: 0.5px;
  }

  .hero-description {
    font-size: 1.15rem;
    color: rgba(255, 255, 255, 0.8);
    margin-bottom: 3rem;
    max-width: 650px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.8;
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .hero-btn {
    padding: 1.2rem 2.8rem;
    border-radius: 60px;
    font-weight: 700;
    font-size: 1.1rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .hero-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s ease;
  }

  .hero-btn:hover::before {
    left: 100%;
  }

  .hero-btn-primary {
    background: linear-gradient(135deg, #ffffff, #f0f0f0);
    color: #4338ca;
    box-shadow: 
      0 10px 40px rgba(0, 0, 0, 0.3),
      0 0 0 1px rgba(255, 255, 255, 0.1);
  }

  .hero-btn-primary:hover {
    transform: translateY(-6px) scale(1.02);
    box-shadow: 
      0 20px 60px rgba(0, 0, 0, 0.4),
      0 0 60px rgba(99, 102, 241, 0.3);
    color: #4338ca;
  }

  .hero-btn-secondary {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(20px);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .hero-btn-secondary:hover {
    background: rgba(255, 255, 255, 0.2);
    transform: translateY(-6px);
    border-color: rgba(255, 255, 255, 0.5);
    color: white;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
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
    letter-spacing: 4px;
    margin-bottom: 1rem;
    padding: 0.6rem 1.8rem;
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
    border-radius: 50px;
    border: 1px solid rgba(99, 102, 241, 0.2);
  }

  .section-title {
    font-size: 3.2rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    letter-spacing: -1px;
  }

  .section-subtitle {
    color: #6B7280;
    font-size: 1.25rem;
    max-width: 700px;
    margin: 0 auto;
    line-height: 1.8;
  }

  /* ========================================
     Learning Paths Section - Premium
  ======================================== */
  .paths-section {
    margin: 6rem 0;
    padding: 4rem 0;
  }

  .path-container {
    margin-bottom: 3rem;
    background: white;
    border-radius: 28px;
    box-shadow: 
      0 20px 60px rgba(0, 0, 0, 0.08),
      0 1px 3px rgba(0, 0, 0, 0.05);
    overflow: hidden;
    border: 1px solid rgba(0, 0, 0, 0.05);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    animation: cardEntrance 0.8s ease-out backwards;
  }

  .path-container:nth-child(1) { animation-delay: 0.1s; }
  .path-container:nth-child(2) { animation-delay: 0.2s; }
  .path-container:nth-child(3) { animation-delay: 0.3s; }
  .path-container:nth-child(4) { animation-delay: 0.4s; }
  .path-container:nth-child(5) { animation-delay: 0.5s; }
  .path-container:nth-child(6) { animation-delay: 0.6s; }
  .path-container:nth-child(7) { animation-delay: 0.7s; }

  .path-container:hover {
    transform: translateY(-8px);
    box-shadow: 
      0 40px 80px rgba(0, 0, 0, 0.12),
      0 1px 3px rgba(0, 0, 0, 0.05);
  }

  .path-header {
    padding: 1.8rem 2.5rem;
    display: flex;
    align-items: center;
    gap: 1.2rem;
    color: white;
    position: relative;
    overflow: hidden;
  }

  .path-header::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
    background-size: 200% 100%;
    animation: shimmer 3s ease-in-out infinite;
  }

  .path-header-icon {
    font-size: 2.5rem;
    filter: drop-shadow(0 4px 10px rgba(0, 0, 0, 0.3));
    position: relative;
    z-index: 1;
  }

  .path-header-content {
    flex: 1;
    position: relative;
    z-index: 1;
  }

  .path-header-title {
    font-size: 1.5rem;
    font-weight: 800;
    margin-bottom: 0.3rem;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
    letter-spacing: -0.5px;
  }

  .path-header-subtitle {
    font-size: 0.95rem;
    opacity: 0.9;
  }

  .path-header-goal {
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 0.6rem 1.2rem;
    border-radius: 50px;
    font-size: 0.9rem;
    font-weight: 700;
    border: 1px solid rgba(255, 255, 255, 0.3);
    position: relative;
    z-index: 1;
    white-space: nowrap;
  }

  /* Path Colors - Premium Gradients */
  .path-ap { background: linear-gradient(135deg, #3B82F6 0%, #1D4ED8 50%, #1E40AF 100%); }
  .path-acsl { background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 50%, #6D28D9 100%); }
  .path-usaco { background: linear-gradient(135deg, #10B981 0%, #059669 50%, #047857 100%); }
  .path-ml { background: linear-gradient(135deg, #F59E0B 0%, #D97706 50%, #B45309 100%); }
  .path-math { background: linear-gradient(135deg, #EF4444 0%, #DC2626 50%, #B91C1C 100%); }
  .path-wq { background: linear-gradient(135deg, #06B6D4 0%, #0891B2 50%, #0E7490 100%); }
  .path-himcm { background: linear-gradient(135deg, #EC4899 0%, #DB2777 50%, #BE185D 100%); }

  /* Timeline - Premium Design */
  .path-timeline {
    padding: 2.5rem;
    display: flex;
    align-items: stretch;
    gap: 0;
    overflow-x: auto;
    position: relative;
    background: linear-gradient(180deg, #FAFAFA 0%, #FFFFFF 100%);
  }

  .path-timeline::-webkit-scrollbar {
    height: 6px;
  }

  .path-timeline::-webkit-scrollbar-track {
    background: #F3F4F6;
    border-radius: 3px;
  }

  .path-timeline::-webkit-scrollbar-thumb {
    background: linear-gradient(90deg, #6366f1, #8b5cf6);
    border-radius: 3px;
  }

  .timeline-step {
    flex: 1;
    min-width: 170px;
    display: flex;
    flex-direction: column;
    position: relative;
  }

  .timeline-connector {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 0.3rem;
    min-width: 40px;
  }

  .timeline-arrow {
    font-size: 1.8rem;
    font-weight: 300;
    background: linear-gradient(90deg, #9CA3AF, #6B7280);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: arrowFlow 2s ease-in-out infinite;
  }

  .step-card {
    background: white;
    border-radius: 18px;
    padding: 1.5rem;
    height: 100%;
    border: 2px solid #E5E7EB;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.04);
  }

  .step-card:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
  }

  .step-number {
    position: absolute;
    top: -14px;
    left: 1.2rem;
    width: 32px;
    height: 32px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.85rem;
    font-weight: 800;
    color: white;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
  }

  .step-ap .step-number { background: linear-gradient(135deg, #3B82F6, #1D4ED8); }
  .step-acsl .step-number { background: linear-gradient(135deg, #8B5CF6, #6D28D9); }
  .step-usaco .step-number { background: linear-gradient(135deg, #10B981, #059669); }
  .step-ml .step-number { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .step-math .step-number { background: linear-gradient(135deg, #EF4444, #DC2626); }
  .step-wq .step-number { background: linear-gradient(135deg, #06B6D4, #0891B2); }
  .step-himcm .step-number { background: linear-gradient(135deg, #EC4899, #DB2777); }

  .step-duration {
    display: inline-block;
    padding: 0.35rem 0.9rem;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
    background: linear-gradient(135deg, #F3F4F6, #E5E7EB);
    color: #4B5563;
    letter-spacing: 0.3px;
  }

  .step-title {
    font-size: 1.05rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
    line-height: 1.3;
  }

  .step-description {
    font-size: 0.85rem;
    color: #6B7280;
    line-height: 1.6;
  }

  /* Final Goal Step - Premium Gold Design */
  .step-goal {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 50%, #FCD34D 100%);
    border-color: #F59E0B;
    box-shadow: 
      0 4px 20px rgba(245, 158, 11, 0.3),
      inset 0 1px 0 rgba(255, 255, 255, 0.5);
  }

  .step-goal:hover {
    box-shadow: 
      0 15px 40px rgba(245, 158, 11, 0.4),
      inset 0 1px 0 rgba(255, 255, 255, 0.5);
  }

  .step-goal .step-number {
    background: linear-gradient(135deg, #F59E0B, #D97706);
    box-shadow: 0 4px 20px rgba(245, 158, 11, 0.5);
  }

  .step-goal .step-title {
    color: #92400E;
  }

  .step-goal .step-description {
    color: #A16207;
    font-weight: 600;
  }

  .step-goal .step-duration {
    background: linear-gradient(135deg, #FDE68A, #FCD34D);
    color: #92400E;
  }

  /* ========================================
     Why Choose Us Section - Premium
  ======================================== */
  .why-section {
    margin: 6rem 0;
    padding: 5rem 3rem;
    background: linear-gradient(180deg, #F9FAFB 0%, #F3F4F6 50%, #F9FAFB 100%);
    border-radius: 40px;
    position: relative;
    overflow: hidden;
  }

  .why-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(ellipse at 0% 0%, rgba(99, 102, 241, 0.08) 0%, transparent 50%),
      radial-gradient(ellipse at 100% 100%, rgba(16, 185, 129, 0.06) 0%, transparent 50%);
    pointer-events: none;
  }

  .why-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 3rem;
    position: relative;
    z-index: 1;
  }

  .why-card {
    background: white;
    border-radius: 24px;
    padding: 2.5rem 2rem;
    text-align: center;
    box-shadow: 
      0 10px 40px rgba(0, 0, 0, 0.04),
      0 1px 3px rgba(0, 0, 0, 0.02);
    border: 1px solid rgba(0, 0, 0, 0.04);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .why-card::before {
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

  .why-card:hover::before {
    transform: scaleX(1);
  }

  .why-card:hover {
    transform: translateY(-10px);
    box-shadow: 
      0 30px 60px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.02);
  }

  .why-icon {
    font-size: 3rem;
    margin-bottom: 1.2rem;
    display: block;
  }

  .why-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.6rem;
  }

  .why-description {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.7;
  }

  /* ========================================
     Stats Section - Premium Dark
  ======================================== */
  .stats-section {
    background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%);
    border-radius: 40px;
    padding: 5rem 3rem;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 
      0 50px 100px rgba(0, 0, 0, 0.3),
      inset 0 0 100px rgba(99, 102, 241, 0.1);
  }

  .stats-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(ellipse at 20% 50%, rgba(99, 102, 241, 0.2) 0%, transparent 50%),
      radial-gradient(ellipse at 80% 50%, rgba(139, 92, 246, 0.15) 0%, transparent 50%);
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
    padding: 2rem;
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(10px);
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.1);
    transition: all 0.4s ease;
  }

  .stat-item:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-5px);
  }

  .stat-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    filter: drop-shadow(0 5px 20px rgba(0, 0, 0, 0.3));
  }

  .stat-number {
    font-size: 4rem;
    font-weight: 900;
    color: white;
    text-shadow: 0 4px 30px rgba(0, 0, 0, 0.3);
    margin-bottom: 0.5rem;
    line-height: 1;
    background: linear-gradient(135deg, #ffffff, #c7d2fe);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .stat-label {
    color: rgba(255, 255, 255, 0.8);
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-weight: 600;
  }

  /* ========================================
     CTA Section - Premium
  ======================================== */
  .cta-section {
    background: white;
    border-radius: 40px;
    padding: 6rem 4rem;
    margin: 6rem 0;
    text-align: center;
    box-shadow: 
      0 30px 80px rgba(0, 0, 0, 0.08),
      0 1px 3px rgba(0, 0, 0, 0.02);
    border: 1px solid rgba(0, 0, 0, 0.04);
    position: relative;
    overflow: hidden;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 6px;
    background: linear-gradient(90deg, #6366f1, #8b5cf6, #ec4899, #f59e0b, #10b981);
    background-size: 200% 100%;
    animation: gradientFlow 5s linear infinite;
  }

  .cta-icon {
    font-size: 5rem;
    margin-bottom: 2rem;
    animation: float 5s ease-in-out infinite;
    filter: drop-shadow(0 10px 30px rgba(0, 0, 0, 0.2));
  }

  .cta-title {
    font-size: 3.2rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1.2rem;
    letter-spacing: -1px;
  }

  .cta-description {
    font-size: 1.3rem;
    color: #6B7280;
    margin-bottom: 3rem;
    max-width: 650px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.8;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-btn {
    padding: 1.2rem 3rem;
    border-radius: 60px;
    font-weight: 700;
    font-size: 1.1rem;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }

  .cta-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s ease;
  }

  .cta-btn:hover::before {
    left: 100%;
  }

  .cta-btn-primary {
    background: linear-gradient(135deg, #6366f1, #8b5cf6);
    color: white;
    box-shadow: 
      0 10px 40px rgba(99, 102, 241, 0.4),
      0 0 0 1px rgba(99, 102, 241, 0.1);
  }

  .cta-btn-primary:hover {
    transform: translateY(-6px) scale(1.02);
    box-shadow: 
      0 20px 60px rgba(99, 102, 241, 0.5),
      0 0 60px rgba(99, 102, 241, 0.2);
    color: white;
  }

  .cta-btn-secondary {
    background: #F3F4F6;
    color: #4B5563;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
  }

  .cta-btn-secondary:hover {
    background: #E5E7EB;
    transform: translateY(-6px);
    color: #1F2937;
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
  }

  /* ========================================
     Responsive Design - Premium
  ======================================== */
  @media (max-width: 1200px) {
    .path-timeline {
      flex-wrap: nowrap;
      overflow-x: auto;
      padding-bottom: 1.5rem;
    }
    
    .timeline-step {
      min-width: 160px;
    }

    .why-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 900px) {
    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 1.5rem;
    }

    .path-header {
      flex-wrap: wrap;
    }

    .path-header-goal {
      width: 100%;
      text-align: center;
      margin-top: 0.8rem;
    }

    .hero-title {
      font-size: 3.5rem;
    }
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 2.8rem;
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

    .cta-title {
      font-size: 2rem;
    }

    .path-timeline {
      flex-direction: column;
      gap: 1rem;
    }

    .timeline-connector {
      transform: rotate(90deg);
      padding: 0.5rem 0;
      min-width: auto;
    }

    .timeline-step {
      min-width: 100%;
    }

    .floating-icons {
      display: none;
    }

    .hero-section {
      border-radius: 24px;
    }
  }

  @media (max-width: 480px) {
    .hero-buttons,
    .cta-buttons {
      flex-direction: column;
      align-items: center;
    }

    .hero-btn,
    .cta-btn {
      width: 100%;
      max-width: 300px;
      justify-content: center;
      text-align: center;
    }

    .stats-grid {
      grid-template-columns: 1fr;
    }

    .stat-item {
      padding: 1.5rem;
    }

    .stat-number {
      font-size: 3rem;
    }

    .hero-title {
      font-size: 2.2rem;
    }

    .cta-section {
      padding: 3rem 1.5rem;
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
  
  <div class="floating-icons">
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🚀</span>
    <span class="floating-icon">🎯</span>
    <span class="floating-icon">🏆</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">⚡</span>
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
      <span class="en-content">AIcoding Academy</span>
      <span class="zh-content">AIcoding 学院</span>
    </h1>
    
    <p class="hero-subtitle">
      <span class="en-content">Empowering Future Tech Leaders</span>
      <span class="zh-content">培养未来科技领袖</span>
    </p>
    
    <p class="hero-description">
      <span class="en-content">7 specialized learning tracks designed for programming mastery, competition excellence, and academic achievement. Your journey to success starts here.</span>
      <span class="zh-content">7条专业学习路线，专为编程精通、竞赛卓越和学术成就而设计。您的成功之旅从这里开始。</span>
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

<!-- Learning Paths Section -->
<section class="paths-section">
  <div class="section-header">
    <span class="section-eyebrow">
      <span class="en-content">Learning Paths</span>
      <span class="zh-content">学习路径</span>
    </span>
    <h2 class="section-title">
      <span class="en-content">7 Tracks to Excellence</span>
      <span class="zh-content">7条卓越之路</span>
    </h2>
    <p class="section-subtitle">
      <span class="en-content">Each track has a clear progression from fundamentals to mastery. Find the path that matches your goals.</span>
      <span class="zh-content">每条路线都有清晰的从基础到精通的进阶路径。找到符合您目标的路线。</span>
    </p>
  </div>

  <!-- Track 1: AP Computer Science -->
  <div class="path-container">
    <div class="path-header path-ap">
      <span class="path-header-icon">📘</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">AP Computer Science Track</span>
          <span class="zh-content">AP计算机科学路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">Master AP CSA & AP CSP for college credit</span>
          <span class="zh-content">掌握AP CSA和AP CSP获得大学学分</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Score 5 on AP Exams</span>
        <span class="zh-content">🎯 目标：AP考试满分5分</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Java Fundamentals</span>
            <span class="zh-content">Java基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Variables, loops, arrays, OOP basics, methods</span>
            <span class="zh-content">变量、循环、数组、面向对象基础、方法</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AP CSP Prep</span>
            <span class="zh-content">AP CSP备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Computing concepts, data, algorithms, internet</span>
            <span class="zh-content">计算概念、数据、算法、互联网</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AP CSA Prep</span>
            <span class="zh-content">AP CSA备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced OOP, inheritance, recursion, ArrayLists</span>
            <span class="zh-content">高级OOP、继承、递归、ArrayList</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ap">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2 months</span>
            <span class="zh-content">2个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Exam Practice</span>
            <span class="zh-content">模拟冲刺</span>
          </h4>
          <p class="step-description">
            <span class="en-content">FRQ training, mock exams → Score 5!</span>
            <span class="zh-content">FRQ训练、模拟考试 → 满分5分！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 2: ACSL -->
  <div class="path-container">
    <div class="path-header path-acsl">
      <span class="path-header-icon">💻</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">ACSL Competition Track</span>
          <span class="zh-content">ACSL竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">American Computer Science League</span>
          <span class="zh-content">美国计算机科学联赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: ACSL Finals</span>
        <span class="zh-content">🎯 目标：ACSL决赛</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Programming Basics</span>
            <span class="zh-content">编程基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python/Java basics, problem-solving fundamentals</span>
            <span class="zh-content">Python/Java基础，问题解决入门</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Junior</span>
            <span class="zh-content">ACSL初级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Number systems, Boolean algebra, graph theory</span>
            <span class="zh-content">数制、布尔代数、图论基础</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Intermediate</span>
            <span class="zh-content">ACSL中级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Bit manipulation, regex, prefix/postfix</span>
            <span class="zh-content">位运算、正则表达式、前缀/后缀</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-acsl">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ACSL Senior</span>
            <span class="zh-content">ACSL高级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced topics → Qualify for Finals!</span>
            <span class="zh-content">高级主题 → 进入决赛！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 3: USACO - UPDATED -->
  <div class="path-container">
    <div class="path-header path-usaco">
      <span class="path-header-icon">🐄</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">USACO Competition Track</span>
          <span class="zh-content">USACO竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">USA Computing Olympiad</span>
          <span class="zh-content">美国计算机奥林匹克</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Platinum Division</span>
        <span class="zh-content">🎯 目标：白金级</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Python → Bronze</span>
            <span class="zh-content">Python → 铜级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python basics, simulation, ad hoc problems</span>
            <span class="zh-content">Python基础、模拟、专项问题</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">4-5 months</span>
            <span class="zh-content">4-5个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Java → Silver</span>
            <span class="zh-content">Java → 银级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Java OOP, sorting, binary search, greedy</span>
            <span class="zh-content">Java面向对象、排序、二分、贪心</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">6-8 months</span>
            <span class="zh-content">6-8个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Gold Level</span>
            <span class="zh-content">金级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">DFS/BFS, DP basics, DSU, trees, graphs</span>
            <span class="zh-content">DFS/BFS、DP基础、并查集、树、图</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-usaco">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">8-12 months</span>
            <span class="zh-content">8-12个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">C++ → Platinum</span>
            <span class="zh-content">C++ → 白金级</span>
          </h4>
          <p class="step-description">
            <span class="en-content">C++ STL, advanced DP, segment trees → Platinum!</span>
            <span class="zh-content">C++ STL、高级DP、线段树 → 白金级！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 4: Machine Learning / AI - UPDATED -->
  <div class="path-container">
    <div class="path-header path-ml">
      <span class="path-header-icon">🤖</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">AI/ML Competition Track</span>
          <span class="zh-content">AI/ML竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">USAAIO & Kaggle Competitions</span>
          <span class="zh-content">USAAIO和Kaggle竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: USAAIO Award / Kaggle Medal</span>
        <span class="zh-content">🎯 目标：USAAIO获奖 / Kaggle奖牌</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Python for Data</span>
            <span class="zh-content">Python数据基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python, NumPy, Pandas, data visualization</span>
            <span class="zh-content">Python、NumPy、Pandas、数据可视化</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">5-6 months</span>
            <span class="zh-content">5-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">ML & Deep Learning</span>
            <span class="zh-content">机器学习与深度学习</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Sklearn, PyTorch, CNN, RNN, transformers</span>
            <span class="zh-content">Sklearn、PyTorch、CNN、RNN、Transformer</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">USAAIO Prep</span>
            <span class="zh-content">USAAIO备赛</span>
          </h4>
          <p class="step-description">
            <span class="en-content">AI concepts, problem solving, competition prep</span>
            <span class="zh-content">AI概念、问题求解、竞赛准备</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-ml">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Kaggle Projects</span>
            <span class="zh-content">Kaggle实战</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Real competitions → USAAIO Award / Kaggle Medal!</span>
            <span class="zh-content">真实竞赛 → USAAIO获奖 / Kaggle奖牌！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 5: Math Competition -->
  <div class="path-container">
    <div class="path-header path-math">
      <span class="path-header-icon">🔢</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">Math Competition Track</span>
          <span class="zh-content">数学竞赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">AMC → AIME → USAMO</span>
          <span class="zh-content">AMC → AIME → USAMO</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: AIME / USAMO Qualification</span>
        <span class="zh-content">🎯 目标：AIME资格 / USAMO</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AMC 8 Prep</span>
            <span class="zh-content">AMC 8备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Number sense, basic geometry, counting</span>
            <span class="zh-content">数感、基础几何、计数</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">4-6 months</span>
            <span class="zh-content">4-6个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AMC 10/12</span>
            <span class="zh-content">AMC 10/12</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Algebra, geometry, probability, number theory</span>
            <span class="zh-content">代数、几何、概率、数论</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">6-8 months</span>
            <span class="zh-content">6-8个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">AIME Prep</span>
            <span class="zh-content">AIME备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Advanced techniques, proof strategies</span>
            <span class="zh-content">高级技巧、证明策略</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-math">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">6-12 months</span>
            <span class="zh-content">6-12个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">USAMO Prep</span>
            <span class="zh-content">USAMO备考</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Olympiad problems → USAMO Qualifier!</span>
            <span class="zh-content">奥赛问题 → USAMO资格！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 6: WorldQuant -->
  <div class="path-container">
    <div class="path-header path-wq">
      <span class="path-header-icon">📈</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">WorldQuant Challenge Track</span>
          <span class="zh-content">WorldQuant挑战赛路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">Quantitative Finance Competition</span>
          <span class="zh-content">量化金融竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Gold Badge / Top 100</span>
        <span class="zh-content">🎯 目标：金牌徽章 / 前100名</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Python & Stats</span>
            <span class="zh-content">Python与统计</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Python, statistics, probability fundamentals</span>
            <span class="zh-content">Python、统计学、概率基础</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Finance Basics</span>
            <span class="zh-content">金融基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Markets, trading, financial data analysis</span>
            <span class="zh-content">市场、交易、金融数据分析</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Alpha Research</span>
            <span class="zh-content">Alpha研究</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Factor modeling, alpha generation, backtesting</span>
            <span class="zh-content">因子建模、Alpha生成、回测</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-wq">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Competition</span>
            <span class="zh-content">竞赛实战</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Submit alphas → Gold Badge!</span>
            <span class="zh-content">提交Alpha → 金牌徽章！</span>
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Track 7: HiMCM -->
  <div class="path-container">
    <div class="path-header path-himcm">
      <span class="path-header-icon">📋</span>
      <div class="path-header-content">
        <h3 class="path-header-title">
          <span class="en-content">HiMCM Modeling Track</span>
          <span class="zh-content">HiMCM数学建模路线</span>
        </h3>
        <p class="path-header-subtitle">
          <span class="en-content">High School Mathematical Contest in Modeling</span>
          <span class="zh-content">高中数学建模竞赛</span>
        </p>
      </div>
      <span class="path-header-goal">
        <span class="en-content">🎯 Goal: Outstanding Award</span>
        <span class="zh-content">🎯 目标：杰出奖</span>
      </span>
    </div>
    <div class="path-timeline">
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">1</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Math & Python</span>
            <span class="zh-content">数学与Python</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Calculus, statistics, Python for data analysis</span>
            <span class="zh-content">微积分、统计、Python数据分析</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">2</span>
          <span class="step-duration">
            <span class="en-content">3-4 months</span>
            <span class="zh-content">3-4个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Modeling Basics</span>
            <span class="zh-content">建模基础</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Optimization, simulation, differential equations</span>
            <span class="zh-content">优化、模拟、微分方程</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card">
          <span class="step-number">3</span>
          <span class="step-duration">
            <span class="en-content">2-3 months</span>
            <span class="zh-content">2-3个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Paper Writing</span>
            <span class="zh-content">论文写作</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Technical writing, LaTeX, report structure</span>
            <span class="zh-content">技术写作、LaTeX、报告结构</span>
          </p>
        </div>
      </div>
      <div class="timeline-connector">
        <span class="timeline-arrow">→</span>
      </div>
      <div class="timeline-step step-himcm">
        <div class="step-card step-goal">
          <span class="step-number">🏆</span>
          <span class="step-duration">
            <span class="en-content">2 months</span>
            <span class="zh-content">2个月</span>
          </span>
          <h4 class="step-title">
            <span class="en-content">Competition</span>
            <span class="zh-content">竞赛实战</span>
          </h4>
          <p class="step-description">
            <span class="en-content">Practice problems → Outstanding Award!</span>
            <span class="zh-content">练习问题 → 杰出奖！</span>
          </p>
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
        <span class="en-content">Clear Roadmap</span>
        <span class="zh-content">清晰路线</span>
      </h4>
      <p class="why-description">
        <span class="en-content">Structured progression with milestone tracking</span>
        <span class="zh-content">结构化进阶，里程碑跟踪</span>
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
      <div class="stat-icon">🛤️</div>
      <div class="stat-number">7</div>
      <div class="stat-label">
        <span class="en-content">Learning Tracks</span>
        <span class="zh-content">学习路线</span>
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
    <span class="en-content">Choose your track and begin your path to excellence. Schedule a free consultation to find the perfect fit.</span>
    <span class="zh-content">选择您的路线，开始卓越之旅。预约免费咨询，找到最适合您的路径。</span>
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
