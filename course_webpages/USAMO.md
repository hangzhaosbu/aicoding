---
layout: default
title: USAMO/USAJMO Training
title_zh: USAMO/USAJMO竞赛培训
description: Master Proof-Based Olympiad Mathematics & Qualify for MOP
description_zh: 征服证明型奥赛数学，晋级MOP
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
    25% { transform: translateY(-12px) rotate(-2deg); }
    75% { transform: translateY(12px) rotate(2deg); }
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

  @keyframes emeraldShine {
    0%, 100% { 
      text-shadow: 0 0 20px rgba(16, 185, 129, 0.5);
    }
    50% { 
      text-shadow: 0 0 40px rgba(16, 185, 129, 0.8), 0 0 60px rgba(16, 185, 129, 0.4);
    }
  }

  @keyframes trophyFloat {
    0%, 100% { transform: translateY(0) rotate(-3deg) scale(1); }
    50% { transform: translateY(-20px) rotate(3deg) scale(1.05); }
  }

  @keyframes medalGlow {
    0%, 100% { box-shadow: 0 0 20px rgba(255, 215, 0, 0.3); }
    50% { box-shadow: 0 0 40px rgba(255, 215, 0, 0.6), 0 0 60px rgba(255, 215, 0, 0.3); }
  }

  /* Course Hero - Ultra Premium Emerald/Green Theme */
  .course-hero {
    background: linear-gradient(135deg, #10B981 0%, #059669 25%, #047857 50%, #065F46 75%, #064E3B 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.4);
    min-height: 520px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '∴';
    position: absolute;
    font-size: 25rem;
    font-weight: 900;
    opacity: 0.06;
    right: -50px;
    top: -80px;
    font-family: "Times New Roman", serif;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.12) 0%, transparent 70%);
    animation: rotateGlow 25s linear infinite;
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
    font-size: 2.8rem;
    opacity: 0.12;
    animation: float 12s ease-in-out infinite;
  }

  .floating-icon:nth-child(1) { left: 4%; top: 12%; animation-delay: 0s; }
  .floating-icon:nth-child(2) { left: 93%; top: 18%; animation-delay: 2s; }
  .floating-icon:nth-child(3) { left: 10%; top: 78%; animation-delay: 4s; }
  .floating-icon:nth-child(4) { left: 90%; top: 75%; animation-delay: 6s; }
  .floating-icon:nth-child(5) { left: 50%; top: 6%; animation-delay: 1s; }
  .floating-icon:nth-child(6) { left: 75%; top: 90%; animation-delay: 3s; }
  .floating-icon:nth-child(7) { left: 5%; top: 50%; animation-delay: 5s; }

  .national-badge {
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
    animation: pulse 2s ease-in-out infinite, medalGlow 3s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .national-badge::before {
    content: '🏆';
  }

  .course-hero h1 {
    color: white !important;
    font-size: 3.8rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out, emeraldShine 3s ease-in-out infinite;
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
    background: linear-gradient(135deg, #10B981 0%, #059669 50%, #047857 100%);
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

  /* What is USAMO Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #34D399, #10B981, #059669, #047857) 1;
  }

  .intro-section::before {
    content: '🏆';
    position: absolute;
    font-size: 14rem;
    opacity: 0.03;
    right: -40px;
    bottom: -40px;
    animation: trophyFloat 6s ease-in-out infinite;
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
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(16, 185, 129, 0.15);
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
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 50%, #A7F3D0 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .exam-format-section::before {
    content: '✍️';
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
    color: #065F46;
    margin-bottom: 1rem;
  }

  .exam-format-section > p {
    text-align: center;
    color: #047857;
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
    border-top: 4px solid #10B981;
  }

  .format-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 50px rgba(16, 185, 129, 0.2);
  }

  .format-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .format-value {
    font-size: 2rem;
    font-weight: 800;
    color: #059669;
    margin-bottom: 0.5rem;
  }

  .format-label {
    font-size: 0.95rem;
    color: #6B7280;
    font-weight: 600;
  }

  /* Dual Competition Section */
  .dual-competition-section {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 4rem 0;
  }

  @media (max-width: 900px) {
    .dual-competition-section {
      grid-template-columns: 1fr;
    }
  }

  .competition-card {
    padding: 3rem;
    border-radius: 30px;
    position: relative;
    overflow: hidden;
    transition: all 0.4s ease;
  }

  .competition-card:hover {
    transform: translateY(-10px);
  }

  .competition-card.usamo {
    background: linear-gradient(135deg, #10B981 0%, #059669 50%, #047857 100%);
    box-shadow: 0 25px 50px rgba(16, 185, 129, 0.3);
  }

  .competition-card.usajmo {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 50%, #6D28D9 100%);
    box-shadow: 0 25px 50px rgba(139, 92, 246, 0.3);
  }

  .competition-card::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 60%);
    animation: rotateGlow 20s linear infinite;
  }

  .competition-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    color: white;
    padding: 0.4rem 1rem;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 700;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .competition-card h3 {
    color: white;
    font-size: 2rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
    position: relative;
    z-index: 1;
  }

  .competition-card .subtitle {
    color: rgba(255, 255, 255, 0.9);
    font-size: 1rem;
    margin-bottom: 1.5rem;
    position: relative;
    z-index: 1;
  }

  .competition-details {
    position: relative;
    z-index: 1;
  }

  .competition-detail {
    display: flex;
    align-items: center;
    gap: 0.8rem;
    color: rgba(255, 255, 255, 0.95);
    padding: 0.6rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.15);
  }

  .competition-detail:last-child {
    border-bottom: none;
  }

  .competition-detail-icon {
    font-size: 1.2rem;
  }

  /* Awards Section */
  .awards-section {
    background: linear-gradient(135deg, #1F2937 0%, #374151 50%, #4B5563 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .awards-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(16, 185, 129, 0.1) 0%, transparent 50%);
    animation: rotateGlow 20s linear infinite;
  }

  .awards-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #34D399 !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .awards-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .awards-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 800px) {
    .awards-grid {
      grid-template-columns: 1fr;
    }
  }

  .awards-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
  }

  .awards-card h3 {
    font-size: 1.5rem;
    font-weight: 800;
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
  }

  .awards-card.usamo h3 { color: #059669; }
  .awards-card.usajmo h3 { color: #7C3AED; }

  .award-tier {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1rem;
    border-radius: 15px;
    margin-bottom: 1rem;
    transition: all 0.3s ease;
  }

  .award-tier:last-child {
    margin-bottom: 0;
  }

  .award-tier:hover {
    transform: translateX(5px);
  }

  .award-tier.gold {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
  }

  .award-tier.silver {
    background: linear-gradient(135deg, #F3F4F6 0%, #E5E7EB 100%);
  }

  .award-tier.bronze {
    background: linear-gradient(135deg, #FED7AA 0%, #FDBA74 100%);
  }

  .award-tier.winner {
    background: linear-gradient(135deg, #DDD6FE 0%, #C4B5FD 100%);
  }

  .award-tier.honorable {
    background: linear-gradient(135deg, #D1FAE5 0%, #A7F3D0 100%);
  }

  .award-medal {
    font-size: 2rem;
  }

  .award-info h4 {
    font-weight: 700;
    color: #1F2937;
    font-size: 1.1rem;
    margin-bottom: 0.2rem;
  }

  .award-info p {
    color: #6B7280;
    font-size: 0.9rem;
  }

  /* Pathway Section */
  .pathway-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .pathway-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .pathway-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .pathway-visual {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1.5rem;
    flex-wrap: wrap;
    max-width: 1100px;
    margin: 0 auto;
  }

  .pathway-step {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    min-width: 140px;
    transition: all 0.4s ease;
    position: relative;
  }

  .pathway-step:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(16, 185, 129, 0.2);
  }

  .pathway-step.highlighted {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
    box-shadow: 0 15px 30px rgba(16, 185, 129, 0.3);
  }

  .pathway-step.highlighted .pathway-step-name {
    color: white;
  }

  .pathway-step.mop {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
    box-shadow: 0 15px 30px rgba(245, 158, 11, 0.3);
  }

  .pathway-step.mop .pathway-step-name {
    color: white;
  }

  .pathway-step.imo {
    background: linear-gradient(135deg, #EF4444 0%, #DC2626 100%);
    color: white;
    box-shadow: 0 15px 30px rgba(239, 68, 68, 0.3);
  }

  .pathway-step.imo .pathway-step-name {
    color: white;
  }

  .pathway-step-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .pathway-step-name {
    font-weight: 700;
    color: #1F2937;
    font-size: 1rem;
  }

  .pathway-arrow {
    font-size: 2rem;
    color: #10B981;
  }

  @media (max-width: 900px) {
    .pathway-visual {
      flex-direction: column;
      max-width: 200px;
    }
    .pathway-arrow {
      transform: rotate(90deg);
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
    border-left-color: #10B981;
    background: linear-gradient(to right, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }
  .topic-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #3B82F6;
    background: linear-gradient(to right, rgba(59, 130, 246, 0.03) 0%, white 30%);
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
    background: linear-gradient(90deg, transparent, rgba(16, 185, 129, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .topic-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.15);
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

  .topic-card:nth-child(1) .topic-icon { background: linear-gradient(135deg, #10B981, #059669); }
  .topic-card:nth-child(2) .topic-icon { background: linear-gradient(135deg, #3B82F6, #2563EB); }
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
    content: '∴';
    font-weight: bold;
    margin-right: 0.8rem;
    flex-shrink: 0;
  }

  .topic-card:nth-child(1) .topic-list li::before { color: #10B981; }
  .topic-card:nth-child(2) .topic-list li::before { color: #3B82F6; }
  .topic-card:nth-child(3) .topic-list li::before { color: #8B5CF6; }
  .topic-card:nth-child(4) .topic-list li::before { color: #F59E0B; }

  /* Proof Writing Section */
  .proof-section {
    background: linear-gradient(135deg, #10B981 0%, #059669 50%, #047857 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.3);
  }

  .proof-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .proof-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .proof-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .proof-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .proof-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
    }
  }

  .proof-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .proof-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .proof-card-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .proof-card h3 {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .proof-card p {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Qualification Section */
  .qualification-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .qualification-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .qualification-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .qualification-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
  }

  @media (max-width: 700px) {
    .qualification-grid {
      grid-template-columns: 1fr;
    }
  }

  .qualification-card {
    padding: 2rem;
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .qualification-card.usamo {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    border: 2px solid #10B981;
  }

  .qualification-card.usajmo {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
    border: 2px solid #8B5CF6;
  }

  .qualification-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .qualification-card h3 {
    font-size: 1.3rem;
    font-weight: 700;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .qualification-card.usamo h3 { color: #059669; }
  .qualification-card.usajmo h3 { color: #7C3AED; }

  .qualification-formula {
    background: white;
    padding: 1.5rem;
    border-radius: 15px;
    text-align: center;
    margin-bottom: 1rem;
  }

  .qualification-card.usamo .qualification-formula {
    border: 2px solid #10B981;
  }

  .qualification-card.usajmo .qualification-formula {
    border: 2px solid #8B5CF6;
  }

  .formula-text {
    font-size: 1.1rem;
    font-weight: 700;
    font-family: 'Courier New', monospace;
  }

  .qualification-card.usamo .formula-text { color: #065F46; }
  .qualification-card.usajmo .formula-text { color: #5B21B6; }

  .qualification-note {
    font-size: 0.9rem;
    color: #6B7280;
    line-height: 1.6;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 50%, #A7F3D0 100%);
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
    border-color: #10B981;
    box-shadow: 0 20px 40px rgba(16, 185, 129, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(16, 185, 129, 0.3);
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
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
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
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(16, 185, 129, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .success-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
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
    color: #34D399 !important;
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
    border-top: 5px solid #10B981;
  }

  .date-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .date-card h3 {
    font-size: 1.5rem;
    font-weight: 800;
    color: #059669;
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
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 50%, #A7F3D0 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
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
    color: #10B981;
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

  .testimonial-badge.mop { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .testimonial-badge.usamo { background: linear-gradient(135deg, #10B981, #059669); }
  .testimonial-badge.usajmo { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }

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
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
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
    background: linear-gradient(135deg, #10B981 0%, #059669 25%, #047857 50%, #065F46 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.4);
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
    color: #059669;
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
    background: linear-gradient(90deg, transparent, rgba(16, 185, 129, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #047857;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #059669;
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
    .proof-section,
    .why-choose-section,
    .success-section,
    .dates-section,
    .qualification-section,
    .awards-section {
      padding: 3rem 1.5rem;
    }

    .national-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="national-badge">
    <span class="en-content">NATIONAL OLYMPIAD</span>
    <span class="zh-content">国家奥赛</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">∴</span>
    <span class="floating-icon">∵</span>
    <span class="floating-icon">∎</span>
    <span class="floating-icon">∀</span>
    <span class="floating-icon">∃</span>
    <span class="floating-icon">⟹</span>
    <span class="floating-icon">∈</span>
  </div>
  <h1>
    <span class="en-content">USAMO Training</span>
    <span class="zh-content">USAMO竞赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">USA Mathematical Olympiad & Junior Mathematical Olympiad</span>
    <span class="zh-content">美国数学奥林匹克与青少年数学奥林匹克</span>
  </p>
  <div class="hero-badge">
    <span>🌟</span>
    <span class="en-content">Pathway to MOP & International Mathematical Olympiad</span>
    <span class="zh-content">通往MOP与国际数学奥林匹克的道路</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">6</span>
      <span class="hero-stat-label">
        <span class="en-content">Proof Problems</span>
        <span class="zh-content">证明题</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">9</span>
      <span class="hero-stat-label">
        <span class="en-content">Hours (2 Days)</span>
        <span class="zh-content">小时（2天）</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">~500</span>
      <span class="hero-stat-label">
        <span class="en-content">Qualifiers/Year</span>
        <span class="zh-content">每年晋级人数</span>
      </span>
    </div>
  </div>
</div>

<!-- What is USAMO -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is USA(J)MO?</span>
        <span class="zh-content">什么是USA(J)MO？</span>
      </h2>
      <p>
        <span class="en-content">
          The United States of America Mathematical Olympiad (USAMO) and Junior Mathematical Olympiad (USAJMO) 
          are the most prestigious national-level math competitions in the United States. These proof-based 
          examinations serve as a critical step in selecting the team that represents the USA at the 
          International Mathematical Olympiad (IMO).
        </span>
        <span class="zh-content">
          美国数学奥林匹克（USAMO）和青少年数学奥林匹克（USAJMO）是美国最负盛名的国家级数学竞赛。
          这些证明型考试是选拔代表美国参加国际数学奥林匹克（IMO）团队的关键步骤。
        </span>
      </p>
      <p>
        <span class="en-content">
          Unlike the AMC and AIME which require only numerical answers, USAMO and USAJMO demand complete, 
          rigorous mathematical proofs. This is where true mathematical reasoning and creativity are tested. 
          Top performers are invited to the Mathematical Olympiad Program (MOP).
        </span>
        <span class="zh-content">
          与只需要数值答案的AMC和AIME不同，USAMO和USAJMO要求完整、严谨的数学证明。
          这里是真正测试数学推理和创造力的地方。顶尖选手将被邀请参加数学奥林匹克项目（MOP）。
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">✍️</span>
          <span class="intro-highlight-text">
            <span class="en-content">Proof-Based Exam</span>
            <span class="zh-content">证明型考试</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏆</span>
          <span class="intro-highlight-text">
            <span class="en-content">National Championship</span>
            <span class="zh-content">国家锦标赛</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎓</span>
          <span class="intro-highlight-text">
            <span class="en-content">MOP Invitation</span>
            <span class="zh-content">MOP邀请</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌍</span>
          <span class="intro-highlight-text">
            <span class="en-content">IMO Team Selection</span>
            <span class="zh-content">IMO团队选拔</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 6rem; animation: trophyFloat 5s ease-in-out infinite;">🏆</div>
      <div style="font-size: 2rem; font-weight: 800; color: #059669; margin-top: 1rem;">USA(J)MO</div>
    </div>
  </div>
</div>

<!-- Exam Format -->
<div class="exam-format-section">
  <h2>
    <span class="en-content">✍️ Exam Format</span>
    <span class="zh-content">✍️ 考试形式</span>
  </h2>
  <p>
    <span class="en-content">A rigorous two-day proof-writing examination</span>
    <span class="zh-content">严格的两天证明写作考试</span>
  </p>
  
  <div class="format-grid">
    <div class="format-card">
      <div class="format-icon">📝</div>
      <div class="format-value">6</div>
      <div class="format-label">
        <span class="en-content">Proof Problems</span>
        <span class="zh-content">证明题</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">📅</div>
      <div class="format-value">2</div>
      <div class="format-label">
        <span class="en-content">Days</span>
        <span class="zh-content">天</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">⏱️</div>
      <div class="format-value">9 hrs</div>
      <div class="format-label">
        <span class="en-content">Total Time</span>
        <span class="zh-content">总时长</span>
      </div>
    </div>
    <div class="format-card">
      <div class="format-icon">📊</div>
      <div class="format-value">42</div>
      <div class="format-label">
        <span class="en-content">Max Points</span>
        <span class="zh-content">满分</span>
      </div>
    </div>
  </div>
</div>

<!-- Dual Competition Section -->
<div class="dual-competition-section">
  <div class="competition-card usamo">
    <span class="competition-badge">
      <span class="en-content">AMC 12 PATHWAY</span>
      <span class="zh-content">AMC 12通道</span>
    </span>
    <h3>USAMO</h3>
    <p class="subtitle">
      <span class="en-content">USA Mathematical Olympiad</span>
      <span class="zh-content">美国数学奥林匹克</span>
    </p>
    <div class="competition-details">
      <div class="competition-detail">
        <span class="competition-detail-icon">👤</span>
        <span class="en-content">~250 qualifiers per year</span>
        <span class="zh-content">每年约250人晋级</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">📊</span>
        <span class="en-content">AMC 12 + 10 × AIME index</span>
        <span class="zh-content">AMC 12 + 10 × AIME指数</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">🎯</span>
        <span class="en-content">Top high school students</span>
        <span class="zh-content">顶尖高中生</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">🏆</span>
        <span class="en-content">Gold, Silver, Bronze awards</span>
        <span class="zh-content">金、银、铜奖</span>
      </div>
    </div>
  </div>
  
  <div class="competition-card usajmo">
    <span class="competition-badge">
      <span class="en-content">AMC 10 PATHWAY</span>
      <span class="zh-content">AMC 10通道</span>
    </span>
    <h3>USAJMO</h3>
    <p class="subtitle">
      <span class="en-content">USA Junior Mathematical Olympiad</span>
      <span class="zh-content">美国青少年数学奥林匹克</span>
    </p>
    <div class="competition-details">
      <div class="competition-detail">
        <span class="competition-detail-icon">👤</span>
        <span class="en-content">~250 qualifiers per year</span>
        <span class="zh-content">每年约250人晋级</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">📊</span>
        <span class="en-content">AMC 10 + 10 × AIME index</span>
        <span class="zh-content">AMC 10 + 10 × AIME指数</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">🎯</span>
        <span class="en-content">Grade 10 and below</span>
        <span class="zh-content">10年级及以下</span>
      </div>
      <div class="competition-detail">
        <span class="competition-detail-icon">🏆</span>
        <span class="en-content">Winners recognition (~20%)</span>
        <span class="zh-content">获奖者表彰（约20%）</span>
      </div>
    </div>
  </div>
</div>

<!-- Awards Section -->
<div class="awards-section">
  <h2>
    <span class="en-content">🏅 Awards & Recognition</span>
    <span class="zh-content">🏅 奖项与荣誉</span>
  </h2>
  <p>
    <span class="en-content">Official MAA award distribution for USAMO and USAJMO</span>
    <span class="zh-content">MAA官方USAMO和USAJMO奖项分布</span>
  </p>
  
  <div class="awards-grid">
    <div class="awards-card usamo">
      <h3>
        <span>🏆</span>
        <span>USAMO Awards</span>
      </h3>
      <div class="award-tier gold">
        <span class="award-medal">🥇</span>
        <div class="award-info">
          <h4>Gold</h4>
          <p>
            <span class="en-content">Top ~6% of competitors</span>
            <span class="zh-content">前约6%的参赛者</span>
          </p>
        </div>
      </div>
      <div class="award-tier silver">
        <span class="award-medal">🥈</span>
        <div class="award-info">
          <h4>Silver</h4>
          <p>
            <span class="en-content">Top ~12% of competitors</span>
            <span class="zh-content">前约12%的参赛者</span>
          </p>
        </div>
      </div>
      <div class="award-tier bronze">
        <span class="award-medal">🥉</span>
        <div class="award-info">
          <h4>Bronze</h4>
          <p>
            <span class="en-content">Top ~18% of competitors</span>
            <span class="zh-content">前约18%的参赛者</span>
          </p>
        </div>
      </div>
      <div class="award-tier honorable">
        <span class="award-medal">⭐</span>
        <div class="award-info">
          <h4>Honorable Mention</h4>
          <p>
            <span class="en-content">14+ points</span>
            <span class="zh-content">14分以上</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="awards-card usajmo">
      <h3>
        <span>🏆</span>
        <span>USAJMO Awards</span>
      </h3>
      <div class="award-tier winner">
        <span class="award-medal">🏆</span>
        <div class="award-info">
          <h4>Winner</h4>
          <p>
            <span class="en-content">Top performers</span>
            <span class="zh-content">顶尖选手</span>
          </p>
        </div>
      </div>
      <div class="award-tier silver">
        <span class="award-medal">🎖️</span>
        <div class="award-info">
          <h4>Recognition</h4>
          <p>
            <span class="en-content">~20% of contestants</span>
            <span class="zh-content">约20%的参赛者</span>
          </p>
        </div>
      </div>
      <div class="award-tier honorable">
        <span class="award-medal">⭐</span>
        <div class="award-info">
          <h4>Honorable Mention</h4>
          <p>
            <span class="en-content">14+ points</span>
            <span class="zh-content">14分以上</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Pathway Section -->
<div class="pathway-section">
  <h2>
    <span class="en-content">🌟 Road to IMO</span>
    <span class="zh-content">🌟 通往IMO之路</span>
  </h2>
  <p>
    <span class="en-content">USA(J)MO is your gateway to representing the United States internationally</span>
    <span class="zh-content">USA(J)MO是代表美国参加国际赛事的门户</span>
  </p>
  
  <div class="pathway-visual">
    <div class="pathway-step">
      <div class="pathway-step-icon">📚</div>
      <div class="pathway-step-name">AMC + AIME</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-step highlighted">
      <div class="pathway-step-icon">🏆</div>
      <div class="pathway-step-name">USA(J)MO</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-step mop">
      <div class="pathway-step-icon">🎓</div>
      <div class="pathway-step-name">MOP</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-step imo">
      <div class="pathway-step-icon">🌍</div>
      <div class="pathway-step-name">IMO</div>
    </div>
  </div>
</div>

<!-- Topics Section -->
<div class="topics-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Olympiad Topic Areas</span>
      <span class="zh-content">奥赛核心内容</span>
    </h2>
    <p>
      <span class="en-content">Master these four pillars of proof-based mathematics</span>
      <span class="zh-content">掌握证明型数学的四大支柱</span>
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
            <span class="en-content">Olympiad Algebraic Methods</span>
            <span class="zh-content">奥赛代数方法</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Functional Equations & Inequalities</span><span class="zh-content">函数方程与不等式</span></li>
        <li><span class="en-content">AM-GM, Cauchy-Schwarz, Jensen's</span><span class="zh-content">AM-GM、柯西-施瓦茨、詹森不等式</span></li>
        <li><span class="en-content">Polynomial Theory & Roots</span><span class="zh-content">多项式理论与根</span></li>
        <li><span class="en-content">Sequences & Recurrences</span><span class="zh-content">数列与递推</span></li>
        <li><span class="en-content">Complex Numbers in Proofs</span><span class="zh-content">证明中的复数</span></li>
        <li><span class="en-content">Substitution Techniques</span><span class="zh-content">代换技巧</span></li>
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
            <span class="en-content">Synthetic & Projective Methods</span>
            <span class="zh-content">综合与射影方法</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Power of a Point & Radical Axes</span><span class="zh-content">点的幂与根轴</span></li>
        <li><span class="en-content">Projective Geometry & Cross-Ratio</span><span class="zh-content">射影几何与交比</span></li>
        <li><span class="en-content">Inversion & Transformations</span><span class="zh-content">反演与变换</span></li>
        <li><span class="en-content">Ceva, Menelaus, Stewart</span><span class="zh-content">塞瓦、梅涅劳斯、斯图尔特定理</span></li>
        <li><span class="en-content">Homogeneous Coordinates</span><span class="zh-content">齐次坐标</span></li>
        <li><span class="en-content">Spiral Similarity & Configurations</span><span class="zh-content">螺旋相似与构型</span></li>
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
            <span class="en-content">Discrete Mathematics & Logic</span>
            <span class="zh-content">离散数学与逻辑</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Graph Theory & Extremal Problems</span><span class="zh-content">图论与极值问题</span></li>
        <li><span class="en-content">Pigeonhole & Double Counting</span><span class="zh-content">鸽巢原理与双计数</span></li>
        <li><span class="en-content">Invariants & Monovariants</span><span class="zh-content">不变量与单调量</span></li>
        <li><span class="en-content">Coloring & Game Theory</span><span class="zh-content">着色与博弈论</span></li>
        <li><span class="en-content">Extremal Principle</span><span class="zh-content">极端原理</span></li>
        <li><span class="en-content">Algorithms & Constructions</span><span class="zh-content">算法与构造</span></li>
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
            <span class="en-content">Advanced Integer Properties</span>
            <span class="zh-content">高级整数性质</span>
          </p>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Quadratic Residues & Legendre</span><span class="zh-content">二次剩余与勒让德符号</span></li>
        <li><span class="en-content">Lifting the Exponent (LTE)</span><span class="zh-content">提升指数引理</span></li>
        <li><span class="en-content">Orders & Primitive Roots</span><span class="zh-content">阶与原根</span></li>
        <li><span class="en-content">Vieta Jumping & Descent</span><span class="zh-content">韦达跳跃与下降法</span></li>
        <li><span class="en-content">p-adic Valuation</span><span class="zh-content">p进赋值</span></li>
        <li><span class="en-content">Zsigmondy's Theorem</span><span class="zh-content">齐格蒙迪定理</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Proof Writing Section -->
<div class="proof-section">
  <h2>
    <span class="en-content">✍️ The Art of Proof Writing</span>
    <span class="zh-content">✍️ 证明写作的艺术</span>
  </h2>
  <p>
    <span class="en-content">USAMO grading rewards complete, rigorous solutions</span>
    <span class="zh-content">USAMO评分奖励完整、严谨的解答</span>
  </p>
  
  <div class="proof-grid">
    <div class="proof-card">
      <div class="proof-card-icon">📝</div>
      <h3>
        <span class="en-content">7-Point Scale</span>
        <span class="zh-content">7分制</span>
      </h3>
      <p>
        <span class="en-content">Each problem is scored 0-7. Complete solutions get 7 points; partial credit is rare (mostly 0-1 or 6-7).</span>
        <span class="zh-content">每题0-7分。完整解答得7分；部分分数很少（主要是0-1或6-7分）。</span>
      </p>
    </div>
    
    <div class="proof-card">
      <div class="proof-card-icon">🎯</div>
      <h3>
        <span class="en-content">Key Ideas Matter</span>
        <span class="zh-content">关键思想最重要</span>
      </h3>
      <p>
        <span class="en-content">Graders look for main insights. Having all key ideas = "7-", missing one = "0+". Focus on core reasoning.</span>
        <span class="zh-content">评分员寻找主要见解。有所有关键想法="7-"，缺少一个="0+"。专注于核心推理。</span>
      </p>
    </div>
    
    <div class="proof-card">
      <div class="proof-card-icon">✅</div>
      <h3>
        <span class="en-content">Clarity & Rigor</span>
        <span class="zh-content">清晰与严谨</span>
      </h3>
      <p>
        <span class="en-content">Write clearly, justify each step, and avoid gaps in logic. Elegance helps but completeness is essential.</span>
        <span class="zh-content">写作清晰，证明每一步，避免逻辑漏洞。优雅有帮助，但完整性是必需的。</span>
      </p>
    </div>
  </div>
</div>

<!-- Qualification Section -->
<div class="qualification-section">
  <h2>
    <span class="en-content">🎯 Qualification Index</span>
    <span class="zh-content">🎯 资格指数</span>
  </h2>
  <p>
    <span class="en-content">Your combined AMC and AIME scores determine Olympiad eligibility</span>
    <span class="zh-content">你的AMC和AIME综合成绩决定奥赛资格</span>
  </p>
  
  <div class="qualification-grid">
    <div class="qualification-card usamo">
      <h3>
        <span>🏆</span>
        <span class="en-content">USAMO Index</span>
        <span class="zh-content">USAMO指数</span>
      </h3>
      <div class="qualification-formula">
        <div class="formula-text">AMC 12 + 10 × AIME</div>
      </div>
      <p class="qualification-note">
        <span class="en-content">For students who qualified through AMC 12. Higher AMC score and AIME score lead to higher index. Cutoffs vary by year.</span>
        <span class="zh-content">适用于通过AMC 12晋级的学生。更高的AMC分数和AIME分数带来更高的指数。分数线每年不同。</span>
      </p>
    </div>
    
    <div class="qualification-card usajmo">
      <h3>
        <span>🥇</span>
        <span class="en-content">USAJMO Index</span>
        <span class="zh-content">USAJMO指数</span>
      </h3>
      <div class="qualification-formula">
        <div class="formula-text">AMC 10 + 10 × AIME</div>
      </div>
      <p class="qualification-note">
        <span class="en-content">For students who qualified through AMC 10. Grade 10 and below. A stepping stone to USAMO for younger students.</span>
        <span class="zh-content">适用于通过AMC 10晋级的学生。10年级及以下。年轻学生通往USAMO的踏脚石。</span>
      </p>
    </div>
  </div>
</div>

<!-- Dates Section -->
<div class="dates-section">
  <h2>
    <span class="en-content">📅 2025 Competition Dates</span>
    <span class="zh-content">📅 2025年竞赛日期</span>
  </h2>
  <p>
    <span class="en-content">USAMO and USAJMO are held at official testing sites only</span>
    <span class="zh-content">USAMO和USAJMO仅在官方考点举行</span>
  </p>
  
  <div class="dates-grid">
    <div class="date-card">
      <h3>
        <span class="en-content">Day 1</span>
        <span class="zh-content">第一天</span>
      </h3>
      <div class="date-value">
        <span class="en-content">March 19, 2025</span>
        <span class="zh-content">2025年3月19日</span>
      </div>
      <div class="date-note">
        <span class="en-content">Problems 1-3 • 1:00-5:30 PM ET</span>
        <span class="zh-content">第1-3题 • 东部时间下午1:00-5:30</span>
      </div>
    </div>
    
    <div class="date-card">
      <h3>
        <span class="en-content">Day 2</span>
        <span class="zh-content">第二天</span>
      </h3>
      <div class="date-value">
        <span class="en-content">March 20, 2025</span>
        <span class="zh-content">2025年3月20日</span>
      </div>
      <div class="date-note">
        <span class="en-content">Problems 4-6 • 1:00-5:30 PM ET</span>
        <span class="zh-content">第4-6题 • 东部时间下午1:00-5:30</span>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us for USA(J)MO?</span>
      <span class="zh-content">为什么选择我们的USA(J)MO培训？</span>
    </h2>
    <p>
      <span class="en-content">Expert guidance to master proof-based olympiad mathematics</span>
      <span class="zh-content">专家指导，掌握证明型奥赛数学</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">✍️</div>
      <h3>
        <span class="en-content">Proof Writing Mastery</span>
        <span class="zh-content">证明写作精通</span>
      </h3>
      <p>
        <span class="en-content">Learn to write clear, rigorous proofs that earn full marks from olympiad graders</span>
        <span class="zh-content">学习撰写清晰、严谨的证明，从奥赛评分员那里获得满分</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">40+ Years of Problems</span>
        <span class="zh-content">40+年真题</span>
      </h3>
      <p>
        <span class="en-content">Comprehensive study of every USAMO/USAJMO problem with detailed solutions and insights</span>
        <span class="zh-content">全面研究每道USAMO/USAJMO真题，配有详细解答和见解</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🧠</div>
      <h3>
        <span class="en-content">Advanced Techniques</span>
        <span class="zh-content">高级技巧</span>
      </h3>
      <p>
        <span class="en-content">Master projective geometry, functional equations, extremal combinatorics, and more</span>
        <span class="zh-content">掌握射影几何、函数方程、极值组合等</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📝</div>
      <h3>
        <span class="en-content">Mock Olympiads</span>
        <span class="zh-content">模拟奥赛</span>
      </h3>
      <p>
        <span class="en-content">Full-length practice under competition conditions with detailed feedback on proofs</span>
        <span class="zh-content">竞赛条件下的全真模拟，配有证明的详细反馈</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎓</div>
      <h3>
        <span class="en-content">MOP Preparation</span>
        <span class="zh-content">MOP准备</span>
      </h3>
      <p>
        <span class="en-content">Bridge training for those aiming to qualify for the Mathematical Olympiad Program</span>
        <span class="zh-content">为希望晋级数学奥林匹克项目的学生提供桥梁培训</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 4 students for intensive, personalized proof-writing instruction</span>
        <span class="zh-content">每班最多4人，进行深入、个性化的证明写作指导</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' USA(J)MO Achievements</span>
    <span class="zh-content">🏆 我们学生的USA(J)MO成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">8</span>
      <div class="success-label">
        <span class="en-content">USAMO/USAJMO Winners</span>
        <span class="zh-content">USAMO/USAJMO获奖者</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🎓</div>
      <span class="success-number">5</span>
      <div class="success-label">
        <span class="en-content">MOP Invitees</span>
        <span class="zh-content">MOP受邀者</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">85%</span>
      <div class="success-label">
        <span class="en-content">HM+ Rate</span>
        <span class="zh-content">荣誉提名率</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">2</span>
      <div class="success-label">
        <span class="en-content">IMO Team Members</span>
        <span class="zh-content">IMO国家队成员</span>
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
      <span class="testimonial-badge mop">MOP</span>
      <p class="testimonial-text">
        <span class="en-content">The proof writing training completely transformed my approach. I went from scoring 7 points total to 28 points and qualified for MOP. The personalized feedback on my proofs was invaluable.</span>
        <span class="zh-content">证明写作培训完全改变了我的方法。我从总分7分进步到28分，并晋级MOP。对我证明的个性化反馈非常宝贵。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>David L.</h4>
          <p>
            <span class="en-content">USAMO Silver → MOP Invitee</span>
            <span class="zh-content">USAMO银奖 → MOP受邀</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge usamo">USAMO Gold</span>
      <p class="testimonial-text">
        <span class="en-content">Learning advanced techniques like inversion and projective geometry opened up so many problems for me. The deep dives into each topic area were exactly what I needed to reach the next level.</span>
        <span class="zh-content">学习反演和射影几何等高级技巧为我打开了许多问题。对每个主题领域的深入探讨正是我达到下一个水平所需要的。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Emma W.</h4>
          <p>
            <span class="en-content">USAMO Gold, 11th Grade</span>
            <span class="zh-content">USAMO金奖，11年级</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge usajmo">USAJMO Winner</span>
      <p class="testimonial-text">
        <span class="en-content">As a 9th grader, I was intimidated by proof-based problems. The structured curriculum built my confidence step by step. Now I'm a USAJMO Winner and looking forward to USAMO next year!</span>
        <span class="zh-content">作为9年级学生，我曾被证明题吓倒。系统的课程一步步建立了我的信心。现在我是USAJMO获奖者，期待明年的USAMO！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Kevin Z.</h4>
          <p>
            <span class="en-content">USAJMO Winner, 9th Grade</span>
            <span class="zh-content">USAJMO获奖者，9年级</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Master Olympiad Mathematics!</span>
    <span class="zh-content">征服奥赛数学！</span>
  </h2>
  <p>
    <span class="en-content">Join elite students on the path to MOP and the IMO</span>
    <span class="zh-content">加入精英学生，踏上通往MOP和IMO的道路</span>
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
