---
layout: default
title: AP Computer Science Principles
title_zh: AP计算机科学原理
description: Master Computational Thinking & Ace Your AP CSP Exam
description_zh: 掌握计算思维，征服AP CSP考试
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

  @keyframes bulbGlow {
    0%, 100% { 
      filter: drop-shadow(0 0 20px rgba(255, 200, 100, 0.8));
      transform: translateY(0) rotate(-15deg);
    }
    50% { 
      filter: drop-shadow(0 0 40px rgba(255, 200, 100, 1));
      transform: translateY(-15px) rotate(-10deg);
    }
  }

  @keyframes sparkle {
    0%, 100% { opacity: 0; transform: scale(0) rotate(0deg); }
    50% { opacity: 1; transform: scale(1) rotate(180deg); }
  }

  @keyframes typing {
    from { width: 0; }
    to { width: 100%; }
  }

  /* Course Hero - Ultra Premium Pink/Coral Theme */
  .course-hero {
    background: linear-gradient(135deg, #F472B6 0%, #EC4899 25%, #DB2777 50%, #BE185D 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '💡';
    position: absolute;
    font-size: 18rem;
    opacity: 0.15;
    right: -80px;
    top: -60px;
    animation: bulbGlow 4s ease-in-out infinite;
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

  .new-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 700;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(16, 185, 129, 0.4);
    animation: pulse 2s ease-in-out infinite;
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
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
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

  /* What is AP CSP Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #F472B6, #EC4899, #DB2777) 1;
  }

  .intro-section::before {
    content: '🎨';
    position: absolute;
    font-size: 10rem;
    opacity: 0.03;
    right: -20px;
    bottom: -20px;
  }

  .intro-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
  }

  @media (max-width: 900px) {
    .intro-content {
      grid-template-columns: 1fr;
    }
  }

  .intro-text h2 {
    font-size: 2.2rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1.5rem;
  }

  .intro-text p {
    color: #4B5563;
    font-size: 1.1rem;
    line-height: 1.8;
    margin-bottom: 1.5rem;
  }

  .intro-highlights {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }

  .intro-highlight {
    display: flex;
    align-items: center;
    gap: 0.8rem;
    padding: 1rem;
    background: linear-gradient(135deg, #FDF2F8 0%, #FCE7F3 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(236, 72, 153, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Exam Info Section - Premium */
  .exam-info {
    background: linear-gradient(135deg, #FDF2F8 0%, #FCE7F3 50%, #FBCFE8 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .exam-info::before {
    content: '📝';
    position: absolute;
    font-size: 12rem;
    opacity: 0.05;
    right: -30px;
    bottom: -30px;
  }

  .exam-info h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #831843;
    margin-bottom: 2.5rem;
  }

  .exam-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
  }

  @media (max-width: 700px) {
    .exam-grid {
      grid-template-columns: 1fr;
    }
  }

  .exam-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 3px solid transparent;
    position: relative;
    overflow: hidden;
  }

  .exam-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #F472B6, #EC4899, #DB2777);
  }

  .exam-card:hover {
    transform: translateY(-8px) scale(1.02);
    border-color: #EC4899;
    box-shadow: 0 25px 50px rgba(236, 72, 153, 0.2);
  }

  .exam-card-icon {
    font-size: 3.5rem;
    margin-bottom: 1rem;
  }

  .exam-card-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .exam-card-value {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
    margin-bottom: 0.5rem;
  }

  .exam-card-desc {
    color: #6B7280;
    font-size: 0.95rem;
  }

  /* Big Ideas Section - Premium Cards */
  .big-ideas-section {
    padding: 2rem 0;
  }

  .big-ideas-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .big-ideas-grid {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .big-idea-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
    border-left: 5px solid;
  }

  .big-idea-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-left-color: #EC4899;
    background: linear-gradient(to right, rgba(236, 72, 153, 0.03) 0%, white 30%);
  }
  .big-idea-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #8B5CF6;
    background: linear-gradient(to right, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }
  .big-idea-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-left-color: #3B82F6;
    background: linear-gradient(to right, rgba(59, 130, 246, 0.03) 0%, white 30%);
  }
  .big-idea-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-left-color: #10B981;
    background: linear-gradient(to right, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }
  .big-idea-card:nth-child(5) { 
    animation-delay: 0.3s; 
    border-left-color: #F59E0B;
    background: linear-gradient(to right, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }

  .big-idea-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(236, 72, 153, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .big-idea-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.15);
  }

  .big-idea-header {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }

  .big-idea-number {
    width: 60px;
    height: 60px;
    border-radius: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.5rem;
    color: white;
    flex-shrink: 0;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
  }

  .big-idea-card:nth-child(1) .big-idea-number { background: linear-gradient(135deg, #EC4899, #DB2777); }
  .big-idea-card:nth-child(2) .big-idea-number { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .big-idea-card:nth-child(3) .big-idea-number { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .big-idea-card:nth-child(4) .big-idea-number { background: linear-gradient(135deg, #10B981, #059669); }
  .big-idea-card:nth-child(5) .big-idea-number { background: linear-gradient(135deg, #F59E0B, #D97706); }

  .big-idea-title-group {
    flex: 1;
  }

  .big-idea-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .big-idea-subtitle {
    font-size: 0.9rem;
    color: #6B7280;
  }

  .big-idea-topics {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.4rem 1.5rem;
  }

  @media (max-width: 600px) {
    .big-idea-topics {
      grid-template-columns: 1fr;
    }
  }

  .big-idea-topics li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
  }

  .big-idea-topics li::before {
    content: '→';
    font-weight: bold;
    margin-right: 0.6rem;
    flex-shrink: 0;
  }

  .big-idea-card:nth-child(1) .big-idea-topics li::before { color: #EC4899; }
  .big-idea-card:nth-child(2) .big-idea-topics li::before { color: #8B5CF6; }
  .big-idea-card:nth-child(3) .big-idea-topics li::before { color: #3B82F6; }
  .big-idea-card:nth-child(4) .big-idea-topics li::before { color: #10B981; }
  .big-idea-card:nth-child(5) .big-idea-topics li::before { color: #F59E0B; }

  /* Create Task Section - Special Premium */
  .create-task-section {
    background: linear-gradient(135deg, #7C3AED 0%, #8B5CF6 50%, #A78BFA 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.3);
  }

  .create-task-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .create-task-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .create-task-content {
      grid-template-columns: 1fr;
    }
  }

  .create-task-text h2 {
    color: white !important;
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  }

  .create-task-text p {
    color: rgba(255, 255, 255, 0.95);
    font-size: 1.15rem;
    line-height: 1.8;
    margin-bottom: 1.5rem;
  }

  .create-task-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 0.8rem 1.5rem;
    border-radius: 30px;
    color: white;
    font-weight: 700;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .create-task-steps {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .create-step {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    padding: 1.5rem;
    border-radius: 15px;
    display: flex;
    align-items: center;
    gap: 1rem;
    border: 1px solid rgba(255, 255, 255, 0.2);
    transition: all 0.3s ease;
  }

  .create-step:hover {
    background: rgba(255, 255, 255, 0.25);
    transform: translateX(10px);
  }

  .create-step-number {
    width: 45px;
    height: 45px;
    background: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.2rem;
    color: #7C3AED;
    flex-shrink: 0;
  }

  .create-step-text {
    color: white;
    font-weight: 600;
    font-size: 1.05rem;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #FDF2F8 0%, #FCE7F3 100%);
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
    border-color: #EC4899;
    box-shadow: 0 20px 40px rgba(236, 72, 153, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(236, 72, 153, 0.3);
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
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 50%, #BE185D 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.3);
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
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
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

  /* Comparison Section - CSP vs CSA */
  .comparison-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .comparison-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .comparison-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .comparison-table {
    max-width: 900px;
    margin: 0 auto;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  }

  .comparison-row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    border-bottom: 1px solid #E5E7EB;
  }

  .comparison-row:last-child {
    border-bottom: none;
  }

  .comparison-header {
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
  }

  .comparison-header .comparison-cell {
    color: white;
    font-weight: 700;
    font-size: 1.1rem;
  }

  .comparison-cell {
    padding: 1.2rem 1.5rem;
    text-align: center;
    color: #4B5563;
    font-size: 0.95rem;
  }

  .comparison-cell:first-child {
    background: #F9FAFB;
    font-weight: 600;
    color: #1F2937;
    text-align: left;
  }

  .comparison-row:nth-child(even) {
    background: #FAFAFA;
  }

  @media (max-width: 600px) {
    .comparison-cell {
      padding: 0.8rem;
      font-size: 0.85rem;
    }
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #FDF2F8 0%, #FCE7F3 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
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
    color: #EC4899;
    opacity: 0.2;
    font-family: Georgia, serif;
    line-height: 1;
  }

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
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
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 100%);
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
    background: linear-gradient(135deg, #F472B6 0%, #EC4899 25%, #DB2777 50%, #BE185D 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.4);
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
    color: #EC4899;
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
    background: linear-gradient(90deg, transparent, rgba(236, 72, 153, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #DB2777;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #EC4899;
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

    .intro-section,
    .exam-info,
    .why-choose-section,
    .success-section,
    .create-task-section,
    .comparison-section {
      padding: 3rem 1.5rem;
    }

    .new-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="new-badge">
    <span class="en-content">✨ NEW</span>
    <span class="zh-content">✨ 新课程</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">💡</span>
    <span class="floating-icon">🌐</span>
    <span class="floating-icon">📊</span>
    <span class="floating-icon">🎨</span>
    <span class="floating-icon">🔐</span>
    <span class="floating-icon">⚡</span>
    <span class="floating-icon">🤖</span>
  </div>
  <h1>
    <span class="en-content">AP Computer Science Principles</span>
    <span class="zh-content">AP计算机科学原理</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Computational Thinking & Creative Innovation</span>
    <span class="zh-content">计算思维与创意创新</span>
  </p>
  <div class="hero-badge">
    <span>🎯</span>
    <span class="en-content">Perfect for Beginners • No Coding Required</span>
    <span class="zh-content">零基础友好 · 无需编程经验</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">95%</span>
      <span class="hero-stat-label">
        <span class="en-content">Pass Rate</span>
        <span class="zh-content">通过率</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">88%</span>
      <span class="hero-stat-label">
        <span class="en-content">Score 4+</span>
        <span class="zh-content">4分以上</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">30hrs</span>
      <span class="hero-stat-label">
        <span class="en-content">Training</span>
        <span class="zh-content">培训时长</span>
      </span>
    </div>
  </div>
</div>

<!-- What is AP CSP -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is AP Computer Science Principles?</span>
        <span class="zh-content">什么是AP计算机科学原理？</span>
      </h2>
      <p>
        <span class="en-content">
          AP CSP is the perfect introduction to computer science! Unlike AP CSA which focuses on Java programming, 
          AP CSP explores the broader concepts of computing, data, the internet, and the impact of technology on society. 
          It's designed for students who want to understand how computing shapes our world—no prior coding experience needed!
        </span>
        <span class="zh-content">
          AP CSP是计算机科学的完美入门！与专注于Java编程的AP CSA不同，AP CSP探索更广泛的计算概念、数据、互联网以及技术对社会的影响。
          它专为想要了解计算如何塑造我们世界的学生设计——无需任何编程经验！
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎯</span>
          <span class="intro-highlight-text">
            <span class="en-content">Beginner Friendly</span>
            <span class="zh-content">零基础友好</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎨</span>
          <span class="intro-highlight-text">
            <span class="en-content">Creative Projects</span>
            <span class="zh-content">创意项目</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌐</span>
          <span class="intro-highlight-text">
            <span class="en-content">Real-World Impact</span>
            <span class="zh-content">现实世界影响</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">💻</span>
          <span class="intro-highlight-text">
            <span class="en-content">Any Language OK</span>
            <span class="zh-content">任意编程语言</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 12rem; opacity: 0.8; animation: float 6s ease-in-out infinite;">💡</div>
    </div>
  </div>
</div>

<!-- Exam Information -->
<div class="exam-info">
  <h2>
    <span class="en-content">📅 2025 AP CSP Exam Format</span>
    <span class="zh-content">📅 2025年AP CSP考试形式</span>
  </h2>
  
  <div class="exam-grid">
    <div class="exam-card">
      <div class="exam-card-icon">📝</div>
      <h3 class="exam-card-title">
        <span class="en-content">End-of-Course Exam</span>
        <span class="zh-content">课程结束考试</span>
      </h3>
      <span class="exam-card-value">70</span>
      <p class="exam-card-desc">
        <span class="en-content">Multiple Choice Questions • 2 Hours • 70% of Score</span>
        <span class="zh-content">选择题 · 2小时 · 占总分70%</span>
      </p>
    </div>
    <div class="exam-card">
      <div class="exam-card-icon">🎨</div>
      <h3 class="exam-card-title">
        <span class="en-content">Create Performance Task</span>
        <span class="zh-content">创意项目任务</span>
      </h3>
      <span class="exam-card-value">30%</span>
      <p class="exam-card-desc">
        <span class="en-content">Programming Project • 12 Hours In-Class • 30% of Score</span>
        <span class="zh-content">编程项目 · 12课时 · 占总分30%</span>
      </p>
    </div>
  </div>
</div>

<!-- 5 Big Ideas Section -->
<div class="big-ideas-section">
  <div class="section-header">
    <h2>
      <span class="en-content">The 5 Big Ideas of AP CSP</span>
      <span class="zh-content">AP CSP的5大核心概念</span>
    </h2>
    <p>
      <span class="en-content">Master all five foundational concepts for exam success</span>
      <span class="zh-content">掌握五大基础概念，确保考试成功</span>
    </p>
  </div>

  <div class="big-ideas-grid">
    <!-- Big Idea 1 -->
    <div class="big-idea-card">
      <div class="big-idea-header">
        <div class="big-idea-number">1</div>
        <div class="big-idea-title-group">
          <h3 class="big-idea-title">
            <span class="en-content">Creative Development</span>
            <span class="zh-content">创意开发</span>
          </h3>
          <p class="big-idea-subtitle">
            <span class="en-content">10-13% of Exam</span>
            <span class="zh-content">占考试10-13%</span>
          </p>
        </div>
      </div>
      <ul class="big-idea-topics">
        <li><span class="en-content">Collaboration in Computing</span><span class="zh-content">计算中的协作</span></li>
        <li><span class="en-content">Program Design & Development</span><span class="zh-content">程序设计与开发</span></li>
        <li><span class="en-content">Identifying Errors</span><span class="zh-content">错误识别</span></li>
        <li><span class="en-content">Documentation</span><span class="zh-content">文档编写</span></li>
      </ul>
    </div>

    <!-- Big Idea 2 -->
    <div class="big-idea-card">
      <div class="big-idea-header">
        <div class="big-idea-number">2</div>
        <div class="big-idea-title-group">
          <h3 class="big-idea-title">
            <span class="en-content">Data</span>
            <span class="zh-content">数据</span>
          </h3>
          <p class="big-idea-subtitle">
            <span class="en-content">17-22% of Exam</span>
            <span class="zh-content">占考试17-22%</span>
          </p>
        </div>
      </div>
      <ul class="big-idea-topics">
        <li><span class="en-content">Binary & Data Representation</span><span class="zh-content">二进制与数据表示</span></li>
        <li><span class="en-content">Data Compression</span><span class="zh-content">数据压缩</span></li>
        <li><span class="en-content">Extracting Information</span><span class="zh-content">信息提取</span></li>
        <li><span class="en-content">Metadata & Visualization</span><span class="zh-content">元数据与可视化</span></li>
      </ul>
    </div>

    <!-- Big Idea 3 -->
    <div class="big-idea-card">
      <div class="big-idea-header">
        <div class="big-idea-number">3</div>
        <div class="big-idea-title-group">
          <h3 class="big-idea-title">
            <span class="en-content">Algorithms & Programming</span>
            <span class="zh-content">算法与编程</span>
          </h3>
          <p class="big-idea-subtitle">
            <span class="en-content">30-35% of Exam</span>
            <span class="zh-content">占考试30-35%</span>
          </p>
        </div>
      </div>
      <ul class="big-idea-topics">
        <li><span class="en-content">Variables & Data Types</span><span class="zh-content">变量与数据类型</span></li>
        <li><span class="en-content">Control Structures</span><span class="zh-content">控制结构</span></li>
        <li><span class="en-content">Procedures & Functions</span><span class="zh-content">过程与函数</span></li>
        <li><span class="en-content">Lists & Algorithms</span><span class="zh-content">列表与算法</span></li>
        <li><span class="en-content">Simulation & Randomness</span><span class="zh-content">模拟与随机性</span></li>
        <li><span class="en-content">Algorithm Efficiency</span><span class="zh-content">算法效率</span></li>
      </ul>
    </div>

    <!-- Big Idea 4 -->
    <div class="big-idea-card">
      <div class="big-idea-header">
        <div class="big-idea-number">4</div>
        <div class="big-idea-title-group">
          <h3 class="big-idea-title">
            <span class="en-content">Computing Systems & Networks</span>
            <span class="zh-content">计算系统与网络</span>
          </h3>
          <p class="big-idea-subtitle">
            <span class="en-content">11-15% of Exam</span>
            <span class="zh-content">占考试11-15%</span>
          </p>
        </div>
      </div>
      <ul class="big-idea-topics">
        <li><span class="en-content">The Internet & Protocols</span><span class="zh-content">互联网与协议</span></li>
        <li><span class="en-content">Fault Tolerance</span><span class="zh-content">容错性</span></li>
        <li><span class="en-content">Parallel & Distributed Computing</span><span class="zh-content">并行与分布式计算</span></li>
        <li><span class="en-content">Computer Components</span><span class="zh-content">计算机组件</span></li>
      </ul>
    </div>

    <!-- Big Idea 5 -->
    <div class="big-idea-card">
      <div class="big-idea-header">
        <div class="big-idea-number">5</div>
        <div class="big-idea-title-group">
          <h3 class="big-idea-title">
            <span class="en-content">Impact of Computing</span>
            <span class="zh-content">计算的影响</span>
          </h3>
          <p class="big-idea-subtitle">
            <span class="en-content">21-26% of Exam</span>
            <span class="zh-content">占考试21-26%</span>
          </p>
        </div>
      </div>
      <ul class="big-idea-topics">
        <li><span class="en-content">Beneficial & Harmful Effects</span><span class="zh-content">有益与有害影响</span></li>
        <li><span class="en-content">Digital Divide</span><span class="zh-content">数字鸿沟</span></li>
        <li><span class="en-content">Computing Bias</span><span class="zh-content">计算偏见</span></li>
        <li><span class="en-content">Crowdsourcing & Citizen Science</span><span class="zh-content">众包与公民科学</span></li>
        <li><span class="en-content">Legal & Ethical Concerns</span><span class="zh-content">法律与伦理问题</span></li>
        <li><span class="en-content">Safe Computing & Privacy</span><span class="zh-content">安全计算与隐私</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Create Performance Task Section -->
<div class="create-task-section">
  <div class="create-task-content">
    <div class="create-task-text">
      <h2>
        <span class="en-content">🎨 Create Performance Task</span>
        <span class="zh-content">🎨 创意项目任务</span>
      </h2>
      <p>
        <span class="en-content">
          The Create Task is your chance to shine! You'll develop a program of your choice that demonstrates 
          your understanding of algorithms, abstractions, and programming concepts. We provide step-by-step 
          guidance and feedback to help you earn maximum points.
        </span>
        <span class="zh-content">
          创意任务是你展示才华的机会！你将开发一个自选程序，展示你对算法、抽象和编程概念的理解。
          我们提供逐步指导和反馈，帮助你获得最高分数。
        </span>
      </p>
      <div class="create-task-badge">
        <span class="en-content">Worth 30% of Your Final Score!</span>
        <span class="zh-content">占最终成绩的30%！</span>
      </div>
    </div>
    <div class="create-task-steps">
      <div class="create-step">
        <div class="create-step-number">1</div>
        <span class="create-step-text">
          <span class="en-content">Develop your program idea & plan</span>
          <span class="zh-content">制定程序创意与计划</span>
        </span>
      </div>
      <div class="create-step">
        <div class="create-step-number">2</div>
        <span class="create-step-text">
          <span class="en-content">Write code with algorithms & abstraction</span>
          <span class="zh-content">编写包含算法与抽象的代码</span>
        </span>
      </div>
      <div class="create-step">
        <div class="create-step-number">3</div>
        <span class="create-step-text">
          <span class="en-content">Create video demonstration (1 min)</span>
          <span class="zh-content">制作演示视频（1分钟）</span>
        </span>
      </div>
      <div class="create-step">
        <div class="create-step-number">4</div>
        <span class="create-step-text">
          <span class="en-content">Write personalized project response</span>
          <span class="zh-content">撰写个性化项目说明</span>
        </span>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Choose Our AP CSP Program?</span>
      <span class="zh-content">为什么选择我们的AP CSP课程？</span>
    </h2>
    <p>
      <span class="en-content">Everything you need to succeed on the AP CSP exam</span>
      <span class="zh-content">助你AP CSP考试成功的一切资源</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Beginner Friendly</span>
        <span class="zh-content">零基础友好</span>
      </h3>
      <p>
        <span class="en-content">No prior coding experience needed—we start from scratch!</span>
        <span class="zh-content">无需编程经验——我们从零开始！</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎨</div>
      <h3>
        <span class="en-content">Create Task Mastery</span>
        <span class="zh-content">创意任务精通</span>
      </h3>
      <p>
        <span class="en-content">Step-by-step guidance for the 30% performance task</span>
        <span class="zh-content">针对30%创意任务的逐步指导</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">All 5 Big Ideas</span>
        <span class="zh-content">覆盖5大概念</span>
      </h3>
      <p>
        <span class="en-content">Complete coverage of all exam topics with practice</span>
        <span class="zh-content">完整覆盖所有考试话题并配有练习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">💻</div>
      <h3>
        <span class="en-content">Hands-On Coding</span>
        <span class="zh-content">动手编程</span>
      </h3>
      <p>
        <span class="en-content">Learn with Python, JavaScript, or Scratch—your choice!</span>
        <span class="zh-content">使用Python、JavaScript或Scratch学习——你来选！</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📝</div>
      <h3>
        <span class="en-content">MCQ Practice</span>
        <span class="zh-content">选择题练习</span>
      </h3>
      <p>
        <span class="en-content">Hundreds of practice questions with detailed explanations</span>
        <span class="zh-content">数百道练习题配有详细解析</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized attention</span>
        <span class="zh-content">每班最多6人，个性化关注</span>
      </p>
    </div>
  </div>
</div>

<!-- CSP vs CSA Comparison -->
<div class="comparison-section">
  <h2>
    <span class="en-content">AP CSP vs AP CSA: Which is Right for You?</span>
    <span class="zh-content">AP CSP vs AP CSA：哪个适合你？</span>
  </h2>
  <p>
    <span class="en-content">Understanding the differences to make the best choice</span>
    <span class="zh-content">了解差异，做出最佳选择</span>
  </p>
  
  <div class="comparison-table">
    <div class="comparison-row comparison-header">
      <div class="comparison-cell">
        <span class="en-content">Feature</span>
        <span class="zh-content">特点</span>
      </div>
      <div class="comparison-cell">AP CSP</div>
      <div class="comparison-cell">AP CSA</div>
    </div>
    <div class="comparison-row">
      <div class="comparison-cell">
        <span class="en-content">Difficulty</span>
        <span class="zh-content">难度</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">⭐⭐ Beginner</span>
        <span class="zh-content">⭐⭐ 入门级</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">⭐⭐⭐⭐ Advanced</span>
        <span class="zh-content">⭐⭐⭐⭐ 进阶级</span>
      </div>
    </div>
    <div class="comparison-row">
      <div class="comparison-cell">
        <span class="en-content">Programming</span>
        <span class="zh-content">编程</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">Any language (Python, JS, etc.)</span>
        <span class="zh-content">任意语言（Python、JS等）</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">Java only</span>
        <span class="zh-content">仅限Java</span>
      </div>
    </div>
    <div class="comparison-row">
      <div class="comparison-cell">
        <span class="en-content">Focus</span>
        <span class="zh-content">重点</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">Concepts & Impact</span>
        <span class="zh-content">概念与影响</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">Programming & OOP</span>
        <span class="zh-content">编程与面向对象</span>
      </div>
    </div>
    <div class="comparison-row">
      <div class="comparison-cell">
        <span class="en-content">Exam Format</span>
        <span class="zh-content">考试形式</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">70 MCQ + Create Task</span>
        <span class="zh-content">70道选择题 + 创意项目</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">40 MCQ + 4 FRQ</span>
        <span class="zh-content">40道选择题 + 4道问答题</span>
      </div>
    </div>
    <div class="comparison-row">
      <div class="comparison-cell">
        <span class="en-content">Best For</span>
        <span class="zh-content">适合人群</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">First-time CS students</span>
        <span class="zh-content">首次学习CS的学生</span>
      </div>
      <div class="comparison-cell">
        <span class="en-content">Aspiring CS majors</span>
        <span class="zh-content">志向CS专业的学生</span>
      </div>
    </div>
  </div>
</div>

<!-- Success Section -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' AP CSP Results</span>
    <span class="zh-content">🏆 我们学生的AP CSP成绩</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">95%</span>
      <div class="success-label">
        <span class="en-content">Pass Rate</span>
        <span class="zh-content">通过率</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🎯</div>
      <span class="success-number">88%</span>
      <div class="success-label">
        <span class="en-content">Score 4 or 5</span>
        <span class="zh-content">获得4或5分</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🎨</div>
      <span class="success-number">100%</span>
      <div class="success-label">
        <span class="en-content">Create Task Completed</span>
        <span class="zh-content">创意任务完成率</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">😊</div>
      <span class="success-number">98%</span>
      <div class="success-label">
        <span class="en-content">Student Satisfaction</span>
        <span class="zh-content">学生满意度</span>
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
        <span class="en-content">Score: 5</span>
        <span class="zh-content">5分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">I had zero coding experience before this class. The way they explained concepts made everything click, and my Create Task turned out amazing!</span>
        <span class="zh-content">上课前我完全没有编程经验。他们讲解概念的方式让一切变得清晰，我的创意任务做得非常棒！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👧</div>
        <div class="testimonial-info">
          <h4>Sophia M.</h4>
          <p>
            <span class="en-content">Freshman, Score 5</span>
            <span class="zh-content">高一学生，5分</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Score: 5</span>
        <span class="zh-content">5分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The practice questions were so similar to the actual exam! I felt completely prepared and confident walking into the test.</span>
        <span class="zh-content">练习题和真正考试非常相似！走进考场时我感到完全准备好了，充满信心。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👦</div>
        <div class="testimonial-info">
          <h4>Alex T.</h4>
          <p>
            <span class="en-content">Sophomore, Score 5</span>
            <span class="zh-content">高二学生，5分</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Score: 4</span>
        <span class="zh-content">4分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">I loved learning about how the internet works and the impact of computing on society. It's not just coding—it's understanding our digital world!</span>
        <span class="zh-content">我喜欢学习互联网如何运作以及计算对社会的影响。这不仅仅是编程——是理解我们的数字世界！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩</div>
        <div class="testimonial-info">
          <h4>Maya L.</h4>
          <p>
            <span class="en-content">Junior, Score 4</span>
            <span class="zh-content">高三学生，4分</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Your CS Journey Today!</span>
    <span class="zh-content">今天开始您的计算机科学之旅！</span>
  </h2>
  <p>
    <span class="en-content">Perfect for beginners—no coding experience required</span>
    <span class="zh-content">零基础友好——无需编程经验</span>
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
