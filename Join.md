---
layout: page
title: Join Us
permalink: /join/
---

<style>
  /* ================== 通用样式 ================== */
  .wrapper {
    max-width: 1000px;
    padding-left: 20px;
    padding-right: 20px;
  }
  .join-us-container {
    font-family: sans-serif;
  }
  
  /* ================== 语言切换器样式 ================== */
  .lang-switcher {
    text-align: right;
    margin-bottom: 35px;
  }
  .lang-switcher button {
    background-color: #f0f0f0;
    border: 1px solid #ddd;
    color: #555;
    padding: 8px 15px;
    cursor: pointer;
    font-size: 14px;
    transition: all 0.3s ease;
    border-radius: 6px;
  }
  .lang-switcher button:first-child {
      border-top-right-radius: 0;
      border-bottom-right-radius: 0;
  }
  .lang-switcher button:last-child {
      border-top-left-radius: 0;
      border-bottom-left-radius: 0;
      border-left: none;
  }
  .lang-switcher button.active {
    background-color: #2a7ae2;
    color: white;
    border-color: #2a7ae2;
    font-weight: bold;
  }
  .lang-switcher button:not(.active):hover {
    background-color: #e9e9e9;
  }

  /* 默认隐藏英文内容 */
  .lang-en {
    display: none;
  }
  
  /* ================== 页面原有样式 (无需修改) ================== */
  .welcome-header {
    text-align: center;
    margin-bottom: 40px;
  }
  .welcome-header img {
    border-radius: 8px;
    vertical-align: middle;
  }
  .info-card {
    background-color: #fdfdfd;
    border: 1px solid #e9e9e9;
    border-radius: 12px;
    padding: 25px 30px;
    margin-bottom: 30px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  }
  .info-card h2 {
    font-size: 24px;
    color: #2a7ae2;
    margin-top: 0;
    border-bottom: 2px solid #f0f0f0;
    padding-bottom: 10px;
    margin-bottom: 20px;
  }
  .job-listing-card {
    border: 1px solid #e9e9e9;
    border-radius: 12px;
    margin-bottom: 20px;
    background-color: #fdfdfd;
    transition: all 0.3s ease;
  }
  .job-summary {
    padding: 25px 30px;
    cursor: pointer;
    list-style: none;
  }
  .job-summary::-webkit-details-marker {
    display: none;
  }
  .summary-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
  }
  .summary-header h3 {
    margin: 0;
    font-size: 22px;
    color: #2a7ae2;
  }
  .summary-description {
    margin: 15px 0 0 0;
    color: #555;
    line-height: 1.7;
  }
  .expand-icon {
    font-size: 28px;
    color: #2a7ae2;
    font-weight: bold;
    transition: transform 0.3s ease;
  }
  .job-details {
    padding: 25px 30px;
    border-top: 1px solid #f0f0f0;
  }
  .job-details h4 {
    color: #333;
    font-size: 18px;
    font-weight: 600;
    margin-top: 0;
    margin-bottom: 10px;
  }
  .job-details ul {
    padding-left: 20px;
    line-height: 1.8;
    margin-bottom: 25px;
  }
  .job-details ul:last-child {
      margin-bottom: 0;
  }
  .job-details li {
    margin-bottom: 8px;
  }
  .job-listing-card[open] {
    box-shadow: 0 8px 20px rgba(42, 122, 226, 0.1);
    border-color: #a9c7ec;
  }
  .job-listing-card[open] .expand-icon {
    transform: rotate(45deg);
  }
  .job-listing-card:not([open]):hover {
      border-color: #a9c7ec;
      background-color: #fafdff;
  }

  #floating-decorations {
  position: absolute; /* 改为 absolute，让它随页面滚动 */
  top: 0;
  left: 0;
  width: 100%;
  height: 100%; /* 高度将由JS动态调整以适应内容 */
  z-index: -1;
  pointer-events: none;
  overflow: hidden;
}

/* .deco-image 和 @keyframes 动画样式保持不变 */
.deco-image {
  position: absolute;
  opacity: 1;
  animation: float-animation 8s ease-in-out infinite;
  border-radius: 12px; /* 给图片加个小圆角，看起来更柔和 */
  box-shadow: 0 5px 15px rgba(0,0,0,0.1); /* 加一点阴影，更有层次感 */
}
@keyframes float-animation {
  0% { transform: translateY(0px); }
  50% { transform: translateY(-15px); }
  100% { transform: translateY(0px); }
}

/* ================== 确保主要内容在装饰之上 ================== */
.join-us-container {
    position: relative; /* 必须设置，以使 z-index 生效 */
    z-index: 1; /* 确保 z-index 高于装饰层 */
    background-color: white; /* 确保有背景色，否则装饰会透过来 */
}

</style>
<div id="floating-decorations" aria-hidden="true"></div>
<div class="join-us-container">

  <div class="welcome-header">
    <!-- <img width="200" style="margin-right:25px;" src="/assets/Jilab_logo.png"> -->
    <img width="400" src="{{"/assets/Jilab_logo.gif"| relative_url }}">
  </div>
  
  <!-- 语言切换器 -->
  <div class="lang-switcher">
    <button id="btn-zh" class="active">中文</button>
    <button id="btn-en">English</button>
  </div>

  <!-- =============================== 中文内容区域 =============================== -->
  <div class="lang-zh">
    <p><font size="4"><strong>我们的实验室正在积极招聘博士后和研究助理。如果您有兴趣加入我们的团队，请与我们联系。 邮箱: <a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a></strong></font></p>
    <p><font size="4"><strong>我们欢迎来自不同背景的研究人员加入我们的团队。无论您的背景是<strong style="font-size: 1.2em;">生物学、心理学、物理学、理工科（STEM）还是其他领域</strong>，也无论您是热衷于动手实验、数据挖掘还是建模——只要您愿意并渴望探索大脑如何控制行为的奥秘，我们都欢迎您成为我们团队的一员。</strong></font></p>

    <div class="info-card">
      <h2>中心与课题组简介</h2>
      <p><strong>中心简介：</strong><a href="http://www.cibr.ac.cn/" target="_blank">北京脑科学与类脑研究中心</a>（CIBR）是北京市政府与中国科学院、北京大学等单位共建的新型研发机构，旨在瞄准世界脑科学前沿，产出一批重大原始创新成果。</p>
      <p><strong>课题组简介：</strong>我们致力于理解生物脑高效学习与决策的神经计算机制。将前沿神经生物实验技术与深度学习等理论工具相结合，揭示动物脑优于人工智能的关键机制，并开发有应用价值的类脑AI算法。团队近期研究成果被国际顶会 <a href="/papers/2025_Brain_Bandit_A_Biologica.pdf">ICLR 2025</a> 接收。研究团队获得国自然、中国医学科学院、北京市、字节跳动等多项基金支持。</p>
    </div>
    
    <div class="info-card">
      <h2>开放职位</h2>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>博士后 (Postdoctoral Fellow)</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">独立开展实验室相关方向研究，领导或协助实验室新课题的开发与推进。协助指导学生和技术人员，协助撰写课题相关基金和文章等。</p>
        </summary>
        <div class="job-details">
          <h4>岗位要求</h4>
          <ul>
            <li>即将或已经获得脑科学或理工类专业博士学位</li>
            <li>以第一作者发表或即将发表SCI论文或机器学习领域会议论文</li>
            <li>有计算神经学、物理/数学/统计、计算机/人工智能或其他相关背景</li>
            <li>掌握动力系统理论、统计物理、强化学习或深度学习者优先</li>
            <li>对智能的理论基础、AI4Brain Science等方向有强烈兴趣</li>
            <li>流利的英语读写和日常交流能力</li>
          </ul>
          <h4>薪资待遇</h4>
          <ul>
            <li>提供有竞争力的薪资，享受五险一金、补充医疗保险、班车等福利</li>
            <li>按照国家博士后政策协助解决北京市落户</li>
            <li>每年5万元房补，并协助解决孩子上学问题</li>
            <li>全力支持个人职业发展，提供丰富的国内外会议与合作机会</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>研究助理 (Research Assistant)</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">在PI的指导下参与和协助实验室课题研究，负责实验执行、数据收集与初步分析等工作。</p>
        </summary>
        <div class="job-details">
          <h4>岗位要求</h4>
          <ul>
            <li>本科或硕士毕业</li>
            <li>对大脑的计算机制、类脑算法开发等脑科学与AI交叉方向有浓厚兴趣</li>
            <li>有数学建模和/或深度学习背景经验者优先</li>
            <li>有良好的科研文献搜索、阅读能力，乐于沟通和团队协作</li>
            <li>工作认真，科研热情高，有两年以上工作意向者优先</li>
          </ul>
          <h4>薪资待遇</h4>
          <ul>
            <li>按资历提供有竞争力的薪资，享受五险一金、补充医疗保险等福利</li>
            <li>协助租住员工公寓或昌平区公租房</li>
            <li>协助符合条件者申请北京户口</li>
            <li>全力支持个人职业发展，提供丰富的学习和合作机会</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>深度/强化学习算法工程师</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">将前沿深度学习技术运用在行为或神经数据的分析与建模中，根据课题需要开发、迭代新的深度学习模型与算法，并负责前沿技术的跟踪。</p>
        </summary>
        <div class="job-details">
          <h4>岗位要求</h4>
          <ul>
            <li>计算机、人工智能、自动控制等相关专业硕士及以上学位</li>
            <li>熟练使用Python/C++及TensorFlow/PyTorch等至少一种深度学习框架</li>
            <li>掌握强化学习（如 DQN、DDPG、PPO、SAC 等）并有实际项目经验者优先；</li>
            <li>发表过期刊或会议论文。在 ICML/NeurIPS/IJCAI/AAAI/ICLR/ICRA 等国际会议上发表过学术论文者优先考虑；</li>
            <li>掌握常用深度学习模型并有实际项目经验，掌握深度强化学习者优先</li>
            <li>发表过期刊或会议论文者优先，对脑科学与AI交叉研究有浓厚兴趣</li>
          </ul>
          <h4>薪资待遇</h4>
          <ul>
            <li>提供有竞争力的薪资，按工资全额缴纳五险一金，福利优厚</li>
            <li>协助租住员工公寓或公租房，并协助符合条件者申请北京户口</li>
            <li>提供参加国内外会议、访问交流及继续深造的丰富机会</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>实习生 / 毕设实习生 (Intern)</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">在PI或资深研究人员的指导下，协作或独立完成指定的科研项目，学习前沿研究方法。</p>
        </summary>
        <div class="job-details">
          <h4>岗位要求</h4>
          <ul>
            <li>本科或硕士在读</li>
            <li>能持续实习（三个月以上）者优先</li>
            <li>对大脑的计算机制、类脑算法开发等方向有浓厚兴趣</li>
            <li>有数学建模、数据分析、深度学习等背景经验者优先</li>
            <li>有良好的科研文献搜索、阅读能力，乐于沟通和团队协作</li>
          </ul>
          <h4>薪资待遇</h4>
          <ul>
            <li>提供每月2000-3500元薪酬（根据个人资历和工作安排而定）</li>
            <li>协助租住实习生宿舍，PI直接指导</li>
            <li>对优秀者提供论文署名投稿机会，并推荐在国内外一流院校进一步深造</li>
          </ul>
        </div>
      </details>
    </div>
    <div class="info-card">
      <h2>工作地点与应聘方式</h2>
      <p><strong>工作地点：</strong>北京市昌平区中关村生命科学园---医科路9号院3号楼---北京脑科学与类脑研究所</p>
      <p><strong>应聘方式：</strong>应聘者请发送个人简历、求职信（简述个人职业规划及科研目标），博士后请另提供2-3份推荐信（由推荐人直接寄出）到 <a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a>，邮件标题注明为“<b>姓名+申请职位</b>”（例如：张三+博士后申请）。</p>
    </div>
  </div>

  <!-- =============================== 英文内容区域 =============================== -->
  <div class="lang-en">
    <p style="font-size: 1.1em;"><strong>Our lab is actively recruiting Postdoctoral Fellows and Research Assistants. If you are interested in joining our team, please contact us at: <a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a></strong></p>
    <p style="font-size: 1.1em;"><strong>We welcome researchers from diverse backgrounds to join our team. Whether your background is in <span style="font-size: 1.2em;"><strong>Biology, psychology, physics, STEM, or other fields</strong></span>, and whether you are passionate about wet-lab experiments, data mining, or modeling—as long as you are willing and eager to explore the mysteries of how the brain controls behavior, we welcome you to become a member of our team.</strong></p>

    <div class="info-card">
      <h2>About CIBR and Our Lab</h2>
      <p><strong>About the Center:</strong> The <a href="http://www.cibr.ac.cn/en/" target="_blank">Chinese Institute for Brain Research, Beijing (CIBR)</a>, is a new type of research institution co-established by the Beijing Municipal Government, the Chinese Academy of Sciences, and Peking University. It aims to target the frontiers of brain science and produce significant original innovative achievements.</p>
      <p><strong>About the Lab:</strong> We are dedicated to understanding the neural computation mechanisms of efficient learning and decision-making in the biological brain. By integrating cutting-edge neurobiological experimental techniques with theoretical tools like deep learning, we aim to uncover the key mechanisms that make the animal brain superior to artificial intelligence and develop valuable brain-inspired AI algorithms. Our team's recent research has been accepted by the top international conference <a href="/papers/2025_Brain_Bandit_A_Biologica.pdf">ICLR 2025</a>. The research team is supported by grants from NSFC, CAMS, the Beijing Municipality, and ByteDance, among others.</p>
    </div>

    <div class="info-card">
      <h2>Open Positions</h2>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>Postdoctoral Fellow</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">Independently conduct research in the lab's relevant directions, leading or assisting in the development and advancement of new projects. Assist in mentoring students and technicians, and contribute to writing grant proposals and publications.</p>
        </summary>
        <div class="job-details">
          <h4>Qualifications</h4>
          <ul>
            <li>Ph.D. degree (or expected soon) in brain science or a STEM-related field.</li>
            <li>First-author publication (published or forthcoming) in an SCI-indexed journal or a top machine learning conference.</li>
            <li>Background in computational neuroscience, physics, mathematics, statistics, computer science, artificial intelligence, or other related fields.</li>
            <li>Experience with dynamical systems theory, statistical physics, reinforcement learning, or deep learning is preferred.</li>
            <li>Strong interest in the theoretical foundations of intelligence, AI for Brain Science, and related areas.</li>
            <li>Fluent in English reading, writing, and daily communication.</li>
          </ul>
          <h4>What We Offer</h4>
          <ul>
            <li>A competitive salary and benefits package, including comprehensive social insurance, supplemental medical insurance, shuttle bus services, etc.</li>
            <li>Assistance with obtaining Beijing Hukou (residency permit) in accordance with national postdoctoral policies.</li>
            <li>An annual housing allowance of 50,000 RMB and assistance with children's schooling.</li>
            <li>Full support for career development, with ample opportunities for domestic and international conferences and collaborations.</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>Research Assistant</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">Participate in and assist with lab research projects under the PI's guidance, responsible for experiment execution, data collection, and preliminary analysis.</p>
        </summary>
        <div class="job-details">
          <h4>Qualifications</h4>
          <ul>
            <li>Bachelor's or Master's degree.</li>
            <li>Strong interest in the intersection of brain science and AI, such as the brain's computational mechanisms and the development of brain-inspired algorithms.</li>
            <li>Experience in mathematical modeling and/or deep learning is preferred.</li>
            <li>Good skills in searching and reading scientific literature; a collaborative and communicative team player.</li>
            <li>Diligent, highly motivated for research, with an intention to work for more than two years preferred.</li>
          </ul>
          <h4>What We Offer</h4>
          <ul>
            <li>A competitive salary based on experience, with benefits including comprehensive social insurance and supplemental medical insurance.</li>
            <li>Assistance in applying for employee apartments or public rental housing in Changping District.</li>
            <li>Assistance for qualified candidates in applying for a Beijing Hukou.</li>
            <li>Full support for career development, with abundant learning and collaboration opportunities.</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>Deep/Reinforcement Learning Engineer</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">Apply cutting-edge deep learning techniques to analyze and model behavioral or neural data. Develop and iterate new deep learning models and algorithms as required by projects, and track state-of-the-art technologies.</p>
        </summary>
        <div class="job-details">
          <h4>Qualifications</h4>
          <ul>
            <li>Master's degree or higher in Computer Science, AI, Automatic Control, or a related field.</li>
            <li>Proficient in Python/C++ and at least one deep learning framework such as TensorFlow/PyTorch.</li>
            <li>Proficiency in reinforcement learning (e.g., DQN, DDPG, PPO, SAC, and other algorithms) with practical project experience is preferred.</li>
            <li>Publications in academic journals or conferences are required; in particular, candidates with papers published in top international conferences such as ICML, NeurIPS, IJCAI, AAAI, ICLR, and ICRA will be given priority consideration.</li>
            <li>Practical project experience with common deep learning models; expertise in deep reinforcement learning will be given priority consideration.</li>
            <li>Published journal or conference papers are preferred; strong interest in interdisciplinary research between brain science and AI.</li>
          </ul>
          <h4>What We Offer</h4>
          <ul>
            <li>A competitive salary with full social insurance contributions based on salary, and excellent benefits.</li>
            <li>Assistance with employee or public rental housing and support for qualified candidates applying for a Beijing Hukou.</li>
            <li>Rich opportunities to attend international conferences, participate in academic exchanges, and pursue further education.</li>
          </ul>
        </div>
      </details>
      <details class="job-listing-card">
        <summary class="job-summary">
          <div class="summary-header"><h3>Intern / Thesis Intern</h3><span class="expand-icon">+</span></div>
          <p class="summary-description">Collaborate on or independently complete designated research projects and learn cutting-edge research methods under the guidance of the PI or senior researchers.</p>
        </summary>
        <div class="job-details">
          <h4>Qualifications</h4>
          <ul>
            <li>Currently enrolled in a Bachelor's or Master's program.</li>
            <li>Ability to intern for a continuous period (3 months or more) is preferred.</li>
            <li>Strong interest in the computational mechanisms of the brain, brain-inspired algorithm development, etc.</li>
            <li>Experience in mathematical modeling, data analysis, or deep learning is a plus.</li>
            <li>Good skills in searching and reading scientific literature; a collaborative and communicative team player.</li>
          </ul>
          <h4>What We Offer</h4>
          <ul>
            <li>A monthly stipend of 2,000-3,500 RMB (depending on qualifications and workload).</li>
            <li>Assistance with intern dormitory housing and direct mentorship from the PI.</li>
            <li>Opportunities for co-authorship on publications for outstanding performers, with recommendations for further studies at top domestic and international universities.</li>
          </ul>
        </div>
      </details>
    </div>
    <div class="info-card">
      <h2>Location and How to Apply</h2>
      <p><strong>Location:</strong> Chinese Institute for Brain Research, Beijing (CIBR), Building 3, Yard 9, Yike Road, Zhongguancun Life Science Park, Changping District, Beijing</p>
      <p><strong>How to Apply:</strong> Please send your CV and a cover letter (briefly describing your career goals and research interests) to <a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a>. Postdoctoral applicants should also arrange for 2-3 letters of recommendation to be sent directly by the referees. Please use the subject line "<b>Name + Position Applied For</b>" (e.g., Scarbu + Postdoctoral Application).</p>
    </div>
  </div>

</div>

<!-- JavaScript for Language Switching -->
<script>
  // JavaScript for Language Switching AND Floating Decorations
document.addEventListener('DOMContentLoaded', function() {
  
  // --- 语言切换功能 (保留不变) ---
  const btnZh = document.getElementById('btn-zh');
  const btnEn = document.getElementById('btn-en');
  const contentZh = document.querySelector('.lang-zh');
  const contentEn = document.querySelector('.lang-en');

  btnZh.addEventListener('click', function() {
    contentZh.style.display = 'block';
    contentEn.style.display = 'none';
    btnZh.classList.add('active');
    btnEn.classList.remove('active');
  });

  btnEn.addEventListener('click', function() {
    contentZh.style.display = 'none';
    contentEn.style.display = 'block';
    btnEn.classList.add('active');
    btnZh.classList.remove('active');
  });

  // --- 全新的浮动装饰功能 ---
  const decorationsContainer = document.getElementById('floating-decorations');
  const mainContent = document.querySelector('.join-us-container');

  const siteHeader = document.querySelector('.site-header');

  // 1. 动态获取导航栏的高度
  const headerHeight = siteHeader ? siteHeader.offsetHeight+400 : 60; // 如果获取失败，默认60px

  // 2. 将装饰容器的顶部（top）设置为导航栏的高度，这样它就从导航栏下面开始了
  decorationsContainer.style.top = `${headerHeight}px`;

  // ====================================================================

  // 动态设置装饰层的高度，使其与主要内容等高
  decorationsContainer.style.height = `${mainContent.offsetHeight}px`;
  
  const imageUrls = [
    "{{ '/assets/lab_photo1.jpg' | relative_url }}",
    "{{ '/assets/lab_photo2.jpg' | relative_url }}",
    "{{ '/assets/lab_photo3.jpeg' | relative_url }}",
    "{{ '/assets/lab_photo4.jpeg' | relative_url }}",
    "{{ '/assets/lab_photo5.jpg' | relative_url }}",
    "{{ '/assets/lab_photo6.jpg' | relative_url }}",
    "{{ '/assets/lab_photo7.jpeg' | relative_url }}",
    "{{ '/assets/lab_photo8.jpg' | relative_url }}"
  ];

  const imageCount = 8;
  const imagesPerSide = imageCount / 2;
  const slotHeight = mainContent.offsetHeight / imagesPerSide;

  for (let i = 0; i < imageCount; i++) {
    const img = document.createElement('img');
    img.src = imageUrls[i % imageUrls.length];
    img.className = 'deco-image';

    const size = Math.random() * 350 + 300;
    img.style.width = `${size}px`;
    img.style.height = 'auto';

    const side = i % 2 === 0 ? 'left' : 'right';
    const slotIndex = Math.floor(i / 2); 
    const slotStartTop = slotIndex * slotHeight;
    const top = slotStartTop + (Math.random() * (slotHeight - size));

    const position = Math.random() * 15 + 2; 
    
    img.style.top = `${top}px`;
    img.style[side] = `${position}vw`;
    
    const rotation = Math.random() * 20 - 10;
    img.style.transform = `rotate(${rotation}deg)`;
    img.style.animationDelay = `${Math.random() * -8}s`;

    decorationsContainer.appendChild(img);
  }
});
</script>
