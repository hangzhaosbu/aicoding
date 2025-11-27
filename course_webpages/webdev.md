---
layout: default
title: Full-Stack Web Development
title_zh: 全栈Web开发
description: Build Modern Web Applications from Frontend to Backend
description_zh: 从前端到后端构建现代Web应用
---

<style>
  /* Premium Animations */
  @keyframes gradientWave {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-10px) rotate(-1deg); }
    75% { transform: translateY(10px) rotate(1deg); }
  }

  @keyframes shimmer {
    0% { left: -100%; }
    100% { left: 100%; }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50% { transform: scale(1.05); opacity: 0.9; }
  }

  @keyframes slideInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes rotateGlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes globeSpin {
    0% { transform: rotateY(0deg); }
    100% { transform: rotateY(360deg); }
  }

  @keyframes codeType {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.5; }
  }

  @keyframes borderGlow {
    0%, 100% { box-shadow: 0 0 20px rgba(139, 92, 246, 0.5); }
    50% { box-shadow: 0 0 40px rgba(139, 92, 246, 0.8); }
  }

  /* Course Hero - Ultra Premium Purple/Violet Theme */
  .course-hero {
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 25%, #A78BFA 50%, #6D28D9 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(124, 58, 237, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🌐';
    position: absolute;
    font-size: 18rem;
    opacity: 0.1;
    right: -80px;
    top: -60px;
    animation: float 8s ease-in-out infinite;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotateGlow 20s linear infinite;
  }

  /* Floating icons background */
  .course-hero .icons-bg {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .course-hero .floating-icon {
    position: absolute;
    font-size: 2.5rem;
    opacity: 0.15;
    animation: float 10s ease-in-out infinite;
  }

  .floating-icon:nth-child(1) { left: 5%; top: 15%; animation-delay: 0s; }
  .floating-icon:nth-child(2) { left: 90%; top: 20%; animation-delay: 2s; }
  .floating-icon:nth-child(3) { left: 15%; top: 75%; animation-delay: 4s; }
  .floating-icon:nth-child(4) { left: 85%; top: 70%; animation-delay: 6s; }
  .floating-icon:nth-child(5) { left: 50%; top: 8%; animation-delay: 1s; }
  .floating-icon:nth-child(6) { left: 75%; top: 85%; animation-delay: 3s; }
  .floating-icon:nth-child(7) { left: 8%; top: 50%; animation-delay: 5s; }

  .trending-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #EF4444 0%, #DC2626 100%);
    color: white;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 700;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(239, 68, 68, 0.4);
    animation: pulse 2s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .trending-badge::before {
    content: '🔥';
  }

  .course-hero h1 {
    color: white !important;
    font-size: 4rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out;
  }

  .course-hero .hero-subtitle {
    color: white !important;
    font-size: 1.5rem;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.2s backwards;
    margin-bottom: 1.5rem;
  }

  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 1rem 2rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.1rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.4s backwards;
  }

  .hero-stats {
    display: flex;
    gap: 3rem;
    margin-top: 2rem;
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.6s backwards;
  }

  .hero-stat {
    text-align: center;
  }

  .hero-stat-number {
    font-size: 2.5rem;
    font-weight: 800;
    display: block;
  }

  .hero-stat-label {
    font-size: 0.9rem;
    opacity: 0.9;
  }

  /* Section Headers - Premium */
  .section-header {
    text-align: center;
    color: #1F2937;
    margin: 5rem 0 3rem;
    position: relative;
  }

  .section-header h2 {
    font-size: 2.8rem;
    font-weight: 800;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .section-header p {
    color: #6B7280;
    font-size: 1.2rem;
    max-width: 600px;
    margin: 0 auto;
  }

  /* Tech Stack Showcase */
  .tech-stack-section {
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 50%, #DDD6FE 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .tech-stack-section::before {
    content: '</>';
    position: absolute;
    font-size: 15rem;
    opacity: 0.03;
    right: -30px;
    bottom: -30px;
    font-family: monospace;
    font-weight: 800;
  }

  .tech-stack-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #5B21B6;
    margin-bottom: 3rem;
  }

  .tech-categories {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .tech-categories {
      grid-template-columns: 1fr;
    }
  }

  .tech-category {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .tech-category:hover {
    transform: translateY(-5px);
    border-color: #8B5CF6;
    box-shadow: 0 25px 50px rgba(139, 92, 246, 0.15);
  }

  .tech-category-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 1.5rem;
    padding-bottom: 1rem;
    border-bottom: 2px solid #F3F4F6;
  }

  .tech-category-icon {
    width: 50px;
    height: 50px;
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
  }

  .frontend-icon { background: linear-gradient(135deg, #F59E0B, #EAB308); }
  .backend-icon { background: linear-gradient(135deg, #10B981, #059669); }
  .tools-icon { background: linear-gradient(135deg, #3B82F6, #2563EB); }

  .tech-category-title {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
  }

  .tech-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
  }

  .tech-badge {
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 100%);
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 600;
    color: #5B21B6;
    border: 1px solid #DDD6FE;
    transition: all 0.3s ease;
  }

  .tech-badge:hover {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    color: white;
    border-color: transparent;
    transform: translateY(-2px);
  }

  /* Learning Path Section - Premium Timeline */
  .learning-path-section {
    padding: 4rem 2rem;
    background: white;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .learning-path {
    max-width: 1000px;
    margin: 3rem auto 0;
    position: relative;
  }

  .learning-path::before {
    content: '';
    position: absolute;
    left: 50%;
    top: 0;
    bottom: 0;
    width: 4px;
    background: linear-gradient(to bottom, #8B5CF6, #7C3AED, #6D28D9, #5B21B6);
    transform: translateX(-50%);
    border-radius: 2px;
  }

  @media (max-width: 768px) {
    .learning-path::before {
      left: 30px;
    }
  }

  .path-item {
    display: flex;
    align-items: center;
    margin-bottom: 3rem;
    position: relative;
  }

  .path-item:nth-child(odd) {
    flex-direction: row;
  }

  .path-item:nth-child(even) {
    flex-direction: row-reverse;
  }

  @media (max-width: 768px) {
    .path-item,
    .path-item:nth-child(even) {
      flex-direction: row;
      padding-left: 70px;
    }
  }

  .path-number {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 60px;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.5rem;
    color: white;
    box-shadow: 0 10px 25px rgba(139, 92, 246, 0.4);
    z-index: 1;
  }

  @media (max-width: 768px) {
    .path-number {
      left: 30px;
      width: 50px;
      height: 50px;
      font-size: 1.2rem;
    }
  }

  .path-content {
    width: 45%;
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 100%);
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .path-content:hover {
    transform: translateY(-5px);
    border-color: #8B5CF6;
    box-shadow: 0 20px 40px rgba(139, 92, 246, 0.15);
  }

  @media (max-width: 768px) {
    .path-content {
      width: 100%;
    }
  }

  .path-item:nth-child(odd) .path-content {
    margin-right: auto;
    margin-left: 0;
  }

  .path-item:nth-child(even) .path-content {
    margin-left: auto;
    margin-right: 0;
  }

  @media (max-width: 768px) {
    .path-item:nth-child(odd) .path-content,
    .path-item:nth-child(even) .path-content {
      margin: 0;
    }
  }

  .path-title {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .path-duration {
    font-size: 0.85rem;
    color: #8B5CF6;
    font-weight: 600;
    margin-bottom: 1rem;
    background: rgba(139, 92, 246, 0.1);
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    display: inline-block;
  }

  .path-description {
    color: #4B5563;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Project Showcase Section */
  .projects-section {
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 50%, #A78BFA 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(124, 58, 237, 0.3);
  }

  .projects-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .projects-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .projects-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .projects-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .projects-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .projects-grid {
      grid-template-columns: 1fr;
    }
  }

  .project-card {
    background: white;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .project-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25);
  }

  .project-preview {
    height: 140px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 4rem;
    position: relative;
    overflow: hidden;
  }

  .project-preview::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(to bottom, transparent 50%, rgba(0,0,0,0.05) 100%);
  }

  .project-1 .project-preview { background: linear-gradient(135deg, #FEF3C7, #FDE68A); }
  .project-2 .project-preview { background: linear-gradient(135deg, #DBEAFE, #BFDBFE); }
  .project-3 .project-preview { background: linear-gradient(135deg, #D1FAE5, #A7F3D0); }
  .project-4 .project-preview { background: linear-gradient(135deg, #FCE7F3, #FBCFE8); }
  .project-5 .project-preview { background: linear-gradient(135deg, #E0E7FF, #C7D2FE); }
  .project-6 .project-preview { background: linear-gradient(135deg, #FEE2E2, #FECACA); }

  .project-info {
    padding: 1.5rem;
  }

  .project-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .project-desc {
    color: #6B7280;
    font-size: 0.9rem;
    line-height: 1.5;
    margin-bottom: 1rem;
  }

  .project-tech {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .project-tech span {
    background: #F3F4F6;
    padding: 0.3rem 0.6rem;
    border-radius: 10px;
    font-size: 0.75rem;
    color: #4B5563;
    font-weight: 600;
  }

  /* Curriculum Cards - 2x2 Layout */
  .curriculum-section {
    padding: 2rem 0;
  }

  .curriculum-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .curriculum-cards {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .curriculum-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
    border-top: 5px solid;
  }

  .curriculum-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-top-color: #F59E0B;
    background: linear-gradient(to bottom, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-top-color: #3B82F6;
    background: linear-gradient(to bottom, rgba(59, 130, 246, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-top-color: #10B981;
    background: linear-gradient(to bottom, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-top-color: #8B5CF6;
    background: linear-gradient(to bottom, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }

  .curriculum-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(139, 92, 246, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .curriculum-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.15);
  }

  .curriculum-header {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }

  .curriculum-icon {
    width: 60px;
    height: 60px;
    border-radius: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8rem;
    color: white;
    flex-shrink: 0;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
  }

  .curriculum-card:nth-child(1) .curriculum-icon { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .curriculum-card:nth-child(2) .curriculum-icon { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .curriculum-card:nth-child(3) .curriculum-icon { background: linear-gradient(135deg, #10B981, #059669); }
  .curriculum-card:nth-child(4) .curriculum-icon { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }

  .curriculum-title-group {
    flex: 1;
  }

  .curriculum-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .curriculum-subtitle {
    font-size: 0.9rem;
    color: #6B7280;
  }

  .curriculum-topics {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.4rem 1.5rem;
  }

  @media (max-width: 600px) {
    .curriculum-topics {
      grid-template-columns: 1fr;
    }
  }

  .curriculum-topics li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
  }

  .curriculum-topics li::before {
    content: '→';
    font-weight: bold;
    margin-right: 0.6rem;
    flex-shrink: 0;
  }

  .curriculum-card:nth-child(1) .curriculum-topics li::before { color: #F59E0B; }
  .curriculum-card:nth-child(2) .curriculum-topics li::before { color: #3B82F6; }
  .curriculum-card:nth-child(3) .curriculum-topics li::before { color: #10B981; }
  .curriculum-card:nth-child(4) .curriculum-topics li::before { color: #8B5CF6; }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .why-choose-section::before {
    content: '✨';
    position: absolute;
    font-size: 15rem;
    opacity: 0.05;
    right: -50px;
    top: -50px;
  }

  .why-choose-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 3rem auto 0;
  }

  @media (max-width: 968px) {
    .why-choose-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .why-choose-grid {
      grid-template-columns: 1fr;
    }
  }

  .why-choose-item {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .why-choose-item:hover {
    transform: translateY(-5px);
    border-color: #8B5CF6;
    box-shadow: 0 20px 40px rgba(139, 92, 246, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(139, 92, 246, 0.3);
  }

  .why-choose-item h3 {
    color: #1F2937;
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }

  .why-choose-item p {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Success Section - Premium */
  .success-section {
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 50%, #6D28D9 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(124, 58, 237, 0.3);
    position: relative;
    overflow: hidden;
  }

  .success-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.15) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .success-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 3rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .success-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .success-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .success-grid {
      grid-template-columns: 1fr;
    }
  }

  .success-item {
    text-align: center;
    background: white;
    padding: 2rem 1.5rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .success-item:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .success-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }

  .success-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
    animation: pulse 3s ease-in-out infinite;
  }

  .success-label {
    color: #6B7280;
    font-size: 0.95rem;
    font-weight: 600;
    margin-top: 0.3rem;
  }

  /* Career Paths Section */
  .career-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .career-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .career-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .career-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 1000px) {
    .career-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 550px) {
    .career-grid {
      grid-template-columns: 1fr;
    }
  }

  .career-card {
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .career-card:hover {
    transform: translateY(-5px);
    border-color: #8B5CF6;
    box-shadow: 0 15px 30px rgba(139, 92, 246, 0.15);
    background: white;
  }

  .career-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .career-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .career-salary {
    color: #8B5CF6;
    font-size: 0.9rem;
    font-weight: 600;
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #F5F3FF 0%, #EDE9FE 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .testimonials-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
  }

  @media (max-width: 968px) {
    .testimonials-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .testimonials-grid {
      grid-template-columns: 1fr;
    }
  }

  .testimonial-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    position: relative;
    transition: all 0.3s ease;
  }

  .testimonial-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.12);
  }

  .testimonial-card::before {
    content: '"';
    position: absolute;
    top: 15px;
    left: 20px;
    font-size: 4rem;
    color: #8B5CF6;
    opacity: 0.2;
    font-family: Georgia, serif;
    line-height: 1;
  }

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .testimonial-text {
    color: #4B5563;
    font-size: 1rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
    position: relative;
    z-index: 1;
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
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
  }

  .testimonial-info h4 {
    color: #1F2937;
    font-size: 1rem;
    font-weight: 700;
    margin-bottom: 0.2rem;
  }

  .testimonial-info p {
    color: #6B7280;
    font-size: 0.85rem;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 25%, #A78BFA 50%, #6D28D9 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(124, 58, 237, 0.4);
    margin-top: 4rem;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 60%);
    animation: rotateGlow 12s linear infinite;
  }

  .cta-section h2 {
    color: white !important;
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
  }

  .cta-section p {
    color: white !important;
    font-size: 1.3rem;
    margin: 1rem 0 2rem;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .cta-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    flex-wrap: wrap;
    position: relative;
    z-index: 1;
  }

  .cta-button {
    background: white;
    color: #7C3AED;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
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
    background: linear-gradient(90deg, transparent, rgba(139, 92, 246, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #6D28D9;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #7C3AED;
  }

  /* Responsive adjustments */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2.5rem;
    }

    .course-hero .hero-subtitle {
      font-size: 1.2rem;
    }

    .hero-stats {
      flex-direction: column;
      gap: 1.5rem;
    }
    
    .section-header h2 {
      font-size: 2rem;
    }
    
    .cta-section h2 {
      font-size: 2rem;
    }

    .tech-stack-section,
    .learning-path-section,
    .why-choose-section,
    .success-section,
    .projects-section,
    .career-section {
      padding: 3rem 1.5rem;
    }

    .trending-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="trending-badge">
    <span class="en-content">TRENDING</span>
    <span class="zh-content">热门课程</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">🌐</span>
    <span class="floating-icon">⚛️</span>
    <span class="floating-icon">📱</span>
    <span class="floating-icon">🚀</span>
    <span class="floating-icon">💾</span>
    <span class="floating-icon">☁️</span>
    <span class="floating-icon">🔧</span>
  </div>
  <h1>
    <span class="en-content">Full-Stack Web Development</span>
    <span class="zh-content">全栈Web开发</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Build Modern Web Applications from Scratch</span>
    <span class="zh-content">从零开始构建现代Web应用</span>
  </p>
  <div class="hero-badge">
    <span>💻</span>
    <span class="en-content">Frontend + Backend + Deployment</span>
    <span class="zh-content">前端 + 后端 + 部署</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">10+</span>
      <span class="hero-stat-label">
        <span class="en-content">Real Projects</span>
        <span class="zh-content">实战项目</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">60hrs</span>
      <span class="hero-stat-label">
        <span class="en-content">Training</span>
        <span class="zh-content">培训时长</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">100%</span>
      <span class="hero-stat-label">
        <span class="en-content">Job-Ready Skills</span>
        <span class="zh-content">就业技能</span>
      </span>
    </div>
  </div>
</div>

<!-- Tech Stack Showcase -->
<div class="tech-stack-section">
  <h2>
    <span class="en-content">🛠️ Technologies You'll Master</span>
    <span class="zh-content">🛠️ 你将掌握的技术栈</span>
  </h2>
  
  <div class="tech-categories">
    <div class="tech-category">
      <div class="tech-category-header">
        <div class="tech-category-icon frontend-icon">🎨</div>
        <h3 class="tech-category-title">
          <span class="en-content">Frontend</span>
          <span class="zh-content">前端</span>
        </h3>
      </div>
      <div class="tech-list">
        <span class="tech-badge">HTML5</span>
        <span class="tech-badge">CSS3</span>
        <span class="tech-badge">JavaScript</span>
        <span class="tech-badge">React</span>
        <span class="tech-badge">Vue.js</span>
        <span class="tech-badge">Tailwind CSS</span>
        <span class="tech-badge">TypeScript</span>
      </div>
    </div>
    
    <div class="tech-category">
      <div class="tech-category-header">
        <div class="tech-category-icon backend-icon">⚙️</div>
        <h3 class="tech-category-title">
          <span class="en-content">Backend</span>
          <span class="zh-content">后端</span>
        </h3>
      </div>
      <div class="tech-list">
        <span class="tech-badge">Node.js</span>
        <span class="tech-badge">Express.js</span>
        <span class="tech-badge">MongoDB</span>
        <span class="tech-badge">PostgreSQL</span>
        <span class="tech-badge">REST APIs</span>
        <span class="tech-badge">GraphQL</span>
        <span class="tech-badge">Authentication</span>
      </div>
    </div>
    
    <div class="tech-category">
      <div class="tech-category-header">
        <div class="tech-category-icon tools-icon">🔧</div>
        <h3 class="tech-category-title">
          <span class="en-content">Tools & DevOps</span>
          <span class="zh-content">工具与运维</span>
        </h3>
      </div>
      <div class="tech-list">
        <span class="tech-badge">Git & GitHub</span>
        <span class="tech-badge">VS Code</span>
        <span class="tech-badge">Docker</span>
        <span class="tech-badge">AWS/Vercel</span>
        <span class="tech-badge">CI/CD</span>
        <span class="tech-badge">npm/yarn</span>
        <span class="tech-badge">Webpack</span>
      </div>
    </div>
  </div>
</div>

<!-- Curriculum Section -->
<div class="curriculum-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Complete Curriculum</span>
      <span class="zh-content">完整课程大纲</span>
    </h2>
    <p>
      <span class="en-content">From zero to full-stack developer in 16 weeks</span>
      <span class="zh-content">16周从零成为全栈开发者</span>
    </p>
  </div>

  <div class="curriculum-cards">
    <!-- Frontend Fundamentals -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🎨</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Frontend Fundamentals</span>
            <span class="zh-content">前端基础</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 1-4</span>
            <span class="zh-content">第1-4周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">HTML5 Semantic Structure</span><span class="zh-content">HTML5语义化结构</span></li>
        <li><span class="en-content">CSS3 Flexbox & Grid</span><span class="zh-content">CSS3 Flexbox与Grid</span></li>
        <li><span class="en-content">Responsive Design</span><span class="zh-content">响应式设计</span></li>
        <li><span class="en-content">JavaScript ES6+</span><span class="zh-content">JavaScript ES6+</span></li>
        <li><span class="en-content">DOM Manipulation</span><span class="zh-content">DOM操作</span></li>
        <li><span class="en-content">Async/Await & Fetch</span><span class="zh-content">异步编程与Fetch</span></li>
      </ul>
    </div>

    <!-- React & Modern Frontend -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">⚛️</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">React & Modern Frontend</span>
            <span class="zh-content">React与现代前端</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 5-8</span>
            <span class="zh-content">第5-8周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">React Components & JSX</span><span class="zh-content">React组件与JSX</span></li>
        <li><span class="en-content">State & Props</span><span class="zh-content">状态与属性</span></li>
        <li><span class="en-content">React Hooks</span><span class="zh-content">React Hooks</span></li>
        <li><span class="en-content">React Router</span><span class="zh-content">React路由</span></li>
        <li><span class="en-content">Context & Redux</span><span class="zh-content">Context与Redux</span></li>
        <li><span class="en-content">Tailwind CSS</span><span class="zh-content">Tailwind CSS</span></li>
      </ul>
    </div>

    <!-- Backend Development -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">⚙️</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Backend Development</span>
            <span class="zh-content">后端开发</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 9-12</span>
            <span class="zh-content">第9-12周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Node.js Fundamentals</span><span class="zh-content">Node.js基础</span></li>
        <li><span class="en-content">Express.js Framework</span><span class="zh-content">Express.js框架</span></li>
        <li><span class="en-content">RESTful API Design</span><span class="zh-content">RESTful API设计</span></li>
        <li><span class="en-content">MongoDB & Mongoose</span><span class="zh-content">MongoDB与Mongoose</span></li>
        <li><span class="en-content">Authentication & JWT</span><span class="zh-content">身份验证与JWT</span></li>
        <li><span class="en-content">Error Handling</span><span class="zh-content">错误处理</span></li>
      </ul>
    </div>

    <!-- Full-Stack & Deployment -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🚀</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Full-Stack & Deployment</span>
            <span class="zh-content">全栈与部署</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 13-16</span>
            <span class="zh-content">第13-16周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Full-Stack Integration</span><span class="zh-content">全栈整合</span></li>
        <li><span class="en-content">Git & Version Control</span><span class="zh-content">Git版本控制</span></li>
        <li><span class="en-content">Docker Basics</span><span class="zh-content">Docker基础</span></li>
        <li><span class="en-content">Cloud Deployment</span><span class="zh-content">云部署</span></li>
        <li><span class="en-content">CI/CD Pipeline</span><span class="zh-content">CI/CD流水线</span></li>
        <li><span class="en-content">Capstone Project</span><span class="zh-content">毕业项目</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Projects Showcase -->
<div class="projects-section">
  <h2>
    <span class="en-content">🚀 Real Projects You'll Build</span>
    <span class="zh-content">🚀 你将构建的实战项目</span>
  </h2>
  <p>
    <span class="en-content">Build a portfolio of 10+ impressive projects</span>
    <span class="zh-content">构建10+个令人印象深刻的项目作品集</span>
  </p>
  
  <div class="projects-grid">
    <div class="project-card project-1">
      <div class="project-preview">🛒</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">E-Commerce Store</span>
          <span class="zh-content">电商网站</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">Full shopping cart, payments, user auth</span>
          <span class="zh-content">完整购物车、支付、用户认证</span>
        </p>
        <div class="project-tech">
          <span>React</span>
          <span>Node.js</span>
          <span>Stripe</span>
        </div>
      </div>
    </div>
    
    <div class="project-card project-2">
      <div class="project-preview">💬</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">Real-Time Chat App</span>
          <span class="zh-content">实时聊天应用</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">WebSocket, rooms, file sharing</span>
          <span class="zh-content">WebSocket、聊天室、文件分享</span>
        </p>
        <div class="project-tech">
          <span>Socket.io</span>
          <span>React</span>
          <span>MongoDB</span>
        </div>
      </div>
    </div>
    
    <div class="project-card project-3">
      <div class="project-preview">📝</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">Task Management</span>
          <span class="zh-content">任务管理系统</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">Kanban boards, drag & drop, teams</span>
          <span class="zh-content">看板、拖拽功能、团队协作</span>
        </p>
        <div class="project-tech">
          <span>React DnD</span>
          <span>Express</span>
          <span>PostgreSQL</span>
        </div>
      </div>
    </div>
    
    <div class="project-card project-4">
      <div class="project-preview">📱</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">Social Media Clone</span>
          <span class="zh-content">社交媒体克隆</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">Posts, likes, comments, follows</span>
          <span class="zh-content">帖子、点赞、评论、关注</span>
        </p>
        <div class="project-tech">
          <span>React</span>
          <span>GraphQL</span>
          <span>MongoDB</span>
        </div>
      </div>
    </div>
    
    <div class="project-card project-5">
      <div class="project-preview">📊</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">Analytics Dashboard</span>
          <span class="zh-content">数据分析仪表盘</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">Charts, filters, data visualization</span>
          <span class="zh-content">图表、筛选、数据可视化</span>
        </p>
        <div class="project-tech">
          <span>React</span>
          <span>D3.js</span>
          <span>REST API</span>
        </div>
      </div>
    </div>
    
    <div class="project-card project-6">
      <div class="project-preview">🎬</div>
      <div class="project-info">
        <h3 class="project-title">
          <span class="en-content">Video Streaming Platform</span>
          <span class="zh-content">视频流媒体平台</span>
        </h3>
        <p class="project-desc">
          <span class="en-content">Upload, stream, playlists, search</span>
          <span class="zh-content">上传、流媒体、播放列表、搜索</span>
        </p>
        <div class="project-tech">
          <span>React</span>
          <span>AWS S3</span>
          <span>FFmpeg</span>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Learning Path Timeline -->
<div class="learning-path-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Your Learning Journey</span>
      <span class="zh-content">你的学习旅程</span>
    </h2>
    <p>
      <span class="en-content">A structured path from beginner to job-ready developer</span>
      <span class="zh-content">从初学者到就业开发者的结构化路径</span>
    </p>
  </div>

  <div class="learning-path">
    <div class="path-item">
      <div class="path-number">1</div>
      <div class="path-content">
        <h3 class="path-title">
          <span class="en-content">🎨 Frontend Foundations</span>
          <span class="zh-content">🎨 前端基础</span>
        </h3>
        <span class="path-duration">
          <span class="en-content">Weeks 1-4</span>
          <span class="zh-content">第1-4周</span>
        </span>
        <p class="path-description">
          <span class="en-content">Master HTML, CSS, and JavaScript. Build beautiful responsive websites that work on any device.</span>
          <span class="zh-content">掌握HTML、CSS和JavaScript。构建适配任何设备的精美响应式网站。</span>
        </p>
      </div>
    </div>

    <div class="path-item">
      <div class="path-number">2</div>
      <div class="path-content">
        <h3 class="path-title">
          <span class="en-content">⚛️ React Mastery</span>
          <span class="zh-content">⚛️ React精通</span>
        </h3>
        <span class="path-duration">
          <span class="en-content">Weeks 5-8</span>
          <span class="zh-content">第5-8周</span>
        </span>
        <p class="path-description">
          <span class="en-content">Build dynamic single-page applications with React. Learn modern state management and routing.</span>
          <span class="zh-content">使用React构建动态单页应用。学习现代状态管理和路由。</span>
        </p>
      </div>
    </div>

    <div class="path-item">
      <div class="path-number">3</div>
      <div class="path-content">
        <h3 class="path-title">
          <span class="en-content">⚙️ Backend Power</span>
          <span class="zh-content">⚙️ 后端实力</span>
        </h3>
        <span class="path-duration">
          <span class="en-content">Weeks 9-12</span>
          <span class="zh-content">第9-12周</span>
        </span>
        <p class="path-description">
          <span class="en-content">Create powerful APIs with Node.js and Express. Master databases and authentication.</span>
          <span class="zh-content">使用Node.js和Express创建强大的API。掌握数据库和身份验证。</span>
        </p>
      </div>
    </div>

    <div class="path-item">
      <div class="path-number">4</div>
      <div class="path-content">
        <h3 class="path-title">
          <span class="en-content">🚀 Launch Ready</span>
          <span class="zh-content">🚀 上线就绪</span>
        </h3>
        <span class="path-duration">
          <span class="en-content">Weeks 13-16</span>
          <span class="zh-content">第13-16周</span>
        </span>
        <p class="path-description">
          <span class="en-content">Deploy full-stack apps to the cloud. Build your capstone project and portfolio.</span>
          <span class="zh-content">将全栈应用部署到云端。完成毕业项目和作品集。</span>
        </p>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Learn Full-Stack With Us?</span>
      <span class="zh-content">为什么选择我们学习全栈开发？</span>
    </h2>
    <p>
      <span class="en-content">Everything you need to become a professional developer</span>
      <span class="zh-content">成为专业开发者所需的一切</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Project-Based Learning</span>
        <span class="zh-content">项目驱动学习</span>
      </h3>
      <p>
        <span class="en-content">Learn by building 10+ real-world projects from scratch</span>
        <span class="zh-content">通过从零构建10+实战项目来学习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👨‍💻</div>
      <h3>
        <span class="en-content">Industry Experts</span>
        <span class="zh-content">行业专家</span>
      </h3>
      <p>
        <span class="en-content">Learn from developers working at top tech companies</span>
        <span class="zh-content">向顶级科技公司的开发者学习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📂</div>
      <h3>
        <span class="en-content">Portfolio Ready</span>
        <span class="zh-content">作品集就绪</span>
      </h3>
      <p>
        <span class="en-content">Graduate with a GitHub portfolio that impresses recruiters</span>
        <span class="zh-content">毕业时拥有令招聘者印象深刻的GitHub作品集</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🔄</div>
      <h3>
        <span class="en-content">Latest Technologies</span>
        <span class="zh-content">最新技术</span>
      </h3>
      <p>
        <span class="en-content">Always updated with the newest frameworks and tools</span>
        <span class="zh-content">课程始终更新最新框架和工具</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized code reviews</span>
        <span class="zh-content">每班最多6人，个性化代码审查</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🤝</div>
      <h3>
        <span class="en-content">Career Support</span>
        <span class="zh-content">职业支持</span>
      </h3>
      <p>
        <span class="en-content">Resume review, interview prep, and job placement help</span>
        <span class="zh-content">简历审查、面试准备和就业帮助</span>
      </p>
    </div>
  </div>
</div>

<!-- Career Paths -->
<div class="career-section">
  <h2>
    <span class="en-content">🎯 Career Paths You Can Pursue</span>
    <span class="zh-content">🎯 你可以追求的职业道路</span>
  </h2>
  <p>
    <span class="en-content">Open doors to high-demand tech careers</span>
    <span class="zh-content">开启高需求技术职业的大门</span>
  </p>
  
  <div class="career-grid">
    <div class="career-card">
      <div class="career-icon">🎨</div>
      <h3 class="career-title">
        <span class="en-content">Frontend Developer</span>
        <span class="zh-content">前端开发者</span>
      </h3>
      <p class="career-salary">
        <span class="en-content">$80K - $140K</span>
        <span class="zh-content">年薪 $80K - $140K</span>
      </p>
    </div>
    
    <div class="career-card">
      <div class="career-icon">⚙️</div>
      <h3 class="career-title">
        <span class="en-content">Backend Developer</span>
        <span class="zh-content">后端开发者</span>
      </h3>
      <p class="career-salary">
        <span class="en-content">$90K - $160K</span>
        <span class="zh-content">年薪 $90K - $160K</span>
      </p>
    </div>
    
    <div class="career-card">
      <div class="career-icon">🌐</div>
      <h3 class="career-title">
        <span class="en-content">Full-Stack Developer</span>
        <span class="zh-content">全栈开发者</span>
      </h3>
      <p class="career-salary">
        <span class="en-content">$100K - $180K</span>
        <span class="zh-content">年薪 $100K - $180K</span>
      </p>
    </div>
    
    <div class="career-card">
      <div class="career-icon">🚀</div>
      <h3 class="career-title">
        <span class="en-content">Software Engineer</span>
        <span class="zh-content">软件工程师</span>
      </h3>
      <p class="career-salary">
        <span class="en-content">$110K - $200K</span>
        <span class="zh-content">年薪 $110K - $200K</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Section -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Track Record</span>
    <span class="zh-content">🏆 我们的成绩</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">👨‍🎓</div>
      <span class="success-number">200+</span>
      <div class="success-label">
        <span class="en-content">Students Trained</span>
        <span class="zh-content">培训学生</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">💼</div>
      <span class="success-number">85%</span>
      <div class="success-label">
        <span class="en-content">Job Placement</span>
        <span class="zh-content">就业率</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🚀</div>
      <span class="success-number">50+</span>
      <div class="success-label">
        <span class="en-content">Apps Deployed</span>
        <span class="zh-content">已部署应用</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">4.9</span>
      <div class="success-label">
        <span class="en-content">Student Rating</span>
        <span class="zh-content">学生评分</span>
      </div>
    </div>
  </div>
</div>

<!-- Testimonials -->
<div class="testimonials-section">
  <h2>
    <span class="en-content">Student Success Stories</span>
    <span class="zh-content">学生成功故事</span>
  </h2>
  
  <div class="testimonials-grid">
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Hired @ Google</span>
        <span class="zh-content">入职Google</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">This course transformed my career. The projects I built became my portfolio, which helped me land my dream job at Google!</span>
        <span class="zh-content">这门课程改变了我的职业生涯。我构建的项目成为了我的作品集，帮助我获得了在Google的梦想工作！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>James K.</h4>
          <p>
            <span class="en-content">Software Engineer</span>
            <span class="zh-content">软件工程师</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Startup Founder</span>
        <span class="zh-content">创业公司创始人</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">I went from zero coding knowledge to building my own SaaS product. The skills I learned here made it all possible.</span>
        <span class="zh-content">我从零编程知识到构建自己的SaaS产品。我在这里学到的技能让这一切成为可能。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍💻</div>
        <div class="testimonial-info">
          <h4>Sarah M.</h4>
          <p>
            <span class="en-content">Tech Entrepreneur</span>
            <span class="zh-content">科技创业者</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Career Change</span>
        <span class="zh-content">职业转型</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">As a high school student, this course gave me a huge head start. I'm now freelancing and earning while still in school!</span>
        <span class="zh-content">作为一名高中生，这门课程让我领先一步。我现在在上学的同时还能接自由职业项目赚钱！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Ryan T.</h4>
          <p>
            <span class="en-content">Student Freelancer</span>
            <span class="zh-content">学生自由职业者</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Building the Future Today!</span>
    <span class="zh-content">今天就开始构建未来！</span>
  </h2>
  <p>
    <span class="en-content">Join the most in-demand career in tech</span>
    <span class="zh-content">加入科技领域最热门的职业</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-button">
      <span class="en-content">🚀 Enroll Now</span>
      <span class="zh-content">🚀 立即报名</span>
    </a>
    <a href="./contact.html" class="cta-button cta-button-secondary">
      <span class="en-content">📅 Free Consultation</span>
      <span class="zh-content">📅 免费咨询</span>
    </a>
  </div>
</div>
