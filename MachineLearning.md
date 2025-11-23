---
layout: default
title: AI & Machine Learning Course
title_zh: 人工智能与机器学习课程
description: Master Artificial Intelligence for Competitions and Beyond
description_zh: 掌握人工智能，征服竞赛与未来
---

<style>
  /* Course Hero with Gradient Animation */
  .course-hero {
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 50%, #3B82F6 100%);
    background-size: 200% 200%;
    animation: gradientShift 8s ease infinite;
    padding: 5rem 2rem;
    border-radius: 20px;
    color: white;
    text-align: center;
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(139, 92, 246, 0.3);
  }

  @keyframes gradientShift {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  .course-hero::before {
    content: '🤖';
    position: absolute;
    font-size: 20rem;
    opacity: 0.08;
    right: -100px;
    top: -100px;
    transform: rotate(-15deg);
    animation: float 6s ease-in-out infinite;
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(-15deg); }
    50% { transform: translateY(-20px) rotate(-15deg); }
  }

  .course-hero h1 {
    font-size: 3rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: white !important;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  .course-hero p {
    font-size: 1.3rem;
    opacity: 0.95;
    color: white !important;
    max-width: 600px;
    margin: 0 auto;
  }

  .hero-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
    padding: 0.75rem 1.5rem;
    border-radius: 30px;
    margin-top: 1.5rem;
    font-weight: 600;
    border: 1px solid rgba(255, 255, 255, 0.3);
  }

  /* Overview Section */
  .overview-card {
    background: white;
    padding: 3rem;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    margin-bottom: 3rem;
    position: relative;
    overflow: hidden;
  }

  .overview-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #8B5CF6, #EC4899, #3B82F6);
  }

  /* Curriculum Timeline */
  .curriculum-section {
    background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
    padding: 4rem 3rem;
    border-radius: 20px;
    margin-bottom: 3rem;
  }

  .phase-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
    gap: 3rem;
    margin-top: 3rem;
  }

  .phase-container {
    background: white;
    border-radius: 15px;
    padding: 2rem;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
  }

  .phase-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 2px solid #E5E7EB;
  }

  .phase-icon {
    font-size: 2rem;
  }

  .phase-title {
    font-size: 1.5rem;
    font-weight: 600;
    margin: 0;
  }

  .week-module {
    background: linear-gradient(135deg, #FAFAFA 0%, #FFFFFF 100%);
    padding: 1.5rem;
    border-radius: 12px;
    margin-bottom: 1rem;
    border-left: 4px solid;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
  }

  .week-module::after {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100px;
    height: 100px;
    background: linear-gradient(135deg, transparent 50%, rgba(139, 92, 246, 0.05) 50%);
  }

  .foundation-module {
    border-left-color: #8B5CF6;
  }

  .advanced-module {
    border-left-color: #EC4899;
  }

  .week-module:hover {
    transform: translateX(8px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
    background: white;
  }

  .week-title {
    color: #1F2937;
    font-weight: 600;
    margin-bottom: 0.5rem;
    font-size: 1.1rem;
  }

  .week-content {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Competition Preparation - Premium Cards */
  .competition-section {
    padding: 4rem 0;
    background: white;
    border-radius: 20px;
    margin: 3rem 0;
  }

  .competition-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 3rem;
    padding: 0 2rem;
  }

  @media (max-width: 1200px) {
    .competition-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .competition-grid {
      grid-template-columns: 1fr;
    }
  }

  .competition-card {
    background: white;
    border-radius: 20px;
    padding: 2.5rem;
    text-align: center;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
  }

  .competition-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, #8B5CF6, #EC4899);
    transform: scaleX(0);
    transition: transform 0.3s ease;
  }

  .competition-card:hover::before {
    transform: scaleX(1);
  }

  .competition-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
  }

  .competition-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 20px;
    font-size: 2.5rem;
    position: relative;
  }

  .usaaio-icon {
    background: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);
    color: white;
  }

  .kaggle-icon {
    background: #20BEFF;
    color: white;
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 700;
    font-size: 3rem;
  }

  .research-icon {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
  }

  .portfolio-icon {
    background: linear-gradient(135deg, #F59E0B 0%, #D97706 100%);
    color: white;
  }

  .competition-title {
    font-size: 1.3rem;
    font-weight: 600;
    color: #1F2937;
    margin-bottom: 0.5rem;
  }

  .competition-desc {
    color: #6B7280;
    font-size: 0.95rem;
    line-height: 1.5;
  }

  /* Tools & Technologies - Modern Grid */
  .tools-section {
    background: linear-gradient(135deg, #FEF3C7 0%, #FDE68A 100%);
    padding: 3rem;
    border-radius: 20px;
    margin: 3rem 0;
    position: relative;
    overflow: hidden;
  }

  .tools-section::before {
    content: '⚡';
    position: absolute;
    font-size: 10rem;
    opacity: 0.1;
    right: -30px;
    bottom: -30px;
    transform: rotate(15deg);
  }

  .tools-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
    margin-top: 2rem;
  }

  .tool-badge {
    background: white;
    padding: 0.75rem 1.75rem;
    border-radius: 25px;
    border: 2px solid #F59E0B;
    font-weight: 500;
    transition: all 0.3s;
    cursor: default;
  }

  .tool-badge:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(245, 158, 11, 0.3);
    background: #F59E0B;
    color: white;
  }

  /* Learning Outcomes */
  .outcomes-section {
    background: linear-gradient(135deg, #EDE9FE 0%, #DDD6FE 100%);
    padding: 3rem;
    border-radius: 20px;
    margin: 3rem 0;
  }

  .outcome-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    margin-top: 2rem;
  }

  @media (max-width: 1200px) {
    .outcome-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 768px) {
    .outcome-grid {
      grid-template-columns: 1fr;
    }
  }

  .outcome-item {
    background: white;
    padding: 1.5rem;
    border-radius: 15px;
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    transition: transform 0.3s;
  }

  .outcome-item:hover {
    transform: translateX(5px);
  }

  .outcome-check {
    background: linear-gradient(135deg, #10B981 0%, #059669 100%);
    color: white;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    font-weight: bold;
  }

  /* CTA Section - Premium */
  .cta-section {
    background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 100%);
    padding: 4rem;
    border-radius: 20px;
    text-align: center;
    color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(139, 92, 246, 0.3);
  }

  .cta-section::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
    animation: rotate 20s linear infinite;
  }

  @keyframes rotate {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .cta-section h2 {
    color: white !important;
    font-size: 2.5rem;
    margin-bottom: 1rem;
    position: relative;
    z-index: 1;
  }

  .cta-section p {
    color: white !important;
    font-size: 1.2rem;
    margin: 1rem 0 2rem;
    opacity: 0.95;
    position: relative;
    z-index: 1;
  }

  .cta-button {
    background: white;
    color: #8B5CF6;
    padding: 1rem 3rem;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s;
    position: relative;
    z-index: 1;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  }

  .cta-button:hover {
    transform: translateY(-3px);
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
    color: #8B5CF6;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .course-hero h1 {
      font-size: 2rem;
    }
    
    .phase-grid {
      grid-template-columns: 1fr;
    }
    
    .competition-grid {
      grid-template-columns: 1fr;
      padding: 0 1rem;
    }
  }
</style>

<div class="course-hero">
  <h1>
    <span class="en-content">AI & Machine Learning Mastery</span>
    <span class="zh-content">人工智能与机器学习精通课程</span>
  </h1>
  <p>
    <span class="en-content">16-Week Comprehensive AI Competition Training Program</span>
    <span class="zh-content">16周综合AI竞赛培训计划</span>
  </p>
  <div class="hero-badge">
    <span class="en-content">🎯 USAAIO + Kaggle + Research</span>
    <span class="zh-content">🎯 USAAIO + Kaggle + 研究项目</span>
  </div>
</div>

<!-- Course Overview -->
<div class="overview-card">
  <h2 style="color: #1F2937; margin-bottom: 1.5rem;">
    <span class="en-content">Course Overview</span>
    <span class="zh-content">课程概述</span>
  </h2>
  <p style="font-size: 1.15rem; color: #4B5563; line-height: 1.8;">
    <span class="en-content">
      Master cutting-edge AI and machine learning techniques for competitions like USAAIO, Kaggle, and research projects. 
      This intensive 16-week program covers everything from ML fundamentals to advanced deep learning, preparing students 
      for AI olympiads and real-world applications. Learn from competition winners and published researchers.
    </span>
    <span class="zh-content">
      掌握用于USAAIO、Kaggle等竞赛和研究项目的尖端人工智能和机器学习技术。
      这个密集的16周课程涵盖了从机器学习基础到高级深度学习的所有内容，
      为学生准备AI奥林匹克竞赛和实际应用。向竞赛获胜者和发表论文的研究人员学习。
    </span>
  </p>
</div>

<!-- Detailed Curriculum -->
<div class="curriculum-section">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 1rem;">
    <span class="en-content">16-Week Detailed Curriculum</span>
    <span class="zh-content">16周详细课程大纲</span>
  </h2>
  <p style="text-align: center; color: #6B7280; margin-bottom: 2rem;">
    <span class="en-content">From fundamentals to cutting-edge AI techniques</span>
    <span class="zh-content">从基础到前沿AI技术</span>
  </p>
  
  <div class="phase-grid">
    <!-- Foundation Phase -->
    <div class="phase-container">
      <div class="phase-header">
        <span class="phase-icon">📚</span>
        <h3 class="phase-title" style="color: #8B5CF6;">
          <span class="en-content">Foundation Phase</span>
          <span class="zh-content">基础阶段</span>
        </h3>
      </div>
      
      <div class="week-module foundation-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 1-2: ML Fundamentals</span>
          <span class="zh-content">第1-2周：机器学习基础</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Supervised vs Unsupervised Learning, Linear Regression, Classification Basics, Model Evaluation</span>
          <span class="zh-content">监督学习vs无监督学习，线性回归，分类基础，模型评估</span>
        </p>
      </div>
      
      <div class="week-module foundation-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 3-4: Data Mining Algorithms</span>
          <span class="zh-content">第3-4周：数据挖掘算法</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Decision Trees, Random Forests, XGBoost, Ensemble Methods, Cross-validation</span>
          <span class="zh-content">决策树，随机森林，XGBoost，集成方法，交叉验证</span>
        </p>
      </div>
      
      <div class="week-module foundation-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 5-6: Feature Engineering</span>
          <span class="zh-content">第5-6周：特征工程</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Feature Selection, Dimensionality Reduction, PCA, Data Preprocessing, Handling Imbalanced Data</span>
          <span class="zh-content">特征选择，降维，主成分分析，数据预处理，处理不平衡数据</span>
        </p>
      </div>
      
      <div class="week-module foundation-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 7-8: Neural Networks</span>
          <span class="zh-content">第7-8周：神经网络</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Logistic Regression, Fully Connected Networks, Backpropagation, Optimization Algorithms</span>
          <span class="zh-content">逻辑回归，全连接网络，反向传播，优化算法</span>
        </p>
      </div>
    </div>
    
    <!-- Advanced Phase -->
    <div class="phase-container">
      <div class="phase-header">
        <span class="phase-icon">🚀</span>
        <h3 class="phase-title" style="color: #EC4899;">
          <span class="en-content">Advanced Phase</span>
          <span class="zh-content">高级阶段</span>
        </h3>
      </div>
      
      <div class="week-module advanced-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 9-10: Computer Vision (CNN)</span>
          <span class="zh-content">第9-10周：计算机视觉（CNN）</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Convolutional Networks, Image Classification, Transfer Learning, Data Augmentation</span>
          <span class="zh-content">卷积网络，图像分类，迁移学习，数据增强</span>
        </p>
      </div>
      
      <div class="week-module advanced-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 11-12: Advanced Vision</span>
          <span class="zh-content">第11-12周：高级视觉</span>
        </h4>
        <p class="week-content">
          <span class="en-content">Object Detection (YOLO, R-CNN), Image Segmentation, GANs, Style Transfer</span>
          <span class="zh-content">目标检测（YOLO, R-CNN），图像分割，生成对抗网络，风格迁移</span>
        </p>
      </div>
      
      <div class="week-module advanced-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 13-14: Time Series & Sequences</span>
          <span class="zh-content">第13-14周：时间序列与序列</span>
        </h4>
        <p class="week-content">
          <span class="en-content">RNNs, LSTM, GRU, 1D-CNN, Transformers, Attention Mechanisms</span>
          <span class="zh-content">循环神经网络，LSTM，GRU，一维CNN，Transformers，注意力机制</span>
        </p>
      </div>
      
      <div class="week-module advanced-module">
        <h4 class="week-title">
          <span class="en-content">Weeks 15-16: NLP & Competition Tricks</span>
          <span class="zh-content">第15-16周：自然语言处理与竞赛技巧</span>
        </h4>
        <p class="week-content">
          <span class="en-content">BERT, GPT, Text Classification, Kaggle Strategies, Competition Winning Techniques</span>
          <span class="zh-content">BERT，GPT，文本分类，Kaggle策略，竞赛获胜技巧</span>
        </p>
      </div>
    </div>
  </div>
</div>

<!-- Competition Preparation -->
<div class="competition-section">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 1rem;">
    <span class="en-content">Competition & Research Preparation</span>
    <span class="zh-content">竞赛与研究准备</span>
  </h2>
  <p style="text-align: center; color: #6B7280; margin-bottom: 2rem;">
    <span class="en-content">Excel in top AI competitions and research projects</span>
    <span class="zh-content">在顶级AI竞赛和研究项目中脱颖而出</span>
  </p>
  
  <div class="competition-grid">
    <div class="competition-card">
      <div class="competition-icon usaaio-icon">
        <span style="font-weight: 700;">AI</span>
      </div>
      <h4 class="competition-title">USAAIO</h4>
      <p class="competition-desc">
        <span class="en-content">USA AI Olympiad preparation with past winners' strategies</span>
        <span class="zh-content">美国AI奥林匹克准备，包含往届获胜者策略</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon kaggle-icon">
        K
      </div>
      <h4 class="competition-title">Kaggle</h4>
      <p class="competition-desc">
        <span class="en-content">Master data science competitions with Grandmaster techniques</span>
        <span class="zh-content">使用大师级技术征服数据科学竞赛</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon research-icon">
        📄
      </div>
      <h4 class="competition-title">
        <span class="en-content">Research Papers</span>
        <span class="zh-content">研究论文</span>
      </h4>
      <p class="competition-desc">
        <span class="en-content">Publish in conferences and journals with expert guidance</span>
        <span class="zh-content">在专家指导下发表会议和期刊论文</span>
      </p>
    </div>
    
    <div class="competition-card">
      <div class="competition-icon portfolio-icon">
        💼
      </div>
      <h4 class="competition-title">
        <span class="en-content">Portfolio Projects</span>
        <span class="zh-content">作品集项目</span>
      </h4>
      <p class="competition-desc">
        <span class="en-content">Build industry-level applications for college applications</span>
        <span class="zh-content">为大学申请构建行业级应用</span>
      </p>
    </div>
  </div>
</div>

<!-- Learning Outcomes -->
<div class="outcomes-section">
  <h2 style="text-align: center; color: #1F2937; margin-bottom: 2rem;">
    <span class="en-content">What You'll Achieve</span>
    <span class="zh-content">您将获得的成就</span>
  </h2>
  
  <div class="outcome-grid">
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div>
        <span class="en-content">Master 10+ ML algorithms and frameworks</span>
        <span class="zh-content">掌握10+机器学习算法和框架</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div>
        <span class="en-content">Build competition-winning models</span>
        <span class="zh-content">构建竞赛获胜模型</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div>
        <span class="en-content">Complete 5+ real-world projects</span>
        <span class="zh-content">完成5+实际项目</span>
      </div>
    </div>
    <div class="outcome-item">
      <div class="outcome-check">✓</div>
      <div>
        <span class="en-content">Research paper submission ready</span>
        <span class="zh-content">准备提交研究论文</span>
      </div>
    </div>
  </div>
</div>

<!-- Tools & Technologies -->
<div class="tools-section">
  <h2 style="color: #92400E; text-align: center; margin-bottom: 1rem;">
    <span class="en-content">Tools & Technologies You'll Master</span>
    <span class="zh-content">您将掌握的工具与技术</span>
  </h2>
  
  <div class="tools-grid">
    <span class="tool-badge">Python</span>
    <span class="tool-badge">TensorFlow</span>
    <span class="tool-badge">PyTorch</span>
    <span class="tool-badge">Scikit-learn</span>
    <span class="tool-badge">Keras</span>
    <span class="tool-badge">Pandas</span>
    <span class="tool-badge">NumPy</span>
    <span class="tool-badge">OpenCV</span>
    <span class="tool-badge">NLTK</span>
    <span class="tool-badge">Hugging Face</span>
    <span class="tool-badge">Jupyter</span>
    <span class="tool-badge">Google Colab</span>
  </div>
</div>

<!-- CTA -->
<div class="cta-section">
  <h2>
    <span class="en-content">Join the AI Revolution Today!</span>
    <span class="zh-content">今天就加入AI革命！</span>
  </h2>
  <p>
    <span class="en-content">Limited seats available for personalized mentorship</span>
    <span class="zh-content">个性化指导名额有限</span>
  </p>
  <a href="./contact.html" class="cta-button">
    <span class="en-content">Start Your AI Journey</span>
    <span class="zh-content">开始您的AI之旅</span>
  </a>
</div>
