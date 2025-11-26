---
layout: default
title: WorldQuant Competition Training
title_zh: WorldQuant量化竞赛培训
description: Master Quantitative Finance & Alpha Creation for IQC Success
description_zh: 掌握量化金融与Alpha策略，征服IQC国际量化锦标赛
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

  @keyframes dataFlow {
    0% { background-position: 0% 0%; }
    100% { background-position: 100% 100%; }
  }

  @keyframes chartPulse {
    0%, 100% { transform: scaleY(1); }
    50% { transform: scaleY(1.1); }
  }

  @keyframes stockTicker {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }

  /* Course Hero - Ultra Premium Navy/Gold Finance Theme */
  .course-hero {
    background: linear-gradient(135deg, #0F172A 0%, #1E293B 25%, #334155 50%, #1E293B 75%, #0F172A 100%);
    background-size: 300% 300%;
    animation: gradientWave 15s ease infinite;
    padding: 6rem 2rem;
    border-radius: 30px;
    color: white;
    text-align: center;
    margin-bottom: 4rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(15, 23, 42, 0.5);
    min-height: 520px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '📈';
    position: absolute;
    font-size: 18rem;
    opacity: 0.05;
    right: -30px;
    top: -40px;
  }

  .course-hero::after {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(234, 179, 8, 0.08) 0%, transparent 70%);
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

  .prize-badge {
    position: absolute;
    top: 30px;
    right: 30px;
    background: linear-gradient(135deg, #EAB308 0%, #CA8A04 50%, #A16207 100%);
    color: #422006;
    padding: 0.6rem 1.5rem;
    border-radius: 25px;
    font-weight: 800;
    font-size: 0.9rem;
    z-index: 10;
    box-shadow: 0 8px 20px rgba(234, 179, 8, 0.5);
    animation: pulse 2s ease-in-out infinite;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    border: 2px solid rgba(255, 255, 255, 0.3);
  }

  .prize-badge::before {
    content: '💰';
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
    color: #EAB308 !important;
    font-size: 1.4rem;
    font-weight: 600;
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
    background: rgba(234, 179, 8, 0.15);
    backdrop-filter: blur(10px);
    padding: 1rem 2rem;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.1rem;
    border: 2px solid rgba(234, 179, 8, 0.4);
    position: relative;
    z-index: 1;
    animation: slideInUp 1s ease-out 0.4s backwards;
    color: #FDE68A;
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
    color: #EAB308;
  }

  .hero-stat-label {
    font-size: 0.9rem;
    opacity: 0.9;
    color: #CBD5E1;
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
    background: linear-gradient(135deg, #1E293B 0%, #334155 50%, #475569 100%);
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

  /* What is WorldQuant Section */
  .intro-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    position: relative;
    overflow: hidden;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #EAB308, #CA8A04, #1E293B, #334155) 1;
  }

  .intro-section::before {
    content: '🧠';
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
    background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 100%);
    border-radius: 12px;
    transition: all 0.3s ease;
  }

  .intro-highlight:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(234, 179, 8, 0.2);
  }

  .intro-highlight-icon {
    font-size: 1.5rem;
  }

  .intro-highlight-text {
    font-weight: 600;
    color: #1F2937;
    font-size: 0.95rem;
  }

  /* BRAIN Platform Section */
  .brain-section {
    background: linear-gradient(135deg, #0F172A 0%, #1E293B 50%, #334155 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .brain-section::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(234, 179, 8, 0.08) 0%, transparent 50%);
    animation: rotateGlow 20s linear infinite;
  }

  .brain-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #EAB308 !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .brain-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .brain-features {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1000px) {
    .brain-features {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .brain-features {
      grid-template-columns: 1fr;
    }
  }

  .brain-feature {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .brain-feature:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .brain-feature-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .brain-feature h3 {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .brain-feature p {
    color: #6B7280;
    font-size: 0.9rem;
    line-height: 1.5;
  }

  /* What is Alpha Section */
  .alpha-section {
    background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 50%, #FDE68A 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .alpha-section::before {
    content: 'α';
    position: absolute;
    font-size: 25rem;
    opacity: 0.06;
    right: -50px;
    top: -80px;
    font-family: Georgia, serif;
    font-weight: bold;
  }

  .alpha-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 900px) {
    .alpha-content {
      grid-template-columns: 1fr;
    }
  }

  .alpha-text h2 {
    font-size: 2.2rem;
    font-weight: 800;
    color: #78350F;
    margin-bottom: 1.5rem;
  }

  .alpha-text p {
    color: #92400E;
    font-size: 1.05rem;
    line-height: 1.8;
    margin-bottom: 1rem;
  }

  .alpha-formula {
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  }

  .alpha-formula h3 {
    font-size: 1.2rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 1rem;
    text-align: center;
  }

  .formula-box {
    background: linear-gradient(135deg, #1E293B, #334155);
    padding: 1.5rem;
    border-radius: 15px;
    text-align: center;
    margin-bottom: 1rem;
  }

  .formula-box code {
    color: #EAB308;
    font-size: 1.1rem;
    font-family: 'Monaco', 'Consolas', monospace;
  }

  .formula-metrics {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
  }

  .metric {
    text-align: center;
    padding: 1rem;
    background: #F3F4F6;
    border-radius: 10px;
  }

  .metric-value {
    font-size: 1.2rem;
    font-weight: 800;
    color: #1E293B;
  }

  .metric-label {
    font-size: 0.75rem;
    color: #6B7280;
  }

  /* IQC Competition Section */
  .iqc-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .iqc-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #1E293B 0%, #EAB308 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .iqc-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .iqc-stages {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-bottom: 3rem;
  }

  @media (max-width: 900px) {
    .iqc-stages {
      grid-template-columns: 1fr;
    }
  }

  .iqc-stage {
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    border-top: 4px solid;
    transition: all 0.4s ease;
  }

  .iqc-stage:nth-child(1) { border-top-color: #3B82F6; }
  .iqc-stage:nth-child(2) { border-top-color: #EAB308; }
  .iqc-stage:nth-child(3) { border-top-color: #10B981; }

  .iqc-stage:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  }

  .stage-number {
    width: 60px;
    height: 60px;
    margin: 0 auto 1rem;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    font-weight: 800;
    color: white;
  }

  .iqc-stage:nth-child(1) .stage-number { background: linear-gradient(135deg, #3B82F6, #2563EB); }
  .iqc-stage:nth-child(2) .stage-number { background: linear-gradient(135deg, #EAB308, #CA8A04); }
  .iqc-stage:nth-child(3) .stage-number { background: linear-gradient(135deg, #10B981, #059669); }

  .iqc-stage h3 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .stage-dates {
    font-size: 0.9rem;
    color: #6B7280;
    margin-bottom: 1rem;
    font-weight: 600;
  }

  .iqc-stage p {
    color: #4B5563;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Prize Pool Section */
  .prizes-section {
    background: linear-gradient(135deg, #0F172A 0%, #1E293B 100%);
    padding: 3rem;
    border-radius: 20px;
    margin-top: 3rem;
  }

  .prizes-section h3 {
    text-align: center;
    font-size: 1.8rem;
    font-weight: 800;
    color: #EAB308 !important;
    margin-bottom: 2rem;
  }

  .prizes-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    max-width: 800px;
    margin: 0 auto;
  }

  @media (max-width: 700px) {
    .prizes-grid {
      grid-template-columns: 1fr;
    }
  }

  .prize-card {
    background: white;
    padding: 2rem;
    border-radius: 15px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .prize-card:hover {
    transform: scale(1.05);
  }

  .prize-card.gold {
    background: linear-gradient(135deg, #FEF9C3, #FEF08A);
    box-shadow: 0 10px 30px rgba(234, 179, 8, 0.3);
  }

  .prize-card.silver {
    background: linear-gradient(135deg, #F3F4F6, #E5E7EB);
  }

  .prize-card.bronze {
    background: linear-gradient(135deg, #FED7AA, #FDBA74);
  }

  .prize-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .prize-place {
    font-size: 1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .prize-amount {
    font-size: 1.5rem;
    font-weight: 800;
    color: #1E293B;
  }

  /* Skills Section */
  .skills-section {
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
  }

  .skills-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #1E293B 0%, #475569 100%);
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
    background: white;
    padding: 2rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    border-left: 4px solid;
    transition: all 0.4s ease;
  }

  .skill-card:hover {
    transform: translateX(5px);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.12);
  }

  .skill-card.math { border-left-color: #3B82F6; }
  .skill-card.stats { border-left-color: #10B981; }
  .skill-card.coding { border-left-color: #8B5CF6; }
  .skill-card.finance { border-left-color: #EAB308; }

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
    border-bottom: 1px solid #F3F4F6;
  }

  .skill-topics li:last-child {
    border-bottom: none;
  }

  .skill-topics li::before {
    content: '▸';
    font-weight: bold;
  }

  .skill-card.math .skill-topics li::before { color: #3B82F6; }
  .skill-card.stats .skill-topics li::before { color: #10B981; }
  .skill-card.coding .skill-topics li::before { color: #8B5CF6; }
  .skill-card.finance .skill-topics li::before { color: #EAB308; }

  /* Consultant Program Section */
  .consultant-section {
    background: linear-gradient(135deg, #1E293B 0%, #334155 50%, #475569 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .consultant-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(234, 179, 8, 0.1) 0%, transparent 50%);
    animation: rotateGlow 15s linear infinite;
  }

  .consultant-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: white !important;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .consultant-section > p {
    text-align: center;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1rem;
    margin-bottom: 3rem;
    position: relative;
    z-index: 1;
  }

  .consultant-tiers {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    max-width: 800px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 700px) {
    .consultant-tiers {
      grid-template-columns: 1fr;
    }
  }

  .tier-card {
    background: white;
    padding: 2.5rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
  }

  .tier-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
  }

  .tier-card.grandmaster {
    background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 50%, #FDE68A 100%);
    border: 3px solid #EAB308;
  }

  .tier-card.master {
    background: linear-gradient(135deg, #E0E7FF 0%, #C7D2FE 100%);
    border: 3px solid #6366F1;
  }

  .tier-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .tier-card h3 {
    font-size: 1.5rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .tier-earnings {
    font-size: 2rem;
    font-weight: 800;
    margin: 1rem 0;
  }

  .tier-card.grandmaster .tier-earnings { color: #92400E; }
  .tier-card.master .tier-earnings { color: #4338CA; }

  .tier-period {
    font-size: 0.9rem;
    color: #6B7280;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .why-choose-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #1E293B 0%, #475569 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 3rem;
  }

  .why-choose-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
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
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border: 2px solid transparent;
  }

  .why-choose-item:hover {
    transform: translateY(-5px);
    border-color: #1E293B;
    box-shadow: 0 20px 40px rgba(30, 41, 59, 0.1);
  }

  .why-icon {
    width: 70px;
    height: 70px;
    margin: 0 auto 1.5rem;
    background: linear-gradient(135deg, #1E293B 0%, #334155 100%);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    box-shadow: 0 10px 20px rgba(30, 41, 59, 0.3);
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
    background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 50%, #FDE68A 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
  }

  .success-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #78350F !important;
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
    background: white;
    border-radius: 20px;
    transition: all 0.4s ease;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 200px;
  }

  .success-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.12);
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
    background: linear-gradient(135deg, #92400E 0%, #78350F 100%);
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
    background: linear-gradient(135deg, #F8FAFC 0%, #F1F5F9 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #1E293B 0%, #475569 100%);
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
    color: #1E293B;
    opacity: 0.1;
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

  .testimonial-badge.finals { background: linear-gradient(135deg, #EAB308, #CA8A04); }
  .testimonial-badge.consultant { background: linear-gradient(135deg, #10B981, #059669); }
  .testimonial-badge.top1 { background: linear-gradient(135deg, #3B82F6, #2563EB); }

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
    background: linear-gradient(135deg, #1E293B 0%, #334155 100%);
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
    background: linear-gradient(135deg, #0F172A 0%, #1E293B 25%, #334155 50%, #1E293B 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    padding: 5rem 3rem;
    border-radius: 30px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(15, 23, 42, 0.5);
    margin-top: 4rem;
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(234, 179, 8, 0.15) 0%, transparent 60%);
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
    color: #CBD5E1 !important;
    font-size: 1.3rem;
    margin: 1rem 0 2rem;
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
    background: linear-gradient(135deg, #EAB308 0%, #CA8A04 100%);
    color: #422006;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 700;
    font-size: 1.2rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(234, 179, 8, 0.3);
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
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(234, 179, 8, 0.4);
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid #EAB308;
    color: #EAB308;
  }

  .cta-button-secondary:hover {
    background: #EAB308;
    color: #422006;
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
    .brain-section,
    .alpha-section,
    .iqc-section,
    .skills-section,
    .consultant-section,
    .why-choose-section,
    .success-section {
      padding: 3rem 1.5rem;
    }

    .prize-badge {
      top: 15px;
      right: 15px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
    }
  }
</style>

<div class="course-hero">
  <span class="prize-badge">
    <span class="en-content">$100K PRIZE POOL</span>
    <span class="zh-content">$10万奖金池</span>
  </span>
  <div class="icons-bg">
    <span class="floating-icon">📈</span>
    <span class="floating-icon">💹</span>
    <span class="floating-icon">🧠</span>
    <span class="floating-icon">📊</span>
    <span class="floating-icon">💰</span>
    <span class="floating-icon">🔢</span>
    <span class="floating-icon">⚡</span>
  </div>
  <h1>
    <span class="en-content">WorldQuant Training</span>
    <span class="zh-content">WorldQuant量化竞赛培训</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">International Quant Championship & BRAIN Platform</span>
    <span class="zh-content">国际量化锦标赛 & BRAIN平台</span>
  </p>
  <div class="hero-badge">
    <span>🌐</span>
    <span class="en-content">80,000+ Participants • 142 Countries • 11,000 Universities</span>
    <span class="zh-content">8万+参赛者 • 142个国家 • 11000所大学</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">$100K</span>
      <span class="hero-stat-label">
        <span class="en-content">Prize Pool</span>
        <span class="zh-content">奖金池</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">125K+</span>
      <span class="hero-stat-label">
        <span class="en-content">Data Fields</span>
        <span class="zh-content">数据字段</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">3</span>
      <span class="hero-stat-label">
        <span class="en-content">Stages</span>
        <span class="zh-content">竞赛阶段</span>
      </span>
    </div>
  </div>
</div>

<!-- What is WorldQuant -->
<div class="intro-section">
  <div class="intro-content">
    <div class="intro-text">
      <h2>
        <span class="en-content">What is WorldQuant?</span>
        <span class="zh-content">什么是WorldQuant？</span>
      </h2>
      <p>
        <span class="en-content">
          WorldQuant is a global quantitative asset management firm founded in 2007 by Igor Tulchinsky. 
          With the belief that "talent is global, but opportunity is not," WorldQuant has grown to over 
          1,000 employees across 27 offices worldwide, managing sophisticated investment strategies.
        </span>
        <span class="zh-content">
          WorldQuant是一家全球量化资产管理公司，由Igor Tulchinsky于2007年创立。
          秉持"人才遍布全球，但机遇并非如此"的理念，WorldQuant已发展到全球27个办公室超过1000名员工，
          管理着复杂的投资策略。
        </span>
      </p>
      <p>
        <span class="en-content">
          Through the WorldQuant BRAIN platform and International Quant Championship (IQC), they identify 
          top quant talent globally. Top performers may be offered research consultant positions, 
          internships, or full-time employment opportunities.
        </span>
        <span class="zh-content">
          通过WorldQuant BRAIN平台和国际量化锦标赛(IQC)，他们在全球发掘顶尖量化人才。
          表现优异者可能获得研究顾问职位、实习或全职工作机会。
        </span>
      </p>
      <div class="intro-highlights">
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🌍</span>
          <span class="intro-highlight-text">
            <span class="en-content">27 Global Offices</span>
            <span class="zh-content">27个全球办公室</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">💼</span>
          <span class="intro-highlight-text">
            <span class="en-content">Career Opportunities</span>
            <span class="zh-content">职业机会</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🧠</span>
          <span class="intro-highlight-text">
            <span class="en-content">225K+ BRAIN Users</span>
            <span class="zh-content">22.5万+ BRAIN用户</span>
          </span>
        </div>
        <div class="intro-highlight">
          <span class="intro-highlight-icon">🏆</span>
          <span class="intro-highlight-text">
            <span class="en-content">9,000+ Consultants</span>
            <span class="zh-content">9000+研究顾问</span>
          </span>
        </div>
      </div>
    </div>
    <div class="intro-visual" style="text-align: center;">
      <div style="font-size: 6rem; animation: float 5s ease-in-out infinite;">🧠</div>
      <div style="font-size: 2rem; font-weight: 800; color: #1E293B; margin-top: 1rem;">BRAIN</div>
    </div>
  </div>
</div>

<!-- BRAIN Platform Section -->
<div class="brain-section">
  <h2>
    <span class="en-content">🧠 WorldQuant BRAIN Platform</span>
    <span class="zh-content">🧠 WorldQuant BRAIN平台</span>
  </h2>
  <p>
    <span class="en-content">An interactive simulation environment for building and testing alpha strategies</span>
    <span class="zh-content">用于构建和测试Alpha策略的交互式模拟环境</span>
  </p>
  
  <div class="brain-features">
    <div class="brain-feature">
      <div class="brain-feature-icon">📊</div>
      <h3>
        <span class="en-content">125K+ Data Fields</span>
        <span class="zh-content">12.5万+数据字段</span>
      </h3>
      <p>
        <span class="en-content">Market, economic & alternative datasets</span>
        <span class="zh-content">市场、经济和另类数据集</span>
      </p>
    </div>
    <div class="brain-feature">
      <div class="brain-feature-icon">⚡</div>
      <h3>
        <span class="en-content">Real-time Backtesting</span>
        <span class="zh-content">实时回测</span>
      </h3>
      <p>
        <span class="en-content">Test alpha ideas instantly with simulation</span>
        <span class="zh-content">通过模拟即时测试Alpha想法</span>
      </p>
    </div>
    <div class="brain-feature">
      <div class="brain-feature-icon">🤖</div>
      <h3>
        <span class="en-content">ML & AI Tools</span>
        <span class="zh-content">机器学习与AI工具</span>
      </h3>
      <p>
        <span class="en-content">Integrated machine learning modules</span>
        <span class="zh-content">集成机器学习模块</span>
      </p>
    </div>
    <div class="brain-feature">
      <div class="brain-feature-icon">🐍</div>
      <h3>
        <span class="en-content">Python API</span>
        <span class="zh-content">Python API</span>
      </h3>
      <p>
        <span class="en-content">Advanced features via Python integration</span>
        <span class="zh-content">通过Python集成高级功能</span>
      </p>
    </div>
  </div>
</div>

<!-- What is Alpha Section -->
<div class="alpha-section">
  <div class="alpha-content">
    <div class="alpha-text">
      <h2>
        <span class="en-content">What is an Alpha?</span>
        <span class="zh-content">什么是Alpha？</span>
      </h2>
      <p>
        <span class="en-content">
          In WorldQuant's context, <strong>Alphas</strong> are mathematical models that seek to predict 
          the future price movements of financial instruments. They assign weights to securities 
          based on predictions of expected returns.
        </span>
        <span class="zh-content">
          在WorldQuant的语境中，<strong>Alpha</strong>是一种数学模型，旨在预测金融工具的未来价格走势。
          它们根据预期收益的预测为证券分配权重。
        </span>
      </p>
      <p>
        <span class="en-content">
          Alphas are evaluated based on their Sharpe ratio (risk-adjusted returns), turnover 
          (trading frequency), and a custom "fitness" metric. High-quality alphas generate 
          stable returns with low correlation to existing strategies.
        </span>
        <span class="zh-content">
          Alpha基于其夏普比率（风险调整收益）、换手率（交易频率）和自定义的"适应度"指标进行评估。
          高质量的Alpha能够产生稳定的收益，且与现有策略的相关性较低。
        </span>
      </p>
    </div>
    <div class="alpha-formula">
      <h3>
        <span class="en-content">Alpha Performance Metrics</span>
        <span class="zh-content">Alpha性能指标</span>
      </h3>
      <div class="formula-box">
        <code>Fitness = √(|Returns| / max(turnover, 0.125)) × Sharpe</code>
      </div>
      <div class="formula-metrics">
        <div class="metric">
          <div class="metric-value">Sharpe</div>
          <div class="metric-label">
            <span class="en-content">Risk-adjusted</span>
            <span class="zh-content">风险调整</span>
          </div>
        </div>
        <div class="metric">
          <div class="metric-value">Returns</div>
          <div class="metric-label">
            <span class="en-content">Profitability</span>
            <span class="zh-content">盈利能力</span>
          </div>
        </div>
        <div class="metric">
          <div class="metric-value">Turnover</div>
          <div class="metric-label">
            <span class="en-content">Trading freq</span>
            <span class="zh-content">交易频率</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- IQC Competition Section -->
<div class="iqc-section">
  <h2>
    <span class="en-content">🏆 International Quant Championship (IQC)</span>
    <span class="zh-content">🏆 国际量化锦标赛 (IQC)</span>
  </h2>
  <p>
    <span class="en-content">WorldQuant's flagship global competition for aspiring quants</span>
    <span class="zh-content">WorldQuant面向有志成为量化分析师者的旗舰全球竞赛</span>
  </p>
  
  <div class="iqc-stages">
    <div class="iqc-stage">
      <div class="stage-number">1</div>
      <h3>
        <span class="en-content">Qualifier Round</span>
        <span class="zh-content">资格赛</span>
      </h3>
      <div class="stage-dates">Mar - May</div>
      <p>
        <span class="en-content">Teams of 1-4 from same university compete by building alphas. Top teams advance to represent their institution.</span>
        <span class="zh-content">来自同一大学的1-4人团队通过构建Alpha竞争。顶尖团队晋级代表其院校。</span>
      </p>
    </div>
    <div class="iqc-stage">
      <div class="stage-number">2</div>
      <h3>
        <span class="en-content">National/Regional</span>
        <span class="zh-content">国家/地区赛</span>
      </h3>
      <div class="stage-dates">May - July</div>
      <p>
        <span class="en-content">Virtual qualifying round + final presentation. Top 8 teams per region advance to final round.</span>
        <span class="zh-content">虚拟资格赛 + 决赛演示。每个地区前8名团队晋级决赛轮。</span>
      </p>
    </div>
    <div class="iqc-stage">
      <div class="stage-number">3</div>
      <h3>
        <span class="en-content">Global Finals</span>
        <span class="zh-content">全球总决赛</span>
      </h3>
      <div class="stage-dates">September (Singapore)</div>
      <p>
        <span class="en-content">In-person competition in Singapore. Live alpha challenge and presentation to WorldQuant senior management.</span>
        <span class="zh-content">新加坡现场比赛。向WorldQuant高管进行实时Alpha挑战和演示。</span>
      </p>
    </div>
  </div>
  
  <div class="prizes-section">
    <h3>
      <span class="en-content">💰 Prize Pool: $100,000</span>
      <span class="zh-content">💰 奖金池：$100,000</span>
    </h3>
    <div class="prizes-grid">
      <div class="prize-card gold">
        <div class="prize-icon">🥇</div>
        <div class="prize-place">
          <span class="en-content">1st Place</span>
          <span class="zh-content">第一名</span>
        </div>
        <div class="prize-amount">$20,000</div>
      </div>
      <div class="prize-card silver">
        <div class="prize-icon">🥈</div>
        <div class="prize-place">
          <span class="en-content">2nd Place</span>
          <span class="zh-content">第二名</span>
        </div>
        <div class="prize-amount">$10,000</div>
      </div>
      <div class="prize-card bronze">
        <div class="prize-icon">🥉</div>
        <div class="prize-place">
          <span class="en-content">3rd Place</span>
          <span class="zh-content">第三名</span>
        </div>
        <div class="prize-amount">$5,000</div>
      </div>
    </div>
  </div>
</div>

<!-- Skills Section -->
<div class="skills-section">
  <h2>
    <span class="en-content">🎯 Skills for Alpha Creation</span>
    <span class="zh-content">🎯 Alpha创建所需技能</span>
  </h2>
  <p>
    <span class="en-content">Master these core competencies to excel in quantitative finance</span>
    <span class="zh-content">掌握这些核心能力，在量化金融领域脱颖而出</span>
  </p>
  
  <div class="skills-grid">
    <div class="skill-card math">
      <h3><span>📐</span>
        <span class="en-content">Mathematics</span>
        <span class="zh-content">数学</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Linear Algebra & Matrix Operations</span><span class="zh-content">线性代数与矩阵运算</span></li>
        <li><span class="en-content">Calculus & Optimization</span><span class="zh-content">微积分与优化</span></li>
        <li><span class="en-content">Differential Equations</span><span class="zh-content">微分方程</span></li>
        <li><span class="en-content">Numerical Methods</span><span class="zh-content">数值方法</span></li>
      </ul>
    </div>
    
    <div class="skill-card stats">
      <h3><span>📊</span>
        <span class="en-content">Statistics & Probability</span>
        <span class="zh-content">统计与概率</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Statistical Inference & Hypothesis Testing</span><span class="zh-content">统计推断与假设检验</span></li>
        <li><span class="en-content">Time Series Analysis</span><span class="zh-content">时间序列分析</span></li>
        <li><span class="en-content">Regression & Correlation</span><span class="zh-content">回归与相关性</span></li>
        <li><span class="en-content">Stochastic Processes</span><span class="zh-content">随机过程</span></li>
      </ul>
    </div>
    
    <div class="skill-card coding">
      <h3><span>💻</span>
        <span class="en-content">Programming</span>
        <span class="zh-content">编程</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Python (Pandas, NumPy, SciPy)</span><span class="zh-content">Python (Pandas, NumPy, SciPy)</span></li>
        <li><span class="en-content">Data Manipulation & Analysis</span><span class="zh-content">数据处理与分析</span></li>
        <li><span class="en-content">Machine Learning (scikit-learn)</span><span class="zh-content">机器学习 (scikit-learn)</span></li>
        <li><span class="en-content">SQL & Database Queries</span><span class="zh-content">SQL与数据库查询</span></li>
      </ul>
    </div>
    
    <div class="skill-card finance">
      <h3><span>💹</span>
        <span class="en-content">Quantitative Finance</span>
        <span class="zh-content">量化金融</span>
      </h3>
      <ul class="skill-topics">
        <li><span class="en-content">Portfolio Theory & Risk Management</span><span class="zh-content">投资组合理论与风险管理</span></li>
        <li><span class="en-content">Factor Models & Asset Pricing</span><span class="zh-content">因子模型与资产定价</span></li>
        <li><span class="en-content">Derivatives & Options</span><span class="zh-content">衍生品与期权</span></li>
        <li><span class="en-content">Market Microstructure</span><span class="zh-content">市场微观结构</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- Consultant Program Section -->
<div class="consultant-section">
  <h2>
    <span class="en-content">💼 BRAIN Research Consultant Program</span>
    <span class="zh-content">💼 BRAIN研究顾问计划</span>
  </h2>
  <p>
    <span class="en-content">Top performers can become paid research consultants with WorldQuant</span>
    <span class="zh-content">表现优异者可成为WorldQuant的有偿研究顾问</span>
  </p>
  
  <div class="consultant-tiers">
    <div class="tier-card grandmaster">
      <div class="tier-icon">👑</div>
      <h3>Grandmaster</h3>
      <div class="tier-earnings">$8,000+</div>
      <div class="tier-period">
        <span class="en-content">per quarter potential</span>
        <span class="zh-content">每季度潜在收入</span>
      </div>
    </div>
    <div class="tier-card master">
      <div class="tier-icon">⭐</div>
      <h3>Master</h3>
      <div class="tier-earnings">$2,000+</div>
      <div class="tier-period">
        <span class="en-content">per quarter potential</span>
        <span class="zh-content">每季度潜在收入</span>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <h2>
    <span class="en-content">Why Train With Us for WorldQuant?</span>
    <span class="zh-content">为什么选择我们的WorldQuant培训？</span>
  </h2>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">Alpha Strategy Mastery</span>
        <span class="zh-content">Alpha策略精通</span>
      </h3>
      <p>
        <span class="en-content">Learn proven techniques for creating high-performing, uncorrelated alphas</span>
        <span class="zh-content">学习经过验证的技术，创建高性能、低相关性的Alpha</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🧠</div>
      <h3>
        <span class="en-content">BRAIN Platform Training</span>
        <span class="zh-content">BRAIN平台培训</span>
      </h3>
      <p>
        <span class="en-content">Hands-on guidance using WorldQuant's simulation platform and tools</span>
        <span class="zh-content">使用WorldQuant模拟平台和工具的实践指导</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Data Science Skills</span>
        <span class="zh-content">数据科学技能</span>
      </h3>
      <p>
        <span class="en-content">Python, machine learning, and statistical analysis for quant finance</span>
        <span class="zh-content">用于量化金融的Python、机器学习和统计分析</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">IQC Competition Prep</span>
        <span class="zh-content">IQC竞赛准备</span>
      </h3>
      <p>
        <span class="en-content">Targeted training for International Quant Championship success</span>
        <span class="zh-content">针对国际量化锦标赛成功的定向培训</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">💡</div>
      <h3>
        <span class="en-content">Expert Mentorship</span>
        <span class="zh-content">专家指导</span>
      </h3>
      <p>
        <span class="en-content">Learn from experienced quants with industry knowledge</span>
        <span class="zh-content">向具有行业知识的资深量化分析师学习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized attention and feedback</span>
        <span class="zh-content">每班最多6人，个性化关注和反馈</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Stats -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' WorldQuant Achievements</span>
    <span class="zh-content">🏆 我们学生的WorldQuant成就</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <div class="success-icon">🥇</div>
      <span class="success-number">Top&nbsp;1%</span>
      <div class="success-label">
        <span class="en-content">IQC Ranking</span>
        <span class="zh-content">IQC排名</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🏅</div>
      <span class="success-number">15+</span>
      <div class="success-label">
        <span class="en-content">Consultants</span>
        <span class="zh-content">研究顾问</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">📈</div>
      <span class="success-number">500+</span>
      <div class="success-label">
        <span class="en-content">Alphas Created</span>
        <span class="zh-content">Alpha创建</span>
      </div>
    </div>
    <div class="success-item">
      <div class="success-icon">🌍</div>
      <span class="success-number">3</span>
      <div class="success-label">
        <span class="en-content">Finalists</span>
        <span class="zh-content">决赛选手</span>
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
        <span class="en-content">The training transformed my understanding of quantitative finance. I went from knowing basic Python to creating alphas that ranked in the top 1% globally. Made it to Singapore finals!</span>
        <span class="zh-content">培训彻底改变了我对量化金融的理解。我从只会基础Python到创建全球排名前1%的Alpha。成功晋级新加坡决赛！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>David C.</h4>
          <p>
            <span class="en-content">IQC 2024 Finalist, Stanford</span>
            <span class="zh-content">IQC 2024决赛选手，斯坦福</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge consultant">Consultant</span>
      <p class="testimonial-text">
        <span class="en-content">Learning the BRAIN platform systematically helped me become a paid research consultant. The alpha strategies taught here directly apply to real-world quant work.</span>
        <span class="zh-content">系统地学习BRAIN平台帮助我成为了付费研究顾问。这里教授的Alpha策略直接适用于真实的量化工作。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍🎓</div>
        <div class="testimonial-info">
          <h4>Sarah L.</h4>
          <p>
            <span class="en-content">BRAIN Research Consultant</span>
            <span class="zh-content">BRAIN研究顾问</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge top1">Top 1%</span>
      <p class="testimonial-text">
        <span class="en-content">Started with zero finance knowledge. The step-by-step curriculum built my skills from statistics fundamentals to creating production-quality alphas. Ranked top 1% in Stage 1!</span>
        <span class="zh-content">从零金融知识开始。循序渐进的课程让我从统计基础到创建生产级Alpha。在第一阶段排名前1%！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>Kevin W.</h4>
          <p>
            <span class="en-content">IQC 2025 Top 1%, MIT</span>
            <span class="zh-content">IQC 2025前1%，MIT</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Master Quantitative Finance!</span>
    <span class="zh-content">精通量化金融！</span>
  </h2>
  <p>
    <span class="en-content">Join our training program and compete for $100K in prizes</span>
    <span class="zh-content">加入我们的培训计划，竞争$10万奖金</span>
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
