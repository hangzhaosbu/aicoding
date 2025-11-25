---
layout: default
title: USACO Training
title_zh: USACO 培训
description: USA Computing Olympiad Competition Preparation
description_zh: 美国计算机奥林匹克竞赛准备
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

  @keyframes slideInLeft {
    from {
      opacity: 0;
      transform: translateX(-30px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  @keyframes slideInRight {
    from {
      opacity: 0;
      transform: translateX(30px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  @keyframes rotateGlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes trophyBounce {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  @keyframes sparkle {
    0%, 100% { opacity: 0; transform: scale(0); }
    50% { opacity: 1; transform: scale(1); }
  }

  @keyframes progressFill {
    from { width: 0; }
    to { width: 100%; }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 25%, #FF6B6B 50%, #4ECDC4 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.4);
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🏆';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: trophyBounce 6s ease-in-out infinite;
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

  /* Floating medals background */
  .course-hero .medals-bg {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    overflow: hidden;
    pointer-events: none;
  }

  .course-hero .medal {
    position: absolute;
    font-size: 3rem;
    opacity: 0.15;
    animation: float 10s ease-in-out infinite;
  }

  .medal:nth-child(1) { left: 5%; top: 15%; animation-delay: 0s; }
  .medal:nth-child(2) { left: 85%; top: 20%; animation-delay: 2s; }
  .medal:nth-child(3) { left: 15%; top: 75%; animation-delay: 4s; }
  .medal:nth-child(4) { left: 75%; top: 70%; animation-delay: 6s; }
  .medal:nth-child(5) { left: 50%; top: 10%; animation-delay: 1s; }
  .medal:nth-child(6) { left: 90%; top: 50%; animation-delay: 3s; }

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
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
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

  /* Level Cards - 2x2 Premium Design */
  .level-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 3rem;
    margin: 4rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .level-cards {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .level-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: flex;
    flex-direction: column;
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
  }

  .level-card:nth-child(1) { animation-delay: 0.1s; }
  .level-card:nth-child(2) { animation-delay: 0.2s; }
  .level-card:nth-child(3) { animation-delay: 0.3s; }
  .level-card:nth-child(4) { animation-delay: 0.4s; }

  .level-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
    animation: shimmer 3s infinite;
  }

  .level-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
  }

  .bronze { 
    border-top: 6px solid #CD7F32;
    background: linear-gradient(to bottom, rgba(205, 127, 50, 0.08) 0%, white 40%);
  }
  
  .bronze:hover {
    box-shadow: 0 30px 60px rgba(205, 127, 50, 0.3);
  }
  
  .silver { 
    border-top: 6px solid #A8A8A8;
    background: linear-gradient(to bottom, rgba(168, 168, 168, 0.08) 0%, white 40%);
  }
  
  .silver:hover {
    box-shadow: 0 30px 60px rgba(168, 168, 168, 0.3);
  }
  
  .gold { 
    border-top: 6px solid #FFD700;
    background: linear-gradient(to bottom, rgba(255, 215, 0, 0.08) 0%, white 40%);
  }
  
  .gold:hover {
    box-shadow: 0 30px 60px rgba(255, 215, 0, 0.4);
  }
  
  .platinum { 
    border-top: 6px solid;
    border-image: linear-gradient(90deg, #E5E4E2, #A0D2DB, #E5E4E2) 1;
    background: linear-gradient(to bottom, rgba(160, 210, 219, 0.1) 0%, white 40%);
  }
  
  .platinum:hover {
    box-shadow: 0 30px 60px rgba(160, 210, 219, 0.3);
  }

  .level-header {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    margin-bottom: 1.5rem;
  }

  .level-icon {
    font-size: 4rem;
    animation: pulse 3s ease-in-out infinite;
  }

  .bronze .level-icon { animation-delay: 0s; }
  .silver .level-icon { animation-delay: 0.5s; }
  .gold .level-icon { animation-delay: 1s; }
  .platinum .level-icon { animation-delay: 1.5s; }

  .level-title-group {
    flex: 1;
  }

  .level-name {
    font-size: 1.6rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .level-subtitle {
    font-size: 1rem;
    font-weight: 500;
    color: #6B7280;
  }

  .level-badge {
    padding: 0.4rem 1rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .bronze .level-badge {
    background: rgba(205, 127, 50, 0.15);
    color: #CD7F32;
  }

  .silver .level-badge {
    background: rgba(168, 168, 168, 0.15);
    color: #808080;
  }

  .gold .level-badge {
    background: rgba(255, 215, 0, 0.15);
    color: #B8860B;
  }

  .platinum .level-badge {
    background: rgba(160, 210, 219, 0.2);
    color: #5F9EA0;
  }

  .level-topics {
    color: #6B7280;
    line-height: 1.7;
    flex-grow: 1;
  }

  .level-topics ul {
    padding-left: 0;
    margin: 0;
    list-style: none;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.5rem 1.5rem;
  }

  @media (max-width: 600px) {
    .level-topics ul {
      grid-template-columns: 1fr;
    }
  }

  .level-topics li {
    font-size: 0.95rem;
    padding-left: 1.5rem;
    position: relative;
    padding-top: 0.3rem;
    padding-bottom: 0.3rem;
  }

  .level-topics li::before {
    content: '→';
    position: absolute;
    left: 0;
    color: #9CA3AF;
    font-weight: bold;
  }

  .bronze .level-topics li::before { color: #CD7F32; }
  .silver .level-topics li::before { color: #A8A8A8; }
  .gold .level-topics li::before { color: #FFD700; }
  .platinum .level-topics li::before { color: #5F9EA0; }

  /* Why Choose Us Section */
  .why-choose-section {
    background: linear-gradient(135deg, #F0F9FF 0%, #E0F2FE 100%);
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
    border-color: #FFD700;
    box-shadow: 0 20px 40px rgba(255, 215, 0, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(255, 165, 0, 0.3);
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

  /* Timeline - Premium Design */
  .timeline-section {
    padding: 4rem 2rem;
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
    max-width: 1100px;
    margin: 3rem auto;
    padding: 0 2rem;
  }

  .timeline::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 5%;
    right: 5%;
    height: 6px;
    background: linear-gradient(90deg, #CD7F32 0%, #A8A8A8 33%, #FFD700 66%, #5F9EA0 100%);
    z-index: 0;
    border-radius: 3px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }

  .timeline-item {
    background: white;
    padding: 1.5rem 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    z-index: 1;
    position: relative;
    text-align: center;
    flex: 1;
    margin: 0 0.75rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 3px solid transparent;
  }

  .timeline-item:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .timeline-item:nth-child(1) { border-color: #CD7F32; }
  .timeline-item:nth-child(2) { border-color: #A8A8A8; }
  .timeline-item:nth-child(3) { border-color: #FFD700; }
  .timeline-item:nth-child(4) { border-color: #5F9EA0; }

  .timeline-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }

  .timeline-level {
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
    font-size: 1.1rem;
  }

  .timeline-duration {
    font-size: 0.85rem;
    color: #6B7280;
    background: #F3F4F6;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    display: inline-block;
  }

  @media (max-width: 900px) {
    .timeline {
      flex-direction: column;
      gap: 2rem;
    }
    
    .timeline::before {
      top: 0;
      bottom: 0;
      left: 50%;
      width: 6px;
      height: 90%;
      transform: translateX(-50%);
    }

    .timeline-item {
      margin: 0;
      width: 80%;
      max-width: 300px;
    }
  }

  /* Training Features - Premium Grid */
  .training-features {
    background: white;
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
  }

  .training-features::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #FFD700, #FFA500, #FF6B6B, #4ECDC4);
  }

  .training-features h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;
    max-width: 1200px;
    margin: 0 auto;
  }

  @media (max-width: 968px) {
    .features-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 640px) {
    .features-grid {
      grid-template-columns: 1fr;
    }
  }

  .feature-item {
    text-align: center;
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 100%);
    padding: 2.5rem;
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
  }

  .feature-item::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 215, 0, 0.1), transparent);
    transition: left 0.5s;
  }

  .feature-item:hover::before {
    left: 100%;
  }

  .feature-item:hover {
    transform: translateY(-8px) scale(1.02);
    box-shadow: 0 20px 40px rgba(255, 165, 0, 0.2);
    border-color: #FFD700;
    background: white;
  }

  .feature-icon {
    font-size: 3.5rem;
    margin-bottom: 1.5rem;
    display: inline-block;
    animation: float 6s ease-in-out infinite;
  }

  .feature-item:nth-child(odd) .feature-icon {
    animation-delay: 0s;
  }

  .feature-item:nth-child(even) .feature-icon {
    animation-delay: 3s;
  }

  .feature-title {
    color: #1F2937;
    font-size: 1.3rem;
    font-weight: 700;
    margin-bottom: 0.8rem;
  }

  .feature-description {
    color: #6B7280;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* Success Stories - Premium Stats */
  .success-section {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 50%, #FF8C00 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.3);
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

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin: 2rem 0;
    position: relative;
    z-index: 1;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
  }

  @media (max-width: 968px) {
    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 480px) {
    .stats-grid {
      grid-template-columns: 1fr;
    }
  }

  .stat-item {
    text-align: center;
    background: white;
    padding: 2rem 1.5rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .stat-item:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .stat-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .stat-number {
    font-size: 3rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FF8C00 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #6B7280;
    font-size: 1rem;
    margin-top: 0.3rem;
    font-weight: 600;
  }

  /* Contest Dates Section */
  .contest-dates {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .contest-dates h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 2rem;
  }

  .contest-calendar {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    margin-top: 2rem;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
  }

  @media (max-width: 1000px) {
    .contest-calendar {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 550px) {
    .contest-calendar {
      grid-template-columns: 1fr;
    }
  }

  .contest-month {
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 100%);
    padding: 1.5rem;
    border-radius: 20px;
    border-left: 5px solid;
    transition: all 0.4s ease;
    position: relative;
    overflow: hidden;
  }

  .contest-month:nth-child(1) { border-left-color: #CD7F32; }
  .contest-month:nth-child(2) { border-left-color: #A8A8A8; }
  .contest-month:nth-child(3) { border-left-color: #FFD700; }
  .contest-month:nth-child(4) { border-left-color: #5F9EA0; }

  .contest-month:hover {
    transform: translateY(-5px) translateX(5px);
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.12);
  }

  .contest-month h3 {
    color: #1F2937;
    font-size: 1.15rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .contest-month p {
    color: #6B7280;
    font-size: 0.95rem;
    font-weight: 500;
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
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
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
    color: #FFD700;
    opacity: 0.3;
    font-family: Georgia, serif;
    line-height: 1;
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
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
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

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    font-size: 0.75rem;
    font-weight: 600;
  }

  .badge-gold {
    background: rgba(255, 215, 0, 0.2);
    color: #B8860B;
  }

  .badge-platinum {
    background: rgba(160, 210, 219, 0.3);
    color: #5F9EA0;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 25%, #FF6B6B 50%, #4ECDC4 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(255, 165, 0, 0.4);
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
    color: #FFA500;
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
    background: linear-gradient(90deg, transparent, rgba(255, 165, 0, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #FF8C00;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #FFA500;
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

    .training-features,
    .success-section,
    .contest-dates {
      padding: 3rem 1.5rem;
    }
  }
</style>

<div class="course-hero">
  <div class="medals-bg">
    <span class="medal">🥉</span>
    <span class="medal">🥈</span>
    <span class="medal">🥇</span>
    <span class="medal">💎</span>
    <span class="medal">⭐</span>
    <span class="medal">🏅</span>
  </div>
  <h1>
    <span class="en-content">USACO Training Program</span>
    <span class="zh-content">USACO 培训计划</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Your Path from Bronze to Platinum & Beyond</span>
    <span class="zh-content">从铜牌到白金的进阶之路</span>
  </p>
  <div class="hero-badge">
    <span>🎯</span>
    <span class="en-content">Elite Competition Training</span>
    <span class="zh-content">精英竞赛培训</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">92%</span>
      <span class="hero-stat-label">
        <span class="en-content">Promotion Rate</span>
        <span class="zh-content">晋级率</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">30+</span>
      <span class="hero-stat-label">
        <span class="en-content">Students</span>
        <span class="zh-content">学生</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">5+</span>
      <span class="hero-stat-label">
        <span class="en-content">Gold & Platinum</span>
        <span class="zh-content">金牌&白金</span>
      </span>
    </div>
  </div>
</div>

<!-- Course Overview -->
<div class="section-header">
  <h2>
    <span class="en-content">Complete Competition Curriculum</span>
    <span class="zh-content">完整竞赛课程体系</span>
  </h2>
  <p>
    <span class="en-content">Progressive training through all USACO divisions with proven results</span>
    <span class="zh-content">通过所有USACO级别的渐进式培训，成果显著</span>
  </p>
</div>

<!-- Level Cards - 2x2 Layout -->
<div class="level-cards">
  <!-- Bronze Level -->
  <div class="level-card bronze">
    <div class="level-header">
      <div class="level-icon">🥉</div>
      <div class="level-title-group">
        <h3 class="level-name">
          <span class="en-content">Bronze Division</span>
          <span class="zh-content">铜牌组</span>
        </h3>
        <p class="level-subtitle">
          <span class="en-content">Foundation Building</span>
          <span class="zh-content">基础构建</span>
        </p>
      </div>
      <span class="level-badge">
        <span class="en-content">Beginner</span>
        <span class="zh-content">入门</span>
      </span>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">USACO Contest Format</span>
          <span class="zh-content">USACO 竞赛格式</span>
        </li>
        <li>
          <span class="en-content">File I/O & Edge Cases</span>
          <span class="zh-content">文件输入输出与边界情况</span>
        </li>
        <li>
          <span class="en-content">Complete Search</span>
          <span class="zh-content">完全搜索</span>
        </li>
        <li>
          <span class="en-content">Greedy Algorithms</span>
          <span class="zh-content">贪心算法</span>
        </li>
        <li>
          <span class="en-content">Ad Hoc Problems</span>
          <span class="zh-content">特殊问题</span>
        </li>
        <li>
          <span class="en-content">Basic Sorting</span>
          <span class="zh-content">基础排序</span>
        </li>
        <li>
          <span class="en-content">Simulation</span>
          <span class="zh-content">模拟</span>
        </li>
        <li>
          <span class="en-content">Rectangle Geometry</span>
          <span class="zh-content">矩形几何</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Silver Level -->
  <div class="level-card silver">
    <div class="level-header">
      <div class="level-icon">🥈</div>
      <div class="level-title-group">
        <h3 class="level-name">
          <span class="en-content">Silver Division</span>
          <span class="zh-content">银牌组</span>
        </h3>
        <p class="level-subtitle">
          <span class="en-content">Core Algorithms</span>
          <span class="zh-content">核心算法</span>
        </p>
      </div>
      <span class="level-badge">
        <span class="en-content">Intermediate</span>
        <span class="zh-content">进阶</span>
      </span>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Graph Traversal (DFS/BFS)</span>
          <span class="zh-content">图遍历（深搜/广搜）</span>
        </li>
        <li>
          <span class="en-content">Flood Fill Algorithms</span>
          <span class="zh-content">洪水填充算法</span>
        </li>
        <li>
          <span class="en-content">Binary Search</span>
          <span class="zh-content">二分搜索</span>
        </li>
        <li>
          <span class="en-content">Two Pointers</span>
          <span class="zh-content">双指针技术</span>
        </li>
        <li>
          <span class="en-content">Prefix Sums</span>
          <span class="zh-content">前缀和</span>
        </li>
        <li>
          <span class="en-content">Custom Sorting</span>
          <span class="zh-content">自定义排序</span>
        </li>
        <li>
          <span class="en-content">Tree Algorithms</span>
          <span class="zh-content">树算法</span>
        </li>
        <li>
          <span class="en-content">Stacks & Queues</span>
          <span class="zh-content">栈与队列</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Gold Level -->
  <div class="level-card gold">
    <div class="level-header">
      <div class="level-icon">🥇</div>
      <div class="level-title-group">
        <h3 class="level-name">
          <span class="en-content">Gold Division</span>
          <span class="zh-content">金牌组</span>
        </h3>
        <p class="level-subtitle">
          <span class="en-content">Advanced Techniques</span>
          <span class="zh-content">高级技术</span>
        </p>
      </div>
      <span class="level-badge">
        <span class="en-content">Advanced</span>
        <span class="zh-content">高级</span>
      </span>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Dynamic Programming</span>
          <span class="zh-content">动态规划</span>
        </li>
        <li>
          <span class="en-content">Dijkstra's Algorithm</span>
          <span class="zh-content">Dijkstra 算法</span>
        </li>
        <li>
          <span class="en-content">Minimum Spanning Tree</span>
          <span class="zh-content">最小生成树</span>
        </li>
        <li>
          <span class="en-content">Disjoint Set Union</span>
          <span class="zh-content">并查集</span>
        </li>
        <li>
          <span class="en-content">Topological Sort</span>
          <span class="zh-content">拓扑排序</span>
        </li>
        <li>
          <span class="en-content">Hashing Techniques</span>
          <span class="zh-content">哈希技术</span>
        </li>
        <li>
          <span class="en-content">Point Update Range Sum</span>
          <span class="zh-content">点更新区间求和</span>
        </li>
        <li>
          <span class="en-content">Euler Tour Technique</span>
          <span class="zh-content">欧拉遍历</span>
        </li>
      </ul>
    </div>
  </div>

  <!-- Platinum Level -->
  <div class="level-card platinum">
    <div class="level-header">
      <div class="level-icon">💎</div>
      <div class="level-title-group">
        <h3 class="level-name">
          <span class="en-content">Platinum Division</span>
          <span class="zh-content">白金组</span>
        </h3>
        <p class="level-subtitle">
          <span class="en-content">Expert Mastery</span>
          <span class="zh-content">专家精通</span>
        </p>
      </div>
      <span class="level-badge">
        <span class="en-content">Expert</span>
        <span class="zh-content">专家</span>
      </span>
    </div>
    <div class="level-topics">
      <ul>
        <li>
          <span class="en-content">Advanced DP & Optimization</span>
          <span class="zh-content">高级动态规划与优化</span>
        </li>
        <li>
          <span class="en-content">Network Flow</span>
          <span class="zh-content">网络流</span>
        </li>
        <li>
          <span class="en-content">Computational Geometry</span>
          <span class="zh-content">计算几何</span>
        </li>
        <li>
          <span class="en-content">Segment Trees</span>
          <span class="zh-content">线段树</span>
        </li>
        <li>
          <span class="en-content">Heavy-Light Decomposition</span>
          <span class="zh-content">树链剖分</span>
        </li>
        <li>
          <span class="en-content">String Algorithms (KMP, Z)</span>
          <span class="zh-content">字符串算法（KMP, Z）</span>
        </li>
        <li>
          <span class="en-content">FFT & Number Theory</span>
          <span class="zh-content">FFT 与数论</span>
        </li>
        <li>
          <span class="en-content">Centroid Decomposition</span>
          <span class="zh-content">点分治</span>
        </li>
      </ul>
    </div>
  </div>
</div>

<!-- Why Choose Us Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Choose Us</span>
      <span class="zh-content">为什么选择我们</span>
    </h2>
    <p>
      <span class="en-content">What sets our USACO training apart</span>
      <span class="zh-content">我们USACO培训的独特优势</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">🎓</div>
      <h3>
        <span class="en-content">Expert Instructors</span>
        <span class="zh-content">专业导师</span>
      </h3>
      <p>
        <span class="en-content">Learn from USACO Finalists with proven competition experience</span>
        <span class="zh-content">向拥有丰富竞赛经验的USACO决赛选手学习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Class Size</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 4 students per class for personalized attention</span>
        <span class="zh-content">每班最多4人，确保个性化关注</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📈</div>
      <h3>
        <span class="en-content">Proven Results</span>
        <span class="zh-content">成绩卓越</span>
      </h3>
      <p>
        <span class="en-content">92% promotion rate with multiple Gold & Platinum achievers</span>
        <span class="zh-content">92%晋级率，多名学生达到金牌和白金</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">Curated Problems</span>
        <span class="zh-content">精选题库</span>
      </h3>
      <p>
        <span class="en-content">1000+ hand-picked problems with detailed solutions</span>
        <span class="zh-content">1000+精选题目配有详细解答</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">💻</div>
      <h3>
        <span class="en-content">Weekly Contests</span>
        <span class="zh-content">每周竞赛</span>
      </h3>
      <p>
        <span class="en-content">Simulated USACO contests to build real competition skills</span>
        <span class="zh-content">模拟USACO竞赛，培养实战能力</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Strategic Coaching</span>
        <span class="zh-content">策略指导</span>
      </h3>
      <p>
        <span class="en-content">Contest tactics, time management, and problem-solving strategies</span>
        <span class="zh-content">竞赛策略、时间管理和解题思路</span>
      </p>
    </div>
  </div>
</div>

<!-- Timeline Section -->
<div class="timeline-section">
  <div class="section-header" style="margin-top: 0;">
    <h2 style="color: #1F2937; background: none; -webkit-text-fill-color: #1F2937;">
      <span class="en-content">Your Journey to Success</span>
      <span class="zh-content">您的成功之路</span>
    </h2>
    <p>
      <span class="en-content">Typical progression timeline with dedicated practice</span>
      <span class="zh-content">通过专注练习的典型进阶时间线</span>
    </p>
  </div>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-icon">🥉</div>
      <div class="timeline-level">
        <span class="en-content">Bronze</span>
        <span class="zh-content">铜牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">3-6 months</span>
        <span class="zh-content">3-6个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-icon">🥈</div>
      <div class="timeline-level">
        <span class="en-content">Silver</span>
        <span class="zh-content">银牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">6-12 months</span>
        <span class="zh-content">6-12个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-icon">🥇</div>
      <div class="timeline-level">
        <span class="en-content">Gold</span>
        <span class="zh-content">金牌</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">12-18 months</span>
        <span class="zh-content">12-18个月</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-icon">💎</div>
      <div class="timeline-level">
        <span class="en-content">Platinum</span>
        <span class="zh-content">白金</span>
      </div>
      <div class="timeline-duration">
        <span class="en-content">18+ months</span>
        <span class="zh-content">18个月+</span>
      </div>
    </div>
  </div>
</div>

<!-- Contest Dates -->
<div class="contest-dates">
  <h2>
    <span class="en-content">2024-2025 Contest Schedule</span>
    <span class="zh-content">2024-2025 竞赛日程</span>
  </h2>
  
  <div class="contest-calendar">
    <div class="contest-month">
      <h3>
        <span>📅</span>
        <span class="en-content">December Contest</span>
        <span class="zh-content">12月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Dec 20-23, 2024</span>
        <span class="zh-content">2024年12月20-23日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span>📅</span>
        <span class="en-content">January Contest</span>
        <span class="zh-content">1月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Jan 24-27, 2025</span>
        <span class="zh-content">2025年1月24-27日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span>📅</span>
        <span class="en-content">February Contest</span>
        <span class="zh-content">2月竞赛</span>
      </h3>
      <p>
        <span class="en-content">Feb 21-24, 2025</span>
        <span class="zh-content">2025年2月21-24日</span>
      </p>
    </div>
    
    <div class="contest-month">
      <h3>
        <span>🏆</span>
        <span class="en-content">US Open</span>
        <span class="zh-content">美国公开赛</span>
      </h3>
      <p>
        <span class="en-content">March 14-17, 2025</span>
        <span class="zh-content">2025年3月14-17日</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stories -->
<div class="success-section">
  <h2>
    <span class="en-content">Proven Track Record</span>
    <span class="zh-content">卓越成绩</span>
  </h2>
  
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-icon">👨‍🎓</div>
      <div class="stat-number">30+</div>
      <div class="stat-label">
        <span class="en-content">Students Trained</span>
        <span class="zh-content">培训学生</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">📈</div>
      <div class="stat-number">92%</div>
      <div class="stat-label">
        <span class="en-content">Promotion Rate</span>
        <span class="zh-content">晋级率</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">🥇</div>
      <div class="stat-number">5+</div>
      <div class="stat-label">
        <span class="en-content">Gold & Above</span>
        <span class="zh-content">金牌及以上</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">💎</div>
      <div class="stat-number">2</div>
      <div class="stat-label">
        <span class="en-content">Platinum Students</span>
        <span class="zh-content">白金学生</span>
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
      <span class="testimonial-badge badge-gold">
        <span class="en-content">Gold</span>
        <span class="zh-content">金牌</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The structured curriculum and weekly contests helped me progress from Silver to Gold in just 6 months. The problem-solving strategies I learned here were game-changers.</span>
        <span class="zh-content">结构化的课程和每周竞赛帮助我在短短6个月内从银牌晋升到金牌。我在这里学到的解题策略非常关键。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Kevin L.</h4>
          <p>
            <span class="en-content">Junior, Silver → Gold</span>
            <span class="zh-content">高中生，银牌→金牌</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-platinum">
        <span class="en-content">Platinum</span>
        <span class="zh-content">白金</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The small class size meant I got personalized attention on my weak areas. My instructor's experience in competitions made all the difference.</span>
        <span class="zh-content">小班教学意味着我在薄弱环节得到了个性化关注。导师的竞赛经验对我帮助很大。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍💻</div>
        <div class="testimonial-info">
          <h4>Sarah W.</h4>
          <p>
            <span class="en-content">Senior, Gold → Platinum</span>
            <span class="zh-content">高中生，金牌→白金</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge badge-gold">
        <span class="en-content">Gold</span>
        <span class="zh-content">金牌</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">Started with zero competitive programming experience. The Bronze course built my foundation perfectly, and I reached Gold within a year!</span>
        <span class="zh-content">从零竞赛编程经验开始。铜牌课程为我打下了完美的基础，一年内我就达到了金牌！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Michael C.</h4>
          <p>
            <span class="en-content">Sophomore, Bronze → Gold</span>
            <span class="zh-content">高中生，铜牌→金牌</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Your USACO Journey Today!</span>
    <span class="zh-content">今天开始您的USACO之旅！</span>
  </h2>
  <p>
    <span class="en-content">Join the ranks of our Gold and Platinum achievers</span>
    <span class="zh-content">加入我们金牌和白金获得者的行列</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-button">
      <span class="en-content">🚀 Begin Training Now</span>
      <span class="zh-content">🚀 立即开始培训</span>
    </a>
    <a href="./contact.html" class="cta-button cta-button-secondary">
      <span class="en-content">📅 Schedule Consultation</span>
      <span class="zh-content">📅 预约咨询</span>
    </a>
  </div>
</div>
