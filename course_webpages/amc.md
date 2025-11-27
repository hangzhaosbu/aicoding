---
layout: default
title: AMC 8/10/12 Competition Training
title_zh: AMC 8/10/12 数学竞赛培训
description: Master the American Mathematics Competitions & Qualify for AIME
description_zh: 征服美国数学竞赛，晋级AIME
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

  @keyframes medalShine {
    0%, 100% { 
      filter: drop-shadow(0 0 8px currentColor);
    }
    50% { 
      filter: drop-shadow(0 0 20px currentColor);
    }
  }

  @keyframes numberPop {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.1); }
  }

  /* Course Hero - Ultra Premium Multi-Color Theme */
  .course-hero {
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 25%, #EC4899 50%, #F59E0B 75%, #10B981 100%);
    background-size: 400% 400%;
    animation: gradientWave 20s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(59, 130, 246, 0.4);
    min-height: 500px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '∑';
    position: absolute;
    font-size: 20rem;
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
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
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

  .maa-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
    color: #1F2937;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 700;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(255, 215, 0, 0.4);
    animation: pulse 2s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .maa-badge::before {
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
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 50%, #EC4899 100%);
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

  /* What is AMC Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #3B82F6, #8B5CF6, #EC4899, #F59E0B) 1;
  }

  .intro-section::before {
    content: 'π';
    position: absolute;
    font-size: 15rem;
    opacity: 0.03;
    right: -30px;
    bottom: -50px;
    font-family: "Times New Roman", serif;
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
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(59, 130, 246, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Competition Pathway Section */
  .pathway-section {
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 50%, #FCE7F3 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .pathway-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 100%);
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

  .pathway-flow {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0.8rem;
    flex-wrap: nowrap;
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 1rem;
  }

  .pathway-item {
    background: white;
    padding: 1.2rem 1rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s ease;
    min-width: 100px;
    flex: 1;
    max-width: 130px;
  }

  .pathway-item:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .pathway-item.amc8 { border-top: 4px solid #3B82F6; }
  .pathway-item.amc10 { border-top: 4px solid #8B5CF6; }
  .pathway-item.amc12 { border-top: 4px solid #EC4899; }
  .pathway-item.aime { border-top: 4px solid #F59E0B; }
  .pathway-item.usamo { border-top: 4px solid #10B981; }
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
    color: #9CA3AF;
    flex-shrink: 0;
  }

  @media (max-width: 1000px) {
    .pathway-flow {
      flex-wrap: wrap;
      max-width: 600px;
    }
    .pathway-item {
      min-width: 120px;
      max-width: 150px;
    }
    .pathway-arrow:nth-of-type(3) {
      display: none;
    }
  }

  @media (max-width: 768px) {
    .pathway-flow {
      flex-direction: column;
      max-width: 200px;
    }
    .pathway-arrow {
      transform: rotate(90deg);
    }
  }

  /* AMC Competition Sections - Individual */
  .amc-section {
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .amc-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
    animation: shimmer 4s infinite;
  }

  /* AMC 8 Section - Blue Theme */
  .amc8-section {
    background: linear-gradient(135deg, #3B82F6 0%, #2563EB 50%, #1D4ED8 100%);
    box-shadow: 0 30px 60px rgba(59, 130, 246, 0.3);
  }

  /* AMC 10 Section - Purple Theme */
  .amc10-section {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 50%, #6D28D9 100%);
    box-shadow: 0 30px 60px rgba(139, 92, 246, 0.3);
  }

  /* AMC 12 Section - Pink/Gold Theme */
  .amc12-section {
    background: linear-gradient(135deg, #EC4899 0%, #DB2777 50%, #BE185D 100%);
    box-shadow: 0 30px 60px rgba(236, 72, 153, 0.3);
  }

  .amc-section-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: start;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .amc-section-content {
      grid-template-columns: 1fr;
    }
  }

  .amc-section-header {
    color: white;
  }

  .amc-level-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 0.5rem 1.5rem;
    border-radius: 25px;
    font-weight: 700;
    font-size: 0.9rem;
    margin-bottom: 1rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .amc-section-header h2 {
    color: white !important;
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  }

  .amc-section-header p {
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
  }

  .amc-details {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }

  .amc-detail-item {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    padding: 1rem;
    border-radius: 15px;
    border: 1px solid rgba(255, 255, 255, 0.2);
  }

  .amc-detail-label {
    font-size: 0.85rem;
    opacity: 0.8;
    margin-bottom: 0.3rem;
    color: white;
  }

  .amc-detail-value {
    font-size: 1.1rem;
    font-weight: 700;
    color: white;
  }

  /* Topics Cards */
  .amc-topics-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .amc-topics-card h3 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .amc-topics-list {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: 1fr;
    gap: 0.6rem;
  }

  .amc-topics-list li {
    padding: 0.6rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
    border-bottom: 1px solid #F3F4F6;
  }

  .amc-topics-list li:last-child {
    border-bottom: none;
  }

  .amc-topics-list li::before {
    content: '→';
    font-weight: bold;
    margin-right: 0.8rem;
    flex-shrink: 0;
  }

  .amc8-section .amc-topics-list li::before { color: #3B82F6; }
  .amc10-section .amc-topics-list li::before { color: #8B5CF6; }
  .amc12-section .amc-topics-list li::before { color: #EC4899; }

  /* Awards Section */
  .awards-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .awards-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .awards-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .awards-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .awards-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
    }
  }

  .award-card {
    text-align: center;
    padding: 2rem;
    border-radius: 20px;
    transition: all 0.4s ease;
    position: relative;
  }

  .award-card:hover {
    transform: translateY(-8px);
  }

  .award-card.amc8 {
    background: linear-gradient(135deg, #DBEAFE 0%, #BFDBFE 100%);
  }

  .award-card.amc10 {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
  }

  .award-card.amc12 {
    background: linear-gradient(135deg, #FCE7F3 0%, #FBCFE8 100%);
  }

  .award-card h3 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1.5rem;
  }

  .award-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.8rem 0;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  }

  .award-item:last-child {
    border-bottom: none;
  }

  .award-name {
    font-weight: 600;
    color: #4B5563;
    font-size: 0.95rem;
  }

  .award-score {
    font-weight: 700;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.9rem;
  }

  .award-card.amc8 .award-score { background: #3B82F6; color: white; }
  .award-card.amc10 .award-score { background: #8B5CF6; color: white; }
  .award-card.amc12 .award-score { background: #EC4899; color: white; }

  /* Curriculum Section - 2x2 Layout */
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
    border-left: 5px solid;
  }

  .curriculum-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-left-color: #3B82F6;
    background: linear-gradient(to right, rgba(59, 130, 246, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #8B5CF6;
    background: linear-gradient(to right, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-left-color: #EC4899;
    background: linear-gradient(to right, rgba(236, 72, 153, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-left-color: #F59E0B;
    background: linear-gradient(to right, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }

  .curriculum-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(59, 130, 246, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .curriculum-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(59, 130, 246, 0.15);
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

  .curriculum-card:nth-child(1) .curriculum-icon { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .curriculum-card:nth-child(2) .curriculum-icon { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .curriculum-card:nth-child(3) .curriculum-icon { background: linear-gradient(135deg, #EC4899, #DB2777); }
  .curriculum-card:nth-child(4) .curriculum-icon { background: linear-gradient(135deg, #F59E0B, #D97706); }

  .curriculum-title-group {
    flex: 1;
  }

  .curriculum-title {
    font-size: 1.3rem;
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

  .curriculum-card:nth-child(1) .curriculum-topics li::before { color: #3B82F6; }
  .curriculum-card:nth-child(2) .curriculum-topics li::before { color: #8B5CF6; }
  .curriculum-card:nth-child(3) .curriculum-topics li::before { color: #EC4899; }
  .curriculum-card:nth-child(4) .curriculum-topics li::before { color: #F59E0B; }

  /* Competition Dates Section */
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
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
  }

  .dates-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .dates-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .dates-grid {
      grid-template-columns: 1fr;
      max-width: 400px;
    }
  }

  .date-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .date-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .date-card.amc8 { border-top: 5px solid #3B82F6; }
  .date-card.amc10 { border-top: 5px solid #8B5CF6; }
  .date-card.amc12 { border-top: 5px solid #EC4899; }

  .date-card h3 {
    font-size: 1.5rem;
    font-weight: 800;
    margin-bottom: 1rem;
  }

  .date-card.amc8 h3 { color: #3B82F6; }
  .date-card.amc10 h3 { color: #8B5CF6; }
  .date-card.amc12 h3 { color: #EC4899; }

  .date-value {
    font-size: 1.1rem;
    color: #4B5563;
    margin-bottom: 0.5rem;
  }

  .date-note {
    font-size: 0.85rem;
    color: #9CA3AF;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 50%, #FCE7F3 100%);
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
    border-color: #3B82F6;
    box-shadow: 0 20px 40px rgba(59, 130, 246, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(59, 130, 246, 0.3);
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
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 50%, #EC4899 100%);
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
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(59, 130, 246, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .success-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 100%);
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
    background: linear-gradient(135deg, #EEF2FF 0%, #E0E7FF 50%, #FCE7F3 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 100%);
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
    color: #3B82F6;
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

  .testimonial-badge.aime { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .testimonial-badge.dhr { background: linear-gradient(135deg, #10B981, #059669); }
  .testimonial-badge.hr { background: linear-gradient(135deg, #3B82F6, #2563EB); }

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
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 100%);
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
    background: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 25%, #EC4899 50%, #F59E0B 75%, #10B981 100%);
    background-size: 400% 400%;
    animation: gradientWave 15s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(59, 130, 246, 0.4);
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
    color: #3B82F6;
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
    background: linear-gradient(90deg, transparent, rgba(59, 130, 246, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #1D4ED8;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #3B82F6;
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
    .pathway-section,
    .why-choose-section,
    .success-section,
    .awards-section,
    .dates-section {
      padding: 3rem 1.5rem;
    }

    .amc-section {
      padding: 3rem 1.5rem;
    }

    .amc-section-header h2 {
      font-size: 2rem;
    }

    .maa-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="maa-badge">
    <span class="en-content">SINCE 1950</span>
    <span class="zh-content">始于1950年</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">∑</span>
    <span class="floating-icon">π</span>
    <span class="floating-icon">∫</span>
    <span class="floating-icon">√</span>
    <span class="floating-icon">∞</span>
    <span class="floating-icon">Δ</span>
    <span class="floating-icon">θ</span>
  </div>
  <h1>
    <span class="en-content">AMC 8 / 10 / 12 Training</span>
    <span class="zh-content">AMC 8 / 10 / 12 培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">America's Premier K-12 Math Competition Since 1950</span>
    <span class="zh-content">美国首屈一指的K-12数学竞赛，始于1950年</span>
  </p>
  <div class="hero-badge">
    <span>🏆</span>
    <span class="en-content">Pathway to AIME → USAMO → IMO</span>
    <span class="zh-content">通往 AIME → USAMO → IMO 的道路</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">300K+</span>
      <span class="hero-stat-label">
        <span class="en-content">Annual Participants</span>
        <span class="zh-content">年度参赛者</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">50+</span>
      <span class="hero-stat-label">
        <span class="en-content">States & 30 Countries</span>
        <span class="zh-content">州与30个国家</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">75</span>
      <span class="hero-stat-label">
        <span class="en-content">Years of Excellence</span>
        <span class="zh-content">年卓越历史</span>
      </span>
    </div>
  </div>
</div>

<!-- What is AMC -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is the AMC?</span>
        <span class="zh-content">什么是AMC？</span>
      </h2>
      <p>
        <span class="en-content">
          Founded in 1950, the American Mathematics Competitions (AMC) is the preeminent math competition 
          for students K-12, organized by the Mathematical Association of America (MAA). Today, over 300,000 
          students in 50 states and over 30 countries take the AMC to bolster their confidence and passion for math.
        </span>
        <span class="zh-content">
          美国数学竞赛（AMC）始于1950年，是由美国数学协会（MAA）组织的K-12学生首选数学竞赛。
          如今，超过30万名来自50个州和30多个国家的学生参加AMC，以增强他们对数学的信心和热情。
        </span>
      </p>
      <p>
        <span class="en-content">
          AMC scores are highly valued by top universities including MIT, Caltech, Stanford, and Ivy League schools. 
          Both MIT and Caltech have entry blanks on their official admission forms for AMC and AIME scores!
        </span>
        <span class="zh-content">
          AMC成绩被MIT、Caltech、Stanford和常春藤盟校等顶尖大学高度重视。
          MIT和Caltech的官方录取申请表上都有AMC和AIME成绩的填写栏！
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🎓</span>
          <span class="intro-highlight-text">
            <span class="en-content">Top College Recognition</span>
            <span class="zh-content">顶尖大学认可</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌎</span>
          <span class="intro-highlight-text">
            <span class="en-content">International Prestige</span>
            <span class="zh-content">国际声望</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">📈</span>
          <span class="intro-highlight-text">
            <span class="en-content">Problem-Solving Skills</span>
            <span class="zh-content">问题解决能力</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏅</span>
          <span class="intro-highlight-text">
            <span class="en-content">Path to Math Olympiad</span>
            <span class="zh-content">通往数学奥赛</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 8rem; opacity: 0.8; animation: float 6s ease-in-out infinite; background: linear-gradient(135deg, #3B82F6, #8B5CF6, #EC4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 900; font-family: 'Times New Roman', serif;">AMC</div>
    </div>
  </div>
</div>

<!-- Competition Pathway -->
<div class="pathway-section">
  <h2>
    <span class="en-content">🏆 The Math Olympiad Pathway</span>
    <span class="zh-content">🏆 数学奥赛晋级之路</span>
  </h2>
  <p>
    <span class="en-content">Your journey from AMC to the International Mathematical Olympiad</span>
    <span class="zh-content">从AMC到国际数学奥林匹克的进阶之路</span>
  </p>
  
  <div class="pathway-flow">
    <div class="pathway-item amc8">
      <div class="pathway-icon">📘</div>
      <div class="pathway-name">AMC 8</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item amc10">
      <div class="pathway-icon">📙</div>
      <div class="pathway-name">AMC 10</div>
    </div>
    <span class="pathway-arrow">→</span>
    <div class="pathway-item amc12">
      <div class="pathway-icon">📕</div>
      <div class="pathway-name">AMC 12</div>
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
    <div class="pathway-item imo">
      <div class="pathway-icon">🌟</div>
      <div class="pathway-name">IMO</div>
    </div>
  </div>
</div>

<!-- AMC 8 Section -->
<div class="amc-section amc8-section">
  <div class="amc-section-content">
    <div class="amc-section-header">
      <span class="amc-level-badge">
        <span class="en-content">MIDDLE SCHOOL</span>
        <span class="zh-content">初中组</span>
      </span>
      <h2>AMC 8</h2>
      <p>
        <span class="en-content">
          The AMC 8 is a great way to introduce younger students to mathematical problem-solving 
          beyond the standard school curriculum. It focuses on middle school mathematics topics 
          and builds a strong foundation for future competitions.
        </span>
        <span class="zh-content">
          AMC 8是向年轻学生介绍超越标准学校课程的数学问题解决能力的绝佳方式。
          它专注于初中数学主题，为未来的竞赛奠定坚实基础。
        </span>
      </p>
      <div class="amc-details">
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Questions</span>
            <span class="zh-content">题目数量</span>
          </div>
          <div class="amc-detail-value">25</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Time Limit</span>
            <span class="zh-content">时间限制</span>
          </div>
          <div class="amc-detail-value">40 min</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Eligibility</span>
            <span class="zh-content">参赛资格</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Grade 8 & below</span>
            <span class="zh-content">8年级及以下</span>
          </div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Max Age</span>
            <span class="zh-content">最大年龄</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Under 15.5</span>
            <span class="zh-content">15.5岁以下</span>
          </div>
        </div>
      </div>
    </div>
    <div class="amc-topics-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered</span>
        <span class="zh-content">考试内容</span>
      </h3>
      <ul class="amc-topics-list">
        <li><span class="en-content">Counting & Probability</span><span class="zh-content">计数与概率</span></li>
        <li><span class="en-content">Estimation & Proportional Reasoning</span><span class="zh-content">估算与比例推理</span></li>
        <li><span class="en-content">Elementary Geometry</span><span class="zh-content">基础几何</span></li>
        <li><span class="en-content">Pythagorean Theorem</span><span class="zh-content">勾股定理</span></li>
        <li><span class="en-content">Spatial Visualization</span><span class="zh-content">空间可视化</span></li>
        <li><span class="en-content">Interpreting Graphs & Tables</span><span class="zh-content">图表解读</span></li>
        <li><span class="en-content">Beginning Algebra</span><span class="zh-content">初级代数</span></li>
        <li><span class="en-content">Linear Functions</span><span class="zh-content">线性函数</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- AMC 10 Section -->
<div class="amc-section amc10-section">
  <div class="amc-section-content">
    <div class="amc-section-header">
      <span class="amc-level-badge">
        <span class="en-content">HIGH SCHOOL I</span>
        <span class="zh-content">高中初级组</span>
      </span>
      <h2>AMC 10</h2>
      <p>
        <span class="en-content">
          The AMC 10 provides students with an opportunity to develop their problem-solving skills. 
          It serves as the first step in qualifying for the USA team in prestigious international 
          mathematics competitions, including the International Mathematical Olympiad.
        </span>
        <span class="zh-content">
          AMC 10为学生提供发展问题解决能力的机会。它是获得美国代表队资格参加国际数学奥林匹克等
          著名国际数学竞赛的第一步。
        </span>
      </p>
      <div class="amc-details">
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Questions</span>
            <span class="zh-content">题目数量</span>
          </div>
          <div class="amc-detail-value">25</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Time Limit</span>
            <span class="zh-content">时间限制</span>
          </div>
          <div class="amc-detail-value">75 min</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Eligibility</span>
            <span class="zh-content">参赛资格</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Grade 10 & below</span>
            <span class="zh-content">10年级及以下</span>
          </div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Max Age</span>
            <span class="zh-content">最大年龄</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Under 17.5</span>
            <span class="zh-content">17.5岁以下</span>
          </div>
        </div>
      </div>
    </div>
    <div class="amc-topics-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered</span>
        <span class="zh-content">考试内容</span>
      </h3>
      <ul class="amc-topics-list">
        <li><span class="en-content">Elementary Algebra</span><span class="zh-content">初等代数</span></li>
        <li><span class="en-content">Basic Geometry</span><span class="zh-content">基础几何</span></li>
        <li><span class="en-content">Area & Volume Formulas</span><span class="zh-content">面积与体积公式</span></li>
        <li><span class="en-content">Elementary Number Theory</span><span class="zh-content">初等数论</span></li>
        <li><span class="en-content">Elementary Probability</span><span class="zh-content">初等概率</span></li>
        <li><span class="en-content">Coordinate Geometry</span><span class="zh-content">坐标几何</span></li>
        <li><span class="en-content">Algebraic Expressions</span><span class="zh-content">代数表达式</span></li>
        <li><span class="en-content">Sequences & Series</span><span class="zh-content">数列与级数</span></li>
      </ul>
      <p style="margin-top: 1rem; font-size: 0.9rem; color: #9CA3AF;">
        <span class="en-content">* Excludes: Trigonometry, Advanced Algebra, Advanced Geometry</span>
        <span class="zh-content">* 不包含：三角函数、高等代数、高等几何</span>
      </p>
    </div>
  </div>
</div>

<!-- AMC 12 Section -->
<div class="amc-section amc12-section">
  <div class="amc-section-content">
    <div class="amc-section-header">
      <span class="amc-level-badge">
        <span class="en-content">HIGH SCHOOL II</span>
        <span class="zh-content">高中高级组</span>
      </span>
      <h2>AMC 12</h2>
      <p>
        <span class="en-content">
          The AMC 12 helps students develop their problem-solving abilities and serves as the 
          first step in qualifying for the USA team in prestigious international mathematics 
          competitions. It covers the full high school mathematics curriculum.
        </span>
        <span class="zh-content">
          AMC 12帮助学生发展问题解决能力，是获得美国代表队资格参加著名国际数学竞赛的第一步。
          它涵盖完整的高中数学课程。
        </span>
      </p>
      <div class="amc-details">
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Questions</span>
            <span class="zh-content">题目数量</span>
          </div>
          <div class="amc-detail-value">25</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Time Limit</span>
            <span class="zh-content">时间限制</span>
          </div>
          <div class="amc-detail-value">75 min</div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Eligibility</span>
            <span class="zh-content">参赛资格</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Grade 12 & below</span>
            <span class="zh-content">12年级及以下</span>
          </div>
        </div>
        <div class="amc-detail-item">
          <div class="amc-detail-label">
            <span class="en-content">Max Age</span>
            <span class="zh-content">最大年龄</span>
          </div>
          <div class="amc-detail-value">
            <span class="en-content">Under 19.5</span>
            <span class="zh-content">19.5岁以下</span>
          </div>
        </div>
      </div>
    </div>
    <div class="amc-topics-card">
      <h3>
        <span>📚</span>
        <span class="en-content">Topics Covered</span>
        <span class="zh-content">考试内容</span>
      </h3>
      <ul class="amc-topics-list">
        <li><span class="en-content">All AMC 10 Topics</span><span class="zh-content">所有AMC 10内容</span></li>
        <li><span class="en-content">Trigonometry</span><span class="zh-content">三角函数</span></li>
        <li><span class="en-content">Advanced Algebra</span><span class="zh-content">高等代数</span></li>
        <li><span class="en-content">Advanced Geometry</span><span class="zh-content">高等几何</span></li>
        <li><span class="en-content">Logarithms & Exponentials</span><span class="zh-content">对数与指数</span></li>
        <li><span class="en-content">Complex Numbers</span><span class="zh-content">复数</span></li>
        <li><span class="en-content">Polynomials</span><span class="zh-content">多项式</span></li>
        <li><span class="en-content">Functions & Graphs</span><span class="zh-content">函数与图像</span></li>
      </ul>
      <p style="margin-top: 1rem; font-size: 0.9rem; color: #9CA3AF;">
        <span class="en-content">* Excludes: Calculus</span>
        <span class="zh-content">* 不包含：微积分</span>
      </p>
    </div>
  </div>
</div>

<!-- Awards Section -->
<div class="awards-section">
  <h2>
    <span class="en-content">🏅 Awards & Recognition</span>
    <span class="zh-content">🏅 奖项与认可</span>
  </h2>
  <p>
    <span class="en-content">2024-2025 Award Cutoff Scores</span>
    <span class="zh-content">2024-2025年奖项分数线</span>
  </p>
  
  <div class="awards-grid">
    <div class="award-card amc8">
      <h3>AMC 8</h3>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Distinguished Honor Roll (Top 1%)</span>
          <span class="zh-content">杰出荣誉榜（前1%）</span>
        </span>
        <span class="award-score">22+</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Honor Roll (Top 5%)</span>
          <span class="zh-content">荣誉榜（前5%）</span>
        </span>
        <span class="award-score">18+</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Achievement Roll (≤6th)</span>
          <span class="zh-content">成就奖（6年级以下）</span>
        </span>
        <span class="award-score">15+</span>
      </div>
    </div>
    
    <div class="award-card amc10">
      <h3>AMC 10</h3>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">AIME Qualification</span>
          <span class="zh-content">AIME晋级</span>
        </span>
        <span class="award-score">~100</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Distinguished Honor Roll (Top 1%)</span>
          <span class="zh-content">杰出荣誉榜（前1%）</span>
        </span>
        <span class="award-score">~135</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Honor Roll (Top 5%)</span>
          <span class="zh-content">荣誉榜（前5%）</span>
        </span>
        <span class="award-score">~110</span>
      </div>
    </div>
    
    <div class="award-card amc12">
      <h3>AMC 12</h3>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">AIME Qualification</span>
          <span class="zh-content">AIME晋级</span>
        </span>
        <span class="award-score">~85</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Distinguished Honor Roll (Top 1%)</span>
          <span class="zh-content">杰出荣誉榜（前1%）</span>
        </span>
        <span class="award-score">~137</span>
      </div>
      <div class="award-item">
        <span class="award-name">
          <span class="en-content">Honor Roll (Top 5%)</span>
          <span class="zh-content">荣誉榜（前5%）</span>
        </span>
        <span class="award-score">~115</span>
      </div>
    </div>
  </div>
</div>

<!-- Competition Dates -->
<div class="dates-section">
  <h2>
    <span class="en-content">📅 2025-2026 Competition Dates</span>
    <span class="zh-content">📅 2025-2026年竞赛日期</span>
  </h2>
  <p>
    <span class="en-content">Mark your calendar for these important dates</span>
    <span class="zh-content">在日历上标记这些重要日期</span>
  </p>
  
  <div class="dates-grid">
    <div class="date-card amc10">
      <h3>AMC 10/12 A</h3>
      <div class="date-value">
        <span class="en-content">November 5, 2025</span>
        <span class="zh-content">2025年11月5日</span>
      </div>
      <div class="date-note">
        <span class="en-content">First test date option</span>
        <span class="zh-content">第一考试日期选项</span>
      </div>
    </div>
    
    <div class="date-card amc12">
      <h3>AMC 10/12 B</h3>
      <div class="date-value">
        <span class="en-content">November 13, 2025</span>
        <span class="zh-content">2025年11月13日</span>
      </div>
      <div class="date-note">
        <span class="en-content">Second test date option</span>
        <span class="zh-content">第二考试日期选项</span>
      </div>
    </div>
    
    <div class="date-card amc8">
      <h3>AMC 8</h3>
      <div class="date-value">
        <span class="en-content">January 22-28, 2026</span>
        <span class="zh-content">2026年1月22-28日</span>
      </div>
      <div class="date-note">
        <span class="en-content">One-week testing window</span>
        <span class="zh-content">一周考试窗口</span>
      </div>
    </div>
  </div>
</div>

<!-- Curriculum Section -->
<div class="curriculum-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Our Training Curriculum</span>
      <span class="zh-content">我们的培训课程</span>
    </h2>
    <p>
      <span class="en-content">Comprehensive preparation for all AMC levels</span>
      <span class="zh-content">全面覆盖所有AMC级别的备考课程</span>
    </p>
  </div>

  <div class="curriculum-cards">
    <!-- Algebra -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">📐</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Algebra Mastery</span>
            <span class="zh-content">代数精通</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Foundation to Advanced</span>
            <span class="zh-content">从基础到高级</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Polynomial Operations</span><span class="zh-content">多项式运算</span></li>
        <li><span class="en-content">Systems of Equations</span><span class="zh-content">方程组</span></li>
        <li><span class="en-content">Inequalities</span><span class="zh-content">不等式</span></li>
        <li><span class="en-content">Functions & Graphs</span><span class="zh-content">函数与图像</span></li>
        <li><span class="en-content">Sequences & Series</span><span class="zh-content">数列与级数</span></li>
        <li><span class="en-content">Complex Numbers</span><span class="zh-content">复数</span></li>
      </ul>
    </div>

    <!-- Geometry -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">📏</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Geometry Excellence</span>
            <span class="zh-content">几何卓越</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Plane & Solid Geometry</span>
            <span class="zh-content">平面与立体几何</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Triangle Properties</span><span class="zh-content">三角形性质</span></li>
        <li><span class="en-content">Circle Theorems</span><span class="zh-content">圆的定理</span></li>
        <li><span class="en-content">Coordinate Geometry</span><span class="zh-content">坐标几何</span></li>
        <li><span class="en-content">3D Geometry</span><span class="zh-content">三维几何</span></li>
        <li><span class="en-content">Trigonometry</span><span class="zh-content">三角函数</span></li>
        <li><span class="en-content">Transformations</span><span class="zh-content">变换</span></li>
      </ul>
    </div>

    <!-- Number Theory -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🔢</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Number Theory</span>
            <span class="zh-content">数论</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Primes & Divisibility</span>
            <span class="zh-content">质数与整除</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Prime Factorization</span><span class="zh-content">质因数分解</span></li>
        <li><span class="en-content">GCD & LCM</span><span class="zh-content">最大公因数与最小公倍数</span></li>
        <li><span class="en-content">Modular Arithmetic</span><span class="zh-content">模运算</span></li>
        <li><span class="en-content">Diophantine Equations</span><span class="zh-content">丢番图方程</span></li>
        <li><span class="en-content">Divisibility Rules</span><span class="zh-content">整除规则</span></li>
        <li><span class="en-content">Number Bases</span><span class="zh-content">进制转换</span></li>
      </ul>
    </div>

    <!-- Combinatorics -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🎲</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Combinatorics & Probability</span>
            <span class="zh-content">组合与概率</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Counting Techniques</span>
            <span class="zh-content">计数技巧</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Permutations & Combinations</span><span class="zh-content">排列与组合</span></li>
        <li><span class="en-content">Probability Theory</span><span class="zh-content">概率论</span></li>
        <li><span class="en-content">Pascal's Triangle</span><span class="zh-content">帕斯卡三角</span></li>
        <li><span class="en-content">Inclusion-Exclusion</span><span class="zh-content">容斥原理</span></li>
        <li><span class="en-content">Expected Value</span><span class="zh-content">期望值</span></li>
        <li><span class="en-content">Pigeonhole Principle</span><span class="zh-content">鸽巢原理</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us?</span>
      <span class="zh-content">为什么选择我们？</span>
    </h2>
    <p>
      <span class="en-content">Your path to AMC success and beyond</span>
      <span class="zh-content">通往AMC成功及更高目标的道路</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Targeted Practice</span>
        <span class="zh-content">针对性练习</span>
      </h3>
      <p>
        <span class="en-content">Thousands of past AMC problems organized by topic and difficulty</span>
        <span class="zh-content">按主题和难度整理的数千道AMC历年真题</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Progress Tracking</span>
        <span class="zh-content">进度追踪</span>
      </h3>
      <p>
        <span class="en-content">Regular mock tests and detailed performance analytics</span>
        <span class="zh-content">定期模拟测试和详细的成绩分析</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🧠</div>
      <h3>
        <span class="en-content">Problem-Solving Strategies</span>
        <span class="zh-content">问题解决策略</span>
      </h3>
      <p>
        <span class="en-content">Learn efficient techniques used by top scorers</span>
        <span class="zh-content">学习高分选手使用的高效技巧</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">⏱️</div>
      <h3>
        <span class="en-content">Time Management</span>
        <span class="zh-content">时间管理</span>
      </h3>
      <p>
        <span class="en-content">Master pacing strategies for timed competition conditions</span>
        <span class="zh-content">掌握限时竞赛条件下的节奏策略</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🏆</div>
      <h3>
        <span class="en-content">AIME Pathway</span>
        <span class="zh-content">AIME晋级之路</span>
      </h3>
      <p>
        <span class="en-content">Structured progression from AMC to AIME qualification</span>
        <span class="zh-content">从AMC到AIME晋级的系统化进阶</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 8 students for personalized attention</span>
        <span class="zh-content">每班最多8人，个性化关注</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' Achievements</span>
    <span class="zh-content">🏆 我们学生的成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">50+</span>
      <div class="success-label">
        <span class="en-content">AIME Qualifiers</span>
        <span class="zh-content">AIME晋级者</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">⭐</div>
      <span class="success-number">85%</span>
      <div class="success-label">
        <span class="en-content">Honor Roll Rate</span>
        <span class="zh-content">荣誉榜比例</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">+30</span>
      <div class="success-label">
        <span class="en-content">Avg Score Improvement</span>
        <span class="zh-content">平均分数提升</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🎯</div>
      <span class="success-number">5</span>
      <div class="success-label">
        <span class="en-content">Perfect Scorers</span>
        <span class="zh-content">满分获得者</span>
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
      <span class="testimonial-badge aime">AIME Qualifier</span>
      <p class="testimonial-text">
        <span class="en-content">I went from scoring 80 on AMC 10 to qualifying for AIME in just one year. The structured curriculum and problem-solving strategies made all the difference!</span>
        <span class="zh-content">我在短短一年内从AMC 10的80分进步到晋级AIME。系统化的课程和问题解决策略起到了关键作用！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Kevin Z.</h4>
          <p>
            <span class="en-content">9th Grade, AMC 10 Score: 112</span>
            <span class="zh-content">9年级，AMC 10成绩：112</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge dhr">DHR</span>
      <p class="testimonial-text">
        <span class="en-content">As a 6th grader, I achieved Distinguished Honor Roll on AMC 8! The teachers helped me understand concepts way beyond my grade level in a fun way.</span>
        <span class="zh-content">作为6年级学生，我在AMC 8获得了杰出荣誉榜！老师们以有趣的方式帮我理解远超年级水平的概念。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Emily L.</h4>
          <p>
            <span class="en-content">6th Grade, AMC 8 Score: 23</span>
            <span class="zh-content">6年级，AMC 8成绩：23</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge hr">Honor Roll</span>
      <p class="testimonial-text">
        <span class="en-content">The mock tests and time management training were invaluable. I finally learned how to pace myself and not panic during the actual competition.</span>
        <span class="zh-content">模拟测试和时间管理培训非常宝贵。我终于学会了如何掌控节奏，在实际竞赛中不再慌张。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Jason W.</h4>
          <p>
            <span class="en-content">11th Grade, AMC 12 Score: 118</span>
            <span class="zh-content">11年级，AMC 12成绩：118</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Your AMC Journey Today!</span>
    <span class="zh-content">今天开始你的AMC之旅！</span>
  </h2>
  <p>
    <span class="en-content">Join 300,000+ students worldwide in America's premier math competition</span>
    <span class="zh-content">加入全球30万+学生，参与美国顶级数学竞赛</span>
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
