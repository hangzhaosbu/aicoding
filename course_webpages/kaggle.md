---
layout: default
title: Kaggle Competition Training
title_zh: Kaggle竞赛培训
description: Master Data Science Competitions & Climb the Kaggle Ranks
description_zh: 征服数据科学竞赛，攀登Kaggle排行榜
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
      filter: drop-shadow(0 0 10px currentColor);
    }
    50% { 
      filter: drop-shadow(0 0 25px currentColor);
    }
  }

  @keyframes rankUp {
    0% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
    100% { transform: translateY(0); }
  }

  /* Course Hero - Ultra Premium Kaggle Blue Theme */
  .course-hero {
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 25%, #0077B5 50%, #005A8C 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(32, 190, 255, 0.4);
    min-height: 480px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: 'K';
    position: absolute;
    font-size: 25rem;
    font-weight: 900;
    opacity: 0.08;
    right: -50px;
    top: -80px;
    font-family: Arial, sans-serif;
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

  .kaggle-badge {
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

  .kaggle-badge::before {
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
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
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

  /* What is Kaggle Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #20BEFF, #0099DD, #0077B5) 1;
  }

  .intro-section::before {
    content: '📊';
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
    background: linear-gradient(135deg, #E0F7FF 0%, #B3ECFF 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(32, 190, 255, 0.15);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Kaggle Tiers Section - Premium */
  .tiers-section {
    background: linear-gradient(135deg, #E0F7FF 0%, #B3ECFF 50%, #80DFFF 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .tiers-section::before {
    content: '🎖️';
    position: absolute;
    font-size: 12rem;
    opacity: 0.05;
    right: -30px;
    bottom: -30px;
  }

  .tiers-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #005A8C;
    margin-bottom: 1rem;
  }

  .tiers-section > p {
    text-align: center;
    color: #0077B5;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .tiers-grid {
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    flex-wrap: wrap;
    max-width: 1200px;
    margin: 0 auto;
  }

  .tier-card {
    background: white;
    padding: 2rem 1.5rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    flex: 1;
    min-width: 180px;
    max-width: 200px;
    position: relative;
    overflow: hidden;
  }

  .tier-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
  }

  .tier-novice::before { background: #9CA3AF; }
  .tier-contributor::before { background: #06B6D4; }
  .tier-expert::before { background: #8B5CF6; }
  .tier-master::before { background: #F59E0B; }
  .tier-grandmaster::before { background: linear-gradient(90deg, #FFD700, #FFA500, #FFD700); }

  .tier-card:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.15);
  }

  .tier-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    display: block;
  }

  .tier-novice .tier-icon { color: #9CA3AF; }
  .tier-contributor .tier-icon { color: #06B6D4; }
  .tier-expert .tier-icon { color: #8B5CF6; animation: medalShine 2s ease-in-out infinite; }
  .tier-master .tier-icon { color: #F59E0B; animation: medalShine 2s ease-in-out infinite; }
  .tier-grandmaster .tier-icon { color: #FFD700; animation: medalShine 2s ease-in-out infinite, rankUp 3s ease-in-out infinite; }

  .tier-name {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .tier-requirement {
    font-size: 0.85rem;
    color: #6B7280;
    line-height: 1.5;
  }

  .tier-count {
    font-size: 0.8rem;
    color: #9CA3AF;
    margin-top: 0.8rem;
    padding-top: 0.8rem;
    border-top: 1px solid #E5E7EB;
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
    border-left: 5px solid;
  }

  .curriculum-card:nth-child(1) { 
    animation-delay: 0.1s; 
    border-left-color: #20BEFF;
    background: linear-gradient(to right, rgba(32, 190, 255, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(2) { 
    animation-delay: 0.15s; 
    border-left-color: #8B5CF6;
    background: linear-gradient(to right, rgba(139, 92, 246, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(3) { 
    animation-delay: 0.2s; 
    border-left-color: #F59E0B;
    background: linear-gradient(to right, rgba(245, 158, 11, 0.03) 0%, white 30%);
  }
  .curriculum-card:nth-child(4) { 
    animation-delay: 0.25s; 
    border-left-color: #10B981;
    background: linear-gradient(to right, rgba(16, 185, 129, 0.03) 0%, white 30%);
  }

  .curriculum-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(32, 190, 255, 0.03), transparent);
    animation: shimmer 3s infinite;
  }

  .curriculum-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(32, 190, 255, 0.15);
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

  .curriculum-card:nth-child(1) .curriculum-icon { background: linear-gradient(135deg, #20BEFF, #0099DD); }
  .curriculum-card:nth-child(2) .curriculum-icon { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .curriculum-card:nth-child(3) .curriculum-icon { background: linear-gradient(135deg, #F59E0B, #D97706); }
  .curriculum-card:nth-child(4) .curriculum-icon { background: linear-gradient(135deg, #10B981, #059669); }

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

  .curriculum-card:nth-child(1) .curriculum-topics li::before { color: #20BEFF; }
  .curriculum-card:nth-child(2) .curriculum-topics li::before { color: #8B5CF6; }
  .curriculum-card:nth-child(3) .curriculum-topics li::before { color: #F59E0B; }
  .curriculum-card:nth-child(4) .curriculum-topics li::before { color: #10B981; }

  /* Competition Types Section */
  .competition-types-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .competition-types-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .competition-types-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .competition-types-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 1000px) {
    .competition-types-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .competition-types-grid {
      grid-template-columns: 1fr;
    }
  }

  .comp-type-card {
    background: linear-gradient(135deg, #F0F9FF 0%, #E0F7FF 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .comp-type-card:hover {
    transform: translateY(-5px);
    border-color: #20BEFF;
    box-shadow: 0 15px 30px rgba(32, 190, 255, 0.15);
    background: white;
  }

  .comp-type-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .comp-type-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .comp-type-desc {
    font-size: 0.9rem;
    color: #6B7280;
    line-height: 1.5;
  }

  /* Winning Strategies Section */
  .strategies-section {
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 50%, #0077B5 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(32, 190, 255, 0.3);
  }

  .strategies-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .strategies-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .strategies-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .strategies-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .strategies-grid {
      grid-template-columns: 1fr;
      max-width: 500px;
    }
  }

  .strategy-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s ease;
  }

  .strategy-card:hover {
    transform: translateY(-8px) scale(1.02);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .strategy-number {
    width: 50px;
    height: 50px;
    background: linear-gradient(135deg, #20BEFF, #0077B5);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.5rem;
    color: white;
    margin-bottom: 1rem;
  }

  .strategy-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .strategy-desc {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #E0F7FF 0%, #B3ECFF 100%);
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
    border-color: #20BEFF;
    box-shadow: 0 20px 40px rgba(32, 190, 255, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(32, 190, 255, 0.3);
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
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
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
    background: linear-gradient(135deg, #E0F7FF 0%, #B3ECFF 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(32, 190, 255, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .success-number {
    font-size: 2.8rem;
    font-weight: 800;
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
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

  /* Tools Section */
  .tools-section {
    background: linear-gradient(135deg, #F0F9FF 0%, #E0F7FF 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .tools-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 2rem;
  }

  .tools-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  .tool-badge {
    background: white;
    padding: 0.75rem 1.75rem;
    border-radius: 25px;
    border: 2px solid #20BEFF;
    font-weight: 600;
    color: #0077B5;
    transition: all 0.3s ease;
    box-shadow: 0 4px 12px rgba(32, 190, 255, 0.1);
  }

  .tool-badge:hover {
    background: linear-gradient(135deg, #20BEFF, #0077B5);
    color: white;
    border-color: transparent;
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(32, 190, 255, 0.3);
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #E0F7FF 0%, #B3ECFF 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #20BEFF 0%, #0077B5 100%);
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
    color: #20BEFF;
    opacity: 0.2;
    font-family: Georgia, serif;
    line-height: 1;
  }

  .testimonial-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 100%);
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 15px;
    font-size: 0.8rem;
    font-weight: 600;
  }

  .testimonial-badge.expert { background: linear-gradient(135deg, #8B5CF6, #7C3AED); }
  .testimonial-badge.master { background: linear-gradient(135deg, #F59E0B, #D97706); }

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
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 100%);
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
    background: linear-gradient(135deg, #20BEFF 0%, #0099DD 25%, #0077B5 50%, #005A8C 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(32, 190, 255, 0.4);
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
    color: #0077B5;
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
    background: linear-gradient(90deg, transparent, rgba(32, 190, 255, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #005A8C;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #0077B5;
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
    .tiers-section,
    .why-choose-section,
    .success-section,
    .strategies-section,
    .competition-types-section {
      padding: 3rem 1.5rem;
    }

    .kaggle-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="kaggle-badge">
    <span class="en-content">COMPETITION</span>
    <span class="zh-content">竞赛培训</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">📊</span>
    <span class="floating-icon">🤖</span>
    <span class="floating-icon">🏅</span>
    <span class="floating-icon">📈</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">💻</span>
    <span class="floating-icon">🎯</span>
  </div>
  <h1>
    <span class="en-content">Kaggle Competition Training</span>
    <span class="zh-content">Kaggle竞赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Master Data Science Competitions & Climb the Ranks</span>
    <span class="zh-content">征服数据科学竞赛，攀登排行榜</span>
  </p>
  <div class="hero-badge">
    <span>🏆</span>
    <span class="en-content">World's Largest Data Science Community</span>
    <span class="zh-content">全球最大数据科学社区</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">23M+</span>
      <span class="hero-stat-label">
        <span class="en-content">Kaggle Users</span>
        <span class="zh-content">Kaggle用户</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">612</span>
      <span class="hero-stat-label">
        <span class="en-content">Grandmasters</span>
        <span class="zh-content">大师级选手</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">$1M+</span>
      <span class="hero-stat-label">
        <span class="en-content">Prize Pools</span>
        <span class="zh-content">奖金池</span>
      </span>
    </div>
  </div>
</div>

<!-- What is Kaggle -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is Kaggle?</span>
        <span class="zh-content">什么是Kaggle？</span>
      </h2>
      <p>
        <span class="en-content">
          Kaggle is the world's largest data science competition platform and online community, now owned by Google. 
          With over 23 million users across 194 countries, Kaggle hosts competitions where data scientists compete 
          to produce the best machine learning models for real-world problems from companies like Google, Microsoft, 
          and NVIDIA.
        </span>
        <span class="zh-content">
          Kaggle是全球最大的数据科学竞赛平台和在线社区，现由Google拥有。拥有超过2300万用户，遍布194个国家，
          Kaggle举办各类竞赛，数据科学家们竞相为Google、Microsoft、NVIDIA等公司的实际问题构建最佳机器学习模型。
        </span>
      </p>
      <p>
        <span class="en-content">
          Kaggle achievements are highly respected in the data science world and can significantly boost your 
          college applications and career prospects. Our training prepares you to compete and win!
        </span>
        <span class="zh-content">
          Kaggle成就在数据科学领域备受尊重，能显著提升你的大学申请和职业前景。我们的培训让你有能力参赛并获胜！
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏢</span>
          <span class="intro-highlight-text">
            <span class="en-content">Google Owned</span>
            <span class="zh-content">Google旗下</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">💰</span>
          <span class="intro-highlight-text">
            <span class="en-content">Real Prize Money</span>
            <span class="zh-content">真实奖金</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">📈</span>
          <span class="intro-highlight-text">
            <span class="en-content">Career Boost</span>
            <span class="zh-content">职业提升</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌐</span>
          <span class="intro-highlight-text">
            <span class="en-content">Global Recognition</span>
            <span class="zh-content">全球认可</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 10rem; opacity: 0.8; animation: float 6s ease-in-out infinite; color: #20BEFF; font-weight: 900; font-family: Arial, sans-serif;">K</div>
    </div>
  </div>
</div>

<!-- Kaggle Tiers Section -->
<div class="tiers-section">
  <h2>
    <span class="en-content">🏅 Kaggle Progression Tiers</span>
    <span class="zh-content">🏅 Kaggle等级体系</span>
  </h2>
  <p>
    <span class="en-content">Climb the ranks from Novice to Grandmaster</span>
    <span class="zh-content">从新手攀登至大师级</span>
  </p>
  
  <div class="tiers-grid">
    <div class="tier-card tier-novice">
      <span class="tier-icon">⚪</span>
      <h3 class="tier-name">Novice</h3>
      <p class="tier-requirement">
        <span class="en-content">Starting point for all Kagglers</span>
        <span class="zh-content">所有Kaggle用户的起点</span>
      </p>
      <p class="tier-count">92K+ users</p>
    </div>
    
    <div class="tier-card tier-contributor">
      <span class="tier-icon">🔵</span>
      <h3 class="tier-name">Contributor</h3>
      <p class="tier-requirement">
        <span class="en-content">Complete profile & make submissions</span>
        <span class="zh-content">完善资料并提交作品</span>
      </p>
      <p class="tier-count">64K+ users</p>
    </div>
    
    <div class="tier-card tier-expert">
      <span class="tier-icon">🟣</span>
      <h3 class="tier-name">Expert</h3>
      <p class="tier-requirement">
        <span class="en-content">2 Bronze medals in competitions</span>
        <span class="zh-content">竞赛中获得2枚铜牌</span>
      </p>
      <p class="tier-count">7K+ users</p>
    </div>
    
    <div class="tier-card tier-master">
      <span class="tier-icon">🟠</span>
      <h3 class="tier-name">Master</h3>
      <p class="tier-requirement">
        <span class="en-content">1 Gold + 2 Silver medals</span>
        <span class="zh-content">1金牌 + 2银牌</span>
      </p>
      <p class="tier-count">2,973 users</p>
    </div>
    
    <div class="tier-card tier-grandmaster">
      <span class="tier-icon">👑</span>
      <h3 class="tier-name">Grandmaster</h3>
      <p class="tier-requirement">
        <span class="en-content">5 Gold medals (1 solo)</span>
        <span class="zh-content">5金牌（含1个人金牌）</span>
      </p>
      <p class="tier-count">612 users</p>
    </div>
  </div>
</div>

<!-- Curriculum Section -->
<div class="curriculum-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Complete Competition Curriculum</span>
      <span class="zh-content">完整竞赛课程体系</span>
    </h2>
    <p>
      <span class="en-content">Master all skills needed to win Kaggle competitions</span>
      <span class="zh-content">掌握赢得Kaggle竞赛所需的全部技能</span>
    </p>
  </div>

  <div class="curriculum-cards">
    <!-- Foundation -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">📚</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">ML Foundations</span>
            <span class="zh-content">机器学习基础</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 1-4</span>
            <span class="zh-content">第1-4周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Linear & Logistic Regression</span><span class="zh-content">线性与逻辑回归</span></li>
        <li><span class="en-content">Decision Trees & Random Forests</span><span class="zh-content">决策树与随机森林</span></li>
        <li><span class="en-content">Cross-validation Strategies</span><span class="zh-content">交叉验证策略</span></li>
        <li><span class="en-content">Evaluation Metrics (AUC, F1, RMSE)</span><span class="zh-content">评估指标（AUC、F1、RMSE）</span></li>
        <li><span class="en-content">Handling Missing Data</span><span class="zh-content">处理缺失数据</span></li>
        <li><span class="en-content">Exploratory Data Analysis (EDA)</span><span class="zh-content">探索性数据分析</span></li>
      </ul>
    </div>

    <!-- Feature Engineering -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">⚙️</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Feature Engineering</span>
            <span class="zh-content">特征工程</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 5-8</span>
            <span class="zh-content">第5-8周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Feature Creation & Selection</span><span class="zh-content">特征创建与选择</span></li>
        <li><span class="en-content">Target Encoding & Embeddings</span><span class="zh-content">目标编码与嵌入</span></li>
        <li><span class="en-content">Time Series Features</span><span class="zh-content">时间序列特征</span></li>
        <li><span class="en-content">Text Feature Extraction (TF-IDF)</span><span class="zh-content">文本特征提取</span></li>
        <li><span class="en-content">Dimensionality Reduction (PCA)</span><span class="zh-content">降维（PCA）</span></li>
        <li><span class="en-content">Feature Importance Analysis</span><span class="zh-content">特征重要性分析</span></li>
      </ul>
    </div>

    <!-- Advanced Models -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🚀</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Advanced Models</span>
            <span class="zh-content">高级模型</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 9-12</span>
            <span class="zh-content">第9-12周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">XGBoost & LightGBM</span><span class="zh-content">XGBoost与LightGBM</span></li>
        <li><span class="en-content">CatBoost for Categorical Data</span><span class="zh-content">CatBoost处理类别数据</span></li>
        <li><span class="en-content">Neural Networks (Tabular)</span><span class="zh-content">神经网络（表格数据）</span></li>
        <li><span class="en-content">CNN for Image Competitions</span><span class="zh-content">CNN图像竞赛</span></li>
        <li><span class="en-content">Transformers for NLP</span><span class="zh-content">Transformers自然语言处理</span></li>
        <li><span class="en-content">Hyperparameter Tuning (Optuna)</span><span class="zh-content">超参数调优（Optuna）</span></li>
      </ul>
    </div>

    <!-- Winning Techniques -->
    <div class="curriculum-card">
      <div class="curriculum-header">
        <div class="curriculum-icon">🏆</div>
        <div class="curriculum-title-group">
          <h3 class="curriculum-title">
            <span class="en-content">Winning Techniques</span>
            <span class="zh-content">获胜技巧</span>
          </h3>
          <p class="curriculum-subtitle">
            <span class="en-content">Weeks 13-16</span>
            <span class="zh-content">第13-16周</span>
          </p>
        </div>
      </div>
      <ul class="curriculum-topics">
        <li><span class="en-content">Ensemble Methods & Stacking</span><span class="zh-content">集成方法与堆叠</span></li>
        <li><span class="en-content">Blending & Model Averaging</span><span class="zh-content">混合与模型平均</span></li>
        <li><span class="en-content">Pseudo Labeling</span><span class="zh-content">伪标签技术</span></li>
        <li><span class="en-content">Local Validation vs LB Strategy</span><span class="zh-content">本地验证vs排行榜策略</span></li>
        <li><span class="en-content">Competition Shake-up Tactics</span><span class="zh-content">竞赛排名波动战术</span></li>
        <li><span class="en-content">Post-processing Tricks</span><span class="zh-content">后处理技巧</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Competition Types -->
<div class="competition-types-section">
  <h2>
    <span class="en-content">🎯 Competition Categories We Cover</span>
    <span class="zh-content">🎯 我们覆盖的竞赛类别</span>
  </h2>
  <p>
    <span class="en-content">Train for all major Kaggle competition types</span>
    <span class="zh-content">为所有主要Kaggle竞赛类型做准备</span>
  </p>
  
  <div class="competition-types-grid">
    <div class="comp-type-card">
      <div class="comp-type-icon">📊</div>
      <h3 class="comp-type-title">
        <span class="en-content">Tabular Data</span>
        <span class="zh-content">表格数据</span>
      </h3>
      <p class="comp-type-desc">
        <span class="en-content">Structured data prediction with XGBoost, LightGBM, CatBoost</span>
        <span class="zh-content">使用XGBoost、LightGBM、CatBoost进行结构化数据预测</span>
      </p>
    </div>
    
    <div class="comp-type-card">
      <div class="comp-type-icon">🖼️</div>
      <h3 class="comp-type-title">
        <span class="en-content">Computer Vision</span>
        <span class="zh-content">计算机视觉</span>
      </h3>
      <p class="comp-type-desc">
        <span class="en-content">Image classification, object detection, segmentation</span>
        <span class="zh-content">图像分类、目标检测、图像分割</span>
      </p>
    </div>
    
    <div class="comp-type-card">
      <div class="comp-type-icon">📝</div>
      <h3 class="comp-type-title">
        <span class="en-content">NLP</span>
        <span class="zh-content">自然语言处理</span>
      </h3>
      <p class="comp-type-desc">
        <span class="en-content">Text classification, NER, question answering with BERT/GPT</span>
        <span class="zh-content">文本分类、命名实体识别、问答系统</span>
      </p>
    </div>
    
    <div class="comp-type-card">
      <div class="comp-type-icon">📈</div>
      <h3 class="comp-type-title">
        <span class="en-content">Time Series</span>
        <span class="zh-content">时间序列</span>
      </h3>
      <p class="comp-type-desc">
        <span class="en-content">Forecasting, anomaly detection, trend analysis</span>
        <span class="zh-content">预测、异常检测、趋势分析</span>
      </p>
    </div>
  </div>
</div>

<!-- Winning Strategies -->
<div class="strategies-section">
  <h2>
    <span class="en-content">🏆 Grandmaster Winning Strategies</span>
    <span class="zh-content">🏆 大师级获胜策略</span>
  </h2>
  <p>
    <span class="en-content">Learn battle-tested techniques from top Kagglers</span>
    <span class="zh-content">学习顶级Kaggle选手的实战技巧</span>
  </p>
  
  <div class="strategies-grid">
    <div class="strategy-card">
      <div class="strategy-number">1</div>
      <h3 class="strategy-title">
        <span class="en-content">Strong Local Validation</span>
        <span class="zh-content">强大的本地验证</span>
      </h3>
      <p class="strategy-desc">
        <span class="en-content">Build a reliable cross-validation scheme that mirrors the test set distribution. Trust your CV over the public leaderboard.</span>
        <span class="zh-content">构建可靠的交叉验证方案，反映测试集分布。相信你的CV而非公开排行榜。</span>
      </p>
    </div>
    
    <div class="strategy-card">
      <div class="strategy-number">2</div>
      <h3 class="strategy-title">
        <span class="en-content">Creative Feature Engineering</span>
        <span class="zh-content">创意特征工程</span>
      </h3>
      <p class="strategy-desc">
        <span class="en-content">The secret weapon of top Kagglers. Create domain-specific features that capture hidden patterns in the data.</span>
        <span class="zh-content">顶级Kaggle选手的秘密武器。创建捕捉数据隐藏模式的领域特定特征。</span>
      </p>
    </div>
    
    <div class="strategy-card">
      <div class="strategy-number">3</div>
      <h3 class="strategy-title">
        <span class="en-content">Ensemble Everything</span>
        <span class="zh-content">集成一切</span>
      </h3>
      <p class="strategy-desc">
        <span class="en-content">Combine diverse models through stacking, blending, and weighted averaging to push into gold medal territory.</span>
        <span class="zh-content">通过堆叠、混合和加权平均组合多样化模型，冲击金牌区域。</span>
      </p>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Train With Us for Kaggle?</span>
      <span class="zh-content">为什么选择我们的Kaggle培训？</span>
    </h2>
    <p>
      <span class="en-content">Your path to Kaggle medals and data science mastery</span>
      <span class="zh-content">通往Kaggle奖牌和数据科学精通的道路</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">🏅</div>
      <h3>
        <span class="en-content">Medal-Focused Training</span>
        <span class="zh-content">以奖牌为导向的培训</span>
      </h3>
      <p>
        <span class="en-content">Our curriculum is designed specifically to help you win Kaggle medals</span>
        <span class="zh-content">我们的课程专门设计帮助你赢得Kaggle奖牌</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Real Competition Practice</span>
        <span class="zh-content">真实竞赛实践</span>
      </h3>
      <p>
        <span class="en-content">Work on actual Kaggle competitions with expert guidance and code review</span>
        <span class="zh-content">在专家指导和代码审查下参与实际Kaggle竞赛</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🔧</div>
      <h3>
        <span class="en-content">Grandmaster Techniques</span>
        <span class="zh-content">大师级技术</span>
      </h3>
      <p>
        <span class="en-content">Learn advanced tricks used by Kaggle Grandmasters to win competitions</span>
        <span class="zh-content">学习Kaggle大师用于赢得竞赛的高级技巧</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">☁️</div>
      <h3>
        <span class="en-content">GPU Computing Access</span>
        <span class="zh-content">GPU计算资源</span>
      </h3>
      <p>
        <span class="en-content">Access to Kaggle Notebooks with free GPU/TPU for training models</span>
        <span class="zh-content">使用Kaggle Notebooks免费GPU/TPU训练模型</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📂</div>
      <h3>
        <span class="en-content">Portfolio Building</span>
        <span class="zh-content">作品集构建</span>
      </h3>
      <p>
        <span class="en-content">Build an impressive Kaggle profile for college apps and job applications</span>
        <span class="zh-content">为大学申请和求职构建出色的Kaggle档案</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized feedback and code reviews</span>
        <span class="zh-content">每班最多6人，个性化反馈和代码审查</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' Kaggle Achievements</span>
    <span class="zh-content">🏆 我们学生的Kaggle成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">15+</span>
      <div class="success-label">
        <span class="en-content">Medals Won</span>
        <span class="zh-content">获得奖牌</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🏅</div>
      <span class="success-number">8</span>
      <div class="success-label">
        <span class="en-content">Expert Titles</span>
        <span class="zh-content">Expert称号</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🎯</div>
      <span class="success-number">Top 5%</span>
      <div class="success-label">
        <span class="en-content">Average Finish</span>
        <span class="zh-content">平均排名</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📊</div>
      <span class="success-number">50+</span>
      <div class="success-label">
        <span class="en-content">Competitions Entered</span>
        <span class="zh-content">参与竞赛</span>
      </div>
    </div>
  </div>
</div>

<!-- Tools Section -->
<div class="tools-section">
  <h2>
    <span class="en-content">🛠️ Tools & Libraries You'll Master</span>
    <span class="zh-content">🛠️ 你将掌握的工具与库</span>
  </h2>
  
  <div class="tools-grid">
    <span class="tool-badge">Python</span>
    <span class="tool-badge">XGBoost</span>
    <span class="tool-badge">LightGBM</span>
    <span class="tool-badge">CatBoost</span>
    <span class="tool-badge">scikit-learn</span>
    <span class="tool-badge">PyTorch</span>
    <span class="tool-badge">TensorFlow</span>
    <span class="tool-badge">Pandas</span>
    <span class="tool-badge">NumPy</span>
    <span class="tool-badge">Optuna</span>
    <span class="tool-badge">Hugging Face</span>
    <span class="tool-badge">OpenCV</span>
    <span class="tool-badge">Albumentations</span>
    <span class="tool-badge">Kaggle Notebooks</span>
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
      <span class="testimonial-badge expert">Expert</span>
      <p class="testimonial-text">
        <span class="en-content">I went from complete beginner to Kaggle Expert in just 6 months. The feature engineering techniques I learned were game-changers for my competition scores!</span>
        <span class="zh-content">我在短短6个月内从完全新手成长为Kaggle Expert。我学到的特征工程技术彻底改变了我的竞赛成绩！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Michael C.</h4>
          <p>
            <span class="en-content">3 Bronze Medals</span>
            <span class="zh-content">3枚铜牌</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge master">Master</span>
      <p class="testimonial-text">
        <span class="en-content">The ensemble and stacking techniques helped me break into the gold medal zone. My Kaggle profile was a major factor in my MIT admission!</span>
        <span class="zh-content">集成和堆叠技术帮助我冲进金牌区域。我的Kaggle档案是MIT录取的重要因素！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍💻</div>
        <div class="testimonial-info">
          <h4>Emily Z.</h4>
          <p>
            <span class="en-content">1 Gold, 3 Silver Medals</span>
            <span class="zh-content">1金3银牌</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">Bronze Medal</span>
      <p class="testimonial-text">
        <span class="en-content">As a high schooler, I never thought I could compete with data scientists. Now I've won my first medal and I'm hooked on Kaggle competitions!</span>
        <span class="zh-content">作为高中生，我从没想过能与数据科学家竞争。现在我赢得了第一枚奖牌，完全爱上了Kaggle竞赛！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Jason L.</h4>
          <p>
            <span class="en-content">Junior, First Medal Winner</span>
            <span class="zh-content">高二学生，首枚奖牌获得者</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Start Winning Kaggle Medals!</span>
    <span class="zh-content">开始赢得Kaggle奖牌！</span>
  </h2>
  <p>
    <span class="en-content">Join the world's best data science community and compete with the best</span>
    <span class="zh-content">加入全球最佳数据科学社区，与顶尖选手竞争</span>
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
