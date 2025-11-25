---
layout: default
title: AI & Machine Learning Course
title_zh: 人工智能与机器学习课程
description: Master Artificial Intelligence for Competitions and Beyond
description_zh: 掌握人工智能，征服竞赛与未来
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

  @keyframes robotBounce {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  @keyframes neuralPulse {
    0%, 100% { opacity: 0.1; transform: scale(1); }
    50% { opacity: 0.15; transform: scale(1.05); }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 25%, #3B82F6 50%, #10B981 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.4);
    min-height: 400px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🤖';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: robotBounce 6s ease-in-out infinite;
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
    font-size: 3rem;
    opacity: 0.1;
    animation: float 10s ease-in-out infinite;
  }

  .floating-icon:nth-child(1) { left: 10%; top: 20%; animation-delay: 0s; }
  .floating-icon:nth-child(2) { left: 80%; top: 30%; animation-delay: 2s; }
  .floating-icon:nth-child(3) { left: 20%; top: 70%; animation-delay: 4s; }
  .floating-icon:nth-child(4) { left: 70%; top: 60%; animation-delay: 6s; }

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

  .course-hero p {
    color: white !important;
    font-size: 1.5rem;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.2s backwards;
  }

  .hero-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 1rem 2rem;
    border-radius: 50px;
    margin-top: 1.5rem;
    font-weight: 700;
    font-size: 1.1rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.4s backwards;
  }

  /* Section Headers - Premium */
  .section-header {
    text-align: center;
    color: #1F2937;
    margin: 5rem 0 3rem;
    position: relative;
  }

  .section-header h2 {
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .section-header p {
    color: #6B7280;
    font-size: 1.2rem;
  }

  /* Phase Cards - Premium Design (4-column like USACO) */
  .phase-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 4rem auto;
    max-width: 1600px;
    padding: 0 2rem;
  }

  @media (max-width: 1400px) {
    .phase-cards {
      grid-template-columns: repeat(2, 1fr);
      gap: 2.5rem;
    }
  }

  @media (max-width: 768px) {
    .phase-cards {
      grid-template-columns: 1fr;
    }
  }

  .phase-card {
    background: white;
    padding: 2rem 1.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: flex;
    flex-direction: column;
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
    min-width: 0;
  }

  .phase-card:nth-child(1) { animation-delay: 0.1s; }
  .phase-card:nth-child(2) { animation-delay: 0.2s; }
  .phase-card:nth-child(3) { animation-delay: 0.3s; }
  .phase-card:nth-child(4) { animation-delay: 0.4s; }

  .phase-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
    animation: shimmer 3s infinite;
  }

  .phase-card:hover {
    transform: translateY(-10px) scale(1.03);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
  }

  .phase-foundation { 
    border-top: 6px solid #8B5CF6;
    background: linear-gradient(to bottom, rgba(139, 92, 246, 0.08) 0%, white 40%);
  }
  
  .phase-foundation:hover {
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.3);
  }
  
  .phase-intermediate { 
    border-top: 6px solid #EC4899;
    background: linear-gradient(to bottom, rgba(236, 72, 153, 0.08) 0%, white 40%);
  }
  
  .phase-intermediate:hover {
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.3);
  }
  
  .phase-advanced { 
    border-top: 6px solid #3B82F6;
    background: linear-gradient(to bottom, rgba(59, 130, 246, 0.08) 0%, white 40%);
  }
  
  .phase-advanced:hover {
    box-shadow: 0 30px 60px rgba(59, 130, 246, 0.4);
  }
  
  .phase-expert { 
    border-top: 6px solid;
    border-image: linear-gradient(90deg, #10B981, #059669, #10B981) 1;
    background: linear-gradient(to bottom, rgba(16, 185, 129, 0.1) 0%, white 40%);
  }
  
  .phase-expert:hover {
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.3);
  }

  .phase-header {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .phase-icon {
    font-size: 3.5rem;
    margin-bottom: 0.8rem;
    display: inline-block;
    animation: pulse 3s ease-in-out infinite;
  }

  .phase-foundation .phase-icon { animation-delay: 0s; }
  .phase-intermediate .phase-icon { animation-delay: 0.5s; }
  .phase-advanced .phase-icon { animation-delay: 1s; }
  .phase-expert .phase-icon { animation-delay: 1.5s; }

  .phase-name {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
    white-space: nowrap;
  }

  .phase-subtitle {
    font-size: 0.95rem;
    font-weight: 500;
    color: #6B7280;
    margin-bottom: 1.2rem;
    white-space: nowrap;
  }

  .phase-topics {
    color: #6B7280;
    line-height: 1.6;
    flex-grow: 1;
  }

  .phase-topics ul {
    padding-left: 0;
    margin: 0;
    list-style: none;
  }

  .phase-topics li {
    margin: 0.5rem 0;
    font-size: 0.9rem;
    padding-left: 1.5rem;
    position: relative;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  @media (max-width: 1600px) {
    .phase-topics li {
      white-space: normal;
      font-size: 0.85rem;
    }
  }

  .phase-topics li::before {
    content: '→';
    position: absolute;
    left: 0;
    font-weight: bold;
  }

  .phase-foundation .phase-topics li::before { color: #8B5CF6; }
  .phase-intermediate .phase-topics li::before { color: #EC4899; }
  .phase-advanced .phase-topics li::before { color: #3B82F6; }
  .phase-expert .phase-topics li::before { color: #10B981; }

  /* Timeline Section */
  .timeline-section {
    padding: 4rem 0;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .timeline {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    max-width: 1000px;
    margin: 3rem auto;
    padding: 0 2rem;
  }

  .timeline::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 5%;
    right: 5%;
    height: 4px;
    background: linear-gradient(90deg, #8B5CF6 0%, #EC4899 33%, #3B82F6 66%, #10B981 100%);
    z-index: 0;
    border-radius: 2px;
  }

  .timeline-item {
    background: white;
    padding: 1.5rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    z-index: 1;
    position: relative;
    text-align: center;
    flex: 1;
    margin: 0 1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
  }

  .timeline-item:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .timeline-item:nth-child(1):hover { border-color: #8B5CF6; }
  .timeline-item:nth-child(2):hover { border-color: #EC4899; }
  .timeline-item:nth-child(3):hover { border-color: #3B82F6; }
  .timeline-item:nth-child(4):hover { border-color: #10B981; }

  .timeline-phase {
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
    font-size: 1.2rem;
  }

  .timeline-duration {
    font-size: 0.9rem;
    color: #6B7280;
  }

  @media (max-width: 768px) {
    .timeline {
      flex-direction: column;
      gap: 2rem;
    }
    
    .timeline::before {
      top: 0;
      bottom: 0;
      left: 50%;
      width: 4px;
      height: 90%;
    }
  }

  /* Competition Preparation - Premium Cards */
  .competition-section {
    background: white;
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
  }

  .competition-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #8B5CF6, #EC4899, #3B82F6, #10B981);
    animation: shimmer 3s infinite;
  }

  .competition-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 3rem;
  }

  .competition-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 3rem;
  }

  @media (max-width: 1200px) {
    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .competition-grid {
      grid-template-columns: 1fr;
    }
  }

  .competition-card {
    text-align: center;
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 2.5rem;
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
  }

  .competition-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(139, 92, 246, 0.1), transparent);
    transition: left 0.5s;
  }

  .competition-card:hover::before {
    left: 100%;
  }

  .competition-card:hover {
    transform: translateY(-5px) scale(1.02);
    box-shadow: 0 15px 30px rgba(139, 92, 246, 0.2);
    border-color: #8B5CF6;
    background: white;
  }

  .competition-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 20px;
    font-size: 2.5rem;
    animation: float 6s ease-in-out infinite;
  }

  .competition-card:nth-child(odd) .competition-icon {
    animation-delay: 0s;
  }

  .competition-card:nth-child(even) .competition-icon {
    animation-delay: 3s;
  }

  .usaaio-icon {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    color: white;
    font-weight: 700;
    font-size: 1.5rem;
  }

  .kaggle-icon {
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 100%);
    color: white;
    font-weight: 700;
    font-size: 2rem;
  }

  .research-icon {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
  }

  .portfolio-icon {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
  }

  .competition-title {
    color: #1F2937;
    font-size: 1.3rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
  }

  .competition-desc {
    color: #6B7280;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* Success Stories - Premium Stats */
  .success-section {
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.3);
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
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
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

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 3rem;
    margin: 2rem 0;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 968px) {
    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .stats-grid {
      grid-template-columns: 1fr;
    }
  }

  .stat-item {
    text-align: center;
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .stat-item:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .stat-number {
    font-size: 3rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    display: inline-block;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #6B7280;
    font-size: 1rem;
    margin-top: 0.5rem;
    font-weight: 600;
  }

  /* Tools & Technologies - Premium Grid */
  .tools-section {
    background: linear-gradient(135deg, #EDE9FE 0%, #FCE7F3 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .tools-section::before {
    content: '⚡';
    position: absolute;
    font-size: 15rem;
    opacity: 0.05;
    right: -50px;
    bottom: -50px;
    transform: rotate(15deg);
    animation: neuralPulse 4s ease-in-out infinite;
  }

  .tools-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
  }

  .tools-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
    margin-top: 2rem;
  }

  .tool-badge {
    background: white;
    padding: 0.75rem 1.75rem;
    border-radius: 25px;
    border: 2px solid #8B5CF6;
    font-weight: 600;
    transition: all 0.3s;
    cursor: default;
    box-shadow: 0 4px 12px rgba(139, 92, 246, 0.1);
  }

  .tool-badge:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(139, 92, 246, 0.3);
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    color: white;
    border-color: transparent;
  }

  /* Learning Outcomes - Premium */
  .outcomes-section {
    background: white;
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .outcomes-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 3rem;
  }

  .outcome-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 1200px) {
    .outcome-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .outcome-grid {
      grid-template-columns: 1fr;
    }
  }

  .outcome-item {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 1.5rem;
    border-radius: 15px;
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    transition: all 0.3s;
    border: 2px solid transparent;
  }

  .outcome-item:hover {
    transform: translateX(5px);
    border-color: #8B5CF6;
    background: white;
    box-shadow: 0 10px 20px rgba(139, 92, 246, 0.1);
  }

  .outcome-check {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    font-weight: bold;
  }

  .outcome-text {
    color: #4B5563;
    font-size: 1rem;
    line-height: 1.5;
  }

  /* Course Schedule Section */
  .schedule-section {
    background: white;
    padding: 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .schedule-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 2rem;
  }

  .schedule-calendar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 1200px) {
    .schedule-calendar {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .schedule-calendar {
      grid-template-columns: 1fr;
    }
  }

  .schedule-item {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 1.5rem;
    border-radius: 15px;
    border-left: 4px solid #8B5CF6;
    transition: all 0.3s;
  }

  .schedule-item:nth-child(2) { border-left-color: #EC4899; }
  .schedule-item:nth-child(3) { border-left-color: #3B82F6; }
  .schedule-item:nth-child(4) { border-left-color: #10B981; }

  .schedule-item:hover {
    transform: translateX(5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .schedule-item h3 {
    color: #1F2937;
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }

  .schedule-item p {
    color: #6B7280;
    font-size: 0.95rem;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 25%, #3B82F6 50%, #10B981 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 4rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.4);
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
    margin-bottom: 1.5rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
  }

  .cta-section p {
    color: white !important;
    font-size: 1.3rem;
    margin: 1.5rem 0;
    opacity: 0.95;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .cta-button {
    background: white;
    color: #8B5CF6;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    margin-top: 1.5rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
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
    color: #7C3AED;
  }

  /* Responsive adjustments */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2.5rem;
    }
    
    .section-header h2 {
      font-size: 2rem;
    }
    
    .cta-section h2 {
      font-size: 2rem;
    }

    .competition-section,
    .tools-section,
    .outcomes-section,
    .schedule-section {
      padding: 2rem;
    }
  }
</style>

<div class="course-hero">
  <div class="icons-bg">
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">🔬</span>
    <span class="floating-icon">📊</span>
    <span class="floating-icon">💡</span>
  </div>
  <h1>
    <span class="en-content">AI & Machine Learning Mastery</span>
    <span class="zh-content">人工智能与机器学习精通课程</span>
  </h1>
  <p>
    <span class="en-content">16-Week Comprehensive AI Competition Training Program</span>
    <span class="zh-content">16周综合AI竞赛培训计划</span>
  </p>
  <div class="hero-badge">
    <span class="en-content">🎯 USAAIO + Kaggle + Research Projects</span>
    <span class="zh-content">🎯 USAAIO + Kaggle + 研究项目</span>
  </div>
</div>

<!-- Course Overview -->
<div class="section-header">
  <h2>
    <span class="en-content">Complete AI Curriculum</span>
    <span class="zh-content">完整AI课程体系</span>
  </h2>
  <p>
    <span class="en-content">Progressive training from fundamentals to cutting-edge techniques</span>
    <span class="zh-content">从基础到前沿技术的渐进式培训</span>
  </p>
</div>

<!-- Phase Cards (4-column like USACO) -->
<div class="phase-cards">
  <!-- Foundation Phase -->
  <div class="phase-card phase-foundation">
    <div class="phase-header">
      <div class="phase-icon">📚</div>
      <h3 class="phase-name">
        <span class="en-content">Foundation</span>
        <span class="zh-content">基础阶段</span>
      </h3>
      <p class="phase-subtitle">
        <span class="en-content">Weeks 1-4</span>
        <span class="zh-content">第1-4周</span>
      </p>
    </div>
    <div class="phase-topics">
      <ul>
        <li>
          <span class="en-content">ML Fundamentals & Types</span>
          <span class="zh-content">机器学习基础与类型</span>
        </li>
        <li>
          <span class="en-content">Linear & Logistic Regression</span>
          <span class="zh-content">线性与逻辑回归</span>
        </li>
        <li>
          <span class="en-content">Decision Trees & Forests</span>
          <span class="zh-content">决策树与随机森林</span>
        </li>
        <li>
          <span class="en-content">Model Evaluation Metrics</span>
          <span class="zh-content">模型评估指标</span>
        </li>
        <li>
          <span class="en-content">Cross-validation</span>
          <span class="zh-content">交叉验证</span>
        </li>
        <li>
          <span class="en-content">XGBoost & Ensemble Methods</span>
          <span class="zh-content">XGBoost与集成方法</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Intermediate Phase -->
  <div class="phase-card phase-intermediate">
    <div class="phase-header">
      <div class="phase-icon">⚙️</div>
      <h3 class="phase-name">
        <span class="en-content">Intermediate</span>
        <span class="zh-content">进阶阶段</span>
      </h3>
      <p class="phase-subtitle">
        <span class="en-content">Weeks 5-8</span>
        <span class="zh-content">第5-8周</span>
      </p>
    </div>
    <div class="phase-topics">
      <ul>
        <li>
          <span class="en-content">Feature Engineering</span>
          <span class="zh-content">特征工程</span>
        </li>
        <li>
          <span class="en-content">Dimensionality Reduction (PCA)</span>
          <span class="zh-content">降维（主成分分析）</span>
        </li>
        <li>
          <span class="en-content">Neural Network Basics</span>
          <span class="zh-content">神经网络基础</span>
        </li>
        <li>
          <span class="en-content">Backpropagation</span>
          <span class="zh-content">反向传播</span>
        </li>
        <li>
          <span class="en-content">Optimization Algorithms</span>
          <span class="zh-content">优化算法</span>
        </li>
        <li>
          <span class="en-content">Regularization Techniques</span>
          <span class="zh-content">正则化技术</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Advanced Phase -->
  <div class="phase-card phase-advanced">
    <div class="phase-header">
      <div class="phase-icon">🚀</div>
      <h3 class="phase-name">
        <span class="en-content">Advanced</span>
        <span class="zh-content">高级阶段</span>
      </h3>
      <p class="phase-subtitle">
        <span class="en-content">Weeks 9-12</span>
        <span class="zh-content">第9-12周</span>
      </p>
    </div>
    <div class="phase-topics">
      <ul>
        <li>
          <span class="en-content">CNN for Computer Vision</span>
          <span class="zh-content">CNN计算机视觉</span>
        </li>
        <li>
          <span class="en-content">Transfer Learning</span>
          <span class="zh-content">迁移学习</span>
        </li>
        <li>
          <span class="en-content">Object Detection (YOLO)</span>
          <span class="zh-content">目标检测（YOLO）</span>
        </li>
        <li>
          <span class="en-content">Image Segmentation</span>
          <span class="zh-content">图像分割</span>
        </li>
        <li>
          <span class="en-content">GANs & Style Transfer</span>
          <span class="zh-content">GAN与风格迁移</span>
        </li>
        <li>
          <span class="en-content">Data Augmentation</span>
          <span class="zh-content">数据增强</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Expert Phase -->
  <div class="phase-card phase-expert">
    <div class="phase-header">
      <div class="phase-icon">🏆</div>
      <h3 class="phase-name">
        <span class="en-content">Expert</span>
        <span class="zh-content">专家阶段</span>
      </h3>
      <p class="phase-subtitle">
        <span class="en-content">Weeks 13-16</span>
        <span class="zh-content">第13-16周</span>
      </p>
    </div>
    <div class="phase-topics">
      <ul>
        <li>
          <span class="en-content">RNN, LSTM, GRU</span>
          <span class="zh-content">循环神经网络系列</span>
        </li>
        <li>
          <span class="en-content">Transformers & Attention</span>
          <span class="zh-content">Transformers与注意力</span>
        </li>
        <li>
          <span class="en-content">BERT & GPT Models</span>
          <span class="zh-content">BERT与GPT模型</span>
        </li>
        <li>
          <span class="en-content">NLP Applications</span>
          <span class="zh-content">自然语言处理应用</span>
        </li>
        <li>
          <span class="en-content">Kaggle Winning Strategies</span>
          <span class="zh-content">Kaggle获胜策略</span>
        </li>
        <li>
          <span class="en-content">Competition Tricks</span>
          <span class="zh-content">竞赛技巧</span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- Timeline Section -->
<div class="timeline-section">
  <div class="section-header">
    <h2 style="color: #1F2937;">
      <span class="en-content">Your Learning Journey</span>
      <span class="zh-content">您的学习之旅</span>
    </h2>
    <p>
      <span class="en-content">16 weeks to AI competition mastery</span>
      <span class="zh-content">16周掌握AI竞赛</span>
    </p>
  </div>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-phase">
        <span class="en-content">Foundation</span>
        <span class="zh-content">基础</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">Weeks 1-4</span>
        <span class="zh-content">第1-4周</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-phase">
        <span class="en-content">Intermediate</span>
        <span class="zh-content">进阶</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">Weeks 5-8</span>
        <span class="zh-content">第5-8周</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-phase">
        <span class="en-content">Advanced</span>
        <span class="zh-content">高级</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">Weeks 9-12</span>
        <span class="zh-content">第9-12周</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-phase">
        <span class="en-content">Expert</span>
        <span class="zh-content">专家</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">Weeks 13-16</span>
        <span class="zh-content">第13-16周</span>
      </div>
    </div>
  </div>
</div>

<!-- Competition Preparation -->
<div class="competition-section">
  <h2>
    <span class="en-content">Competition & Research Preparation</span>
    <span class="zh-content">竞赛与研究准备</span>
  </h2>
  
  <div class="competition-grid">
    <div class="competition-card">
      <div class="competition-icon usaaio-icon">AI</div>
      <h4 class="competition-title">USAAIO</h4>
      <p class="competition-desc">
        <span class="en-content">USA AI Olympiad preparation with past winners' strategies</span>
        <span class="zh-content">美国AI奥林匹克准备，包含往届获胜者策略</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon kaggle-icon">K</div>
      <h4 class="competition-title">Kaggle</h4>
      <p class="competition-desc">
        <span class="en-content">Master data science competitions with Grandmaster techniques</span>
        <span class="zh-content">使用大师级技术征服数据科学竞赛</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon research-icon">📄</div>
      <h4 class="competition-title">
        <span class="en-content">Research Papers</span>
        <span class="zh-content">研究论文</span>
      </h4>
      <p class="competition-desc">
        <span class="en-content">Publish in conferences and journals with expert guidance</span>
        <span class="zh-content">在专家指导下发表会议和期刊论文</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon portfolio-icon">💼</div>
      <h4 class="competition-title">
        <span class="en-content">Portfolio Projects</span>
        <span class="zh-content">作品集项目</span>
      </h4>
      <p class="competition-desc">
        <span class="en-content">Build industry-level applications for college applications</span>
        <span class="zh-content">为大学申请构建行业级应用</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stories / Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">Proven Track Record</span>
    <span class="zh-content">卓越成绩</span>
  </h2>
  
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">50+</div>
      <div class="stat-label">
        <span class="en-content">Students Trained</span>
        <span class="zh-content">培训学生</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">85%</div>
      <div class="stat-label">
        <span class="en-content">Competition Success</span>
        <span class="zh-content">竞赛成功率</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">10+</div>
      <div class="stat-label">
        <span class="en-content">Kaggle Medals</span>
        <span class="zh-content">Kaggle奖牌</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">5</div>
      <div class="stat-label">
        <span class="en-content">Research Papers</span>
        <span class="zh-content">研究论文</span>
      </div>
    </div>
  </div>
</div>

<!-- Course Schedule -->
<div class="schedule-section">
  <h2>
    <span class="en-content">2024-2025 Competition Calendar</span>
    <span class="zh-content">2024-2025 竞赛日历</span>
  </h2>
  
  <div class="schedule-calendar">
    <div class="schedule-item">
      <h3>
        <span class="en-content">USAAIO Qualifier</span>
        <span class="zh-content">USAAIO资格赛</span>
      </h3>
      <p>
        <span class="en-content">January 2025</span>
        <span class="zh-content">2025年1月</span>
      </p>
    </div>
    
    <div class="schedule-item">
      <h3>
        <span class="en-content">Kaggle Competitions</span>
        <span class="zh-content">Kaggle竞赛</span>
      </h3>
      <p>
        <span class="en-content">Year-round</span>
        <span class="zh-content">全年进行</span>
      </p>
    </div>
    
    <div class="schedule-item">
      <h3>
        <span class="en-content">USAAIO Finals</span>
        <span class="zh-content">USAAIO决赛</span>
      </h3>
      <p>
        <span class="en-content">April 2025</span>
        <span class="zh-content">2025年4月</span>
      </p>
    </div>
    
    <div class="schedule-item">
      <h3>
        <span class="en-content">Research Deadlines</span>
        <span class="zh-content">论文截止日期</span>
      </h3>
      <p>
        <span class="en-content">Conference-specific</span>
        <span class="zh-content">根据会议而定</span>
      </p>
    </div>
  </div>
</div>

<!-- Learning Outcomes -->
<div class="outcomes-section">
  <h2>
    <span class="en-content">What You'll Achieve</span>
    <span class="zh-content">您将获得的成就</span>
  </h2>
  
  <div class="outcome-grid">
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div class="outcome-text">
        <span class="en-content">Master 10+ ML algorithms and frameworks</span>
        <span class="zh-content">掌握10+机器学习算法和框架</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div class="outcome-text">
        <span class="en-content">Build competition-winning models</span>
        <span class="zh-content">构建竞赛获胜模型</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div class="outcome-text">
        <span class="en-content">Complete 5+ real-world projects</span>
        <span class="zh-content">完成5+实际项目</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div class="outcome-text">
        <span class="en-content">Research paper submission ready</span>
        <span class="zh-content">准备提交研究论文</span>
      </div>
    </div>
  </div>
</div>

<!-- Tools & Technologies -->
<div class="tools-section">
  <h2>
    <span class="en-content">Tools & Technologies You'll Master</span>
    <span class="zh-content">您将掌握的工具与技术</span>
  </h2>
  
  <div class="tools-grid">
    <span class="tool-badge">Python</span>
    <span class="tool-badge">TensorFlow</span>
    <span class="tool-badge">PyTorch</span>
    <span class="tool-badge">Scikit-learn</span>
    <span class="tool-badge">Keras</span>
    <span class="tool-badge">Pandas</span>
    <span class="tool-badge">NumPy</span>
    <span class="tool-badge">OpenCV</span>
    <span class="tool-badge">NLTK</span>
    <span class="tool-badge">Hugging Face</span>
    <span class="tool-badge">Jupyter</span>
    <span class="tool-badge">Google Colab</span>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Join the AI Revolution Today!</span>
    <span class="zh-content">今天就加入AI革命！</span>
  </h2>
  <p>
    <span class="en-content">Limited seats available for personalized mentorship</span>
    <span class="zh-content">个性化指导名额有限</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Start Your AI Journey</span>
    <span class="zh-content">开始您的AI之旅</span>
  </a>
</div>
