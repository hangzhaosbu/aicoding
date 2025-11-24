---
layout: default
title: Our Courses
title_zh: 我们的课程
description: Comprehensive Programming Curriculum for All Levels
description_zh: 全方位编程课程，适合各个水平
---

<style>
  /* Advanced Animations */
  @keyframes gradientWave {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes gradientPulse {
    0%, 100% { background-position: 0% 0%; }
    25% { background-position: 100% 100%; }
    50% { background-position: 0% 100%; }
    75% { background-position: 100% 0%; }
  }

  @keyframes gradientRotate {
    0% { background-position: 0% 0%; transform: rotate(0deg); }
    100% { background-position: 100% 100%; transform: rotate(360deg); }
  }

  @keyframes gradientDiagonal {
    0% { background-position: 0% 0%; }
    50% { background-position: 100% 100%; }
    100% { background-position: 0% 0%; }
  }

  @keyframes curvedShimmer {
    0% { 
      left: -100%;
      transform: rotate(0deg);
    }
    50% {
      transform: rotate(5deg);
    }
    100% { 
      left: 100%;
      transform: rotate(0deg);
    }
  }

  @keyframes waveShimmer {
    0% { 
      left: -100%;
      top: 0%;
    }
    25% {
      top: 20%;
    }
    50% {
      top: -20%;
    }
    75% {
      top: 10%;
    }
    100% { 
      left: 100%;
      top: 0%;
    }
  }

  @keyframes spiralShimmer {
    0% { 
      left: -100%;
      transform: rotate(0deg) scale(1);
    }
    50% {
      transform: rotate(180deg) scale(1.2);
    }
    100% { 
      left: 100%;
      transform: rotate(360deg) scale(1);
    }
  }

  /* Different gradient backgrounds */
  .gradient-animated-bg {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #4facfe 100%);
    background-size: 300% 300%;
    animation: gradientWave 12s ease infinite;
  }

  .gradient-sunset {
    background: linear-gradient(135deg, #FA709A 0%, #FEE140 30%, #FA709A 60%, #E8526F 100%);
    background-size: 400% 400%;
    animation: gradientPulse 15s ease infinite;
  }

  .gradient-ocean {
    background: linear-gradient(135deg, #00C9FF 0%, #92FE9D 25%, #00C9FF 50%, #FC466B 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
  }

  .gradient-aurora {
    background: linear-gradient(135deg, #3BF0E4 0%, #BCA1F7 25%, #FFB2E6 50%, #3BF0E4 100%);
    background-size: 400% 400%;
    animation: gradientDiagonal 14s ease infinite;
  }

  .gradient-fire {
    background: linear-gradient(135deg, #F093FB 0%, #F5576C 25%, #FFA500 50%, #FFEB3B 100%);
    background-size: 300% 300%;
    animation: gradientWave 11s ease infinite;
  }

  .gradient-forest {
    background: linear-gradient(135deg, #00B09B 0%, #96C93D 25%, #00B09B 50%, #52C234 100%);
    background-size: 350% 350%;
    animation: gradientPulse 13s ease infinite;
  }

  .gradient-cosmic {
    background: linear-gradient(135deg, #8E2DE2 0%, #4A00E0 25%, #8E2DE2 50%, #000428 100%);
    background-size: 400% 400%;
    animation: gradientDiagonal 16s ease infinite;
  }

  .gradient-candy {
    background: linear-gradient(135deg, #FF6B9D 0%, #C44569 25%, #FFC0CB 50%, #F06292 100%);
    background-size: 300% 300%;
    animation: gradientWave 12s ease infinite;
  }

  .gradient-neon {
    background: linear-gradient(135deg, #00FFF0 0%, #FF00E4 25%, #7000FF 50%, #00FFF0 100%);
    background-size: 400% 400%;
    animation: gradientPulse 10s ease infinite;
  }

  /* Curved shimmer effects */
  .course-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: none;
    animation: curvedShimmer 4s infinite;
  }

  .course-card:nth-child(2)::before {
    animation: waveShimmer 4.5s infinite;
  }

  .course-card:nth-child(3)::before {
    animation: spiralShimmer 5s infinite;
  }

  .course-card:nth-child(4)::before {
    background: radial-gradient(circle, rgba(255, 255, 255, 0.4), transparent 70%);
    animation: curvedShimmer 3.5s infinite;
  }

  .course-card:nth-child(5)::before {
    background: conic-gradient(from 45deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    animation: waveShimmer 4s infinite;
  }

  .course-card:nth-child(6)::before {
    background: linear-gradient(135deg, transparent, rgba(255, 255, 255, 0.4), transparent);
    animation: spiralShimmer 4.5s infinite;
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    25% { transform: translateY(-10px) rotate(-2deg); }
    75% { transform: translateY(10px) rotate(2deg); }
  }

  @keyframes shimmer {
    0% { left: -100%; }
    100% { left: 100%; }
  }

  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
  }

  /* Page Header - Ultra Premium */
  .page-header-custom {
    min-height: 50vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 4rem 2rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    border-radius: 30px;
    margin-bottom: 5rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
  }

  .page-header-custom::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotate 15s linear infinite;
    pointer-events: none;
  }

  .page-header-custom::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 30%;
    width: 500px;
    height: 500px;
    background: radial-gradient(circle at center, rgba(255,255,255,0.3) 0%, rgba(255,255,255,0.15) 20%, transparent 60%);
    transform: translate(-50%, -50%);
    filter: blur(40px);
    animation: shimmerGlow 4s ease-in-out infinite;
    pointer-events: none;
  }

  /* Diagonal corner shimmer effect - improved */
  .page-header-custom .diagonal-shimmer-1,
  .page-header-custom .diagonal-shimmer-2 {
    position: absolute;
    width: 150%;
    height: 20px;
    background: linear-gradient(90deg, 
      transparent 0%, 
      rgba(255,255,255,0.1) 20%,
      rgba(255,255,255,0.3) 50%, 
      rgba(255,255,255,0.1) 80%,
      transparent 100%);
    filter: blur(20px);
    pointer-events: none;
  }

  .page-header-custom .diagonal-shimmer-1 {
    top: -10px;
    left: -150%;
    transform: rotate(45deg);
    animation: diagonalSweep1 8s ease-in-out infinite;
  }

  .page-header-custom .diagonal-shimmer-2 {
    bottom: -10px;
    right: -150%;
    transform: rotate(-45deg);
    animation: diagonalSweep2 8s ease-in-out infinite;
    animation-delay: 4s;
  }

  @keyframes diagonalSweep1 {
    0% {
      left: -150%;
      top: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      left: 50%;
      top: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      left: 150%;
      top: 110%;
      opacity: 0;
    }
  }

  @keyframes diagonalSweep2 {
    0% {
      right: -150%;
      bottom: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      right: 50%;
      bottom: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      right: 150%;
      bottom: 110%;
      opacity: 0;
    }
  }

  @keyframes shimmerGlow {
    0%, 100% {
      opacity: 0.3;
      transform: translate(-50%, -50%) scale(0.8);
    }
    50% {
      opacity: 0.6;
      transform: translate(-50%, -50%) scale(1.2);
    }
  }

  .page-title {
    font-size: 4rem;
    font-weight: 800;
    color: white;
    text-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
    animation: float 6s ease-in-out infinite;
  }

  .page-description {
    font-size: 1.4rem;
    color: rgba(255, 255, 255, 0.95);
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: relative;
    z-index: 1;
  }

  /* Learning Path - Premium Design */
  .learning-path {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 25%, #C7D2FE 50%, #DBEAFE 100%);
    border-radius: 30px;
    padding: 4rem 3rem;
    margin: 5rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.15);
    border: 2px solid rgba(139, 92, 246, 0.2);
  }

  .learning-path::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(139, 92, 246, 0.1), transparent);
    animation: shimmer 8s infinite;
  }

  .path-title {
    font-size: 2.5rem;
    font-weight: 700;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 3rem;
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .path-steps {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    position: relative;
    z-index: 1;
  }

  @media (max-width: 1200px) {
    .path-steps {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .path-steps {
      grid-template-columns: 1fr;
    }
  }

  .path-step {
    background: white;
    backdrop-filter: blur(10px);
    padding: 2rem;
    border-radius: 20px;
    text-align: center;
    border: 2px solid rgba(139, 92, 246, 0.2);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  }

  .path-step:hover {
    transform: translateY(-10px) scale(1.05);
    border-color: #667eea;
    box-shadow: 0 20px 40px rgba(102, 126, 234, 0.3);
  }

  .step-number {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 1rem;
    font-weight: 700;
    font-size: 1.5rem;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.4);
  }

  .step-title {
    font-weight: 700;
    color: #1F2937;
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
  }

  .step-description {
    font-size: 1rem;
    color: #6B7280;
    font-weight: 500;
  }

  /* Course Categories - Ultra Modern */
  .course-category {
    margin-bottom: 6rem;
  }

  .category-header {
    text-align: center;
    margin-bottom: 3rem;
  }

  .category-title {
    font-size: 3rem;
    font-weight: 800;
    color: #1F2937;
    margin-bottom: 1rem;
    position: relative;
    display: inline-block;
  }

  .category-title::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 100px;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2);
    border-radius: 3px;
  }

  .category-subtitle {
    color: #6B7280;
    font-size: 1.2rem;
    margin-top: 1rem;
  }

  /* Course Grid - Premium Cards */
  .courses-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 3rem;
    margin-top: 3rem;
  }

  .courses-grid-2x3 {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 3rem;
    margin-top: 3rem;
  }

  @media (max-width: 1400px) {
    .courses-grid {
      grid-template-columns: repeat(2, 1fr);
    }
    .courses-grid-2x3 {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .courses-grid {
      grid-template-columns: 1fr;
    }
    .courses-grid-2x3 {
      grid-template-columns: 1fr;
    }
  }

  .course-card {
    background: white;
    border-radius: 25px;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    border: 1px solid rgba(229, 231, 235, 0.5);
    display: flex;
    flex-direction: column;
    position: relative;
    animation: slideIn 0.6s ease-out;
  }

  .course-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.6s;
  }

  .course-card:hover::before {
    left: 100%;
  }

  .course-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.2);
  }

  .course-image {
    width: 100%;
    height: 250px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 5rem;
    color: white;
    position: relative;
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
  }

  .course-content {
    padding: 2rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .course-title {
    font-size: 1.6rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .course-subtitle {
    color: #6B7280;
    font-size: 1rem;
    margin-bottom: 1.5rem;
    line-height: 1.5;
  }

  .course-features {
    list-style: none;
    margin: 1rem 0;
    flex-grow: 1;
  }

  .course-features li {
    padding: 0.6rem 0;
    color: #4B5563;
    display: flex;
    align-items: center;
    font-size: 0.95rem;
    transition: transform 0.3s;
  }

  .course-features li:hover {
    transform: translateX(5px);
  }

  .course-features li::before {
    content: "→";
    color: #10B981;
    font-weight: bold;
    margin-right: 1rem;
    font-size: 1.2rem;
  }

  .enroll-btn {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white !important;
    padding: 1rem 2rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    text-align: center;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
    position: relative;
    overflow: hidden;
  }

  .enroll-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: left 0.5s;
  }

  .enroll-btn:hover::before {
    left: 100%;
  }

  .enroll-btn:hover {
    transform: translateY(-3px) scale(1.05);
    box-shadow: 0 15px 40px rgba(102, 126, 234, 0.4);
    color: white !important;
  }

  .age-tag {
    background: linear-gradient(135deg, #EEF2FF 0%, #DDD6FE 100%);
    color: #4F46E5;
    padding: 0.4rem 1rem;
    border-radius: 25px;
    font-size: 0.9rem;
    font-weight: 600;
    box-shadow: 0 2px 10px rgba(79, 70, 229, 0.1);
  }

  .level-tag {
    background: linear-gradient(135deg, #ECFDF5 0%, #D1FAE5 100%);
    color: #10B981;
    padding: 0.4rem 1rem;
    border-radius: 25px;
    font-size: 0.9rem;
    font-weight: 600;
    box-shadow: 0 2px 10px rgba(16, 185, 129, 0.1);
  }

  .course-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1.5rem;
    border-top: 1px solid #E5E7EB;
    margin-top: auto;
    margin-bottom: 1.5rem;
  }

  .badge-container {
    position: absolute;
    top: 1rem;
    right: 1rem;
    z-index: 2;
  }

  .popular-badge {
    background: linear-gradient(135deg, #EF4444 0%, #DC2626 100%);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 25px;
    font-size: 0.85rem;
    font-weight: 700;
    box-shadow: 0 5px 15px rgba(239, 68, 68, 0.4);
    animation: pulse 2s ease-in-out infinite;
  }

  .new-badge {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 25px;
    font-size: 0.85rem;
    font-weight: 700;
    box-shadow: 0 5px 15px rgba(16, 185, 129, 0.4);
    animation: pulse 2s ease-in-out infinite;
  }

  .hot-badge {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 25px;
    font-size: 0.85rem;
    font-weight: 700;
    box-shadow: 0 5px 15px rgba(245, 158, 11, 0.4);
    animation: pulse 2s ease-in-out infinite;
  }

  /* Competition Grid - Special Design */
  .competition-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(280px, 1fr));
    gap: 2rem;
    margin-top: 3rem;
    justify-content: center;
  }

  @media (max-width: 1200px) {
    .competition-grid {
      grid-template-columns: repeat(3, minmax(250px, 1fr));
      gap: 1.5rem;
    }
  }

  @media (max-width: 900px) {
    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .competition-grid {
      grid-template-columns: 1fr;
    }
  }

  .competition-card {
    background: white;
    border-radius: 20px;
    padding: 2rem;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
    border: 2px solid transparent;
    min-height: 280px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .competition-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
    transform: scaleX(0);
    transition: transform 0.4s ease;
  }

  .competition-card:hover::before {
    transform: scaleX(1);
  }

  .competition-card:hover {
    transform: translateY(-5px) scale(1.03);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
    border-color: #667eea;
  }

  .competition-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    display: block;
    animation: float 4s ease-in-out infinite;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .kaggle-logo {
    display: inline-block;
    font-family: 'Arial Black', sans-serif;
    font-weight: 900;
    font-size: 3.5rem;
    color: #20BEFF;
    text-shadow: 0 2px 10px rgba(32, 190, 255, 0.4);
    margin-bottom: 1rem;
    animation: float 4s ease-in-out infinite;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .competition-name {
    font-size: 1.3rem;
    font-weight: 700;
    color: #1F2937;
    margin-bottom: 0.5rem;
    min-height: 35px;
  }

  .competition-desc {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.5;
    flex-grow: 1;
    margin-bottom: 1.5rem;
  }

  /* CTA Section - Ultimate Premium */
  .cta-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 100%);
    background-size: 300% 300%;
    animation: gradientWave 10s ease infinite;
    border-radius: 30px;
    padding: 5rem 3rem;
    text-align: center;
    color: white;
    margin: 6rem 0;
    position: relative;
    overflow: hidden;
    box-shadow: 0 30px 60px rgba(102, 126, 234, 0.4);
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotate 15s linear infinite;
    pointer-events: none;
  }

  .cta-section::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 20%;
    width: 600px;
    height: 600px;
    background: radial-gradient(circle at center, rgba(255,255,255,0.3) 0%, rgba(255,255,255,0.15) 20%, transparent 60%);
    transform: translate(-50%, -50%);
    filter: blur(40px);
    animation: shimmerGlow 4s ease-in-out infinite;
    pointer-events: none;
  }

  /* Diagonal corner shimmer effect - improved */
  .cta-section .diagonal-shimmer-1,
  .cta-section .diagonal-shimmer-2 {
    position: absolute;
    width: 150%;
    height: 20px;
    background: linear-gradient(90deg, 
      transparent 0%, 
      rgba(255,255,255,0.1) 20%,
      rgba(255,255,255,0.3) 50%, 
      rgba(255,255,255,0.1) 80%,
      transparent 100%);
    filter: blur(20px);
    pointer-events: none;
  }

  .cta-section .diagonal-shimmer-1 {
    top: -10px;
    left: -150%;
    transform: rotate(45deg);
    animation: diagonalSweep1 8s ease-in-out infinite;
  }

  .cta-section .diagonal-shimmer-2 {
    bottom: -10px;
    right: -150%;
    transform: rotate(-45deg);
    animation: diagonalSweep2 8s ease-in-out infinite;
    animation-delay: 4s;
  }

  @keyframes diagonalSweep1 {
    0% {
      left: -150%;
      top: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      left: 50%;
      top: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      left: 150%;
      top: 110%;
      opacity: 0;
    }
  }

  @keyframes diagonalSweep2 {
    0% {
      right: -150%;
      bottom: -10px;
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    50% {
      right: 50%;
      bottom: 50%;
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      right: 150%;
      bottom: 110%;
      opacity: 0;
    }
  }

  @keyframes shimmerGlow {
    0%, 100% {
      opacity: 0.3;
      transform: translate(-50%, -50%) scale(0.8);
    }
    50% {
      opacity: 0.6;
      transform: translate(-50%, -50%) scale(1.2);
    }
  }

  @keyframes rotate {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .cta-title {
    font-size: 3rem;
    font-weight: 800;
    margin-bottom: 1rem;
    color: white !important;
    position: relative;
    z-index: 1;
    text-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  }

  .cta-description {
    font-size: 1.3rem;
    margin-bottom: 2rem;
    opacity: 0.95;
    color: white !important;
    position: relative;
    z-index: 1;
  }

  .cta-button {
    background: white;
    color: #667eea;
    padding: 1.2rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1.1rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    display: inline-block;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    position: relative;
    z-index: 1;
  }

  .cta-button:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    color: #667eea;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .page-title {
      font-size: 2.5rem;
    }

    .courses-grid {
      grid-template-columns: 1fr;
    }

    .competition-grid {
      grid-template-columns: 1fr;
    }

    .category-title {
      font-size: 2rem;
    }

    .cta-title {
      font-size: 2rem;
    }
  }
</style>

<div class="page-header-custom">
  <div class="diagonal-shimmer-1"></div>
  <div class="diagonal-shimmer-2"></div>
  <h1 class="page-title">
    <span class="en-content">Course Catalog</span>
    <span class="zh-content">课程目录</span>
  </h1>
  <p class="page-description">
    <span class="en-content">World-Class Programming Education for Future Innovators</span>
    <span class="zh-content">为未来创新者提供世界级编程教育</span>
  </p>
</div>

<!-- Learning Path -->
<div class="learning-path">
  <h2 class="path-title">
    <span class="en-content">🚀 Your Learning Journey</span>
    <span class="zh-content">🚀 您的学习之旅</span>
  </h2>
  <div class="path-steps">
    <div class="path-step">
      <div class="step-number">1</div>
      <div class="step-title">
        <span class="en-content">Foundation</span>
        <span class="zh-content">基础</span>
      </div>
      <div class="step-description">
        <span class="en-content">Python/Java Basics</span>
        <span class="zh-content">Python/Java 基础</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">2</div>
      <div class="step-title">
        <span class="en-content">Core Concepts</span>
        <span class="zh-content">核心概念</span>
      </div>
      <div class="step-description">
        <span class="en-content">Data Structures</span>
        <span class="zh-content">数据结构</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">3</div>
      <div class="step-title">
        <span class="en-content">Advanced</span>
        <span class="zh-content">进阶</span>
      </div>
      <div class="step-description">
        <span class="en-content">Algorithms</span>
        <span class="zh-content">算法</span>
      </div>
    </div>
    <div class="path-step">
      <div class="step-number">4</div>
      <div class="step-title">
        <span class="en-content">Specialization</span>
        <span class="zh-content">专业化</span>
      </div>
      <div class="step-description">
        <span class="en-content">AI/ML or Competitions</span>
        <span class="zh-content">人工智能或竞赛</span>
      </div>
    </div>
  </div>
</div>

<!-- Programming Languages -->
<div class="course-category">
  <div class="category-header">
    <h2 class="category-title">
      <span class="en-content">💻 Programming Languages</span>
      <span class="zh-content">💻 编程语言</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Master the world's most powerful programming languages</span>
      <span class="zh-content">掌握世界上最强大的编程语言</span>
    </p>
  </div>
  
  <div class="courses-grid">
    <!-- Python Course -->
    <div class="course-card">
      <div class="course-image gradient-sunset">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        🐍
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Python Fundamental I & II</span>
          <span class="zh-content">Python 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Complete Python Programming Journey</span>
          <span class="zh-content">完整的Python编程之旅</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Variables, Data Types, Control Flow</span>
            <span class="zh-content">变量、数据类型、控制流</span>
          </li>
          <li>
            <span class="en-content">Functions, OOP Concepts</span>
            <span class="zh-content">函数、面向对象概念</span>
          </li>
          <li>
            <span class="en-content">File Handling & Libraries</span>
            <span class="zh-content">文件处理与库</span>
          </li>
          <li>
            <span class="en-content">Real-world Projects</span>
            <span class="zh-content">实际项目</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./python.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Java Course -->
    <div class="course-card">
      <div class="course-image gradient-ocean">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">POPULAR</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        ☕
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Java Fundamental I & II</span>
          <span class="zh-content">Java 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Object-Oriented Programming Mastery</span>
          <span class="zh-content">面向对象编程精通</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Java Syntax & Structure</span>
            <span class="zh-content">Java语法与结构</span>
          </li>
          <li>
            <span class="en-content">OOP Principles & Design</span>
            <span class="zh-content">面向对象原则与设计</span>
          </li>
          <li>
            <span class="en-content">Collections Framework</span>
            <span class="zh-content">集合框架</span>
          </li>
          <li>
            <span class="en-content">GUI Development</span>
            <span class="zh-content">GUI开发</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 10-18</span>
            <span class="zh-content">年龄: 10-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./java.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- C++ Course -->
    <div class="course-card">
      <div class="course-image gradient-cosmic">
        ⚙️
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">C++ Fundamental I & II</span>
          <span class="zh-content">C++ 基础 I & II</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">System Programming & Performance</span>
          <span class="zh-content">系统编程与性能</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Memory Management</span>
            <span class="zh-content">内存管理</span>
          </li>
          <li>
            <span class="en-content">Pointers & References</span>
            <span class="zh-content">指针与引用</span>
          </li>
          <li>
            <span class="en-content">STL & Templates</span>
            <span class="zh-content">STL与模板</span>
          </li>
          <li>
            <span class="en-content">Competitive Programming</span>
            <span class="zh-content">竞赛编程</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Intermediate</span>
            <span class="zh-content">中级</span>
          </span>
        </div>
        <a href="./cplusplus.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</div>

<!-- Computer Science Core -->
<div class="course-category">
  <div class="category-header">
    <h2 class="category-title">
      <span class="en-content">📚 Computer Science Core</span>
      <span class="zh-content">📚 计算机科学核心</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Essential foundations for every programmer</span>
      <span class="zh-content">每个程序员的必备基础</span>
    </p>
  </div>
  
  <div class="courses-grid-2x3">
    <!-- Data Structures -->
    <div class="course-card">
      <div class="course-image gradient-aurora">
        🗂️
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Data Structures</span>
          <span class="zh-content">数据结构</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Foundation of Efficient Programming</span>
          <span class="zh-content">高效编程的基础</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Arrays, Linked Lists, Stacks</span>
            <span class="zh-content">数组、链表、栈</span>
          </li>
          <li>
            <span class="en-content">Trees & Graphs</span>
            <span class="zh-content">树与图</span>
          </li>
          <li>
            <span class="en-content">Hash Tables & Heaps</span>
            <span class="zh-content">哈希表与堆</span>
          </li>
          <li>
            <span class="en-content">Time & Space Complexity</span>
            <span class="zh-content">时间与空间复杂度</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 12-18</span>
            <span class="zh-content">年龄: 12-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Intermediate</span>
            <span class="zh-content">中级</span>
          </span>
        </div>
        <a href="./datastructure.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Algorithms -->
    <div class="course-card">
      <div class="course-image gradient-fire">
        🧮
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Algorithms</span>
          <span class="zh-content">算法</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Problem Solving & Optimization</span>
          <span class="zh-content">问题解决与优化</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Sorting & Searching</span>
            <span class="zh-content">排序与搜索</span>
          </li>
          <li>
            <span class="en-content">Dynamic Programming</span>
            <span class="zh-content">动态规划</span>
          </li>
          <li>
            <span class="en-content">Graph Algorithms</span>
            <span class="zh-content">图算法</span>
          </li>
          <li>
            <span class="en-content">Greedy & Divide-Conquer</span>
            <span class="zh-content">贪心与分治</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 13-18</span>
            <span class="zh-content">年龄: 13-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Advanced</span>
            <span class="zh-content">高级</span>
          </span>
        </div>
        <a href="./algorithm.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Machine Learning -->
    <div class="course-card">
      <div class="course-image gradient-neon">
        <div class="badge-container">
          <span class="hot-badge">
            <span class="en-content">HOT</span>
            <span class="zh-content">热门</span>
          </span>
        </div>
        🤖
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Machine Learning & AI</span>
          <span class="zh-content">机器学习与人工智能</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Future of Technology</span>
          <span class="zh-content">技术的未来</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Neural Networks</span>
            <span class="zh-content">神经网络</span>
          </li>
          <li>
            <span class="en-content">Deep Learning</span>
            <span class="zh-content">深度学习</span>
          </li>
          <li>
            <span class="en-content">Computer Vision</span>
            <span class="zh-content">计算机视觉</span>
          </li>
          <li>
            <span class="en-content">NLP & AI Projects</span>
            <span class="zh-content">自然语言处理与AI项目</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Advanced</span>
            <span class="zh-content">高级</span>
          </span>
        </div>
        <a href="./MachineLearning.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- AP CSA -->
    <div class="course-card">
      <div class="course-image gradient-forest">
        📘
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">AP Computer Science A</span>
          <span class="zh-content">AP计算机科学A</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">College-Level Java Programming</span>
          <span class="zh-content">大学水平Java编程</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Complete AP CSA Curriculum</span>
            <span class="zh-content">完整的AP CSA课程</span>
          </li>
          <li>
            <span class="en-content">Practice Exams</span>
            <span class="zh-content">模拟考试</span>
          </li>
          <li>
            <span class="en-content">FRQ Training</span>
            <span class="zh-content">自由回答题训练</span>
          </li>
          <li>
            <span class="en-content">Score 5 Guarantee</span>
            <span class="zh-content">5分保证</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Intermediate</span>
            <span class="zh-content">中级</span>
          </span>
        </div>
        <a href="./APCSA.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- AP CSP -->
    <div class="course-card">
      <div class="course-image gradient-candy">
        <div class="badge-container">
          <span class="new-badge">
            <span class="en-content">NEW</span>
            <span class="zh-content">新</span>
          </span>
        </div>
        💡
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">AP Computer Science Principles</span>
          <span class="zh-content">AP计算机科学原理</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Computational Thinking & Creativity</span>
          <span class="zh-content">计算思维与创造力</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">Computational Thinking</span>
            <span class="zh-content">计算思维</span>
          </li>
          <li>
            <span class="en-content">Data & Information</span>
            <span class="zh-content">数据与信息</span>
          </li>
          <li>
            <span class="en-content">Internet & Computing</span>
            <span class="zh-content">互联网与计算</span>
          </li>
          <li>
            <span class="en-content">Creative Performance Task</span>
            <span class="zh-content">创意表现任务</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 14-18</span>
            <span class="zh-content">年龄: 14-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">Beginner</span>
            <span class="zh-content">初级</span>
          </span>
        </div>
        <a href="./APCSP.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>

    <!-- Web Development - New Course -->
    <div class="course-card">
      <div class="course-image gradient-animated-bg">
        <div class="badge-container">
          <span class="popular-badge">
            <span class="en-content">TRENDING</span>
            <span class="zh-content">趋势</span>
          </span>
        </div>
        🌐
      </div>
      <div class="course-content">
        <h3 class="course-title">
          <span class="en-content">Full-Stack Web Development</span>
          <span class="zh-content">全栈网页开发</span>
        </h3>
        <p class="course-subtitle">
          <span class="en-content">Build Modern Web Applications</span>
          <span class="zh-content">构建现代网页应用</span>
        </p>
        <ul class="course-features">
          <li>
            <span class="en-content">HTML5, CSS3, JavaScript</span>
            <span class="zh-content">HTML5, CSS3, JavaScript</span>
          </li>
          <li>
            <span class="en-content">React, Vue, Angular</span>
            <span class="zh-content">React, Vue, Angular</span>
          </li>
          <li>
            <span class="en-content">Node.js & Database Design</span>
            <span class="zh-content">Node.js与数据库设计</span>
          </li>
          <li>
            <span class="en-content">Deploy Real Applications</span>
            <span class="zh-content">部署真实应用</span>
          </li>
        </ul>
        <div class="course-footer">
          <span class="age-tag">
            <span class="en-content">Age: 13-18</span>
            <span class="zh-content">年龄: 13-18</span>
          </span>
          <span class="level-tag">
            <span class="en-content">All Levels</span>
            <span class="zh-content">所有级别</span>
          </span>
        </div>
        <a href="./webdev.html" class="enroll-btn">
          <span class="en-content">Learn More</span>
          <span class="zh-content">了解更多</span>
        </a>
      </div>
    </div>
  </div>
</div>

<!-- Competition Training -->
<div class="course-category">
  <div class="category-header">
    <h2 class="category-title">
      <span class="en-content">🏆 Competition Training</span>
      <span class="zh-content">🏆 竞赛培训</span>
    </h2>
    <p class="category-subtitle">
      <span class="en-content">Excel in world-renowned competitions</span>
      <span class="zh-content">在世界知名竞赛中脱颖而出</span>
    </p>
  </div>
  
  <div class="competition-grid">
    <!-- USACO -->
    <div class="competition-card">
      <span class="competition-icon">🥇</span>
      <h3 class="competition-name">USACO</h3>
      <p class="competition-desc">
        <span class="en-content">USA Computing Olympiad</span>
        <span class="zh-content">美国计算机奥林匹克</span>
      </p>
      <a href="./USACO.html" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- USAAIO -->
    <div class="competition-card">
      <span class="competition-icon">🤖</span>
      <h3 class="competition-name">USAAIO</h3>
      <p class="competition-desc">
        <span class="en-content">USA AI Olympiad</span>
        <span class="zh-content">美国人工智能奥林匹克</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- Kaggle -->
    <div class="competition-card">
      <span class="kaggle-logo">K</span>
      <h3 class="competition-name">Kaggle</h3>
      <p class="competition-desc">
        <span class="en-content">Data Science Competitions</span>
        <span class="zh-content">数据科学竞赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- AMC 8/10/12 -->
    <div class="competition-card">
      <span class="competition-icon">🔢</span>
      <h3 class="competition-name">AMC 8/10/12</h3>
      <p class="competition-desc">
        <span class="en-content">American Mathematics Competitions</span>
        <span class="zh-content">美国数学竞赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- AIME -->
    <div class="competition-card">
      <span class="competition-icon">📐</span>
      <h3 class="competition-name">AIME</h3>
      <p class="competition-desc">
        <span class="en-content">American Invitational Math Exam</span>
        <span class="zh-content">美国数学邀请赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- USAMO -->
    <div class="competition-card">
      <span class="competition-icon">🎯</span>
      <h3 class="competition-name">USAMO</h3>
      <p class="competition-desc">
        <span class="en-content">USA Mathematical Olympiad</span>
        <span class="zh-content">美国数学奥林匹克</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- ACSL -->
    <div class="competition-card">
      <span class="competition-icon">💻</span>
      <h3 class="competition-name">ACSL</h3>
      <p class="competition-desc">
        <span class="en-content">Computer Science League</span>
        <span class="zh-content">计算机科学联赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- WorldQuant -->
    <div class="competition-card">
      <span class="competition-icon">📈</span>
      <h3 class="competition-name">WorldQuant</h3>
      <p class="competition-desc">
        <span class="en-content">Quantitative Finance Challenge</span>
        <span class="zh-content">量化金融挑战赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>

    <!-- HiMCM -->
    <div class="competition-card">
      <span class="competition-icon">📋</span>
      <h3 class="competition-name">HiMCM</h3>
      <p class="competition-desc">
        <span class="en-content">Mathematical Modeling Contest</span>
        <span class="zh-content">数学建模竞赛</span>
      </p>
      <a href="#" class="enroll-btn">
        <span class="en-content">Learn More</span>
        <span class="zh-content">了解更多</span>
      </a>
    </div>
  </div>
</div>

<!-- CTA Section -->
<div class="cta-section">
  <div class="diagonal-shimmer-1"></div>
  <div class="diagonal-shimmer-2"></div>
  <h2 class="cta-title">
    <span class="en-content">Ready to Excel?</span>
    <span class="zh-content">准备好卓越了吗？</span>
  </h2>
  <p class="cta-description">
    <span class="en-content">Customized learning paths for every student's unique journey</span>
    <span class="zh-content">为每个学生的独特旅程定制学习路径</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Start Your Journey Today</span>
    <span class="zh-content">今天开始您的旅程</span>
  </a>
</div>
