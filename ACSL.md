---
layout: default
title: ACSL Competition Training
title_zh: ACSL计算机科学联赛培训
description: Master Computer Science Concepts & Programming for ACSL Success
description_zh: 掌握计算机科学概念与编程，征服ACSL竞赛
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

  @keyframes codeType {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.5; }
  }

  @keyframes binaryFlow {
    0% { background-position: 0% 0%; }
    100% { background-position: 100% 100%; }
  }

  /* Course Hero - Ultra Premium Purple/Violet Theme */
  .course-hero {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 25%, #6D28D9 50%, #5B21B6 75%, #4C1D95 100%);
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
    min-height: 520px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '{ }';
    position: absolute;
    font-size: 20rem;
    font-weight: 900;
    opacity: 0.06;
    right: -30px;
    top: -40px;
    font-family: 'Courier New', monospace;
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
    font-size: 2.5rem;
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

  .since-badge {
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

  .since-badge::before {
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
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 50%, #6D28D9 100%);
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

  /* What is ACSL Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #A78BFA, #8B5CF6, #7C3AED, #6D28D9) 1;
  }

  .intro-section::before {
    content: '💻';
    position: absolute;
    font-size: 14rem;
    opacity: 0.03;
    right: -40px;
    bottom: -40px;
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
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(139, 92, 246, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Divisions Overview Section */
  .divisions-overview {
    background: linear-gradient(135deg, #1F2937 0%, #374151 50%, #4B5563 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .divisions-overview::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(139, 92, 246, 0.1) 0%, transparent 50%);
    animation: rotateGlow 20s linear infinite;
  }

  .divisions-overview h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #A78BFA !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .divisions-overview > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .divisions-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 1.5rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1100px) {
    .divisions-grid {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media (max-width: 700px) {
    .divisions-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .divisions-grid {
      grid-template-columns: 1fr;
    }
  }

  .division-mini-card {
    background: white;
    padding: 1.5rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border-top: 4px solid;
  }

  .division-mini-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .division-mini-card.senior { border-top-color: #EF4444; }
  .division-mini-card.intermediate { border-top-color: #F59E0B; }
  .division-mini-card.junior { border-top-color: #10B981; }
  .division-mini-card.classroom { border-top-color: #3B82F6; }
  .division-mini-card.elementary { border-top-color: #EC4899; }

  .division-mini-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .division-mini-name {
    font-weight: 700;
    color: #1F2937;
    font-size: 1rem;
    margin-bottom: 0.3rem;
  }

  .division-mini-grades {
    font-size: 0.85rem;
    color: #6B7280;
  }

  /* Individual Division Sections */
  .division-section {
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 3rem 0;
    position: relative;
    overflow: hidden;
  }

  .division-section.senior {
    background: linear-gradient(135deg, #FEF2F2 0%, #FECACA 50%, #FCA5A5 100%);
  }

  .division-section.intermediate {
    background: linear-gradient(135deg, #FFFBEB 0%, #FEF3C7 50%, #FDE68A 100%);
  }

  .division-section.junior {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 50%, #A7F3D0 100%);
  }

  .division-section.classroom {
    background: linear-gradient(135deg, #EFF6FF 0%, #DBEAFE 50%, #BFDBFE 100%);
  }

  .division-section.elementary {
    background: linear-gradient(135deg, #FDF2F8 0%, #FCE7F3 50%, #FBCFE8 100%);
  }

  .division-header {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    margin-bottom: 2rem;
  }

  .division-icon-large {
    width: 80px;
    height: 80px;
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.5rem;
    color: white;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  }

  .division-section.senior .division-icon-large { background: linear-gradient(135deg, #EF4444, #DC2626); }
  .division-section.intermediate .division-icon-large { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .division-section.junior .division-icon-large { background: linear-gradient(135deg, #10B981, #059669); }
  .division-section.classroom .division-icon-large { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .division-section.elementary .division-icon-large { background: linear-gradient(135deg, #EC4899, #DB2777); }

  .division-title-group h2 {
    font-size: 2rem;
    font-weight: 800;
    margin-bottom: 0.3rem;
  }

  .division-section.senior .division-title-group h2 { color: #B91C1C; }
  .division-section.intermediate .division-title-group h2 { color: #B45309; }
  .division-section.junior .division-title-group h2 { color: #047857; }
  .division-section.classroom .division-title-group h2 { color: #1D4ED8; }
  .division-section.elementary .division-title-group h2 { color: #BE185D; }

  .division-title-group p {
    color: #6B7280;
    font-size: 1.1rem;
  }

  .division-badge {
    display: inline-block;
    padding: 0.4rem 1rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 700;
    color: white;
    margin-left: auto;
  }

  .division-section.senior .division-badge { background: linear-gradient(135deg, #EF4444, #DC2626); }
  .division-section.intermediate .division-badge { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .division-section.junior .division-badge { background: linear-gradient(135deg, #10B981, #059669); }
  .division-section.classroom .division-badge { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .division-section.elementary .division-badge { background: linear-gradient(135deg, #EC4899, #DB2777); }

  .division-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  @media (max-width: 900px) {
    .division-content {
      grid-template-columns: 1fr;
    }
  }

  .division-info-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  }

  .division-info-card h3 {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .format-item {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 0.8rem 0;
    border-bottom: 1px solid #F3F4F6;
  }

  .format-item:last-child {
    border-bottom: none;
  }

  .format-icon {
    font-size: 1.5rem;
  }

  .format-text {
    flex: 1;
  }

  .format-label {
    font-size: 0.85rem;
    color: #6B7280;
  }

  .format-value {
    font-weight: 700;
    color: #1F2937;
  }

  .topics-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .topics-list li {
    padding: 0.6rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
    border-bottom: 1px solid #F3F4F6;
  }

  .topics-list li:last-child {
    border-bottom: none;
  }

  .topics-list li::before {
    content: '▸';
    font-weight: bold;
  }

  .division-section.senior .topics-list li::before { color: #EF4444; }
  .division-section.intermediate .topics-list li::before { color: #F59E0B; }
  .division-section.junior .topics-list li::before { color: #10B981; }
  .division-section.classroom .topics-list li::before { color: #3B82F6; }
  .division-section.elementary .topics-list li::before { color: #EC4899; }

  /* Contest Schedule Section */
  .schedule-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .schedule-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .schedule-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .contest-schedule-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .contest-schedule-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .contest-schedule-grid {
      grid-template-columns: 1fr;
    }
  }

  .contest-card {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border-top: 4px solid #8B5CF6;
  }

  .contest-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(139, 92, 246, 0.2);
  }

  .contest-number {
    font-size: 2.5rem;
    font-weight: 800;
    color: #7C3AED;
    margin-bottom: 0.5rem;
  }

  .contest-topics {
    list-style: none;
    padding: 0;
    margin: 1rem 0 0;
    text-align: left;
  }

  .contest-topics li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.9rem;
    border-bottom: 1px solid rgba(139, 92, 246, 0.15);
  }

  .contest-topics li:last-child {
    border-bottom: none;
  }

  /* Finals Section */
  .finals-section {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 50%, #6D28D9 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.3);
  }

  .finals-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .finals-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .finals-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .finals-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 800px) {
    .finals-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
    }
  }

  .finals-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .finals-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .finals-card-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .finals-card h3 {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .finals-card p {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  .qualification-scores {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    max-width: 600px;
    margin: 3rem auto 0;
    position: relative;
    z-index: 1;
  }

  .qualification-scores h3 {
    text-align: center;
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1.5rem;
  }

  .qual-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.8rem 1rem;
    border-radius: 10px;
    margin-bottom: 0.5rem;
  }

  .qual-item:nth-child(odd) {
    background: #F3F4F6;
  }

  .qual-division {
    font-weight: 600;
    color: #1F2937;
  }

  .qual-score {
    font-weight: 800;
    color: #7C3AED;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 50%, #C4B5FD 100%);
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
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
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
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(139, 92, 246, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
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

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 50%, #C4B5FD 100%);
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
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .testimonial-badge.finals { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .testimonial-badge.senior { background: linear-gradient(135deg, #EF4444, #DC2626); }
  .testimonial-badge.junior { background: linear-gradient(135deg, #10B981, #059669); }

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
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 25%, #6D28D9 50%, #5B21B6 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
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
    color: #5B21B6;
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
    .division-section,
    .schedule-section,
    .finals-section,
    .why-choose-section,
    .success-section {
      padding: 3rem 1.5rem;
    }

    .since-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }

    .division-header {
      flex-direction: column;
      text-align: center;
    }

    .division-badge {
      margin-left: 0;
      margin-top: 1rem;
    }
  }
</style>

<div class="course-hero">
  <span class="since-badge">
    <span class="en-content">SINCE 1978</span>
    <span class="zh-content">始于1978</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🔢</span>
    <span class="floating-icon">⚡</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">📊</span>
    <span class="floating-icon">🔗</span>
    <span class="floating-icon">⌨️</span>
  </div>
  <h1>
    <span class="en-content">ACSL Training</span>
    <span class="zh-content">ACSL计算机科学联赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">American Computer Science League</span>
    <span class="zh-content">美国计算机科学联赛</span>
  </p>
  <div class="hero-badge">
    <span>🌐</span>
    <span class="en-content">300+ Schools Worldwide • NASSP Approved</span>
    <span class="zh-content">全球300+学校参与 • NASSP认证</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">47+</span>
      <span class="hero-stat-label">
        <span class="en-content">Years</span>
        <span class="zh-content">年历史</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">5</span>
      <span class="hero-stat-label">
        <span class="en-content">Divisions</span>
        <span class="zh-content">个组别</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">4</span>
      <span class="hero-stat-label">
        <span class="en-content">Contests/Year</span>
        <span class="zh-content">场比赛/年</span>
      </span>
    </div>
  </div>
</div>

<!-- What is ACSL -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is ACSL?</span>
        <span class="zh-content">什么是ACSL？</span>
      </h2>
      <p>
        <span class="en-content">
          The American Computer Science League (ACSL) is one of the oldest and most prestigious computer science 
          competitions, founded in 1978. It tests students on fundamental CS concepts including number systems, 
          Boolean algebra, data structures, graph theory, and programming.
        </span>
        <span class="zh-content">
          美国计算机科学联赛（ACSL）是历史最悠久、最负盛名的计算机科学竞赛之一，成立于1978年。
          它测试学生的基础CS概念，包括数制、布尔代数、数据结构、图论和编程。
        </span>
      </p>
      <p>
        <span class="en-content">
          ACSL is approved by the National Association of Secondary School Principals (NASSP) and is an 
          institutional member of the Computer Science Teachers Association. Students compete in teams, 
          with top performers invited to the prestigious Finals competition.
        </span>
        <span class="zh-content">
          ACSL获得全国中学校长协会（NASSP）认证，是计算机科学教师协会的机构成员。
          学生以团队形式参赛，表现优异者将被邀请参加享有盛誉的总决赛。
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏫</span>
          <span class="intro-highlight-text">
            <span class="en-content">300+ Schools Worldwide</span>
            <span class="zh-content">全球300+学校</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎯</span>
          <span class="intro-highlight-text">
            <span class="en-content">Team & Individual Awards</span>
            <span class="zh-content">团队与个人奖项</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">💻</span>
          <span class="intro-highlight-text">
            <span class="en-content">Online Platform</span>
            <span class="zh-content">在线平台</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏆</span>
          <span class="intro-highlight-text">
            <span class="en-content">Finals Invitations</span>
            <span class="zh-content">总决赛邀请</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 6rem; animation: float 5s ease-in-out infinite;">💻</div>
      <div style="font-size: 2rem; font-weight: 800; color: #7C3AED; margin-top: 1rem;">ACSL</div>
    </div>
  </div>
</div>

<!-- Divisions Overview -->
<div class="divisions-overview">
  <h2>
    <span class="en-content">📊 Five Competition Divisions</span>
    <span class="zh-content">📊 五个竞赛组别</span>
  </h2>
  <p>
    <span class="en-content">Choose the division that best matches your skill level and grade</span>
    <span class="zh-content">选择最适合你技能水平和年级的组别</span>
  </p>
  
  <div class="divisions-grid">
    <div class="division-mini-card senior">
      <div class="division-mini-icon">🔴</div>
      <div class="division-mini-name">Senior</div>
      <div class="division-mini-grades">
        <span class="en-content">Grades 9-12</span>
        <span class="zh-content">9-12年级</span>
      </div>
    </div>
    <div class="division-mini-card intermediate">
      <div class="division-mini-icon">🟠</div>
      <div class="division-mini-name">Intermediate</div>
      <div class="division-mini-grades">
        <span class="en-content">Grades 9-12</span>
        <span class="zh-content">9-12年级</span>
      </div>
    </div>
    <div class="division-mini-card junior">
      <div class="division-mini-icon">🟢</div>
      <div class="division-mini-name">Junior</div>
      <div class="division-mini-grades">
        <span class="en-content">Grades 6-9</span>
        <span class="zh-content">6-9年级</span>
      </div>
    </div>
    <div class="division-mini-card classroom">
      <div class="division-mini-icon">🔵</div>
      <div class="division-mini-name">Classroom</div>
      <div class="division-mini-grades">
        <span class="en-content">All Grades</span>
        <span class="zh-content">所有年级</span>
      </div>
    </div>
    <div class="division-mini-card elementary">
      <div class="division-mini-icon">🩷</div>
      <div class="division-mini-name">Elementary</div>
      <div class="division-mini-grades">
        <span class="en-content">Grades 3-6</span>
        <span class="zh-content">3-6年级</span>
      </div>
    </div>
  </div>
</div>

<!-- SENIOR DIVISION -->
<div class="division-section senior">
  <div class="division-header">
    <div class="division-icon-large">🔴</div>
    <div class="division-title-group">
      <h2>
        <span class="en-content">Senior Division</span>
        <span class="zh-content">高级组</span>
      </h2>
      <p>
        <span class="en-content">For experienced programmers, especially AP Computer Science students</span>
        <span class="zh-content">面向有编程经验的学生，特别是AP计算机科学学生</span>
      </p>
    </div>
    <span class="division-badge">
      <span class="en-content">GRADES 9-12</span>
      <span class="zh-content">9-12年级</span>
    </span>
  </div>
  
  <div class="division-content">
    <div class="division-info-card">
      <h3>
        <span>📋</span>
        <span class="en-content">Contest Format</span>
        <span class="zh-content">比赛形式</span>
      </h3>
      <div class="format-item">
        <span class="format-icon">📝</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Short Answer</span>
            <span class="zh-content">简答题</span>
          </div>
          <div class="format-value">
            <span class="en-content">30 min, 6 questions</span>
            <span class="zh-content">30分钟，6道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">💻</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Programming</span>
            <span class="zh-content">编程题</span>
          </div>
          <div class="format-value">
            <span class="en-content">72 hours, 1 problem</span>
            <span class="zh-content">72小时，1道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">⭐</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Max Score</span>
            <span class="zh-content">最高分</span>
          </div>
          <div class="format-value">
            <span class="en-content">10 points per contest</span>
            <span class="zh-content">每场比赛10分</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🏆</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Finals Qualification</span>
            <span class="zh-content">决赛资格</span>
          </div>
          <div class="format-value">
            <span class="en-content">28+ points cumulative</span>
            <span class="zh-content">累计28分以上</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="division-info-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered (12)</span>
        <span class="zh-content">考试内容（12个主题）</span>
      </h3>
      <ul class="topics-list">
        <li><span class="en-content">Computer Number Systems</span><span class="zh-content">计算机数制</span></li>
        <li><span class="en-content">Recursive Functions</span><span class="zh-content">递归函数</span></li>
        <li><span class="en-content">What Does This Program Do?</span><span class="zh-content">程序功能分析</span></li>
        <li><span class="en-content">Prefix/Infix/Postfix Notation</span><span class="zh-content">前缀/中缀/后缀表达式</span></li>
        <li><span class="en-content">Bit-String Flicking</span><span class="zh-content">位串操作</span></li>
        <li><span class="en-content">LISP Programming</span><span class="zh-content">LISP编程</span></li>
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></li>
        <li><span class="en-content">FSAs & Regular Expressions</span><span class="zh-content">有限状态自动机与正则表达式</span></li>
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
        <li><span class="en-content">Digital Electronics</span><span class="zh-content">数字电子学</span></li>
        <li><span class="en-content">Assembly Language</span><span class="zh-content">汇编语言</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- INTERMEDIATE DIVISION -->
<div class="division-section intermediate">
  <div class="division-header">
    <div class="division-icon-large">🟠</div>
    <div class="division-title-group">
      <h2>
        <span class="en-content">Intermediate Division</span>
        <span class="zh-content">中级组</span>
      </h2>
      <p>
        <span class="en-content">For high schoolers with little/no programming experience or advanced middle schoolers</span>
        <span class="zh-content">面向编程经验较少的高中生或优秀初中生</span>
      </p>
    </div>
    <span class="division-badge">
      <span class="en-content">GRADES 9-12</span>
      <span class="zh-content">9-12年级</span>
    </span>
  </div>
  
  <div class="division-content">
    <div class="division-info-card">
      <h3>
        <span>📋</span>
        <span class="en-content">Contest Format</span>
        <span class="zh-content">比赛形式</span>
      </h3>
      <div class="format-item">
        <span class="format-icon">📝</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Short Answer</span>
            <span class="zh-content">简答题</span>
          </div>
          <div class="format-value">
            <span class="en-content">30 min, 6 questions</span>
            <span class="zh-content">30分钟，6道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">💻</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Programming</span>
            <span class="zh-content">编程题</span>
          </div>
          <div class="format-value">
            <span class="en-content">72 hours, 1 problem</span>
            <span class="zh-content">72小时，1道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">⭐</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Max Score</span>
            <span class="zh-content">最高分</span>
          </div>
          <div class="format-value">
            <span class="en-content">10 points per contest</span>
            <span class="zh-content">每场比赛10分</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🏆</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Finals Qualification</span>
            <span class="zh-content">决赛资格</span>
          </div>
          <div class="format-value">
            <span class="en-content">28+ points cumulative</span>
            <span class="zh-content">累计28分以上</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="division-info-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered (12)</span>
        <span class="zh-content">考试内容（12个主题）</span>
      </h3>
      <ul class="topics-list">
        <li><span class="en-content">Computer Number Systems</span><span class="zh-content">计算机数制</span></li>
        <li><span class="en-content">Recursive Functions</span><span class="zh-content">递归函数</span></li>
        <li><span class="en-content">What Does This Program Do?</span><span class="zh-content">程序功能分析</span></li>
        <li><span class="en-content">Prefix/Infix/Postfix Notation</span><span class="zh-content">前缀/中缀/后缀表达式</span></li>
        <li><span class="en-content">Bit-String Flicking</span><span class="zh-content">位串操作</span></li>
        <li><span class="en-content">LISP Programming</span><span class="zh-content">LISP编程</span></li>
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></li>
        <li><span class="en-content">FSAs & Regular Expressions</span><span class="zh-content">有限状态自动机与正则表达式</span></li>
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
        <li><span class="en-content">Digital Electronics</span><span class="zh-content">数字电子学</span></li>
        <li><span class="en-content">Assembly Language</span><span class="zh-content">汇编语言</span></li>
      </ul>
      <p style="font-size: 0.85rem; color: #B45309; margin-top: 1rem; font-style: italic;">
        <span class="en-content">* Same topics as Senior, but less challenging problems</span>
        <span class="zh-content">* 与高级组主题相同，但题目难度较低</span>
      </p>
    </div>
  </div>
</div>

<!-- JUNIOR DIVISION -->
<div class="division-section junior">
  <div class="division-header">
    <div class="division-icon-large">🟢</div>
    <div class="division-title-group">
      <h2>
        <span class="en-content">Junior Division</span>
        <span class="zh-content">初级组</span>
      </h2>
      <p>
        <span class="en-content">For middle school students learning to program (no students above grade 9)</span>
        <span class="zh-content">面向学习编程的初中生（不超过9年级）</span>
      </p>
    </div>
    <span class="division-badge">
      <span class="en-content">GRADES 6-9</span>
      <span class="zh-content">6-9年级</span>
    </span>
  </div>
  
  <div class="division-content">
    <div class="division-info-card">
      <h3>
        <span>📋</span>
        <span class="en-content">Contest Format</span>
        <span class="zh-content">比赛形式</span>
      </h3>
      <div class="format-item">
        <span class="format-icon">📝</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Short Answer</span>
            <span class="zh-content">简答题</span>
          </div>
          <div class="format-value">
            <span class="en-content">30 min, 6 questions</span>
            <span class="zh-content">30分钟，6道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">💻</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Programming</span>
            <span class="zh-content">编程题</span>
          </div>
          <div class="format-value">
            <span class="en-content">72 hours, 1 problem</span>
            <span class="zh-content">72小时，1道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">⭐</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Max Score</span>
            <span class="zh-content">最高分</span>
          </div>
          <div class="format-value">
            <span class="en-content">10 points per contest</span>
            <span class="zh-content">每场比赛10分</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🏆</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Finals Qualification</span>
            <span class="zh-content">决赛资格</span>
          </div>
          <div class="format-value">
            <span class="en-content">28+ points cumulative</span>
            <span class="zh-content">累计28分以上</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="division-info-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered (12)</span>
        <span class="zh-content">考试内容（12个主题）</span>
      </h3>
      <ul class="topics-list">
        <li><span class="en-content">Computer Number Systems</span><span class="zh-content">计算机数制</span></li>
        <li><span class="en-content">Recursive Functions</span><span class="zh-content">递归函数</span></li>
        <li><span class="en-content">What Does This Program Do? - Branching</span><span class="zh-content">程序分析 - 分支</span></li>
        <li><span class="en-content">Prefix/Infix/Postfix Notation</span><span class="zh-content">前缀/中缀/后缀表达式</span></li>
        <li><span class="en-content">Bit-String Flicking</span><span class="zh-content">位串操作</span></li>
        <li><span class="en-content">What Does This Program Do? - Looping</span><span class="zh-content">程序分析 - 循环</span></li>
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></li>
        <li><span class="en-content">What Does This Program Do? - Arrays</span><span class="zh-content">程序分析 - 数组</span></li>
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
        <li><span class="en-content">Digital Electronics</span><span class="zh-content">数字电子学</span></li>
        <li><span class="en-content">What Does This Program Do? - Strings</span><span class="zh-content">程序分析 - 字符串</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- CLASSROOM DIVISION -->
<div class="division-section classroom">
  <div class="division-header">
    <div class="division-icon-large">🔵</div>
    <div class="division-title-group">
      <h2>
        <span class="en-content">Classroom Division</span>
        <span class="zh-content">课堂组</span>
      </h2>
      <p>
        <span class="en-content">Non-programming, ideal for AP CS Principles classes</span>
        <span class="zh-content">无编程，适合AP计算机科学原理课程</span>
      </p>
    </div>
    <span class="division-badge">
      <span class="en-content">ALL GRADES</span>
      <span class="zh-content">所有年级</span>
    </span>
  </div>
  
  <div class="division-content">
    <div class="division-info-card">
      <h3>
        <span>📋</span>
        <span class="en-content">Contest Format</span>
        <span class="zh-content">比赛形式</span>
      </h3>
      <div class="format-item">
        <span class="format-icon">📝</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Short Answer Only</span>
            <span class="zh-content">仅简答题</span>
          </div>
          <div class="format-value">
            <span class="en-content">50 min, 10 questions</span>
            <span class="zh-content">50分钟，10道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🚫</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Programming</span>
            <span class="zh-content">编程题</span>
          </div>
          <div class="format-value">
            <span class="en-content">None required</span>
            <span class="zh-content">无需编程</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">⭐</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Max Score</span>
            <span class="zh-content">最高分</span>
          </div>
          <div class="format-value">
            <span class="en-content">10 points per contest</span>
            <span class="zh-content">每场比赛10分</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🏆</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Finals Qualification</span>
            <span class="zh-content">决赛资格</span>
          </div>
          <div class="format-value">
            <span class="en-content">24+ points cumulative</span>
            <span class="zh-content">累计24分以上</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="division-info-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered (12)</span>
        <span class="zh-content">考试内容（12个主题）</span>
      </h3>
      <ul class="topics-list">
        <li><span class="en-content">Computer Number Systems</span><span class="zh-content">计算机数制</span></li>
        <li><span class="en-content">Recursive Functions</span><span class="zh-content">递归函数</span></li>
        <li><span class="en-content">What Does This Program Do?</span><span class="zh-content">程序功能分析</span></li>
        <li><span class="en-content">Prefix/Infix/Postfix Notation</span><span class="zh-content">前缀/中缀/后缀表达式</span></li>
        <li><span class="en-content">Bit-String Flicking</span><span class="zh-content">位串操作</span></li>
        <li><span class="en-content">LISP</span><span class="zh-content">LISP语言</span></li>
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></li>
        <li><span class="en-content">FSAs & Regular Expressions</span><span class="zh-content">有限状态自动机与正则表达式</span></li>
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
        <li><span class="en-content">Digital Electronics</span><span class="zh-content">数字电子学</span></li>
        <li><span class="en-content">Assembly Language</span><span class="zh-content">汇编语言</span></li>
      </ul>
      <p style="font-size: 0.85rem; color: #1D4ED8; margin-top: 1rem; font-style: italic;">
        <span class="en-content">* Problems from Junior/Intermediate divisions, no programming required</span>
        <span class="zh-content">* 题目来自初级/中级组，无需编程</span>
      </p>
    </div>
  </div>
</div>

<!-- ELEMENTARY DIVISION -->
<div class="division-section elementary">
  <div class="division-header">
    <div class="division-icon-large">🩷</div>
    <div class="division-title-group">
      <h2>
        <span class="en-content">Elementary Division</span>
        <span class="zh-content">小学组</span>
      </h2>
      <p>
        <span class="en-content">Introduction to computer science concepts for young learners</span>
        <span class="zh-content">为低年级学生介绍计算机科学概念</span>
      </p>
    </div>
    <span class="division-badge">
      <span class="en-content">GRADES 3-6</span>
      <span class="zh-content">3-6年级</span>
    </span>
  </div>
  
  <div class="division-content">
    <div class="division-info-card">
      <h3>
        <span>📋</span>
        <span class="en-content">Contest Format</span>
        <span class="zh-content">比赛形式</span>
      </h3>
      <div class="format-item">
        <span class="format-icon">📝</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Short Answer Only</span>
            <span class="zh-content">仅简答题</span>
          </div>
          <div class="format-value">
            <span class="en-content">30 min, 6 questions</span>
            <span class="zh-content">30分钟，6道题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🎯</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Focus</span>
            <span class="zh-content">特点</span>
          </div>
          <div class="format-value">
            <span class="en-content">Single topic per contest</span>
            <span class="zh-content">每场比赛一个主题</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">⭐</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Max Score</span>
            <span class="zh-content">最高分</span>
          </div>
          <div class="format-value">
            <span class="en-content">5 points per contest</span>
            <span class="zh-content">每场比赛5分</span>
          </div>
        </div>
      </div>
      <div class="format-item">
        <span class="format-icon">🏆</span>
        <div class="format-text">
          <div class="format-label">
            <span class="en-content">Finals Qualification</span>
            <span class="zh-content">决赛资格</span>
          </div>
          <div class="format-value">
            <span class="en-content">14+ points cumulative</span>
            <span class="zh-content">累计14分以上</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="division-info-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered (4)</span>
        <span class="zh-content">考试内容（4个主题）</span>
      </h3>
      <ul class="topics-list">
        <li><span class="en-content">Computer Number Systems</span><span class="zh-content">计算机数制</span></li>
        <li><span class="en-content">Prefix/Infix/Postfix Notation</span><span class="zh-content">前缀/中缀/后缀表达式</span></li>
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
      </ul>
      <p style="font-size: 0.85rem; color: #BE185D; margin-top: 1rem; font-style: italic;">
        <span class="en-content">* One topic tested per contest, perfect for beginners!</span>
        <span class="zh-content">* 每场比赛测试一个主题，非常适合初学者！</span>
      </p>
    </div>
  </div>
</div>

<!-- Contest Schedule -->
<div class="schedule-section">
  <h2>
    <span class="en-content">📅 Contest Topics by Round</span>
    <span class="zh-content">📅 各轮比赛主题</span>
  </h2>
  <p>
    <span class="en-content">Senior/Intermediate/Junior divisions - 3 topics per contest</span>
    <span class="zh-content">高级/中级/初级组 - 每场比赛3个主题</span>
  </p>
  
  <div class="contest-schedule-grid">
    <div class="contest-card">
      <div class="contest-number">#1</div>
      <ul class="contest-topics">
        <li><span class="en-content">Number Systems</span><span class="zh-content">数制</span></li>
        <li><span class="en-content">Recursive Functions</span><span class="zh-content">递归函数</span></li>
        <li><span class="en-content">Program Analysis</span><span class="zh-content">程序分析</span></li>
      </ul>
    </div>
    <div class="contest-card">
      <div class="contest-number">#2</div>
      <ul class="contest-topics">
        <li><span class="en-content">Prefix/Infix/Postfix</span><span class="zh-content">前/中/后缀</span></li>
        <li><span class="en-content">Bit-String Flicking</span><span class="zh-content">位串操作</span></li>
        <li><span class="en-content">LISP</span><span class="zh-content">LISP语言</span></li>
      </ul>
    </div>
    <div class="contest-card">
      <div class="contest-number">#3</div>
      <ul class="contest-topics">
        <li><span class="en-content">Boolean Algebra</span><span class="zh-content">布尔代数</span></li>
        <li><span class="en-content">Data Structures</span><span class="zh-content">数据结构</span></li>
        <li><span class="en-content">FSAs & Regex</span><span class="zh-content">FSA与正则</span></li>
      </ul>
    </div>
    <div class="contest-card">
      <div class="contest-number">#4</div>
      <ul class="contest-topics">
        <li><span class="en-content">Graph Theory</span><span class="zh-content">图论</span></li>
        <li><span class="en-content">Digital Electronics</span><span class="zh-content">数字电子</span></li>
        <li><span class="en-content">Assembly Language</span><span class="zh-content">汇编语言</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Finals Section -->
<div class="finals-section">
  <h2>
    <span class="en-content">🏆 ACSL Finals Competition</span>
    <span class="zh-content">🏆 ACSL总决赛</span>
  </h2>
  <p>
    <span class="en-content">Top students from each division are invited to compete in the end-of-year Finals</span>
    <span class="zh-content">各组别顶尖学生将被邀请参加年终总决赛</span>
  </p>
  
  <div class="finals-grid">
    <div class="finals-card">
      <div class="finals-card-icon">💻</div>
      <h3>
        <span class="en-content">Part 1: Programming</span>
        <span class="zh-content">第一部分：编程</span>
      </h3>
      <p>
        <span class="en-content">2 programming problems in 3 hours for Jr/Int/Sr divisions</span>
        <span class="zh-content">初/中/高级组3小时完成2道编程题</span>
      </p>
    </div>
    <div class="finals-card">
      <div class="finals-card-icon">📝</div>
      <h3>
        <span class="en-content">Part 2: Short Problems</span>
        <span class="zh-content">第二部分：简答题</span>
      </h3>
      <p>
        <span class="en-content">20 questions in 1 hour, all divisions participate</span>
        <span class="zh-content">1小时20道题，所有组别参加</span>
      </p>
    </div>
    <div class="finals-card">
      <div class="finals-card-icon">🎖️</div>
      <h3>
        <span class="en-content">Part 3: Awards</span>
        <span class="zh-content">第三部分：颁奖</span>
      </h3>
      <p>
        <span class="en-content">Live stream announcement of medal winners</span>
        <span class="zh-content">直播公布奖牌获得者</span>
      </p>
    </div>
  </div>
  
  <div class="qualification-scores">
    <h3>
      <span class="en-content">📊 Finals Qualification Scores</span>
      <span class="zh-content">📊 决赛晋级分数</span>
    </h3>
    <div class="qual-item">
      <span class="qual-division">Senior / Intermediate / Junior</span>
      <span class="qual-score">28+ pts</span>
    </div>
    <div class="qual-item">
      <span class="qual-division">Classroom</span>
      <span class="qual-score">24+ pts</span>
    </div>
    <div class="qual-item">
      <span class="qual-division">Elementary</span>
      <span class="qual-score">14+ pts</span>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us for ACSL?</span>
      <span class="zh-content">为什么选择我们的ACSL培训？</span>
    </h2>
    <p>
      <span class="en-content">Comprehensive preparation for all ACSL divisions</span>
      <span class="zh-content">针对所有ACSL组别的全面备赛</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">All 12 Topics Covered</span>
        <span class="zh-content">涵盖全部12个主题</span>
      </h3>
      <p>
        <span class="en-content">Systematic training on every ACSL topic with video lessons and practice problems</span>
        <span class="zh-content">系统培训每个ACSL主题，配有视频课程和练习题</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">💻</div>
      <h3>
        <span class="en-content">Programming Practice</span>
        <span class="zh-content">编程练习</span>
      </h3>
      <p>
        <span class="en-content">Hands-on coding in Python, Java, or C++ with past ACSL programming problems</span>
        <span class="zh-content">使用Python、Java或C++进行实践编程，练习历年ACSL编程题</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Past Contests</span>
        <span class="zh-content">历年真题</span>
      </h3>
      <p>
        <span class="en-content">Access to years of previous ACSL contests for comprehensive practice</span>
        <span class="zh-content">获取多年ACSL历年真题进行全面练习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Division-Specific Prep</span>
        <span class="zh-content">组别针对性备赛</span>
      </h3>
      <p>
        <span class="en-content">Customized training paths for Elementary through Senior divisions</span>
        <span class="zh-content">从小学组到高级组的定制培训路径</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🏆</div>
      <h3>
        <span class="en-content">Finals Preparation</span>
        <span class="zh-content">决赛准备</span>
      </h3>
      <p>
        <span class="en-content">Intensive training for students aiming to qualify for ACSL Finals</span>
        <span class="zh-content">为志在晋级ACSL决赛的学生提供强化培训</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 8 students for personalized attention and feedback</span>
        <span class="zh-content">每班最多8人，个性化关注和反馈</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' ACSL Achievements</span>
    <span class="zh-content">🏆 我们学生的ACSL成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">20+</span>
      <div class="success-label">
        <span class="en-content">Finals Qualifiers</span>
        <span class="zh-content">决赛晋级者</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🏅</div>
      <span class="success-number" style="font-size: 2.2rem;">Top&nbsp;10%</span>
      <div class="success-label">
        <span class="en-content">Worldwide Ranking</span>
        <span class="zh-content">全球排名</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">95%</span>
      <div class="success-label">
        <span class="en-content">Score Improvement</span>
        <span class="zh-content">成绩提升率</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">5</span>
      <div class="success-label">
        <span class="en-content">Gold Medals</span>
        <span class="zh-content">金牌</span>
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
      <span class="testimonial-badge finals">Finals</span>
      <p class="testimonial-text">
        <span class="en-content">The systematic approach to all 12 ACSL topics made the difference. I qualified for Finals in my first year and won a silver medal! The programming practice was especially helpful.</span>
        <span class="zh-content">对全部12个ACSL主题的系统学习带来了改变。我第一年就晋级决赛并获得银牌！编程练习特别有帮助。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Jason T.</h4>
          <p>
            <span class="en-content">Senior Division, Finals Silver</span>
            <span class="zh-content">高级组，决赛银牌</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge senior">Senior</span>
      <p class="testimonial-text">
        <span class="en-content">ACSL topics like Boolean algebra and data structures directly helped me in AP Computer Science A. I scored perfect on all 4 contests and got invited to Finals!</span>
        <span class="zh-content">布尔代数和数据结构等ACSL主题直接帮助了我的AP计算机科学A课程。我在全部4场比赛中获得满分并被邀请参加决赛！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Emily W.</h4>
          <p>
            <span class="en-content">Senior Division, Perfect Score</span>
            <span class="zh-content">高级组，满分</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge junior">Junior</span>
      <p class="testimonial-text">
        <span class="en-content">Starting in Elementary division, I learned the basics of computer science. Now in Junior division, I'm ready to tackle programming problems. ACSL has been an amazing journey!</span>
        <span class="zh-content">从小学组开始，我学习了计算机科学的基础知识。现在在初级组，我已经准备好解决编程问题了。ACSL是一段精彩的旅程！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👦</div>
        <div class="testimonial-info">
          <h4>Ryan L.</h4>
          <p>
            <span class="en-content">Junior Division, 7th Grade</span>
            <span class="zh-content">初级组，7年级</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Master Computer Science with ACSL!</span>
    <span class="zh-content">通过ACSL掌握计算机科学！</span>
  </h2>
  <p>
    <span class="en-content">Join our training program and compete at the highest level</span>
    <span class="zh-content">加入我们的培训计划，在最高水平竞争</span>
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
