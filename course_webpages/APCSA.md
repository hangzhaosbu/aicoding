---
layout: default
title: AP Computer Science A
title_zh: AP计算机科学A
description: Excel in AP CSA Exam with Comprehensive Java Training
description_zh: 通过全面的Java培训在AP CSA考试中取得优异成绩
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

  @keyframes codePulse {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-10deg); }
  }

  @keyframes typewriter {
    from { width: 0; }
    to { width: 100%; }
  }

  /* Course Hero - Ultra Premium */
  .course-hero {
    background: linear-gradient(135deg, #10B981 0%, #0891B2 25%, #06B6D4 50%, #14B8A6 100%);
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
    min-height: 450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .course-hero::before {
    content: '💻';
    position: absolute;
    font-size: 20rem;
    opacity: 0.1;
    right: -100px;
    top: -100px;
    animation: codePulse 6s ease-in-out infinite;
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
  .floating-icon:nth-child(5) { left: 50%; top: 10%; animation-delay: 1s; }
  .floating-icon:nth-child(6) { left: 75%; top: 85%; animation-delay: 3s; }

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
    font-size: 2.8rem;
    font-weight: 800;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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

  /* Exam Info Section - Premium */
  .exam-info {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 50%, #A7F3D0 100%);
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    position: relative;
    overflow: hidden;
  }

  .exam-info::before {
    content: '📝';
    position: absolute;
    font-size: 12rem;
    opacity: 0.05;
    right: -30px;
    bottom: -30px;
  }

  .exam-info h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    color: #065F46;
    margin-bottom: 2.5rem;
  }

  .exam-stats {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 900px) {
    .exam-stats {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 500px) {
    .exam-stats {
      grid-template-columns: 1fr;
    }
  }

  .stat-card {
    background: white;
    padding: 2rem 1.5rem;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.08);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 2px solid transparent;
  }

  .stat-card:hover {
    transform: translateY(-8px) scale(1.02);
    border-color: #10B981;
    box-shadow: 0 25px 50px rgba(16, 185, 129, 0.2);
  }

  .stat-icon {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .stat-number {
    font-size: 2.2rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
  }

  .stat-label {
    color: #6B7280;
    font-size: 0.95rem;
    margin-top: 0.3rem;
    font-weight: 600;
  }

  /* Unit Cards - 2x2 Premium Design */
  .curriculum-section {
    padding: 2rem 0;
  }

  .unit-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
    margin: 3rem auto;
    max-width: 1200px;
    padding: 0 2rem;
  }

  @media (max-width: 900px) {
    .unit-cards {
      grid-template-columns: 1fr;
      max-width: 600px;
    }
  }

  .unit-card {
    background: white;
    padding: 2.5rem;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    animation: slideInUp 0.8s ease-out backwards;
    border-top: 5px solid;
    border-image: linear-gradient(90deg, #10B981, #0891B2) 1;
  }

  .unit-card:nth-child(1) { animation-delay: 0.1s; }
  .unit-card:nth-child(2) { animation-delay: 0.15s; }
  .unit-card:nth-child(3) { animation-delay: 0.2s; }
  .unit-card:nth-child(4) { animation-delay: 0.25s; }
  .unit-card:nth-child(5) { animation-delay: 0.3s; }
  .unit-card:nth-child(6) { animation-delay: 0.35s; }

  .unit-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(16, 185, 129, 0.05), transparent);
    animation: shimmer 3s infinite;
  }

  .unit-card:hover {
    transform: translateY(-8px) scale(1.01);
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.15);
  }

  .unit-header {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }

  .unit-number {
    width: 55px;
    height: 55px;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    color: white;
    border-radius: 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.4rem;
    box-shadow: 0 8px 20px rgba(16, 185, 129, 0.3);
    flex-shrink: 0;
  }

  .unit-title-group {
    flex: 1;
  }

  .unit-title {
    font-size: 1.4rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.3rem;
  }

  .unit-weight {
    font-size: 0.9rem;
    font-weight: 600;
    color: #10B981;
    background: rgba(16, 185, 129, 0.1);
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    display: inline-block;
  }

  .topic-list {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.4rem 1.5rem;
  }

  @media (max-width: 600px) {
    .topic-list {
      grid-template-columns: 1fr;
    }
  }

  .topic-list li {
    padding: 0.4rem 0;
    color: #4B5563;
    font-size: 0.95rem;
    display: flex;
    align-items: flex-start;
    line-height: 1.5;
  }

  .topic-list li::before {
    content: '→';
    color: #10B981;
    font-weight: bold;
    margin-right: 0.6rem;
    flex-shrink: 0;
  }

  /* Why Choose Section */
  .why-choose-section {
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
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
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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

  /* Success Section - Premium */
  .success-section {
    background: linear-gradient(135deg, #10B981 0%, #0891B2 50%, #06B6D4 100%);
    padding: 4rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 30px 60px rgba(16, 185, 129, 0.3);
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

  .success-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 768px) {
    .success-grid {
      grid-template-columns: 1fr;
      max-width: 300px;
    }
  }

  .success-item {
    text-align: center;
    background: white;
    padding: 2.5rem 2rem;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }

  .success-item:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.2);
  }

  .success-number {
    font-size: 3.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    display: block;
    animation: pulse 3s ease-in-out infinite;
  }

  .success-label {
    color: #6B7280;
    font-size: 1.1rem;
    font-weight: 600;
    margin-top: 0.5rem;
  }

  /* FRQ Types Section */
  .frq-section {
    background: white;
    padding: 4rem 3rem;
    border-radius: 30px;
    margin: 4rem 0;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
  }

  .frq-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
  }

  .frq-section > p {
    text-align: center;
    color: #6B7280;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .frq-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  @media (max-width: 1000px) {
    .frq-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 550px) {
    .frq-grid {
      grid-template-columns: 1fr;
    }
  }

  .frq-card {
    background: linear-gradient(135deg, #F0FDFA 0%, #CCFBF1 100%);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    transition: all 0.4s ease;
    border: 2px solid transparent;
    position: relative;
    overflow: hidden;
  }

  .frq-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #10B981, #0891B2);
  }

  .frq-card:hover {
    transform: translateY(-5px);
    border-color: #10B981;
    box-shadow: 0 15px 30px rgba(16, 185, 129, 0.15);
    background: white;
  }

  .frq-number {
    width: 50px;
    height: 50px;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 800;
    font-size: 1.3rem;
    margin: 0 auto 1rem;
    box-shadow: 0 8px 20px rgba(16, 185, 129, 0.3);
  }

  .frq-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .frq-desc {
    color: #6B7280;
    font-size: 0.9rem;
    line-height: 1.5;
  }

  /* Testimonials Section */
  .testimonials-section {
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #F0FDF4 0%, #DCFCE7 100%);
    border-radius: 30px;
    margin: 4rem 0;
  }

  .testimonials-section h2 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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
    background: linear-gradient(135deg, #10B981 0%, #0891B2 100%);
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
    background: linear-gradient(135deg, #10B981 0%, #0891B2 25%, #06B6D4 50%, #14B8A6 100%);
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
    color: #10B981;
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
    color: #059669;
  }

  .cta-button-secondary {
    background: transparent;
    border: 3px solid white;
    color: white;
  }

  .cta-button-secondary:hover {
    background: white;
    color: #10B981;
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

    .exam-info,
    .why-choose-section,
    .success-section,
    .frq-section {
      padding: 3rem 1.5rem;
    }
  }
</style>

<div class="course-hero">
  <div class="icons-bg">
    <span class="floating-icon">☕</span>
    <span class="floating-icon">{ }</span>
    <span class="floating-icon">📚</span>
    <span class="floating-icon">🎯</span>
    <span class="floating-icon">⭐</span>
    <span class="floating-icon">🏆</span>
  </div>
  <h1>
    <span class="en-content">AP Computer Science A</span>
    <span class="zh-content">AP计算机科学A</span>
  </h1>
  <p class="hero-subtitle">
    <span class="en-content">Master Java & Score 5 on Your AP Exam</span>
    <span class="zh-content">精通Java，AP考试斩获5分</span>
  </p>
  <div class="hero-badge">
    <span>📘</span>
    <span class="en-content">Official College Board Curriculum + Beyond</span>
    <span class="zh-content">官方大学理事会课程及扩展</span>
  </div>
  <div class="hero-stats">
    <div class="hero-stat">
      <span class="hero-stat-number">92%</span>
      <span class="hero-stat-label">
        <span class="en-content">Score 5</span>
        <span class="zh-content">满分率</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">100%</span>
      <span class="hero-stat-label">
        <span class="en-content">Pass Rate</span>
        <span class="zh-content">通过率</span>
      </span>
    </div>
    <div class="hero-stat">
      <span class="hero-stat-number">40hrs</span>
      <span class="hero-stat-label">
        <span class="en-content">Training</span>
        <span class="zh-content">培训时长</span>
      </span>
    </div>
  </div>
</div>

<!-- Exam Information -->
<div class="exam-info">
  <h2>
    <span class="en-content">📅 2026 AP CSA Exam Information</span>
    <span class="zh-content">📅 2026年AP CSA考试信息</span>
  </h2>
  
  <div class="exam-stats">
    <div class="stat-card">
      <div class="stat-icon">📆</div>
      <span class="stat-number">
        <span class="en-content">May 15</span>
        <span class="zh-content">5月15日</span>
      </span>
      <div class="stat-label">
        <span class="en-content">2026 Exam Date</span>
        <span class="zh-content">2026考试日期</span>
      </div>
    </div>
    <div class="stat-card">
      <div class="stat-icon">⏱️</div>
      <span class="stat-number">
        <span class="en-content">3 Hrs</span>
        <span class="zh-content">3小时</span>
      </span>
      <div class="stat-label">
        <span class="en-content">Exam Duration</span>
        <span class="zh-content">考试时长</span>
      </div>
    </div>
    <div class="stat-card">
      <div class="stat-icon">✅</div>
      <span class="stat-number">40</span>
      <div class="stat-label">
        <span class="en-content">Multiple Choice</span>
        <span class="zh-content">选择题</span>
      </div>
    </div>
    <div class="stat-card">
      <div class="stat-icon">✍️</div>
      <span class="stat-number">4</span>
      <div class="stat-label">
        <span class="en-content">Free Response</span>
        <span class="zh-content">自由回答题</span>
      </div>
    </div>
  </div>
</div>

<!-- Why Choose Section -->
<div class="why-choose-section">
  <div class="section-header" style="margin-top: 0;">
    <h2>
      <span class="en-content">Why Choose Our AP CSA Program?</span>
      <span class="zh-content">为什么选择我们的AP CSA课程？</span>
    </h2>
    <p>
      <span class="en-content">What makes our program the best choice for AP success</span>
      <span class="zh-content">我们课程的独特优势</span>
    </p>
  </div>
  
  <div class="why-choose-grid">
    <div class="why-choose-item">
      <div class="why-icon">📚</div>
      <h3>
        <span class="en-content">Complete Coverage</span>
        <span class="zh-content">完整覆盖</span>
      </h3>
      <p>
        <span class="en-content">All 10 AP units covered in-depth with extended content</span>
        <span class="zh-content">深入涵盖所有10个AP单元及扩展内容</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">✍️</div>
      <h3>
        <span class="en-content">FRQ Mastery</span>
        <span class="zh-content">FRQ精通</span>
      </h3>
      <p>
        <span class="en-content">Intensive practice on all 4 FRQ types with expert feedback</span>
        <span class="zh-content">针对4种FRQ题型的密集练习和专家反馈</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">🎯</div>
      <h3>
        <span class="en-content">5+ Mock Exams</span>
        <span class="zh-content">5+模拟考试</span>
      </h3>
      <p>
        <span class="en-content">Full-length practice tests with detailed score analysis</span>
        <span class="zh-content">完整模拟测试配详细分数分析</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👨‍🏫</div>
      <h3>
        <span class="en-content">Expert Instructors</span>
        <span class="zh-content">专业导师</span>
      </h3>
      <p>
        <span class="en-content">Learn from instructors with proven AP teaching experience</span>
        <span class="zh-content">向经验丰富的AP教学专家学习</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">👥</div>
      <h3>
        <span class="en-content">Small Classes</span>
        <span class="zh-content">小班教学</span>
      </h3>
      <p>
        <span class="en-content">Maximum 6 students for personalized attention</span>
        <span class="zh-content">每班最多6人，个性化关注</span>
      </p>
    </div>
    
    <div class="why-choose-item">
      <div class="why-icon">📊</div>
      <h3>
        <span class="en-content">Progress Tracking</span>
        <span class="zh-content">进度跟踪</span>
      </h3>
      <p>
        <span class="en-content">Weekly assessments to monitor your exam readiness</span>
        <span class="zh-content">每周评估监控考试准备情况</span>
      </p>
    </div>
  </div>
</div>

<!-- Curriculum Section -->
<div class="curriculum-section">
  <div class="section-header">
    <h2>
      <span class="en-content">Complete AP CSA Curriculum</span>
      <span class="zh-content">完整AP CSA课程大纲</span>
    </h2>
    <p>
      <span class="en-content">All 10 official College Board units plus bonus content</span>
      <span class="zh-content">所有10个官方大学理事会单元及额外内容</span>
    </p>
  </div>

  <div class="unit-cards">
    <!-- Unit 1-2 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">1-2</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">Primitive Types & Objects</span>
            <span class="zh-content">基本类型与对象</span>
          </h3>
          <span class="unit-weight">7.5-12.5%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Variables & Data Types</span><span class="zh-content">变量与数据类型</span></li>
        <li><span class="en-content">Expressions & Operators</span><span class="zh-content">表达式与运算符</span></li>
        <li><span class="en-content">Type Casting</span><span class="zh-content">类型转换</span></li>
        <li><span class="en-content">Object Instantiation</span><span class="zh-content">对象实例化</span></li>
        <li><span class="en-content">String Methods</span><span class="zh-content">字符串方法</span></li>
        <li><span class="en-content">Wrapper Classes</span><span class="zh-content">包装类</span></li>
      </ul>
    </div>

    <!-- Unit 3-4 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">3-4</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">Control Flow & Iteration</span>
            <span class="zh-content">控制流与迭代</span>
          </h3>
          <span class="unit-weight">32.5-40%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Boolean Expressions</span><span class="zh-content">布尔表达式</span></li>
        <li><span class="en-content">if/else Statements</span><span class="zh-content">if/else语句</span></li>
        <li><span class="en-content">De Morgan's Laws</span><span class="zh-content">德摩根定律</span></li>
        <li><span class="en-content">while & for Loops</span><span class="zh-content">while和for循环</span></li>
        <li><span class="en-content">Nested Loops</span><span class="zh-content">嵌套循环</span></li>
        <li><span class="en-content">Loop Analysis</span><span class="zh-content">循环分析</span></li>
      </ul>
    </div>

    <!-- Unit 5 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">5</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">Writing Classes</span>
            <span class="zh-content">编写类</span>
          </h3>
          <span class="unit-weight">5-7.5%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Class Anatomy</span><span class="zh-content">类结构</span></li>
        <li><span class="en-content">Constructors</span><span class="zh-content">构造函数</span></li>
        <li><span class="en-content">Instance Variables</span><span class="zh-content">实例变量</span></li>
        <li><span class="en-content">Methods & Parameters</span><span class="zh-content">方法与参数</span></li>
        <li><span class="en-content">Static vs Instance</span><span class="zh-content">静态vs实例</span></li>
        <li><span class="en-content">Scope & Access</span><span class="zh-content">作用域与访问</span></li>
      </ul>
    </div>

    <!-- Unit 6-7 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">6-7</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">Arrays & ArrayList</span>
            <span class="zh-content">数组与动态数组</span>
          </h3>
          <span class="unit-weight">12.5-22.5%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Array Creation</span><span class="zh-content">数组创建</span></li>
        <li><span class="en-content">Array Traversal</span><span class="zh-content">数组遍历</span></li>
        <li><span class="en-content">Array Algorithms</span><span class="zh-content">数组算法</span></li>
        <li><span class="en-content">ArrayList Methods</span><span class="zh-content">ArrayList方法</span></li>
        <li><span class="en-content">Searching & Sorting</span><span class="zh-content">搜索与排序</span></li>
        <li><span class="en-content">Enhanced for Loop</span><span class="zh-content">增强for循环</span></li>
      </ul>
    </div>

    <!-- Unit 8 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">8</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">2D Arrays</span>
            <span class="zh-content">二维数组</span>
          </h3>
          <span class="unit-weight">7.5-10%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">2D Array Declaration</span><span class="zh-content">二维数组声明</span></li>
        <li><span class="en-content">Row & Column Access</span><span class="zh-content">行列访问</span></li>
        <li><span class="en-content">Nested Loop Traversal</span><span class="zh-content">嵌套循环遍历</span></li>
        <li><span class="en-content">Row-Major Order</span><span class="zh-content">行优先顺序</span></li>
        <li><span class="en-content">2D Array Algorithms</span><span class="zh-content">二维数组算法</span></li>
        <li><span class="en-content">Matrix Operations</span><span class="zh-content">矩阵操作</span></li>
      </ul>
    </div>

    <!-- Unit 9-10 -->
    <div class="unit-card">
      <div class="unit-header">
        <div class="unit-number">9-10</div>
        <div class="unit-title-group">
          <h3 class="unit-title">
            <span class="en-content">Inheritance & Recursion</span>
            <span class="zh-content">继承与递归</span>
          </h3>
          <span class="unit-weight">10-17.5%</span>
        </div>
      </div>
      <ul class="topic-list">
        <li><span class="en-content">Superclass & Subclass</span><span class="zh-content">父类与子类</span></li>
        <li><span class="en-content">Method Overriding</span><span class="zh-content">方法重写</span></li>
        <li><span class="en-content">Polymorphism</span><span class="zh-content">多态性</span></li>
        <li><span class="en-content">Recursive Methods</span><span class="zh-content">递归方法</span></li>
        <li><span class="en-content">Binary Search</span><span class="zh-content">二分搜索</span></li>
        <li><span class="en-content">Merge Sort</span><span class="zh-content">归并排序</span></li>
      </ul>
    </div>
  </div>
</div>

<!-- FRQ Types Section -->
<div class="frq-section">
  <h2>
    <span class="en-content">Master All 4 FRQ Types</span>
    <span class="zh-content">精通全部4种FRQ题型</span>
  </h2>
  <p>
    <span class="en-content">Intensive practice on each free-response question type</span>
    <span class="zh-content">针对每种自由回答题型的强化练习</span>
  </p>
  
  <div class="frq-grid">
    <div class="frq-card">
      <div class="frq-number">1</div>
      <h3 class="frq-title">
        <span class="en-content">Methods & Control</span>
        <span class="zh-content">方法与控制</span>
      </h3>
      <p class="frq-desc">
        <span class="en-content">Method writing with loops, conditionals, and logic</span>
        <span class="zh-content">编写包含循环、条件和逻辑的方法</span>
      </p>
    </div>
    
    <div class="frq-card">
      <div class="frq-number">2</div>
      <h3 class="frq-title">
        <span class="en-content">Class Design</span>
        <span class="zh-content">类设计</span>
      </h3>
      <p class="frq-desc">
        <span class="en-content">Complete class implementation from scratch</span>
        <span class="zh-content">从零开始完整实现类</span>
      </p>
    </div>
    
    <div class="frq-card">
      <div class="frq-number">3</div>
      <h3 class="frq-title">
        <span class="en-content">Array/ArrayList</span>
        <span class="zh-content">数组/动态数组</span>
      </h3>
      <p class="frq-desc">
        <span class="en-content">Array manipulation and algorithm design</span>
        <span class="zh-content">数组操作与算法设计</span>
      </p>
    </div>
    
    <div class="frq-card">
      <div class="frq-number">4</div>
      <h3 class="frq-title">
        <span class="en-content">2D Array</span>
        <span class="zh-content">二维数组</span>
      </h3>
      <p class="frq-desc">
        <span class="en-content">2D array traversal and processing</span>
        <span class="zh-content">二维数组遍历与处理</span>
      </p>
    </div>
  </div>
</div>

<!-- Success Section -->
<div class="success-section">
  <h2>
    <span class="en-content">🏆 Our Students' AP Scores</span>
    <span class="zh-content">🏆 我们学生的AP成绩</span>
  </h2>
  
  <div class="success-grid">
    <div class="success-item">
      <span class="success-number">92%</span>
      <div class="success-label">
        <span class="en-content">Score 5</span>
        <span class="zh-content">获得5分</span>
      </div>
    </div>
    <div class="success-item">
      <span class="success-number">8%</span>
      <div class="success-label">
        <span class="en-content">Score 4</span>
        <span class="zh-content">获得4分</span>
      </div>
    </div>
    <div class="success-item">
      <span class="success-number">100%</span>
      <div class="success-label">
        <span class="en-content">Pass Rate</span>
        <span class="zh-content">通过率</span>
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
      <span class="testimonial-badge">
        <span class="en-content">Score: 5</span>
        <span class="zh-content">5分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The FRQ practice sessions were incredibly helpful. I went from struggling with class design questions to acing them on the real exam!</span>
        <span class="zh-content">FRQ练习课程非常有帮助。我从对类设计题目感到困难，到在真正考试中轻松搞定！</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👩‍💻</div>
        <div class="testimonial-info">
          <h4>Emily Z.</h4>
          <p>
            <span class="en-content">Junior, Score 5</span>
            <span class="zh-content">高中生，5分</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Score: 5</span>
        <span class="zh-content">5分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">Started with zero Java knowledge. The curriculum was perfectly paced, and the mock exams prepared me exactly for what to expect.</span>
        <span class="zh-content">从零Java知识开始。课程节奏完美，模拟考试让我完全了解考试内容。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍💻</div>
        <div class="testimonial-info">
          <h4>David L.</h4>
          <p>
            <span class="en-content">Sophomore, Score 5</span>
            <span class="zh-content">高中生，5分</span>
          </p>
        </div>
      </div>
    </div>
    
    <div class="testimonial-card">
      <span class="testimonial-badge">
        <span class="en-content">Score: 5</span>
        <span class="zh-content">5分</span>
      </span>
      <p class="testimonial-text">
        <span class="en-content">The recursion unit clicked after just one session! My instructor explained it in a way my school teacher couldn't.</span>
        <span class="zh-content">只上了一节课就完全理解了递归！导师的讲解方式比学校老师更清晰。</span>
      </p>
      <div class="testimonial-author">
        <div class="testimonial-avatar">👨‍🎓</div>
        <div class="testimonial-info">
          <h4>Jason W.</h4>
          <p>
            <span class="en-content">Junior, Score 5</span>
            <span class="zh-content">高中生，5分</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Ace Your AP CSA Exam!</span>
    <span class="zh-content">在AP CSA考试中取得优异成绩！</span>
  </h2>
  <p>
    <span class="en-content">Join our proven AP preparation program and secure your score of 5</span>
    <span class="zh-content">加入我们经过验证的AP准备课程，确保获得5分</span>
  </p>
  <div class="cta-buttons">
    <a href="./contact.html" class="cta-button">
      <span class="en-content">🚀 Start Preparing Now</span>
      <span class="zh-content">🚀 立即开始准备</span>
    </a>
    <a href="./contact.html" class="cta-button cta-button-secondary">
      <span class="en-content">📅 Schedule Consultation</span>
      <span class="zh-content">📅 预约咨询</span>
    </a>
  </div>
</div>
