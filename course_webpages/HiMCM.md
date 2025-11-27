---
layout: default
title: HiMCM Competition Training
title_zh: HiMCM数学建模竞赛培训
description: Master Mathematical Modeling & Problem Solving for HiMCM Success
description_zh: 掌握数学建模与问题解决，征服HiMCM竞赛
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

  @keyframes modelPulse {
    0%, 100% { box-shadow: 0 0 0 0 rgba(20, 184, 166, 0.4); }
    50% { box-shadow: 0 0 0 15px rgba(20, 184, 166, 0); }
  }

  /* Course Hero - Ultra Premium Teal/Emerald Theme */
  .course-hero {
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 25%, #2DD4BF 50%, #14B8A6 75%, #0F766E 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(15, 118, 110, 0.4);
    min-height: 520px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '∫';
    position: absolute;
    font-size: 22rem;
    font-weight: 300;
    opacity: 0.08;
    right: -20px;
    top: -50px;
    font-family: 'Times New Roman', serif;
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

  .year-badge {
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

  .year-badge::before {
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
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 50%, #2DD4BF 100%);
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

  /* What is HiMCM Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #0D9488, #14B8A6, #2DD4BF, #5EEAD4) 1;
  }

  .intro-section::before {
    content: '📊';
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
    background: linear-gradient(135deg, #CCFBF1 0%, #99F6E4 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(20, 184, 166, 0.2);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Contest Format Section */
  .format-section {
    background: linear-gradient(135deg, #0F766E 0%, #0D9488 50%, #14B8A6 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .format-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.1) 0%, transparent 50%);
    animation: rotateGlow 20s linear infinite;
  }

  .format-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .format-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .format-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1000px) {
    .format-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .format-grid {
      grid-template-columns: 1fr;
    }
  }

  .format-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .format-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .format-card-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .format-card h3 {
    font-size: 1.8rem;
    font-weight: 800;
    color: #0F766E;
    margin-bottom: 0.3rem;
  }

  .format-card p {
    color: #6B7280;
    font-size: 0.95rem;
  }

  /* Timeline Section */
  .timeline-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .timeline-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .timeline {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
    padding: 2rem 0;
  }

  .timeline::before {
    content: '';
    position: absolute;
    top: 50px;
    left: 10%;
    right: 10%;
    height: 4px;
    background: linear-gradient(90deg, #0F766E, #14B8A6, #2DD4BF, #5EEAD4);
    border-radius: 2px;
  }

  @media (max-width: 800px) {
    .timeline {
      flex-direction: column;
      gap: 2rem;
    }
    .timeline::before {
      display: none;
    }
  }

  .timeline-item {
    text-align: center;
    position: relative;
    z-index: 1;
    flex: 1;
  }

  .timeline-dot {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background: linear-gradient(135deg, #0F766E, #14B8A6);
    margin: 0 auto 1rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    box-shadow: 0 10px 25px rgba(15, 118, 110, 0.4);
    animation: modelPulse 2s ease-in-out infinite;
  }

  .timeline-date {
    font-weight: 800;
    color: #0F766E;
    font-size: 1.1rem;
    margin-bottom: 0.3rem;
  }

  .timeline-title {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* Awards Section */
  .awards-section {
    background: linear-gradient(135deg, #CCFBF1 0%, #99F6E4 50%, #5EEAD4 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .awards-section::before {
    content: '🏆';
    position: absolute;
    font-size: 15rem;
    opacity: 0.08;
    right: -30px;
    top: -30px;
  }

  .awards-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #0F766E !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .awards-section > p {
    text-align: center;
    color: #115E59;
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .awards-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 1.5rem;
    max-width: 1100px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1000px) {
    .awards-grid {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media (max-width: 600px) {
    .awards-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  .award-card {
    background: white;
    padding: 1.5rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  }

  .award-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .award-card.outstanding {
    background: linear-gradient(135deg, #FEF9C3, #FEF08A);
    border: 3px solid #EAB308;
  }

  .award-card.finalist {
    background: linear-gradient(135deg, #E0E7FF, #C7D2FE);
    border: 3px solid #6366F1;
  }

  .award-card.meritorious {
    background: linear-gradient(135deg, #D1FAE5, #A7F3D0);
    border: 3px solid #10B981;
  }

  .award-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .award-name {
    font-weight: 700;
    color: #1F2937;
    font-size: 1rem;
    margin-bottom: 0.3rem;
  }

  .award-percent {
    font-size: 0.85rem;
    color: #6B7280;
    font-weight: 600;
  }

  /* Skills Section */
  .skills-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .skills-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .skills-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .skills-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .skills-grid {
      grid-template-columns: 1fr;
    }
  }

  .skill-card {
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
    padding: 2rem;
    border-radius: 20px;
    border-left: 4px solid;
    transition: all 0.4s ease;
  }

  .skill-card:hover {
    transform: translateX(5px);
    box-shadow: 0 15px 40px rgba(20, 184, 166, 0.15);
  }

  .skill-card.modeling { border-left-color: #0F766E; }
  .skill-card.programming { border-left-color: #8B5CF6; }
  .skill-card.stats { border-left-color: #3B82F6; }
  .skill-card.writing { border-left-color: #F59E0B; }

  .skill-card h3 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
  }

  .skill-card h3 span {
    font-size: 1.5rem;
  }

  .skill-topics {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .skill-topics li {
    padding: 0.5rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
    border-bottom: 1px solid rgba(20, 184, 166, 0.15);
  }

  .skill-topics li:last-child {
    border-bottom: none;
  }

  .skill-topics li::before {
    content: '▸';
    font-weight: bold;
  }

  .skill-card.modeling .skill-topics li::before { color: #0F766E; }
  .skill-card.programming .skill-topics li::before { color: #8B5CF6; }
  .skill-card.stats .skill-topics li::before { color: #3B82F6; }
  .skill-card.writing .skill-topics li::before { color: #F59E0B; }

  /* Past Problems Section */
  .problems-section {
    background: linear-gradient(135deg, #0F766E 0%, #0D9488 50%, #14B8A6 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .problems-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.08) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .problems-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .problems-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .problems-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 700px) {
    .problems-grid {
      grid-template-columns: 1fr;
    }
  }

  .problem-card {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    transition: all 0.4s ease;
  }

  .problem-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .problem-year {
    display: inline-block;
    background: linear-gradient(135deg, #0F766E, #14B8A6);
    color: white;
    padding: 0.3rem 1rem;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }

  .problem-card h3 {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .problem-card p {
    color: #6B7280;
    font-size: 0.9rem;
    line-height: 1.6;
  }

  /* Report Structure Section */
  .report-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .report-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .report-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .report-structure {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    max-width: 1000px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .report-structure {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .report-structure {
      grid-template-columns: 1fr;
    }
  }

  .report-item {
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
    padding: 1.5rem;
    border-radius: 15px;
    text-align: center;
    transition: all 0.3s ease;
    border: 2px solid transparent;
  }

  .report-item:hover {
    border-color: #14B8A6;
    transform: translateY(-3px);
  }

  .report-item.important {
    background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 100%);
    border: 2px solid #EAB308;
  }

  .report-item-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }

  .report-item h3 {
    font-size: 1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .report-item p {
    font-size: 0.85rem;
    color: #6B7280;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #CCFBF1 0%, #99F6E4 50%, #5EEAD4 100%);
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

  .why-choose-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #0F766E !important;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .why-choose-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
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
    border-color: #14B8A6;
    box-shadow: 0 20px 40px rgba(20, 184, 166, 0.15);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(15, 118, 110, 0.3);
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
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
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
    padding: 2rem 1.5rem;
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
    border-radius: 20px;
    transition: all 0.4s ease;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 200px;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(20, 184, 166, 0.15);
  }

  .success-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .success-number {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: flex;
    align-items: center;
    justify-content: center;
    animation: pulse 3s ease-in-out infinite;
    white-space: nowrap;
    height: 50px;
  }

  .success-label {
    color: #6B7280;
    font-size: 0.95rem;
    font-weight: 600;
    margin-top: 0.3rem;
    height: 24px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
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
    color: #14B8A6;
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

  .testimonial-badge.outstanding { background: linear-gradient(135deg, #EAB308, #CA8A04); }
  .testimonial-badge.finalist { background: linear-gradient(135deg, #6366F1, #4F46E5); }
  .testimonial-badge.meritorious { background: linear-gradient(135deg, #10B981, #059669); }

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
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 100%);
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
    background: linear-gradient(135deg, #0F766E 0%, #14B8A6 25%, #2DD4BF 50%, #14B8A6 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(15, 118, 110, 0.4);
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
    color: #0F766E;
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
    background: linear-gradient(90deg, transparent, rgba(20, 184, 166, 0.2), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    color: #0D9488;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #0F766E;
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
    .format-section,
    .timeline-section,
    .awards-section,
    .skills-section,
    .problems-section,
    .report-section,
    .why-choose-section,
    .success-section {
      padding: 3rem 1.5rem;
    }

    .year-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="year-badge">
    <span class="en-content">28th YEAR</span>
    <span class="zh-content">第28届</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">📊</span>
    <span class="floating-icon">📐</span>
    <span class="floating-icon">🔢</span>
    <span class="floating-icon">📈</span>
    <span class="floating-icon">🧮</span>
    <span class="floating-icon">💡</span>
    <span class="floating-icon">🌍</span>
  </div>
  <h1>
    <span class="en-content">HiMCM Training</span>
    <span class="zh-content">HiMCM数学建模竞赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">High School Mathematical Contest in Modeling</span>
    <span class="zh-content">美国高中数学建模竞赛</span>
  </p>
  <div class="hero-badge">
    <span>🌐</span>
    <span class="en-content">International Competition • COMAP Organized • Real-World Problems</span>
    <span class="zh-content">国际竞赛 • COMAP主办 • 真实世界问题</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">14</span>
      <span class="hero-stat-label">
        <span class="en-content">Days</span>
        <span class="zh-content">天比赛</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">4</span>
      <span class="hero-stat-label">
        <span class="en-content">Team Members</span>
        <span class="zh-content">人团队</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">18+</span>
      <span class="hero-stat-label">
        <span class="en-content">Countries</span>
        <span class="zh-content">个国家</span>
      </span>
    </div>
  </div>
</div>

<!-- What is HiMCM -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is HiMCM?</span>
        <span class="zh-content">什么是HiMCM？</span>
      </h2>
      <p>
        <span class="en-content">
          The High School Mathematical Contest in Modeling (HiMCM) is an international competition 
          organized by COMAP (Consortium for Mathematics and Its Applications). Teams of up to 4 students 
          collaborate over 14 days to solve real-world problems using mathematical modeling.
        </span>
        <span class="zh-content">
          美国高中数学建模竞赛(HiMCM)是由COMAP（美国数学及其应用联合会）组织的国际竞赛。
          最多4名学生组成的团队在14天内合作解决现实世界问题，运用数学建模方法。
        </span>
      </p>
      <p>
        <span class="en-content">
          Unlike traditional math competitions, HiMCM emphasizes creative problem-solving, teamwork, 
          and technical writing. Students develop mathematical models, analyze data, and write 
          comprehensive reports—skills highly valued by top universities and employers.
        </span>
        <span class="zh-content">
          与传统数学竞赛不同，HiMCM强调创造性解决问题、团队合作和技术写作。
          学生需要开发数学模型、分析数据并撰写综合报告——这些技能深受顶尖大学和雇主重视。
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏫</span>
          <span class="intro-highlight-text">
            <span class="en-content">1,000+ Teams Annually</span>
            <span class="zh-content">每年1000+支队伍</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌍</span>
          <span class="intro-highlight-text">
            <span class="en-content">18+ Countries</span>
            <span class="zh-content">18+个国家</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">📝</span>
          <span class="intro-highlight-text">
            <span class="en-content">25-Page Report</span>
            <span class="zh-content">25页论文</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏆</span>
          <span class="intro-highlight-text">
            <span class="en-content">IM2C Qualification</span>
            <span class="zh-content">IM2C资格赛</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 6rem; animation: float 5s ease-in-out infinite;">📊</div>
      <div style="font-size: 2rem; font-weight: 800; color: #0F766E; margin-top: 1rem;">COMAP</div>
    </div>
  </div>
</div>

<!-- Contest Format Section -->
<div class="format-section">
  <h2>
    <span class="en-content">📋 Contest Format</span>
    <span class="zh-content">📋 比赛形式</span>
  </h2>
  <p>
    <span class="en-content">14-day team-based mathematical modeling challenge</span>
    <span class="zh-content">14天团队数学建模挑战</span>
  </p>
  
  <div class="format-grid">
    <div class="format-card">
      <div class="format-card-icon">👥</div>
      <h3>1-4</h3>
      <p>
        <span class="en-content">Team Members<br>(Same School)</span>
        <span class="zh-content">团队成员<br>（同一学校）</span>
      </p>
    </div>
    <div class="format-card">
      <div class="format-card-icon">📅</div>
      <h3>14</h3>
      <p>
        <span class="en-content">Days to<br>Complete</span>
        <span class="zh-content">天完成<br>时间</span>
      </p>
    </div>
    <div class="format-card">
      <div class="format-card-icon">📄</div>
      <h3>25</h3>
      <p>
        <span class="en-content">Max Pages<br>Report</span>
        <span class="zh-content">页论文<br>上限</span>
      </p>
    </div>
    <div class="format-card">
      <div class="format-card-icon">❓</div>
      <h3>2</h3>
      <p>
        <span class="en-content">Problems<br>to Choose</span>
        <span class="zh-content">道题目<br>选择</span>
      </p>
    </div>
  </div>
</div>

<!-- Timeline Section -->
<div class="timeline-section">
  <h2>
    <span class="en-content">📅 2025 Contest Timeline</span>
    <span class="zh-content">📅 2025年比赛时间线</span>
  </h2>
  
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-dot">📝</div>
      <div class="timeline-date">September</div>
      <div class="timeline-title">
        <span class="en-content">Registration Opens</span>
        <span class="zh-content">注册开放</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-dot">🚀</div>
      <div class="timeline-date">Nov 5</div>
      <div class="timeline-title">
        <span class="en-content">Contest Begins (3PM EST)</span>
        <span class="zh-content">比赛开始</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-dot">📤</div>
      <div class="timeline-date">Nov 18</div>
      <div class="timeline-title">
        <span class="en-content">Submission Deadline</span>
        <span class="zh-content">提交截止</span>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-dot">🏆</div>
      <div class="timeline-date">February</div>
      <div class="timeline-title">
        <span class="en-content">Results Announced</span>
        <span class="zh-content">结果公布</span>
      </div>
    </div>
  </div>
</div>

<!-- Awards Section -->
<div class="awards-section">
  <h2>
    <span class="en-content">🏆 Award Levels</span>
    <span class="zh-content">🏆 奖项级别</span>
  </h2>
  <p>
    <span class="en-content">Recognition based on solution quality and modeling excellence</span>
    <span class="zh-content">根据解决方案质量和建模卓越程度评定</span>
  </p>
  
  <div class="awards-grid">
    <div class="award-card outstanding">
      <div class="award-icon">🥇</div>
      <div class="award-name">Outstanding</div>
      <div class="award-percent">
        <span class="en-content">Top ~1%</span>
        <span class="zh-content">前~1%</span>
      </div>
    </div>
    <div class="award-card finalist">
      <div class="award-icon">🥈</div>
      <div class="award-name">Finalist</div>
      <div class="award-percent">
        <span class="en-content">Top ~5-6%</span>
        <span class="zh-content">前~5-6%</span>
      </div>
    </div>
    <div class="award-card meritorious">
      <div class="award-icon">🥉</div>
      <div class="award-name">Meritorious</div>
      <div class="award-percent">
        <span class="en-content">Top ~14-16%</span>
        <span class="zh-content">前~14-16%</span>
      </div>
    </div>
    <div class="award-card">
      <div class="award-icon">📜</div>
      <div class="award-name">Honorable Mention</div>
      <div class="award-percent">
        <span class="en-content">Top ~24-28%</span>
        <span class="zh-content">前~24-28%</span>
      </div>
    </div>
    <div class="award-card">
      <div class="award-icon">✅</div>
      <div class="award-name">Successful Participant</div>
      <div class="award-percent">
        <span class="en-content">Valid Submission</span>
        <span class="zh-content">有效提交</span>
      </div>
    </div>
  </div>
</div>

<!-- Skills Section -->
<div class="skills-section">
  <h2>
    <span class="en-content">🎯 Skills for Mathematical Modeling</span>
    <span class="zh-content">🎯 数学建模所需技能</span>
  </h2>
  <p>
    <span class="en-content">Master these core competencies to excel in HiMCM</span>
    <span class="zh-content">掌握这些核心能力，在HiMCM中脱颖而出</span>
  </p>
  
  <div class="skills-grid">
    <div class="skill-card modeling">
      <h3><span>📐</span>
        <span class="en-content">Mathematical Modeling</span>
        <span class="zh-content">数学建模</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Optimization & Linear Programming</span><span class="zh-content">优化与线性规划</span></li>
        <li><span class="en-content">Differential Equations</span><span class="zh-content">微分方程</span></li>
        <li><span class="en-content">Graph Theory & Networks</span><span class="zh-content">图论与网络</span></li>
        <li><span class="en-content">Simulation & Monte Carlo</span><span class="zh-content">模拟与蒙特卡洛</span></li>
        <li><span class="en-content">Game Theory</span><span class="zh-content">博弈论</span></li>
      </ul>
    </div>
    
    <div class="skill-card programming">
      <h3><span>💻</span>
        <span class="en-content">Programming & Tools</span>
        <span class="zh-content">编程与工具</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Python (NumPy, Pandas, Matplotlib)</span><span class="zh-content">Python (NumPy, Pandas, Matplotlib)</span></li>
        <li><span class="en-content">MATLAB / R</span><span class="zh-content">MATLAB / R</span></li>
        <li><span class="en-content">Excel & Spreadsheets</span><span class="zh-content">Excel与电子表格</span></li>
        <li><span class="en-content">Data Visualization</span><span class="zh-content">数据可视化</span></li>
        <li><span class="en-content">LaTeX for Report Writing</span><span class="zh-content">LaTeX论文写作</span></li>
      </ul>
    </div>
    
    <div class="skill-card stats">
      <h3><span>📊</span>
        <span class="en-content">Statistics & Data Analysis</span>
        <span class="zh-content">统计与数据分析</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Regression Analysis</span><span class="zh-content">回归分析</span></li>
        <li><span class="en-content">Probability Distributions</span><span class="zh-content">概率分布</span></li>
        <li><span class="en-content">Hypothesis Testing</span><span class="zh-content">假设检验</span></li>
        <li><span class="en-content">Time Series Analysis</span><span class="zh-content">时间序列分析</span></li>
        <li><span class="en-content">Sensitivity Analysis</span><span class="zh-content">敏感性分析</span></li>
      </ul>
    </div>
    
    <div class="skill-card writing">
      <h3><span>✍️</span>
        <span class="en-content">Technical Writing</span>
        <span class="zh-content">技术写作</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Executive Summary Writing</span><span class="zh-content">执行摘要写作</span></li>
        <li><span class="en-content">Model Documentation</span><span class="zh-content">模型文档</span></li>
        <li><span class="en-content">Clear Assumptions & Variables</span><span class="zh-content">清晰假设与变量</span></li>
        <li><span class="en-content">Results Presentation</span><span class="zh-content">结果呈现</span></li>
        <li><span class="en-content">Strengths & Weaknesses Analysis</span><span class="zh-content">优缺点分析</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Past Problems Section -->
<div class="problems-section">
  <h2>
    <span class="en-content">📝 Sample Past Problems</span>
    <span class="zh-content">📝 历年问题样例</span>
  </h2>
  <p>
    <span class="en-content">Real-world challenges that test modeling skills</span>
    <span class="zh-content">测试建模技能的真实世界挑战</span>
  </p>
  
  <div class="problems-grid">
    <div class="problem-card">
      <div class="problem-year">2024</div>
      <h3>
        <span class="en-content">Roller Coaster Ranking System</span>
        <span class="zh-content">过山车排名系统</span>
      </h3>
      <p>
        <span class="en-content">Develop an objective ranking system for roller coasters considering multiple factors</span>
        <span class="zh-content">开发考虑多种因素的过山车客观排名系统</span>
      </p>
    </div>
    <div class="problem-card">
      <div class="problem-year">2024</div>
      <h3>
        <span class="en-content">Drone Light Shows</span>
        <span class="zh-content">无人机灯光秀</span>
      </h3>
      <p>
        <span class="en-content">Design an aerial drone light show with coordinated clusters</span>
        <span class="zh-content">设计协调集群的空中无人机灯光秀</span>
      </p>
    </div>
    <div class="problem-card">
      <div class="problem-year">2023</div>
      <h3>
        <span class="en-content">Dandelion Spread Prediction</span>
        <span class="zh-content">蒲公英传播预测</span>
      </h3>
      <p>
        <span class="en-content">Model invasive species spread considering climate and environmental factors</span>
        <span class="zh-content">考虑气候和环境因素建模入侵物种传播</span>
      </p>
    </div>
    <div class="problem-card">
      <div class="problem-year">2023</div>
      <h3>
        <span class="en-content">Electric Bus Transition</span>
        <span class="zh-content">电动巴士转型</span>
      </h3>
      <p>
        <span class="en-content">Optimize the transition from diesel to electric buses in cities</span>
        <span class="zh-content">优化城市从柴油巴士到电动巴士的转型</span>
      </p>
    </div>
  </div>
</div>

<!-- Report Structure Section -->
<div class="report-section">
  <h2>
    <span class="en-content">📄 Solution Report Structure</span>
    <span class="zh-content">📄 解决方案报告结构</span>
  </h2>
  <p>
    <span class="en-content">Key components of a winning HiMCM paper</span>
    <span class="zh-content">获奖HiMCM论文的关键组成部分</span>
  </p>
  
  <div class="report-structure">
    <div class="report-item important">
      <div class="report-item-icon">⭐</div>
      <h3>
        <span class="en-content">Summary Sheet</span>
        <span class="zh-content">摘要页</span>
      </h3>
      <p>
        <span class="en-content">1 page - Most critical!</span>
        <span class="zh-content">1页 - 最关键！</span>
      </p>
    </div>
    <div class="report-item">
      <div class="report-item-icon">📋</div>
      <h3>
        <span class="en-content">Problem Restatement</span>
        <span class="zh-content">问题重述</span>
      </h3>
      <p>
        <span class="en-content">Clear understanding</span>
        <span class="zh-content">清晰理解</span>
      </p>
    </div>
    <div class="report-item">
      <div class="report-item-icon">📝</div>
      <h3>
        <span class="en-content">Assumptions</span>
        <span class="zh-content">假设条件</span>
      </h3>
      <p>
        <span class="en-content">Justified & reasonable</span>
        <span class="zh-content">合理且有依据</span>
      </p>
    </div>
    <div class="report-item">
      <div class="report-item-icon">🔧</div>
      <h3>
        <span class="en-content">Model Design</span>
        <span class="zh-content">模型设计</span>
      </h3>
      <p>
        <span class="en-content">Mathematical approach</span>
        <span class="zh-content">数学方法</span>
      </p>
    </div>
    <div class="report-item">
      <div class="report-item-icon">📊</div>
      <h3>
        <span class="en-content">Results & Analysis</span>
        <span class="zh-content">结果与分析</span>
      </h3>
      <p>
        <span class="en-content">Data visualization</span>
        <span class="zh-content">数据可视化</span>
      </p>
    </div>
    <div class="report-item">
      <div class="report-item-icon">⚖️</div>
      <h3>
        <span class="en-content">Strengths & Weaknesses</span>
        <span class="zh-content">优缺点分析</span>
      </h3>
      <p>
        <span class="en-content">Critical evaluation</span>
        <span class="zh-content">批判性评估</span>
      </p>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <h2>
    <span class="en-content">Why Train With Us for HiMCM?</span>
    <span class="zh-content">为什么选择我们的HiMCM培训？</span>
  </h2>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">Modeling Techniques</span>
        <span class="zh-content">建模技术</span>
      </h3>
      <p>
        <span class="en-content">Learn optimization, simulation, and statistical modeling approaches</span>
        <span class="zh-content">学习优化、模拟和统计建模方法</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">💻</div>
      <h3>
        <span class="en-content">Programming Skills</span>
        <span class="zh-content">编程技能</span>
      </h3>
      <p>
        <span class="en-content">Python, MATLAB, and data visualization for model implementation</span>
        <span class="zh-content">Python、MATLAB和数据可视化实现模型</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">✍️</div>
      <h3>
        <span class="en-content">Technical Writing</span>
        <span class="zh-content">技术写作</span>
      </h3>
      <p>
        <span class="en-content">Write clear, compelling reports that impress judges</span>
        <span class="zh-content">撰写清晰、有说服力的报告以打动评委</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Past Problem Analysis</span>
        <span class="zh-content">历年问题分析</span>
      </h3>
      <p>
        <span class="en-content">Study winning solutions and understand what makes them successful</span>
        <span class="zh-content">研究获奖方案，了解成功要素</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">Mock Competitions</span>
        <span class="zh-content">模拟竞赛</span>
      </h3>
      <p>
        <span class="en-content">Practice with timed team challenges before the real contest</span>
        <span class="zh-content">在真正比赛前进行计时团队挑战练习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Teams</span>
        <span class="zh-content">小组教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 8 students for personalized mentorship and feedback</span>
        <span class="zh-content">每班最多8人，个性化指导和反馈</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' HiMCM Achievements</span>
    <span class="zh-content">🏆 我们学生的HiMCM成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">5</span>
      <div class="success-label">
        <span class="en-content">Outstanding Winners</span>
        <span class="zh-content">特等奖</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🥈</div>
      <span class="success-number">15+</span>
      <div class="success-label">
        <span class="en-content">Finalists</span>
        <span class="zh-content">决赛入围</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">85%</span>
      <div class="success-label">
        <span class="en-content">Meritorious+</span>
        <span class="zh-content">优异奖+</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🌍</div>
      <span class="success-number">8</span>
      <div class="success-label">
        <span class="en-content">IM2C Qualifiers</span>
        <span class="zh-content">IM2C晋级</span>
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
      <span class="testimonial-badge outstanding">Outstanding</span>
      <p class="testimonial-text">
        <span class="en-content">The modeling techniques and technical writing skills I learned were game-changers. Our team won Outstanding and qualified for IM2C! The mock competitions really prepared us for the pressure.</span>
        <span class="zh-content">我学到的建模技术和技术写作技能是致胜关键。我们团队获得特等奖并晋级IM2C！模拟比赛真正让我们为压力做好了准备。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Michael Z.</h4>
          <p>
            <span class="en-content">HiMCM 2024 Outstanding</span>
            <span class="zh-content">HiMCM 2024特等奖</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge finalist">Finalist</span>
      <p class="testimonial-text">
        <span class="en-content">Learning Python for data visualization transformed our report. The judges commented on how professional our graphs looked. Made Finalist in our first year competing!</span>
        <span class="zh-content">学习Python数据可视化改变了我们的报告。评委评价我们的图表看起来很专业。第一年参赛就成为决赛入围！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Emma L.</h4>
          <p>
            <span class="en-content">HiMCM 2024 Finalist</span>
            <span class="zh-content">HiMCM 2024决赛入围</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge meritorious">Meritorious</span>
      <p class="testimonial-text">
        <span class="en-content">The summary sheet workshop was incredible. That single page can make or break your paper, and our instructor showed us exactly how to write one that captures judges' attention.</span>
        <span class="zh-content">摘要页工作坊非常精彩。那一页可以决定论文成败，我们的导师展示了如何撰写能吸引评委注意力的摘要。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Kevin W.</h4>
          <p>
            <span class="en-content">HiMCM 2024 Meritorious</span>
            <span class="zh-content">HiMCM 2024优异奖</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Master Mathematical Modeling!</span>
    <span class="zh-content">精通数学建模！</span>
  </h2>
  <p>
    <span class="en-content">Join our training program and compete for Outstanding recognition</span>
    <span class="zh-content">加入我们的培训计划，竞争特等奖荣誉</span>
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
