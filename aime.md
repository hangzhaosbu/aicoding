---
layout: default
title: AIME Competition Training
title_zh: AIME竞赛培训
description: Master the American Invitational Mathematics Examination & Qualify for USAMO
description_zh: 征服美国数学邀请赛，晋级USAMO
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

  @keyframes goldShine {
    0%, 100% { 
      text-shadow: 0 0 20px rgba(245, 158, 11, 0.5);
    }
    50% { 
      text-shadow: 0 0 40px rgba(245, 158, 11, 0.8), 0 0 60px rgba(245, 158, 11, 0.4);
    }
  }

  @keyframes medalFloat {
    0%, 100% { transform: translateY(0) rotate(-5deg); }
    50% { transform: translateY(-15px) rotate(5deg); }
  }

  /* Course Hero - Ultra Premium Gold/Amber Theme */
  .course-hero {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 25%, #B45309 50%, #92400E 75%, #78350F 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(245, 158, 11, 0.4);
    min-height: 500px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '∞';
    position: absolute;
    font-size: 22rem;
    font-weight: 900;
    opacity: 0.08;
    right: -30px;
    top: -50px;
    font-family: "Times New Roman", serif;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.15) 0%, transparent 70%);
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
  .floating-icon:nth-child(2) { left: 92%; top: 20%; animation-delay: 2s; }
  .floating-icon:nth-child(3) { left: 12%; top: 75%; animation-delay: 4s; }
  .floating-icon:nth-child(4) { left: 88%; top: 72%; animation-delay: 6s; }
  .floating-icon:nth-child(5) { left: 50%; top: 8%; animation-delay: 1s; }
  .floating-icon:nth-child(6) { left: 78%; top: 88%; animation-delay: 3s; }
  .floating-icon:nth-child(7) { left: 6%; top: 45%; animation-delay: 5s; }

  .invitational-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #FBBF24 0%, #F59E0B 100%);
    color: #78350F;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 800;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(251, 191, 36, 0.5);
    animation: pulse 2s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .invitational-badge::before {
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
    animation: slideInUp 1s ease-out, goldShine 3s ease-in-out infinite;
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
    flex-wrap: wrap;
    justify-content: center;
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
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 50%, #B45309 100%);
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

  /* What is AIME Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #FBBF24, #F59E0B, #D97706, #B45309) 1;
  }

  .intro-section::before {
    content: '🏆';
    position: absolute;
    font-size: 12rem;
    opacity: 0.03;
    right: -30px;
    bottom: -30px;
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
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(245, 158, 11, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Exam Format Section */
  .exam-format-section {
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 50%, #FDE68A 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .exam-format-section::before {
    content: '📝';
    position: absolute;
    font-size: 12rem;
    opacity: 0.05;
    right: -30px;
    bottom: -30px;
  }

  .exam-format-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #92400E;
    margin-bottom: 1rem;
  }

  .exam-format-section > p {
    text-align: center;
    color: #B45309;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .format-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .format-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .format-grid {
      grid-template-columns: 1fr;
    }
  }

  .format-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s ease;
    border-top: 4px solid #F59E0B;
  }

  .format-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 50px rgba(245, 158, 11, 0.2);
  }

  .format-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .format-value {
    font-size: 2rem;
    font-weight: 800;
    color: #D97706;
    margin-bottom: 0.5rem;
  }

  .format-label {
    font-size: 0.95rem;
    color: #6B7280;
    font-weight: 600;
  }

  /* Pathway Section */
  .pathway-section {
    background: linear-gradient(135deg, #1F2937 0%, #374151 50%, #4B5563 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .pathway-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(245, 158, 11, 0.1) 0%, transparent 50%);
    animation: rotateGlow 20s linear infinite;
  }

  .pathway-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #FBBF24 !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
  }

  .pathway-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .pathway-flow {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
    flex-wrap: nowrap;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  .pathway-item {
    background: white;
    padding: 1.5rem 1.2rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
    transition: all 0.4s ease;
    min-width: 110px;
    flex: 1;
    max-width: 140px;
  }

  .pathway-item:hover {
    transform: translateY(-10px);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.3);
  }

  .pathway-item.amc { border-top: 4px solid #3B82F6; }
  .pathway-item.aime { border-top: 4px solid #F59E0B; background: linear-gradient(to bottom, #FFFBEB 0%, white 30%); }
  .pathway-item.usamo { border-top: 4px solid #10B981; }
  .pathway-item.mop { border-top: 4px solid #8B5CF6; }
  .pathway-item.imo { border-top: 4px solid #EF4444; }

  .pathway-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }

  .pathway-name {
    font-weight: 700;
    color: #1F2937;
    font-size: 0.95rem;
  }

  .pathway-arrow {
    font-size: 1.5rem;
    color: #FBBF24;
    flex-shrink: 0;
  }

  @media (max-width: 800px) {
    .pathway-flow {
      flex-wrap: wrap;
      max-width: 400px;
    }
    .pathway-item {
      min-width: 100px;
    }
  }

  /* Topics Section - 2x2 Layout */
  .topics-section {
    padding: 2rem 0;
  }

  .topics-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .topics-cards {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .topic-card {
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

  .topic-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-left-color: #3B82F6;
    background: linear-gradient(to right, rgba(59, 130, 246, 0.03) 0%, white 30%);
  }
  .topic-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #10B981;
    background: linear-gradient(to right, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }
  .topic-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-left-color: #8B5CF6;
    background: linear-gradient(to right, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }
  .topic-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-left-color: #F59E0B;
    background: linear-gradient(to right, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }

  .topic-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(245, 158, 11, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .topic-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(245, 158, 11, 0.15);
  }

  .topic-header {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }

  .topic-icon {
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

  .topic-card:nth-child(1) .topic-icon { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .topic-card:nth-child(2) .topic-icon { background: linear-gradient(135deg, #10B981, #059669); }
  .topic-card:nth-child(3) .topic-icon { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .topic-card:nth-child(4) .topic-icon { background: linear-gradient(135deg, #F59E0B, #D97706); }

  .topic-title-group {
    flex: 1;
  }

  .topic-title {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .topic-subtitle {
    font-size: 0.9rem;
    color: #6B7280;
  }

  .topic-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .topic-list li {
    padding: 0.5rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
    border-bottom: 1px solid #F3F4F6;
  }

  .topic-list li:last-child {
    border-bottom: none;
  }

  .topic-list li::before {
    content: '→';
    font-weight: bold;
    margin-right: 0.8rem;
    flex-shrink: 0;
  }

  .topic-card:nth-child(1) .topic-list li::before { color: #3B82F6; }
  .topic-card:nth-child(2) .topic-list li::before { color: #10B981; }
  .topic-card:nth-child(3) .topic-list li::before { color: #8B5CF6; }
  .topic-card:nth-child(4) .topic-list li::before { color: #F59E0B; }

  /* Difficulty Levels Section */
  .difficulty-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .difficulty-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .difficulty-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .difficulty-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .difficulty-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
    }
  }

  .difficulty-card {
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    position: relative;
    overflow: hidden;
  }

  .difficulty-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
  }

  .difficulty-card.easy {
    background: linear-gradient(to bottom, #DCFCE7 0%, #F0FDF4 100%);
  }
  .difficulty-card.easy::before { background: linear-gradient(90deg, #22C55E, #16A34A); }

  .difficulty-card.medium {
    background: linear-gradient(to bottom, #FEF3C7 0%, #FFFBEB 100%);
  }
  .difficulty-card.medium::before { background: linear-gradient(90deg, #F59E0B, #D97706); }

  .difficulty-card.hard {
    background: linear-gradient(to bottom, #FEE2E2 0%, #FEF2F2 100%);
  }
  .difficulty-card.hard::before { background: linear-gradient(90deg, #EF4444, #DC2626); }

  .difficulty-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .difficulty-range {
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
  }

  .difficulty-card.easy .difficulty-range { color: #16A34A; }
  .difficulty-card.medium .difficulty-range { color: #D97706; }
  .difficulty-card.hard .difficulty-range { color: #DC2626; }

  .difficulty-label {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
  }

  .difficulty-desc {
    font-size: 0.95rem;
    color: #6B7280;
    line-height: 1.6;
  }

  /* Qualification Section */
  .qualification-section {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 50%, #B45309 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(245, 158, 11, 0.3);
  }

  .qualification-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .qualification-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .qualification-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .qualification-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 700px) {
    .qualification-grid {
      grid-template-columns: 1fr;
      max-width: 450px;
    }
  }

  .qualification-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s ease;
  }

  .qualification-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .qualification-card h3 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .qualification-formula {
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 100%);
    padding: 1.5rem;
    border-radius: 15px;
    text-align: center;
    margin-bottom: 1rem;
    border: 2px solid #F59E0B;
  }

  .formula-text {
    font-size: 1.1rem;
    font-weight: 700;
    color: #92400E;
    font-family: 'Courier New', monospace;
  }

  .qualification-note {
    font-size: 0.9rem;
    color: #6B7280;
    line-height: 1.6;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 50%, #FDE68A 100%);
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
    border-color: #F59E0B;
    box-shadow: 0 20px 40px rgba(245, 158, 11, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(245, 158, 11, 0.3);
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

  /* Success Section */
  .success-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .success-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .success-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
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
    padding: 2rem;
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(245, 158, 11, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .success-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
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

  /* Dates Section */
  .dates-section {
    background: linear-gradient(135deg, #1F2937 0%, #374151 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .dates-section::before {
    content: '📅';
    position: absolute;
    font-size: 12rem;
    opacity: 0.03;
    right: -30px;
    bottom: -30px;
  }

  .dates-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #FBBF24 !important;
    margin-bottom: 1rem;
  }

  .dates-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .dates-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 700px;
    margin: 0 auto;
  }

  @media (max-width: 600px) {
    .dates-grid {
      grid-template-columns: 1fr;
    }
  }

  .date-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border-top: 5px solid #F59E0B;
  }

  .date-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .date-card h3 {
    font-size: 1.5rem;
    font-weight: 800;
    color: #D97706;
    margin-bottom: 1rem;
  }

  .date-value {
    font-size: 1.1rem;
    color: #4B5563;
    margin-bottom: 0.5rem;
  }

  .date-note {
    font-size: 0.85rem;
    color: #9CA3AF;
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 50%, #FDE68A 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
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
    color: #F59E0B;
    opacity: 0.2;
    font-family: Georgia, serif;
    line-height: 1;
  }

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .testimonial-badge.usamo { background: linear-gradient(135deg, #10B981, #059669); }
  .testimonial-badge.usajmo { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .testimonial-badge.aime { background: linear-gradient(135deg, #F59E0B, #D97706); }

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
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
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
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 25%, #B45309 50%, #92400E 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(245, 158, 11, 0.4);
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
    color: #D97706;
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
    background: linear-gradient(90deg, transparent, rgba(245, 158, 11, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #92400E;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #D97706;
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
      gap: 1.5rem;
    }

    .hero-stat-number {
      font-size: 2rem;
    }
    
    .section-header h2 {
      font-size: 2rem;
    }
    
    .cta-section h2 {
      font-size: 2rem;
    }

    .intro-section,
    .exam-format-section,
    .qualification-section,
    .why-choose-section,
    .success-section,
    .dates-section,
    .difficulty-section {
      padding: 3rem 1.5rem;
    }

    .invitational-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="invitational-badge">
    <span class="en-content">INVITATIONAL</span>
    <span class="zh-content">邀请赛</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">∑</span>
    <span class="floating-icon">∫</span>
    <span class="floating-icon">π</span>
    <span class="floating-icon">∞</span>
    <span class="floating-icon">√</span>
    <span class="floating-icon">Δ</span>
    <span class="floating-icon">θ</span>
  </div>
  <h1>
    <span class="en-content">AIME Training</span>
    <span class="zh-content">AIME竞赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">American Invitational Mathematics Examination</span>
    <span class="zh-content">美国数学邀请赛</span>
  </p>
  <div class="hero-badge">
    <span>🏆</span>
    <span class="en-content">Gateway to USAMO & International Math Olympiad</span>
    <span class="zh-content">通往USAMO与国际数学奥赛的大门</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">15</span>
      <span class="hero-stat-label">
        <span class="en-content">Questions</span>
        <span class="zh-content">道题目</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">3</span>
      <span class="hero-stat-label">
        <span class="en-content">Hours</span>
        <span class="zh-content">小时</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">Top 2.5%</span>
      <span class="hero-stat-label">
        <span class="en-content">AMC Qualifiers</span>
        <span class="zh-content">AMC晋级者</span>
      </span>
    </div>
  </div>
</div>

<!-- What is AIME -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is the AIME?</span>
        <span class="zh-content">什么是AIME？</span>
      </h2>
      <p>
        <span class="en-content">
          The American Invitational Mathematics Examination (AIME) is a prestigious, invitation-only 
          competition for students who excel on the AMC 10 or AMC 12. Organized by the Mathematical 
          Association of America (MAA), AIME serves as the second stage in the pathway to the 
          International Mathematical Olympiad (IMO).
        </span>
        <span class="zh-content">
          美国数学邀请赛（AIME）是一项享有盛誉的邀请制竞赛，面向在AMC 10或AMC 12中表现优异的学生。
          由美国数学协会（MAA）组织，AIME是通往国际数学奥林匹克（IMO）的第二阶段。
        </span>
      </p>
      <p>
        <span class="en-content">
          The questions on the AIME are significantly more challenging than those on the AMC 10 and AMC 12, 
          requiring deep mathematical insight, creative problem-solving, and mastery of advanced techniques. 
          Top-scoring AIME participants are invited to take the USAMO or USAJMO.
        </span>
        <span class="zh-content">
          AIME的题目比AMC 10和AMC 12难度大得多，需要深刻的数学洞察力、创造性的问题解决能力和高级技巧的掌握。
          AIME高分选手将被邀请参加USAMO或USAJMO。
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎖️</span>
          <span class="intro-highlight-text">
            <span class="en-content">Invitation-Only</span>
            <span class="zh-content">仅限邀请</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎯</span>
          <span class="intro-highlight-text">
            <span class="en-content">Integer Answers (0-999)</span>
            <span class="zh-content">整数答案（0-999）</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏅</span>
          <span class="intro-highlight-text">
            <span class="en-content">USAMO/USAJMO Qualifier</span>
            <span class="zh-content">USAMO/USAJMO资格</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌟</span>
          <span class="intro-highlight-text">
            <span class="en-content">IMO Pathway</span>
            <span class="zh-content">IMO通道</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 6rem; animation: medalFloat 4s ease-in-out infinite;">🥇</div>
      <div style="font-size: 2rem; font-weight: 800; color: #D97706; margin-top: 1rem;">AIME</div>
    </div>
  </div>
</div>

<!-- Exam Format -->
<div class="exam-format-section">
  <h2>
    <span class="en-content">📝 Exam Format</span>
    <span class="zh-content">📝 考试形式</span>
  </h2>
  <p>
    <span class="en-content">Understanding the AIME structure is key to success</span>
    <span class="zh-content">了解AIME结构是成功的关键</span>
  </p>
  
  <div class="format-grid">
    <div class="format-card">
      <div class="format-icon">📊</div>
      <div class="format-value">15</div>
      <div class="format-label">
        <span class="en-content">Questions</span>
        <span class="zh-content">道题目</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">⏱️</div>
      <div class="format-value">3 hrs</div>
      <div class="format-label">
        <span class="en-content">Time Limit</span>
        <span class="zh-content">时间限制</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">🔢</div>
      <div class="format-value">0-999</div>
      <div class="format-label">
        <span class="en-content">Answer Range</span>
        <span class="zh-content">答案范围</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">🚫</div>
      <div class="format-value">
        <span class="en-content">None</span>
        <span class="zh-content">禁止</span>
      </div>
      <div class="format-label">
        <span class="en-content">Calculators</span>
        <span class="zh-content">使用计算器</span>
      </div>
    </div>
  </div>
</div>

<!-- Pathway Section -->
<div class="pathway-section">
  <h2>
    <span class="en-content">🏆 Road to the IMO</span>
    <span class="zh-content">🏆 通往IMO之路</span>
  </h2>
  <p>
    <span class="en-content">AIME is your gateway to the world's most prestigious math competition</span>
    <span class="zh-content">AIME是通往世界最负盛名数学竞赛的大门</span>
  </p>
  
  <div class="pathway-flow">
    <div class="pathway-item amc">
      <div class="pathway-icon">📚</div>
      <div class="pathway-name">AMC 10/12</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item aime">
      <div class="pathway-icon">🥇</div>
      <div class="pathway-name">AIME</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item usamo">
      <div class="pathway-icon">🏆</div>
      <div class="pathway-name">USA(J)MO</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item mop">
      <div class="pathway-icon">🎓</div>
      <div class="pathway-name">MOP</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item imo">
      <div class="pathway-icon">🌟</div>
      <div class="pathway-name">IMO</div>
    </div>
  </div>
</div>

<!-- Topics Section -->
<div class="topics-section">
  <div class="section-header">
    <h2>
      <span class="en-content">AIME Topic Areas</span>
      <span class="zh-content">AIME考试内容</span>
    </h2>
    <p>
      <span class="en-content">Master these four pillars of competition mathematics</span>
      <span class="zh-content">掌握竞赛数学的四大支柱</span>
    </p>
  </div>

  <div class="topics-cards">
    <!-- Algebra -->
    <div class="topic-card">
      <div class="topic-header">
        <div class="topic-icon">📐</div>
        <div class="topic-title-group">
          <h3 class="topic-title">
            <span class="en-content">Algebra</span>
            <span class="zh-content">代数</span>
          </h3>
          <p class="topic-subtitle">
            <span class="en-content">Advanced Algebraic Techniques</span>
            <span class="zh-content">高级代数技巧</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Polynomials & Vieta's Formulas</span><span class="zh-content">多项式与韦达定理</span></li>
        <li><span class="en-content">Functional Equations</span><span class="zh-content">函数方程</span></li>
        <li><span class="en-content">Complex Numbers & Roots of Unity</span><span class="zh-content">复数与单位根</span></li>
        <li><span class="en-content">Sequences & Series</span><span class="zh-content">数列与级数</span></li>
        <li><span class="en-content">Inequalities (AM-GM, Cauchy-Schwarz)</span><span class="zh-content">不等式（AM-GM，柯西-施瓦茨）</span></li>
        <li><span class="en-content">Symmetric Polynomials</span><span class="zh-content">对称多项式</span></li>
        <li><span class="en-content">Logarithms & Exponentials</span><span class="zh-content">对数与指数</span></li>
      </ul>
    </div>

    <!-- Geometry -->
    <div class="topic-card">
      <div class="topic-header">
        <div class="topic-icon">📏</div>
        <div class="topic-title-group">
          <h3 class="topic-title">
            <span class="en-content">Geometry</span>
            <span class="zh-content">几何</span>
          </h3>
          <p class="topic-subtitle">
            <span class="en-content">Euclidean & Coordinate Geometry</span>
            <span class="zh-content">欧几里得与坐标几何</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Circle Theorems (Power of a Point)</span><span class="zh-content">圆定理（点的幂）</span></li>
        <li><span class="en-content">Trigonometry & Law of Sines/Cosines</span><span class="zh-content">三角函数与正弦/余弦定理</span></li>
        <li><span class="en-content">Coordinate Geometry & Vectors</span><span class="zh-content">坐标几何与向量</span></li>
        <li><span class="en-content">Similar & Congruent Triangles</span><span class="zh-content">相似与全等三角形</span></li>
        <li><span class="en-content">Ceva's & Menelaus's Theorems</span><span class="zh-content">塞瓦定理与梅涅劳斯定理</span></li>
        <li><span class="en-content">Ptolemy's Theorem</span><span class="zh-content">托勒密定理</span></li>
        <li><span class="en-content">3D Geometry & Spatial Reasoning</span><span class="zh-content">三维几何与空间推理</span></li>
      </ul>
    </div>

    <!-- Combinatorics -->
    <div class="topic-card">
      <div class="topic-header">
        <div class="topic-icon">🎲</div>
        <div class="topic-title-group">
          <h3 class="topic-title">
            <span class="en-content">Combinatorics</span>
            <span class="zh-content">组合数学</span>
          </h3>
          <p class="topic-subtitle">
            <span class="en-content">Counting & Probability</span>
            <span class="zh-content">计数与概率</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Permutations & Combinations</span><span class="zh-content">排列与组合</span></li>
        <li><span class="en-content">Inclusion-Exclusion Principle</span><span class="zh-content">容斥原理</span></li>
        <li><span class="en-content">Generating Functions</span><span class="zh-content">生成函数</span></li>
        <li><span class="en-content">Recursion & Recurrence Relations</span><span class="zh-content">递归与递推关系</span></li>
        <li><span class="en-content">Probability & Expected Value</span><span class="zh-content">概率与期望值</span></li>
        <li><span class="en-content">Pigeonhole Principle</span><span class="zh-content">鸽巢原理</span></li>
        <li><span class="en-content">Bijections & Counting Arguments</span><span class="zh-content">双射与计数论证</span></li>
      </ul>
    </div>

    <!-- Number Theory -->
    <div class="topic-card">
      <div class="topic-header">
        <div class="topic-icon">🔢</div>
        <div class="topic-title-group">
          <h3 class="topic-title">
            <span class="en-content">Number Theory</span>
            <span class="zh-content">数论</span>
          </h3>
          <p class="topic-subtitle">
            <span class="en-content">Properties of Integers</span>
            <span class="zh-content">整数性质</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Modular Arithmetic</span><span class="zh-content">模运算</span></li>
        <li><span class="en-content">Prime Factorization & Divisibility</span><span class="zh-content">质因数分解与整除</span></li>
        <li><span class="en-content">Fermat's Little Theorem</span><span class="zh-content">费马小定理</span></li>
        <li><span class="en-content">Euler's Totient Function</span><span class="zh-content">欧拉函数</span></li>
        <li><span class="en-content">Diophantine Equations</span><span class="zh-content">丢番图方程</span></li>
        <li><span class="en-content">Chinese Remainder Theorem</span><span class="zh-content">中国剩余定理</span></li>
        <li><span class="en-content">Lifting the Exponent (LTE)</span><span class="zh-content">提升指数引理</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Difficulty Levels -->
<div class="difficulty-section">
  <h2>
    <span class="en-content">📊 Problem Difficulty Distribution</span>
    <span class="zh-content">📊 题目难度分布</span>
  </h2>
  <p>
    <span class="en-content">AIME problems progressively increase in difficulty</span>
    <span class="zh-content">AIME题目难度逐渐递增</span>
  </p>
  
  <div class="difficulty-grid">
    <div class="difficulty-card easy">
      <div class="difficulty-range">1-5</div>
      <div class="difficulty-label">
        <span class="en-content">Foundational</span>
        <span class="zh-content">基础题</span>
      </div>
      <p class="difficulty-desc">
        <span class="en-content">Build confidence with accessible problems. Master these to score 5+ reliably.</span>
        <span class="zh-content">通过可达题目建立信心。掌握这些可稳定得5分以上。</span>
      </p>
    </div>
    
    <div class="difficulty-card medium">
      <div class="difficulty-range">6-10</div>
      <div class="difficulty-label">
        <span class="en-content">Intermediate</span>
        <span class="zh-content">中等题</span>
      </div>
      <p class="difficulty-desc">
        <span class="en-content">Require deeper insight and technique. Scoring 7+ opens USAMO/USAJMO doors.</span>
        <span class="zh-content">需要更深入的洞察力和技巧。得7分以上可开启USAMO/USAJMO之门。</span>
      </p>
    </div>
    
    <div class="difficulty-card hard">
      <div class="difficulty-range">11-15</div>
      <div class="difficulty-label">
        <span class="en-content">Advanced</span>
        <span class="zh-content">高难度题</span>
      </div>
      <p class="difficulty-desc">
        <span class="en-content">Challenge problems requiring creative solutions. Scoring 10+ virtually guarantees USAMO.</span>
        <span class="zh-content">需要创造性解决方案的挑战题。得10分以上几乎确保USAMO资格。</span>
      </p>
    </div>
  </div>
</div>

<!-- Qualification Section -->
<div class="qualification-section">
  <h2>
    <span class="en-content">🎯 Qualification to USAMO/USAJMO</span>
    <span class="zh-content">🎯 USAMO/USAJMO资格</span>
  </h2>
  <p>
    <span class="en-content">Your combined AMC and AIME scores determine Olympiad eligibility</span>
    <span class="zh-content">你的AMC和AIME综合成绩决定奥赛资格</span>
  </p>
  
  <div class="qualification-grid">
    <div class="qualification-card">
      <h3>
        <span>🏆</span>
        <span class="en-content">USAMO Index</span>
        <span class="zh-content">USAMO指数</span>
      </h3>
      <div class="qualification-formula">
        <div class="formula-text">AMC 12 + 20 × AIME</div>
      </div>
      <p class="qualification-note">
        <span class="en-content">For students who qualified through AMC 12. Top scorers are invited to the USA Mathematical Olympiad.</span>
        <span class="zh-content">适用于通过AMC 12晋级的学生。高分者将被邀请参加美国数学奥林匹克。</span>
      </p>
    </div>
    
    <div class="qualification-card">
      <h3>
        <span>🥇</span>
        <span class="en-content">USAJMO Index</span>
        <span class="zh-content">USAJMO指数</span>
      </h3>
      <div class="qualification-formula">
        <div class="formula-text">AMC 10 + 20 × AIME</div>
      </div>
      <p class="qualification-note">
        <span class="en-content">For students who qualified through AMC 10. Top scorers are invited to the USA Junior Mathematical Olympiad.</span>
        <span class="zh-content">适用于通过AMC 10晋级的学生。高分者将被邀请参加美国青少年数学奥林匹克。</span>
      </p>
    </div>
  </div>
</div>

<!-- Dates Section -->
<div class="dates-section">
  <h2>
    <span class="en-content">📅 2025 AIME Competition Dates</span>
    <span class="zh-content">📅 2025年AIME竞赛日期</span>
  </h2>
  <p>
    <span class="en-content">Students may only take AIME once (either I or II)</span>
    <span class="zh-content">学生只能参加一次AIME（I或II）</span>
  </p>
  
  <div class="dates-grid">
    <div class="date-card">
      <h3>AIME I</h3>
      <div class="date-value">
        <span class="en-content">February 6, 2025</span>
        <span class="zh-content">2025年2月6日</span>
      </div>
      <div class="date-note">
        <span class="en-content">Primary test date • 1:30-5:30 PM ET</span>
        <span class="zh-content">主要考试日期 • 东部时间下午1:30-5:30</span>
      </div>
    </div>
    
    <div class="date-card">
      <h3>AIME II</h3>
      <div class="date-value">
        <span class="en-content">February 12, 2025</span>
        <span class="zh-content">2025年2月12日</span>
      </div>
      <div class="date-note">
        <span class="en-content">Alternate date • 1:30-5:30 PM ET</span>
        <span class="zh-content">备用考试日期 • 东部时间下午1:30-5:30</span>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us for AIME?</span>
      <span class="zh-content">为什么选择我们的AIME培训？</span>
    </h2>
    <p>
      <span class="en-content">Expert guidance to maximize your AIME score</span>
      <span class="zh-content">专家指导，最大化你的AIME成绩</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">40+ Years of Problems</span>
        <span class="zh-content">40+年真题</span>
      </h3>
      <p>
        <span class="en-content">Comprehensive practice with every AIME problem since 1983, organized by topic and difficulty</span>
        <span class="zh-content">1983年以来每道AIME真题的全面练习，按主题和难度分类</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🧠</div>
      <h3>
        <span class="en-content">Advanced Techniques</span>
        <span class="zh-content">高级技巧</span>
      </h3>
      <p>
        <span class="en-content">Learn powerful methods: generating functions, complex bashing, projective geometry</span>
        <span class="zh-content">学习强大方法：生成函数、复数运算、射影几何</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Strategic Training</span>
        <span class="zh-content">策略训练</span>
      </h3>
      <p>
        <span class="en-content">Time management, problem selection, and when to "bash" vs. find elegant solutions</span>
        <span class="zh-content">时间管理、题目选择，以及何时"暴力计算"vs寻找优雅解法</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Mock Exams</span>
        <span class="zh-content">模拟考试</span>
      </h3>
      <p>
        <span class="en-content">Timed practice under real conditions with detailed solution analysis</span>
        <span class="zh-content">真实条件下的计时练习，配有详细解答分析</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🏅</div>
      <h3>
        <span class="en-content">USAMO Preparation</span>
        <span class="zh-content">USAMO准备</span>
      </h3>
      <p>
        <span class="en-content">Bridge to proof-based Olympiad mathematics for top performers</span>
        <span class="zh-content">为顶尖学生搭建通往证明型奥赛数学的桥梁</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized problem-solving guidance</span>
        <span class="zh-content">每班最多6人，个性化问题解决指导</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' AIME Achievements</span>
    <span class="zh-content">🏆 我们学生的AIME成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🎯</div>
      <span class="success-number">9.2</span>
      <div class="success-label">
        <span class="en-content">Avg AIME Score</span>
        <span class="zh-content">平均AIME分数</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🏅</div>
      <span class="success-number">15+</span>
      <div class="success-label">
        <span class="en-content">USAMO/USAJMO Qualifiers</span>
        <span class="zh-content">USAMO/USAJMO晋级者</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">+4</span>
      <div class="success-label">
        <span class="en-content">Avg Score Improvement</span>
        <span class="zh-content">平均分数提升</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">3</span>
      <div class="success-label">
        <span class="en-content">MOP Invitees</span>
        <span class="zh-content">MOP受邀者</span>
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
      <span class="testimonial-badge usamo">USAMO</span>
      <p class="testimonial-text">
        <span class="en-content">I went from scoring 6 on my first AIME to 12 on my second attempt. The advanced techniques and strategic training completely transformed my approach to competition math.</span>
        <span class="zh-content">我从第一次AIME的6分进步到第二次的12分。高级技巧和策略训练完全改变了我对竞赛数学的方法。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Alex K.</h4>
          <p>
            <span class="en-content">AIME Score: 12 → USAMO Qualifier</span>
            <span class="zh-content">AIME成绩：12 → USAMO晋级</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge usajmo">USAJMO</span>
      <p class="testimonial-text">
        <span class="en-content">As an 8th grader taking AIME for the first time, I was terrified. The structured problem sets and mock exams gave me the confidence to score 9 and qualify for USAJMO!</span>
        <span class="zh-content">作为第一次参加AIME的8年级学生，我曾经非常害怕。系统的习题集和模拟考试给了我信心，最终得到9分并晋级USAJMO！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Sophie L.</h4>
          <p>
            <span class="en-content">8th Grade, AIME Score: 9</span>
            <span class="zh-content">8年级，AIME成绩：9</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge aime">AIME 10+</span>
      <p class="testimonial-text">
        <span class="en-content">The number theory and combinatorics training was exceptional. I finally understood generating functions and scored my first double-digit AIME score!</span>
        <span class="zh-content">数论和组合数学的训练非常出色。我终于理解了生成函数，并取得了第一个两位数的AIME成绩！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Michael Z.</h4>
          <p>
            <span class="en-content">10th Grade, AIME Score: 11</span>
            <span class="zh-content">10年级，AIME成绩：11</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Elevate Your AIME Performance!</span>
    <span class="zh-content">提升你的AIME成绩！</span>
  </h2>
  <p>
    <span class="en-content">Join elite students on the path to USAMO and beyond</span>
    <span class="zh-content">加入精英学生，踏上通往USAMO及更高目标的道路</span>
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
