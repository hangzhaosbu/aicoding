---
layout: default
title: USA AI Olympiad (USAAIO) Training
title_zh: 美国人工智能奥林匹克竞赛培训
description: Master AI & Represent Team USA at International AI Olympiads
description_zh: 掌握人工智能，代表美国队参加国际AI奥林匹克
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

  @keyframes neuralPulse {
    0%, 100% { 
      box-shadow: 0 0 30px rgba(6, 182, 212, 0.4);
    }
    50% { 
      box-shadow: 0 0 60px rgba(6, 182, 212, 0.8);
    }
  }

  @keyframes dataFlow {
    0% { background-position: 0% 0%; }
    100% { background-position: 100% 100%; }
  }

  /* Course Hero - Ultra Premium Cyan/Blue AI Theme */
  .course-hero {
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 25%, #22D3EE 50%, #0E7490 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.4);
    min-height: 480px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '🤖';
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

  .olympiad-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 700;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(245, 158, 11, 0.4);
    animation: pulse 2s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .olympiad-badge::before {
    content: '🏅';
  }

  .course-hero h1 {
    color: white !important;
    font-size: 3.8rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out;
  }

  .course-hero .hero-subtitle {
    color: white !important;
    font-size: 1.4rem;
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
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .section-header p {
    color: #6B7280;
    font-size: 1.2rem;
    max-width: 700px;
    margin: 0 auto;
  }

  /* What is USAAIO Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #0891B2, #06B6D4, #22D3EE) 1;
  }

  .intro-section::before {
    content: '🧠';
    position: absolute;
    font-size: 10rem;
    opacity: 0.03;
    right: -20px;
    bottom: -20px;
  }

  .intro-content {
    display: grid;
    grid-template-columns: 1.2fr 0.8fr;
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
    font-size: 1.05rem;
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
    background: linear-gradient(135deg, #ECFEFF 0%, #CFFAFE 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(6, 182, 212, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Competition Structure Section */
  .structure-section {
    background: linear-gradient(135deg, #ECFEFF 0%, #CFFAFE 50%, #A5F3FC 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .structure-section::before {
    content: '🏆';
    position: absolute;
    font-size: 12rem;
    opacity: 0.05;
    right: -30px;
    bottom: -30px;
  }

  .structure-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #0E7490;
    margin-bottom: 3rem;
  }

  .structure-timeline {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 0;
    max-width: 1100px;
    margin: 0 auto;
    position: relative;
  }

  .structure-timeline::before {
    content: '';
    position: absolute;
    top: 60px;
    left: 10%;
    right: 10%;
    height: 6px;
    background: linear-gradient(90deg, #0891B2, #06B6D4, #22D3EE, #67E8F9);
    border-radius: 3px;
    z-index: 0;
  }

  @media (max-width: 900px) {
    .structure-timeline {
      flex-direction: column;
      align-items: center;
      gap: 2rem;
    }

    .structure-timeline::before {
      display: none;
    }
  }

  .structure-item {
    flex: 1;
    text-align: center;
    position: relative;
    z-index: 1;
    max-width: 280px;
  }

  .structure-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 1.5rem;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.5rem;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
    position: relative;
    animation: neuralPulse 3s ease-in-out infinite;
  }

  .structure-item:nth-child(1) .structure-icon { 
    background: linear-gradient(135deg, #0891B2, #0E7490);
    animation-delay: 0s;
  }
  .structure-item:nth-child(2) .structure-icon { 
    background: linear-gradient(135deg, #06B6D4, #0891B2);
    animation-delay: 0.5s;
  }
  .structure-item:nth-child(3) .structure-icon { 
    background: linear-gradient(135deg, #22D3EE, #06B6D4);
    animation-delay: 1s;
  }
  .structure-item:nth-child(4) .structure-icon { 
    background: linear-gradient(135deg, #F59E0B, #D97706);
    animation-delay: 1.5s;
  }

  .structure-content {
    background: white;
    padding: 1.5rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  }

  .structure-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .structure-date {
    font-size: 0.9rem;
    color: #0891B2;
    font-weight: 600;
    margin-bottom: 0.5rem;
  }

  .structure-location {
    font-size: 0.85rem;
    color: #6B7280;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.3rem;
  }

  .structure-desc {
    font-size: 0.85rem;
    color: #4B5563;
    margin-top: 0.5rem;
    line-height: 1.5;
  }

  /* Syllabus Cards - 2x2 Layout */
  .syllabus-section {
    padding: 2rem 0;
  }

  .syllabus-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .syllabus-grid {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .syllabus-card {
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

  .syllabus-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-left-color: #0891B2;
    background: linear-gradient(to right, rgba(8, 145, 178, 0.03) 0%, white 30%);
  }
  .syllabus-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #8B5CF6;
    background: linear-gradient(to right, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }
  .syllabus-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-left-color: #10B981;
    background: linear-gradient(to right, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }
  .syllabus-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-left-color: #F59E0B;
    background: linear-gradient(to right, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }
  .syllabus-card:nth-child(5) { 
    animation-delay: 0.3s; 
    border-left-color: #EC4899;
    background: linear-gradient(to right, rgba(236, 72, 153, 0.03) 0%, white 30%);
  }
  .syllabus-card:nth-child(6) { 
    animation-delay: 0.35s; 
    border-left-color: #EF4444;
    background: linear-gradient(to right, rgba(239, 68, 68, 0.03) 0%, white 30%);
  }

  .syllabus-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(6, 182, 212, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .syllabus-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.15);
  }

  .syllabus-header {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }

  .syllabus-icon {
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

  .syllabus-card:nth-child(1) .syllabus-icon { background: linear-gradient(135deg, #0891B2, #0E7490); }
  .syllabus-card:nth-child(2) .syllabus-icon { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .syllabus-card:nth-child(3) .syllabus-icon { background: linear-gradient(135deg, #10B981, #059669); }
  .syllabus-card:nth-child(4) .syllabus-icon { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .syllabus-card:nth-child(5) .syllabus-icon { background: linear-gradient(135deg, #EC4899, #DB2777); }
  .syllabus-card:nth-child(6) .syllabus-icon { background: linear-gradient(135deg, #EF4444, #DC2626); }

  .syllabus-title-group {
    flex: 1;
  }

  .syllabus-title {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .syllabus-badge {
    display: inline-block;
    padding: 0.25rem 0.8rem;
    border-radius: 15px;
    font-size: 0.75rem;
    font-weight: 600;
  }

  .syllabus-card:nth-child(1) .syllabus-badge { background: #ECFEFF; color: #0891B2; }
  .syllabus-card:nth-child(2) .syllabus-badge { background: #F5F3FF; color: #8B5CF6; }
  .syllabus-card:nth-child(3) .syllabus-badge { background: #ECFDF5; color: #10B981; }
  .syllabus-card:nth-child(4) .syllabus-badge { background: #FFFBEB; color: #F59E0B; }
  .syllabus-card:nth-child(5) .syllabus-badge { background: #FDF2F8; color: #EC4899; }
  .syllabus-card:nth-child(6) .syllabus-badge { background: #FEF2F2; color: #EF4444; }

  .syllabus-topics {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.4rem 1.5rem;
  }

  @media (max-width: 600px) {
    .syllabus-topics {
      grid-template-columns: 1fr;
    }
  }

  .syllabus-topics li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
  }

  .syllabus-topics li::before {
    content: '→';
    font-weight: bold;
    margin-right: 0.6rem;
    flex-shrink: 0;
  }

  .syllabus-card:nth-child(1) .syllabus-topics li::before { color: #0891B2; }
  .syllabus-card:nth-child(2) .syllabus-topics li::before { color: #8B5CF6; }
  .syllabus-card:nth-child(3) .syllabus-topics li::before { color: #10B981; }
  .syllabus-card:nth-child(4) .syllabus-topics li::before { color: #F59E0B; }
  .syllabus-card:nth-child(5) .syllabus-topics li::before { color: #EC4899; }
  .syllabus-card:nth-child(6) .syllabus-topics li::before { color: #EF4444; }

  /* Team USA Achievements Section */
  .achievements-section {
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 50%, #0E7490 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.3);
  }

  .achievements-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .achievements-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .achievements-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .achievements-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .achievements-grid {
      grid-template-columns: 1fr;
      max-width: 500px;
    }
  }

  .achievement-card {
    background: white;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .achievement-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25);
  }

  .achievement-header {
    padding: 1.5rem;
    text-align: center;
  }

  .achievement-card:nth-child(1) .achievement-header {
    background: linear-gradient(135deg, #FFD700, #FFA500);
  }
  .achievement-card:nth-child(2) .achievement-header {
    background: linear-gradient(135deg, #C0C0C0, #A8A8A8);
  }
  .achievement-card:nth-child(3) .achievement-header {
    background: linear-gradient(135deg, #CD7F32, #B87333);
  }

  .achievement-year {
    font-size: 0.9rem;
    font-weight: 600;
    color: rgba(255, 255, 255, 0.9);
    margin-bottom: 0.3rem;
  }

  .achievement-title {
    font-size: 1.3rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
  }

  .achievement-body {
    padding: 1.5rem;
  }

  .achievement-medals {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
  }

  .medal-badge {
    padding: 0.4rem 0.8rem;
    border-radius: 15px;
    font-size: 0.85rem;
    font-weight: 600;
    display: flex;
    align-items: center;
    gap: 0.3rem;
  }

  .medal-gold { background: #FEF3C7; color: #D97706; }
  .medal-silver { background: #F3F4F6; color: #6B7280; }
  .medal-bronze { background: #FED7AA; color: #C2410C; }
  .medal-hm { background: #E0E7FF; color: #4F46E5; }

  .achievement-desc {
    color: #6B7280;
    font-size: 0.9rem;
    line-height: 1.6;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #ECFEFF 0%, #CFFAFE 100%);
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
    border-color: #06B6D4;
    box-shadow: 0 20px 40px rgba(6, 182, 212, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #06B6D4 0%, #0891B2 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(6, 182, 212, 0.3);
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

  /* Stats Section */
  .stats-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .stats-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .stats-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .stats-grid {
      grid-template-columns: 1fr;
    }
  }

  .stat-item {
    text-align: center;
    padding: 2rem;
    background: linear-gradient(135deg, #ECFEFF 0%, #CFFAFE 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .stat-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(6, 182, 212, 0.15);
  }

  .stat-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .stat-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
    animation: pulse 3s ease-in-out infinite;
  }

  .stat-label {
    color: #6B7280;
    font-size: 0.95rem;
    font-weight: 600;
    margin-top: 0.3rem;
  }

  /* College Placements Section */
  .placements-section {
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 50%, #22D3EE 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.3);
  }

  .placements-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .placements-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .placements-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .placements-grid {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
    position: relative;
    z-index: 1;
  }

  .placement-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    min-width: 180px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s ease;
  }

  .placement-card:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .placement-logo {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .placement-name {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .placement-count {
    font-size: 2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .placement-label {
    font-size: 0.85rem;
    color: #6B7280;
  }

  /* Sponsors Section */
  .sponsors-section {
    background: white;
    padding: 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    text-align: center;
  }

  .sponsors-section h3 {
    font-size: 1.5rem;
    font-weight: 700;
    color: #6B7280;
    margin-bottom: 2rem;
  }

  .sponsors-grid {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 3rem;
    flex-wrap: wrap;
  }

  .sponsor-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
    padding: 1.5rem;
    background: #F9FAFB;
    border-radius: 15px;
    transition: all 0.3s ease;
    min-width: 140px;
  }

  .sponsor-item:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .sponsor-icon {
    font-size: 2.5rem;
  }

  .sponsor-name {
    font-weight: 600;
    color: #4B5563;
    font-size: 0.9rem;
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #ECFEFF 0%, #CFFAFE 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 100%);
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
    color: #06B6D4;
    opacity: 0.2;
    font-family: Georgia, serif;
    line-height: 1;
  }

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    background: linear-gradient(135deg, #06B6D4 0%, #0891B2 100%);
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
    background: linear-gradient(135deg, #06B6D4 0%, #0891B2 100%);
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
    background: linear-gradient(135deg, #0891B2 0%, #06B6D4 25%, #22D3EE 50%, #0E7490 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(6, 182, 212, 0.4);
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
    color: #0891B2;
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
    background: linear-gradient(90deg, transparent, rgba(6, 182, 212, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #0E7490;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #0891B2;
  }

  /* Responsive adjustments */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2.3rem;
    }

    .course-hero .hero-subtitle {
      font-size: 1.1rem;
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
    .structure-section,
    .why-choose-section,
    .stats-section,
    .achievements-section,
    .placements-section {
      padding: 3rem 1.5rem;
    }

    .olympiad-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="olympiad-badge">
    <span class="en-content">OLYMPIAD</span>
    <span class="zh-content">奥林匹克竞赛</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">🤖</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">📊</span>
    <span class="floating-icon">🔬</span>
    <span class="floating-icon">💡</span>
    <span class="floating-icon">⚡</span>
    <span class="floating-icon">🎯</span>
  </div>
  <h1>
    <span class="en-content">USA AI Olympiad (USAAIO)</span>
    <span class="zh-content">美国人工智能奥林匹克竞赛</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Train for USA-NA-AIO & Represent Team USA at IOAI</span>
    <span class="zh-content">备战USA-NA-AIO，代表美国队参加国际AI奥林匹克</span>
  </p>
  <div class="hero-badge">
    <span>🏅</span>
    <span class="en-content">K-12 Students • U.S. & Canada</span>
    <span class="zh-content">K-12学生 · 美国与加拿大</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">7</span>
      <span class="hero-stat-label">
        <span class="en-content">2025 IOAI Medals</span>
        <span class="zh-content">2025 IOAI奖牌</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">MIT</span>
      <span class="hero-stat-label">
        <span class="en-content">Round 2 & Camp</span>
        <span class="zh-content">第二轮与训练营</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">10</span>
      <span class="hero-stat-label">
        <span class="en-content">Team USA at Top Schools</span>
        <span class="zh-content">顶尖名校录取</span>
      </span>
    </div>
  </div>
</div>

<!-- What is USAAIO -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is USAAIO?</span>
        <span class="zh-content">什么是USAAIO？</span>
      </h2>
      <p>
        <span class="en-content">
          USAAIO (USA AI Olympiad) organizes the USA-North America AI Olympiad (USA-NA-AIO) for K-12 students 
          in the United States and Canada. By organizing Team USA for the IOAI and IAIO, USAAIO enables the 
          United States to be a founding country of these two prestigious international AI Olympiads.
        </span>
        <span class="zh-content">
          USAAIO（美国人工智能奥林匹克）为美国和加拿大的K-12学生组织USA-NA-AIO竞赛。通过组织美国队参加IOAI和IAIO，
          USAAIO使美国成为这两项著名国际AI奥林匹克的创始国。
        </span>
      </p>
      <p>
        <span class="en-content">
          AI Olympiad is neither a pure math Olympiad nor a pure coding Olympiad. To excel, you need strong 
          skills in both mathematical theory and programming implementation. Our training prepares you for both!
        </span>
        <span class="zh-content">
          AI奥林匹克既不是纯数学奥林匹克，也不是纯编程奥林匹克。要想出色表现，你需要在数学理论和编程实现方面都具备扎实的技能。
          我们的培训让你两者兼备！
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎯</span>
          <span class="intro-highlight-text">
            <span class="en-content">Theory + Coding</span>
            <span class="zh-content">理论+编程</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏛️</span>
          <span class="intro-highlight-text">
            <span class="en-content">MIT Partnership</span>
            <span class="zh-content">MIT合作</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌐</span>
          <span class="intro-highlight-text">
            <span class="en-content">International Path</span>
            <span class="zh-content">国际赛道</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">☁️</span>
          <span class="intro-highlight-text">
            <span class="en-content">Google Colab Pro+</span>
            <span class="zh-content">Google Colab Pro+</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 10rem; opacity: 0.8; animation: float 6s ease-in-out infinite;">🤖</div>
    </div>
  </div>
</div>

<!-- Competition Structure -->
<div class="structure-section">
  <h2>
    <span class="en-content">🏆 2026 Competition Structure</span>
    <span class="zh-content">🏆 2026年竞赛结构</span>
  </h2>
  
  <div class="structure-timeline">
    <div class="structure-item">
      <div class="structure-icon">1️⃣</div>
      <div class="structure-content">
        <h3 class="structure-title">
          <span class="en-content">Round 1</span>
          <span class="zh-content">第一轮</span>
        </h3>
        <p class="structure-date">
          <span class="en-content">January 30, 2026</span>
          <span class="zh-content">2026年1月30日</span>
        </p>
        <p class="structure-location">
          📍 <span class="en-content">Schools / Test Sites</span>
          <span class="zh-content">学校/考点</span>
        </p>
        <p class="structure-desc">
          <span class="en-content">3 hours • CPU only • Open to all</span>
          <span class="zh-content">3小时 · 仅CPU · 开放报名</span>
        </p>
      </div>
    </div>
    
    <div class="structure-item">
      <div class="structure-icon">2️⃣</div>
      <div class="structure-content">
        <h3 class="structure-title">
          <span class="en-content">Round 2</span>
          <span class="zh-content">第二轮</span>
        </h3>
        <p class="structure-date">
          <span class="en-content">March/April 2026</span>
          <span class="zh-content">2026年3-4月</span>
        </p>
        <p class="structure-location">
          📍 <span class="en-content">MIT Campus</span>
          <span class="zh-content">MIT校园</span>
        </p>
        <p class="structure-desc">
          <span class="en-content">Full syllabus • GPU (L4) enabled</span>
          <span class="zh-content">完整大纲 · GPU (L4)可用</span>
        </p>
      </div>
    </div>
    
    <div class="structure-item">
      <div class="structure-icon">🏕️</div>
      <div class="structure-content">
        <h3 class="structure-title">
          <span class="en-content">USAAIO Camp</span>
          <span class="zh-content">USAAIO训练营</span>
        </h3>
        <p class="structure-date">
          <span class="en-content">June 2026</span>
          <span class="zh-content">2026年6月</span>
        </p>
        <p class="structure-location">
          📍 <span class="en-content">MIT Campus</span>
          <span class="zh-content">MIT校园</span>
        </p>
        <p class="structure-desc">
          <span class="en-content">Team USA selection training</span>
          <span class="zh-content">美国队选拔训练</span>
        </p>
      </div>
    </div>
    
    <div class="structure-item">
      <div class="structure-icon">🌐</div>
      <div class="structure-content">
        <h3 class="structure-title">
          <span class="en-content">IOAI</span>
          <span class="zh-content">国际AI奥赛</span>
        </h3>
        <p class="structure-date">
          <span class="en-content">August 2026</span>
          <span class="zh-content">2026年8月</span>
        </p>
        <p class="structure-location">
          📍 <span class="en-content">International</span>
          <span class="zh-content">国际赛场</span>
        </p>
        <p class="structure-desc">
          <span class="en-content">Represent Team USA!</span>
          <span class="zh-content">代表美国队！</span>
        </p>
      </div>
    </div>
  </div>
</div>

<!-- Syllabus Section -->
<div class="syllabus-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Official USAAIO Syllabus</span>
      <span class="zh-content">官方USAAIO考纲</span>
    </h2>
    <p>
      <span class="en-content">Master both theory and programming for competition success</span>
      <span class="zh-content">掌握理论与编程，征服AI奥林匹克</span>
    </p>
  </div>

  <div class="syllabus-grid">
    <!-- Mathematical Foundations -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">📐</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">Mathematical Foundations</span>
            <span class="zh-content">数学基础</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 1 & 2</span>
            <span class="zh-content">第1-2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Linear Algebra (matrices, eigenvalues)</span><span class="zh-content">线性代数（矩阵、特征值）</span></li>
        <li><span class="en-content">Probability & Statistics (Bayes' rule)</span><span class="zh-content">概率统计（贝叶斯法则）</span></li>
        <li><span class="en-content">Multi-variable Calculus</span><span class="zh-content">多元微积分</span></li>
        <li><span class="en-content">Convex Optimization</span><span class="zh-content">凸优化</span></li>
        <li><span class="en-content">Gradient Descent Algorithm</span><span class="zh-content">梯度下降算法</span></li>
        <li><span class="en-content">Hoeffding's Inequality</span><span class="zh-content">Hoeffding不等式</span></li>
      </ul>
    </div>

    <!-- Basic Coding -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">💻</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">Python & Data Libraries</span>
            <span class="zh-content">Python与数据库</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 1 & 2</span>
            <span class="zh-content">第1-2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Python Programming</span><span class="zh-content">Python编程</span></li>
        <li><span class="en-content">NumPy (numerical computing)</span><span class="zh-content">NumPy（数值计算）</span></li>
        <li><span class="en-content">pandas (data manipulation)</span><span class="zh-content">pandas（数据处理）</span></li>
        <li><span class="en-content">matplotlib & seaborn</span><span class="zh-content">matplotlib与seaborn</span></li>
        <li><span class="en-content">scikit-learn (ML library)</span><span class="zh-content">scikit-learn（机器学习库）</span></li>
        <li><span class="en-content">Google Colab & Markdown</span><span class="zh-content">Google Colab与Markdown</span></li>
      </ul>
    </div>

    <!-- Machine Learning -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">🤖</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">Machine Learning</span>
            <span class="zh-content">机器学习</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 1 & 2</span>
            <span class="zh-content">第1-2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Linear & Logistic Regression</span><span class="zh-content">线性与逻辑回归</span></li>
        <li><span class="en-content">Support Vector Machines</span><span class="zh-content">支持向量机</span></li>
        <li><span class="en-content">Decision Trees & kNN</span><span class="zh-content">决策树与kNN</span></li>
        <li><span class="en-content">Ensemble Learning</span><span class="zh-content">集成学习</span></li>
        <li><span class="en-content">K-means & PCA</span><span class="zh-content">K-means与PCA</span></li>
        <li><span class="en-content">Cross-validation & Loss Functions</span><span class="zh-content">交叉验证与损失函数</span></li>
      </ul>
    </div>

    <!-- Deep Learning Foundation -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">🧠</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">Deep Learning & PyTorch</span>
            <span class="zh-content">深度学习与PyTorch</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 1 & 2</span>
            <span class="zh-content">第1-2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Multi-layer Perceptron (MLP)</span><span class="zh-content">多层感知机</span></li>
        <li><span class="en-content">Forward & Backpropagation</span><span class="zh-content">前向与反向传播</span></li>
        <li><span class="en-content">Batch Normalization & Dropout</span><span class="zh-content">批归一化与Dropout</span></li>
        <li><span class="en-content">PyTorch Framework</span><span class="zh-content">PyTorch框架</span></li>
        <li><span class="en-content">CNN Basics</span><span class="zh-content">CNN基础</span></li>
        <li><span class="en-content">Hand Computation (by paper)</span><span class="zh-content">手工计算（纸上推导）</span></li>
      </ul>
    </div>

    <!-- Transformers & NLP -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">🔤</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">Transformers & NLP</span>
            <span class="zh-content">Transformers与NLP</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 2 Only</span>
            <span class="zh-content">仅第2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Attention Mechanisms</span><span class="zh-content">注意力机制</span></li>
        <li><span class="en-content">Transformer Architecture</span><span class="zh-content">Transformer架构</span></li>
        <li><span class="en-content">Tokenization & Embeddings</span><span class="zh-content">分词与嵌入</span></li>
        <li><span class="en-content">Pre-training & Fine-tuning</span><span class="zh-content">预训练与微调</span></li>
        <li><span class="en-content">Vision Transformers (ViT)</span><span class="zh-content">视觉Transformer</span></li>
        <li><span class="en-content">Graph Neural Networks</span><span class="zh-content">图神经网络</span></li>
      </ul>
    </div>

    <!-- Computer Vision & Generative AI -->
    <div class="syllabus-card">
      <div class="syllabus-header">
        <div class="syllabus-icon">🎨</div>
        <div class="syllabus-title-group">
          <h3 class="syllabus-title">
            <span class="en-content">CV & Generative AI</span>
            <span class="zh-content">计算机视觉与生成式AI</span>
          </h3>
          <span class="syllabus-badge">
            <span class="en-content">Round 2 Only</span>
            <span class="zh-content">仅第2轮</span>
          </span>
        </div>
      </div>
      <ul class="syllabus-topics">
        <li><span class="en-content">Object Detection & UNet</span><span class="zh-content">目标检测与UNet</span></li>
        <li><span class="en-content">Autoencoder & VAE</span><span class="zh-content">自编码器与VAE</span></li>
        <li><span class="en-content">Generative Adversarial Networks</span><span class="zh-content">生成对抗网络</span></li>
        <li><span class="en-content">Diffusion Models (DDPM)</span><span class="zh-content">扩散模型</span></li>
        <li><span class="en-content">Stable Diffusion</span><span class="zh-content">Stable Diffusion</span></li>
        <li><span class="en-content">Theory + Implementation</span><span class="zh-content">理论+实现</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Team USA Achievements -->
<div class="achievements-section">
  <h2>
    <span class="en-content">🏅 Team USA Achievements</span>
    <span class="zh-content">🏅 美国队荣誉</span>
  </h2>
  <p>
    <span class="en-content">Outstanding results at International AI Olympiads</span>
    <span class="zh-content">国际AI奥林匹克的卓越成绩</span>
  </p>
  
  <div class="achievements-grid">
    <div class="achievement-card">
      <div class="achievement-header">
        <p class="achievement-year">2025</p>
        <h3 class="achievement-title">IOAI Beijing 🇨🇳</h3>
      </div>
      <div class="achievement-body">
        <div class="achievement-medals">
          <span class="medal-badge medal-silver">🥈 3 Silver</span>
          <span class="medal-badge medal-bronze">🥉 3 Bronze</span>
          <span class="medal-badge medal-hm">📜 1 HM</span>
        </div>
        <p class="achievement-desc">
          <span class="en-content">Pranav Sambhu, Lily Shi, William Wang (Silver) • Mahith Gottipati, Robert Joo, Bryan Zhu (Bronze)</span>
          <span class="zh-content">银牌: Pranav Sambhu, Lily Shi, William Wang • 铜牌: Mahith Gottipati, Robert Joo, Bryan Zhu</span>
        </p>
      </div>
    </div>
    
    <div class="achievement-card">
      <div class="achievement-header">
        <p class="achievement-year">2024</p>
        <h3 class="achievement-title">IOAI Bulgaria 🇧🇬</h3>
      </div>
      <div class="achievement-body">
        <div class="achievement-medals">
          <span class="medal-badge medal-gold">🥇 4 Gold</span>
          <span class="medal-badge medal-bronze">🥉 4 Bronze</span>
        </div>
        <p class="achievement-desc">
          <span class="en-content">Team 1 (Gold): Sarang Goel, Christina Lee, Videet Mehta, Angelina Quan</span>
          <span class="zh-content">第一队（金牌）: Sarang Goel, Christina Lee, Videet Mehta, Angelina Quan</span>
        </p>
      </div>
    </div>
    
    <div class="achievement-card">
      <div class="achievement-header">
        <p class="achievement-year">2024</p>
        <h3 class="achievement-title">IAIO Saudi Arabia 🇸🇦</h3>
      </div>
      <div class="achievement-body">
        <div class="achievement-medals">
          <span class="medal-badge medal-bronze">🥉 2 Bronze</span>
        </div>
        <p class="achievement-desc">
          <span class="en-content">Ronok Ghosal and Kevin Peng earned Bronze medals at the inaugural IAIO competition.</span>
          <span class="zh-content">Ronok Ghosal和Kevin Peng在首届IAIO竞赛中获得铜牌。</span>
        </p>
      </div>
    </div>
  </div>
</div>

<!-- 2025 Competition Stats -->
<div class="stats-section">
  <h2>
    <span class="en-content">📊 2025 USA-NA-AIO Statistics</span>
    <span class="zh-content">📊 2025年USA-NA-AIO统计</span>
  </h2>
  
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-icon">👥</div>
      <span class="stat-number">393</span>
      <div class="stat-label">
        <span class="en-content">Round 1 Participants</span>
        <span class="zh-content">第一轮参赛者</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">🎯</div>
      <span class="stat-number">76</span>
      <div class="stat-label">
        <span class="en-content">Round 2 Qualifiers</span>
        <span class="zh-content">晋级第二轮</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">📈</div>
      <span class="stat-number">19.3%</span>
      <div class="stat-label">
        <span class="en-content">Qualification Rate</span>
        <span class="zh-content">晋级率</span>
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-icon">⭐</div>
      <span class="stat-number">217</span>
      <div class="stat-label">
        <span class="en-content">DHR Cutoff (/300)</span>
        <span class="zh-content">DHR分数线</span>
      </div>
    </div>
  </div>
</div>

<!-- College Placements -->
<div class="placements-section">
  <h2>
    <span class="en-content">🎓 Team USA College Placements</span>
    <span class="zh-content">🎓 美国队大学录取</span>
  </h2>
  <p>
    <span class="en-content">Past Team USA members are now at top universities</span>
    <span class="zh-content">历届美国队成员现就读于顶尖大学</span>
  </p>
  
  <div class="placements-grid">
    <div class="placement-card">
      <div class="placement-logo">🏛️</div>
      <h3 class="placement-name">MIT</h3>
      <span class="placement-count">5</span>
      <p class="placement-label">
        <span class="en-content">students</span>
        <span class="zh-content">名学生</span>
      </p>
    </div>
    
    <div class="placement-card">
      <div class="placement-logo">🌲</div>
      <h3 class="placement-name">Stanford</h3>
      <span class="placement-count">3</span>
      <p class="placement-label">
        <span class="en-content">students</span>
        <span class="zh-content">名学生</span>
      </p>
    </div>
    
    <div class="placement-card">
      <div class="placement-logo">🔬</div>
      <h3 class="placement-name">Caltech</h3>
      <span class="placement-count">2</span>
      <p class="placement-label">
        <span class="en-content">students</span>
        <span class="zh-content">名学生</span>
      </p>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us for USAAIO?</span>
      <span class="zh-content">为什么选择我们的USAAIO培训？</span>
    </h2>
    <p>
      <span class="en-content">Comprehensive preparation for AI Olympiad success</span>
      <span class="zh-content">全面准备，助你AI奥赛成功</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📐</div>
      <h3>
        <span class="en-content">Theory + Coding</span>
        <span class="zh-content">理论+编程</span>
      </h3>
      <p>
        <span class="en-content">Master both mathematical foundations and implementation skills required by USAAIO</span>
        <span class="zh-content">掌握USAAIO要求的数学基础和编程实现技能</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Official Syllabus Coverage</span>
        <span class="zh-content">官方大纲覆盖</span>
      </h3>
      <p>
        <span class="en-content">Complete coverage of all topics from mathematical foundations to generative AI</span>
        <span class="zh-content">完整覆盖从数学基础到生成式AI的所有考点</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📝</div>
      <h3>
        <span class="en-content">Past Problem Practice</span>
        <span class="zh-content">真题练习</span>
      </h3>
      <p>
        <span class="en-content">Practice with actual USAAIO problems and simulated competition environments</span>
        <span class="zh-content">使用真实USAAIO题目和模拟竞赛环境练习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🔬</div>
      <h3>
        <span class="en-content">PyTorch Expertise</span>
        <span class="zh-content">PyTorch专业培训</span>
      </h3>
      <p>
        <span class="en-content">Deep learning with PyTorch (required framework, not TensorFlow)</span>
        <span class="zh-content">使用PyTorch进行深度学习（官方要求框架）</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">☁️</div>
      <h3>
        <span class="en-content">Google Colab Training</span>
        <span class="zh-content">Google Colab培训</span>
      </h3>
      <p>
        <span class="en-content">Master the competition platform including Markdown math notation</span>
        <span class="zh-content">掌握竞赛平台，包括Markdown数学公式</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Personalized attention with maximum 6 students per class</span>
        <span class="zh-content">每班最多6人，个性化关注</span>
      </p>
    </div>
  </div>
</div>

<!-- Sponsors -->
<div class="sponsors-section">
  <h3>
    <span class="en-content">USAAIO is supported by</span>
    <span class="zh-content">USAAIO获得以下机构支持</span>
  </h3>
  
  <div class="sponsors-grid">
    <div class="sponsor-item">
      <div class="sponsor-icon">🏛️</div>
      <span class="sponsor-name">MIT</span>
    </div>
    <div class="sponsor-item">
      <div class="sponsor-icon">🎓</div>
      <span class="sponsor-name">Temple University</span>
    </div>
    <div class="sponsor-item">
      <div class="sponsor-icon">🔍</div>
      <span class="sponsor-name">Google</span>
    </div>
    <div class="sponsor-item">
      <div class="sponsor-icon">📈</div>
      <span class="sponsor-name">Jane Street</span>
    </div>
    <div class="sponsor-item">
      <div class="sponsor-icon">🤖</div>
      <span class="sponsor-name">Beaver-Edge AI</span>
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
        <span class="en-content">Round 2 Qualifier</span>
        <span class="zh-content">晋级第二轮</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The combination of theory and coding practice was exactly what I needed. The course helped me understand not just how to use sklearn, but the math behind PCA and SVMs.</span>
        <span class="zh-content">理论与编程练习的结合正是我需要的。课程帮助我不仅学会使用sklearn，还理解了PCA和SVM背后的数学原理。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Kevin L.</h4>
          <p>
            <span class="en-content">High Honor Roll</span>
            <span class="zh-content">高荣誉榜</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Camp Qualifier</span>
        <span class="zh-content">训练营晋级</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">Learning PyTorch from scratch and understanding Transformers architecture prepared me well for Round 2. The deep learning section was incredibly thorough.</span>
        <span class="zh-content">从零学习PyTorch并理解Transformer架构，让我为第二轮做好了充分准备。深度学习部分非常详尽。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍💻</div>
        <div class="testimonial-info">
          <h4>Sarah M.</h4>
          <p>
            <span class="en-content">Distinguished Honor Roll</span>
            <span class="zh-content">杰出荣誉榜</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Honor Roll</span>
        <span class="zh-content">荣誉榜</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">As a freshman, I wasn't sure if I was ready for USAAIO. This course broke down complex topics like diffusion models into understandable pieces. Now I'm aiming for Round 2 next year!</span>
        <span class="zh-content">作为高一学生，我不确定是否准备好参加USAAIO。这门课程将扩散模型等复杂话题分解成易于理解的部分。现在我的目标是明年晋级第二轮！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Jason T.</h4>
          <p>
            <span class="en-content">Freshman, Honor Roll</span>
            <span class="zh-content">高一学生，荣誉榜</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Your USAAIO Journey!</span>
    <span class="zh-content">开启你的USAAIO之旅！</span>
  </h2>
  <p>
    <span class="en-content">Train for the USA-North America AI Olympiad and represent Team USA</span>
    <span class="zh-content">备战USA-NA-AIO，有机会代表美国队参加国际赛</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-button">
      <span class="en-content">🚀 Start Training</span>
      <span class="zh-content">🚀 开始培训</span>
    </a>
    <a href="./contact.html" class="cta-button cta-button-secondary">
      <span class="en-content">📅 Free Consultation</span>
      <span class="zh-content">📅 免费咨询</span>
    </a>
  </div>
</div>
