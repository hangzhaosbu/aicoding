---
layout: default
title: About AIcoding
title_zh: 关于 AIcoding
description: Elite Programming Education by PhD Computer Scientists
description_zh: 由计算机科学博士提供的精英编程教育
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

  /* About Hero - Ultra Premium */
  .about-hero {
    min-height: 60vh;
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

  .about-hero::before {
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

  .about-hero::after {
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

  /* Diagonal corner shimmer effect */
  .about-hero .diagonal-shimmer-1,
  .about-hero .diagonal-shimmer-2 {
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

  .about-hero .diagonal-shimmer-1 {
    top: -10px;
    left: -150%;
    transform: rotate(45deg);
    animation: diagonalSweep1 8s ease-in-out infinite;
  }

  .about-hero .diagonal-shimmer-2 {
    bottom: -10px;
    right: -150%;
    transform: rotate(-45deg);
    animation: diagonalSweep2 8s ease-in-out infinite;
    animation-delay: 4s;
  }

  .about-hero h1 {
    font-size: 4rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
    animation: float 6s ease-in-out infinite;
  }

  .about-hero p {
    font-size: 1.4rem;
    color: rgba(255, 255, 255, 0.95);
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: relative;
    z-index: 1;
  }

  /* Mission Section - Premium Design */
  .mission-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    animation: slideIn 0.8s ease-out;
  }

  .mission-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    animation: shimmer 3s infinite;
  }

  .section-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 2rem;
    text-align: center;
    position: relative;
    display: inline-block;
    width: 100%;
  }

  .section-title::after {
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

  .mission-text {
    font-size: 1.2rem;
    line-height: 1.8;
    color: #4B5563;
    text-align: center;
    max-width: 900px;
    margin: 0 auto;
  }

  /* Values Section - Premium Cards */
  .values-section {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 5rem 3rem;
    border-radius: 30px;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
  }

  .values-section::before {
    content: '';
    position: absolute;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 30% 70%, rgba(102, 126, 234, 0.05), transparent 50%),
                radial-gradient(circle at 70% 30%, rgba(236, 72, 153, 0.05), transparent 50%);
    animation: pulse 15s ease-in-out infinite;
  }

  .values-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2.5rem;
    position: relative;
    z-index: 1;
    margin-top: 3rem;
  }

  .value-card {
    background: white;
    padding: 3rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideIn 0.6s ease-out;
  }

  .value-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.1), transparent);
    animation: shimmer 3s infinite;
  }

  .value-card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.3);
  }

  .value-icon {
    font-size: 3.5rem;
    margin-bottom: 1.5rem;
    text-align: center;
    animation: pulse 3s ease-in-out infinite;
  }

  .value-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #1F2937;
    text-align: center;
    margin-bottom: 1rem;
  }

  .value-description {
    color: #6B7280;
    text-align: center;
    line-height: 1.6;
  }

  /* Instructor Section - Premium Design */
  .instructor-section {
    background: white;
    padding: 5rem 3rem;
    border-radius: 30px;
    margin: 5rem 0;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
  }

  .instructor-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    transform: scaleX(0);
    animation: expand 2s ease-out forwards;
  }

  @keyframes expand {
    to { transform: scaleX(1); }
  }

  .instructor-content {
    display: grid;
    grid-template-columns: 320px 1fr;
    gap: 4rem;
    align-items: center;
    margin-top: 3rem;
    justify-items: center;
  }

  @media (max-width: 900px) {
    .instructor-content {
      grid-template-columns: 1fr;
      text-align: center;
    }
  }

  .instructor-image-container {
    position: relative;
    animation: float 6s ease-in-out infinite;
    width: 100%;
    display: flex;
    justify-content: center;
  }

  .instructor-image-wrapper {
    position: relative;
    width: 280px;
    height: 280px;
  }

  .instructor-image-frame {
    width: 100%;
    height: 100%;
    position: relative;
    padding: 15px;
    background: linear-gradient(135deg, rgba(245,242,235,0.9), white);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    box-shadow: 
      0 10px 40px rgba(0, 0, 0, 0.1),
      inset 0 0 40px rgba(0, 0, 0, 0.05);
    transform: rotate(-2deg);
    transition: transform 0.5s ease;
    animation: morphShape 15s ease-in-out infinite, imageFloat 6s ease-in-out infinite;
  }

  @keyframes morphShape {
    0%, 100% {
      border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    }
    20% {
      border-radius: 50% 50% 50% 50% / 60% 40% 60% 40%;
    }
    40% {
      border-radius: 70% 30% 50% 50% / 50% 60% 40% 60%;
    }
    60% {
      border-radius: 40% 60% 30% 70% / 70% 50% 50% 30%;
    }
    80% {
      border-radius: 60% 40% 60% 40% / 40% 70% 30% 60%;
    }
  }

  @keyframes imageFloat {
    0%, 100% { 
      transform: rotate(-2deg) translateY(0px);
    }
    50% { 
      transform: rotate(-2deg) translateY(-10px);
    }
  }

  .instructor-image-frame::before {
    content: '';
    position: absolute;
    top: -5px;
    left: -5px;
    right: -5px;
    bottom: -5px;
    background: linear-gradient(45deg, 
      #667eea 0%,
      #764ba2 25%,
      #f093fb 50%,
      #f5576c 75%,
      #667eea 100%);
    background-size: 400% 400%;
    border-radius: inherit;
    z-index: -1;
    opacity: 0.7;
    animation: borderGradient 8s ease infinite, morphShapeBorder 15s ease-in-out infinite;
  }

  @keyframes morphShapeBorder {
    0%, 100% {
      border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    }
    20% {
      border-radius: 50% 50% 50% 50% / 60% 40% 60% 40%;
    }
    40% {
      border-radius: 70% 30% 50% 50% / 50% 60% 40% 60%;
    }
    60% {
      border-radius: 40% 60% 30% 70% / 70% 50% 50% 30%;
    }
    80% {
      border-radius: 60% 40% 60% 40% / 40% 70% 30% 60%;
    }
  }

  @keyframes borderGradient {
    0% {
      background-position: 0% 50%;
    }
    50% {
      background-position: 100% 50%;
    }
    100% {
      background-position: 0% 50%;
    }
  }

  /* Wind Effect Layers */
  .wind-effect {
    position: absolute;
    top: -10px;
    left: -10px;
    right: -10px;
    bottom: -10px;
    border: 2px solid rgba(102, 126, 234, 0.3);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    opacity: 0.3;
    animation: windMorph 12s ease-in-out infinite;
    z-index: -2;
  }

  @keyframes windMorph {
    0%, 100% {
      border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
      transform: scale(1) rotate(0deg);
    }
    25% {
      border-radius: 60% 40% 50% 50% / 40% 60% 40% 60%;
      transform: scale(1.02) rotate(5deg);
    }
    50% {
      border-radius: 50% 50% 30% 70% / 60% 40% 60% 40%;
      transform: scale(1) rotate(-5deg);
    }
    75% {
      border-radius: 40% 60% 60% 40% / 50% 50% 50% 50%;
      transform: scale(1.02) rotate(3deg);
    }
  }

  .wind-effect-2 {
    position: absolute;
    top: -15px;
    left: -15px;
    right: -15px;
    bottom: -15px;
    border: 1px solid rgba(240, 147, 251, 0.2);
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
    opacity: 0.2;
    animation: windMorph2 10s ease-in-out infinite;
    animation-delay: -2s;
    z-index: -3;
  }

  @keyframes windMorph2 {
    0%, 100% {
      border-radius: 40% 60% 60% 40% / 50% 50% 50% 50%;
      transform: scale(1) rotate(0deg);
    }
    33% {
      border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
      transform: scale(1.03) rotate(-8deg);
    }
    66% {
      border-radius: 70% 30% 30% 70% / 40% 60% 40% 60%;
      transform: scale(1) rotate(6deg);
    }
  }

  .instructor-image-frame:hover {
    animation-play-state: paused;
    transform: rotate(0deg) scale(1.05);
  }

  .instructor-image-frame:hover::before {
    animation-duration: 3s;
    opacity: 0.9;
  }

  .instructor-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: sepia(5%) contrast(1.05);
    border: 3px solid white;
    border-radius: inherit;
    position: relative;
    z-index: 1;
  }

  /* Decorative Corner Elements */
  .image-corner {
    position: absolute;
    width: 25px;
    height: 25px;
    border: 2px solid rgba(245, 87, 108, 0.6);
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
  }

  .image-corner.bottom-left {
    bottom: 10px;
    left: 10px;
    border-right: none;
    border-top: none;
    border-radius: 0 0 0 30%;
  }

  .image-corner.bottom-right {
    bottom: 10px;
    right: 10px;
    border-left: none;
    border-top: none;
    border-radius: 0 0 30% 0;
  }

  @keyframes cornerGlow {
    0%, 100% {
      opacity: 0.7;
      transform: scale(1);
    }
    50% {
      opacity: 1;
      transform: scale(1.1);
    }
  }

  .image-seal {
    position: absolute;
    bottom: 25px;
    right: 25px;
    width: 50px;
    height: 50px;
    background: linear-gradient(135deg, #f093fb, #f5576c);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-family: 'Noto Serif SC', serif;
    font-weight: 700;
    font-size: 1.1rem;
    box-shadow: 0 3px 15px rgba(245, 87, 108, 0.4);
    transform: rotate(15deg);
    animation: sealRotate 10s ease-in-out infinite;
    z-index: 3;
  }

  @keyframes sealRotate {
    0%, 100% {
      transform: rotate(15deg) scale(1);
    }
    25% {
      transform: rotate(10deg) scale(1.05);
    }
    50% {
      transform: rotate(20deg) scale(1);
    }
    75% {
      transform: rotate(12deg) scale(1.05);
    }
  }

  .instructor-info {
    padding: 0 2rem;
  }

  .instructor-name {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 1rem;
  }

  .instructor-title {
    font-size: 1.3rem;
    color: #6B7280;
    margin-bottom: 2rem;
    font-weight: 600;
  }

  .instructor-bio {
    color: #4B5563;
    line-height: 1.8;
    font-size: 1.1rem;
    margin-bottom: 2rem;
  }

  .instructor-highlights {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-top: 2rem;
  }

  .highlight-badge {
    background: linear-gradient(135deg, #EEF2FF 0%, #DDD6FE 100%);
    color: #4F46E5;
    padding: 0.5rem 1.2rem;
    border-radius: 25px;
    font-size: 0.9rem;
    font-weight: 600;
    box-shadow: 0 2px 10px rgba(79, 70, 229, 0.1);
    transition: all 0.3s;
  }

  .highlight-badge:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(79, 70, 229, 0.2);
  }

  /* Success Stats - Premium */
  .stats-section {
    background: linear-gradient(135deg, #1F2937 0%, #111827 100%);
    border-radius: 30px;
    padding: 5rem 3rem;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
  }

  .stats-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.05), transparent);
    animation: shimmer 8s infinite;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 3rem;
    position: relative;
    z-index: 1;
    margin-top: 3rem;
  }

  .stat-item {
    text-align: center;
    animation: slideIn 1s ease-out;
  }

  .stat-number {
    font-size: 4rem;
    font-weight: 800;
    background: linear-gradient(135deg, #667eea 0%, #EC4899 50%, #F59E0B 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0.5rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #9CA3AF;
    font-size: 1.2rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 500;
  }

  /* Philosophy Section - Premium */
  .philosophy-section {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 5rem 0;
    border-left: 5px solid #F59E0B;
    position: relative;
    overflow: hidden;
  }

  .philosophy-section::after {
    content: '';
    position: absolute;
    top: 50%;
    right: 10%;
    width: 300px;
    height: 300px;
    background: radial-gradient(circle, rgba(245, 158, 11, 0.1) 0%, transparent 70%);
    animation: pulse 4s ease-in-out infinite;
  }

  .philosophy-list {
    list-style: none;
    padding: 0;
    position: relative;
    z-index: 1;
  }

  .philosophy-item {
    padding: 1.5rem 0;
    color: #78350F;
    display: flex;
    align-items: flex-start;
    transition: transform 0.3s;
  }

  .philosophy-item:hover {
    transform: translateX(10px);
  }

  .philosophy-check {
    color: #F59E0B;
    font-weight: bold;
    margin-right: 1.5rem;
    font-size: 1.5rem;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    border-radius: 30px;
    padding: 5rem 3rem;
    text-align: center;
    color: white;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotate 15s linear infinite;
  }

  .cta-section::after {
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

  /* Diagonal shimmer for CTA */
  .cta-section .diagonal-shimmer-1,
  .cta-section .diagonal-shimmer-2 {
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

  .cta-section .diagonal-shimmer-1 {
    top: -10px;
    left: -150%;
    transform: rotate(45deg);
    animation: diagonalSweep1 8s ease-in-out infinite;
  }

  .cta-section .diagonal-shimmer-2 {
    bottom: -10px;
    right: -150%;
    transform: rotate(-45deg);
    animation: diagonalSweep2 8s ease-in-out infinite;
    animation-delay: 4s;
  }

  .cta-content {
    position: relative;
    z-index: 1;
  }

  .cta-title {
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    color: white !important;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  }

  .cta-description {
    font-size: 1.3rem;
    margin-bottom: 2rem;
    opacity: 0.95;
    color: white !important;
  }

  .cta-button {
    background: white;
    color: #667eea;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1.1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
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
    background: linear-gradient(90deg, transparent, rgba(102, 126, 234, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    color: #667eea;
  }

  /* Responsive */
  @media (max-width: 768px) {
    .about-hero h1 {
      font-size: 2.5rem;
    }

    .section-title {
      font-size: 2rem;
    }

    .instructor-content {
      grid-template-columns: 1fr;
    }

    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
    }

    .cta-title {
      font-size: 2rem;
    }
  }
</style>

<div class="about-hero">
  <div class="diagonal-shimmer-1"></div>
  <div class="diagonal-shimmer-2"></div>
  <h1>
    <span class="en-content">About AIcoding Academy</span>
    <span class="zh-content">关于 AIcoding 学院</span>
  </h1>
  <p>
    <span class="en-content">An educational brand created by Ph.D. computer science majors dedicated to excellence</span>
    <span class="zh-content">由计算机科学博士创立的致力于卓越的教育品牌</span>
  </p>
</div>

<!-- Mission Statement -->
<div class="mission-section">
  <h2 class="section-title">
    <span class="en-content">Our Mission</span>
    <span class="zh-content">我们的使命</span>
  </h2>
  <p class="mission-text">
    <span class="en-content">AIcoding is an educational brand created by a group of Ph.D. computer science majors to provide premium tutoring and background improvement services to K-12 students. We bridge the gap between academic excellence and practical programming skills, preparing the next generation of tech innovators.</span>
    <span class="zh-content">AIcoding 是由一群计算机科学博士创立的教育品牌，为K-12学生提供优质的辅导和背景提升服务。我们在学术卓越与实践编程技能之间架起桥梁，培养下一代科技创新者。</span>
  </p>
</div>

<!-- Instructor Introduction -->
<div class="instructor-section">
  <h2 class="section-title">
    <span class="en-content">Meet Our Lead Instructor</span>
    <span class="zh-content">认识我们的首席讲师</span>
  </h2>
  
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
        </div>
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
</div>

<!-- Our Values -->
<div class="values-section">
  <h2 class="section-title">
    <span class="en-content">What Sets Us Apart</span>
    <span class="zh-content">我们的独特之处</span>
  </h2>
  
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
</div>

<!-- Student Success Stats -->
<div class="stats-section">
  <h2 class="section-title" style="color: white;">
    <span class="en-content">Student Success Stories</span>
    <span class="zh-content">学生成功故事</span>
  </h2>
  
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

<!-- Educational Philosophy -->
<div class="philosophy-section">
  <h2 class="section-title" style="color: #92400E;">
    <span class="en-content">Our Educational Philosophy</span>
    <span class="zh-content">我们的教育理念</span>
  </h2>
  
  <ul class="philosophy-list">
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Learning by Doing:</strong>
        <strong class="zh-content">实践学习：</strong>
        <span class="en-content">Hands-on coding from day one with real projects and practical applications</span>
        <span class="zh-content">从第一天起就通过真实项目和实际应用进行编程实践</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Conceptual Understanding:</strong>
        <strong class="zh-content">概念理解：</strong>
        <span class="en-content">Deep comprehension of algorithms and data structures, not just memorization</span>
        <span class="zh-content">深入理解算法和数据结构，而不仅仅是死记硬背</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Competitive Edge:</strong>
        <strong class="zh-content">竞争优势：</strong>
        <span class="en-content">Training students to excel in competitions and stand out in college applications</span>
        <span class="zh-content">培训学生在竞赛中脱颖而出，在大学申请中崭露头角</span>
      </span>
    </li>
    <li class="philosophy-item">
      <span class="philosophy-check">✓</span>
      <span>
        <strong class="en-content">Lifelong Skills:</strong>
        <strong class="zh-content">终身技能：</strong>
        <span class="en-content">Building problem-solving abilities that extend beyond programming</span>
        <span class="zh-content">培养超越编程的问题解决能力</span>
      </span>
    </li>
  </ul>
</div>

<!-- CTA Section -->
<div class="cta-section">
  <div class="diagonal-shimmer-1"></div>
  <div class="diagonal-shimmer-2"></div>
  <div class="cta-content">
    <h2 class="cta-title">
      <span class="en-content">Join the AIcoding Family</span>
      <span class="zh-content">加入 AIcoding 大家庭</span>
    </h2>
    <p class="cta-description">
      <span class="en-content">Experience the difference that expert instruction makes</span>
      <span class="zh-content">体验专家指导的不同之处</span>
    </p>
    <a href="{{ site.baseurl }}/contact.html" class="cta-button">
      <span class="en-content">Get Started Today</span>
      <span class="zh-content">立即开始</span>
    </a>
  </div>
</div>
