---
layout: page
title: People
permalink: /people/
---

<style>
  /* 引入 Font Awesome 图标库，用于标题图标 */
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css');
 /* 减少页面两侧空白 */
  .wrapper {
    max-width: 1000px;
    padding-left: 20px;
    padding-right: 20px;
  }
  /* 整体容器 */
  .people-container {
    font-family: 'Lato', sans-serif; /* 使用更专业的字体 */
  }

  /* 1. 分区标题样式 */
  .people-section-title {
    font-size: 28px;
    font-weight: 700;
    color: #2a7ae2; /* 醒目的蓝色 */
    padding-bottom: 10px;
    border-bottom: 3px solid #2a7ae2;
    margin-top: 50px;
    margin-bottom: 30px;
  }
  .people-section-title .fas {
    margin-right: 15px;
  }
  /* 第一个标题不需要上边距 */
  .people-section-title:first-of-type {
    margin-top: 20px;
  }

  /* 2. 成员卡片布局 (Flexbox) - 保持 PI, Associate Investigator, Lab Manager 的样式 */
  .person-entry {
    display: flex;
    align-items: flex-start; /* 顶部对齐 */
    gap: 25px; /* 图片和信息之间的间距 */
    margin-bottom: 30px;
    padding: 20px;
    border-radius: 12px; /* 圆角 */
    background-color: #fdfdfd;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease-in-out; /* 为悬停效果添加平滑动画 */
  }

  /* 3. 互动效果：鼠标悬停时 */
  .person-entry:hover {
    transform: translateY(-5px) scale(1.05); /* 向上浮起并放大 */
    box-shadow: 0 8px 20px rgba(42, 122, 226, 0.15); /* 蓝色辉光阴影 */
  }

  /* 成员照片样式 */
  .person-photo {
    width: 150px;
    height: 150px;
    border-radius: 50%; /* 圆形头像 */
    object-fit: cover; /* 确保图片不变形 */
    border: 3px solid #fff;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  }

  /* 成员信息区域 */
  .person-info h3 {
    margin-top: 0;
    margin-bottom: 5px;
    font-size: 22px;
    color: #333;
  }

  .person-info .person-title {
    font-style: italic;
    color: #555;
    margin-bottom: 15px;
  }
  
  .person-info p {
    margin: 0 0 10px;
  }
  
  /* 成员链接样式（如 Google Scholar）*/
  .person-links a {
    display: inline-block;
    margin-right: 15px;
    color: #2a7ae2;
    text-decoration: none;
    font-weight: bold;
    font-size: 14px;
  }
  .person-links a:hover {
    text-decoration: underline;
  }
  
  /* ================================================= */
  /* ========= 新增: 网格布局容器 (Grid Layout) ======== */
  /* ================================================= */
  .people-grid {
    display: grid;
    /* 创建响应式列：屏幕宽度足够时最多3列，否则减少为2列或1列 */
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px; /* 网格项之间的间距 */
  }

  /* 调整网格布局内的卡片样式 */
  .people-grid .person-entry {
    flex-direction: column; /* 垂直堆叠照片和信息 */
    align-items: center; /* 居中对齐 */
    text-align: center;
    margin-bottom: 0; /* 网格间距由gap控制，不再需要margin-bottom */
  }

  .people-grid .person-photo {
    width: 120px;
    height: 120px;
  }


  /* 响应式设计：在手机等小屏幕上垂直堆叠 (原有的) */
  @media (max-width: 600px) {
    .person-entry {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
    .person-photo {
      width: 120px;
      height: 120px;
    }
  }
</style>

<div class="people-container">

  <!-- ============================ Principal Investigator ============================ -->
  <h2 class="people-section-title"><i class="fas fa-user-tie"></i>Principal Investigator</h2>
  <div class="person-entry">
    <img class="person-photo" src="{{"/people/NiJi-PrincipleInvestigator.jpg"| relative_url }}" />
    <div class="person-info">
      <h3>Ni Ji (吉妮), Ph.D.</h3>
      <p class="person-title">Principal Investigator</p>
      <p><a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a><br>Room B319</p>
      <div class="person-links">
        <a href="https://scholar.google.com/citations?hl=zh-CN&user=phTqe74AAAAJ" target="_blank">Google Scholar</a>
        <a href="https://www.cibr.ac.cn/science/team/detail/917" target="_blank">Faculty Page</a>
        <a href="{% link CV/Niji.md %}">C.V.</a>
      </div>
    </div>
  </div>

  <!-- ============================ Associate Investigator ============================ -->
  <h2 class="people-section-title"><i class="fas fa-bookmark"></i>Associate Investigator</h2>
  <div class="person-entry">
    <img class="person-photo" src="{{"/people/jiachang.jpg"| relative_url }}" />
    <div class="person-info">
      <h3>Jiachang Hao (郝家畅), Ph.D.</h3>
      <p class="person-title">Associate Investigator</p>
      <p>Ph.D. in Computer science, Beijing University of Posts and Telecommunication</p>
      <p><a href="mailto:haojiachang@cibr.ac.cn">haojiachang@cibr.ac.cn</a></p>
      <div class="person-links">
        <a href="https://scholar.google.com/citations?user=XRR603kAAAAJ&hl=en" target="_blank">Google Scholar</a>
      </div>
    </div>
  </div>

  <!-- ============================ Lab Manager ============================ -->
  <h2 class="people-section-title"><i class="fas fa-list"></i>Lab Manager</h2>
  <div class="person-entry">
    <img class="person-photo" src="/people/Zhangwendi-LabManager5.pNg" />
    <div class="person-info">
      <h3>Wendi Zhang (张文迪), M.S.</h3>
      <p class="person-title">Lab Manager</p>
      <p><a href="mailto:zhangwendi@cibr.ac.cn">zhangwendi@cibr.ac.cn</a><br>Floor B3</p>
      <!-- <div class="person-links">
        <a href="https://scholar.google.com/citations?user=XRR603kAAAAJ&hl=en" target="_blank">Google Scholar</a>
      </div> -->
    </div>
  </div>

  <!-- ============================ Ph.D. Students ============================ -->
  <h2 class="people-section-title"><i class="fas fa-user-graduate"></i>Ph.D. Students</h2>
  
  <!-- 将所有博士生和员工放在一个新的网格容器中 -->
  <div class="people-grid">
    <div class="person-entry">
      <img class="person-photo" src="/people/Zexi Su-PhDstudent.png" />
      <div class="person-info">
        <h3>Zexi Su (苏则茜), B.S.</h3>
        <p class="person-title">2022-present Ph.D. Student</p>
        <p>Peking University & CIBR</p>
        <p><a href="mailto:suzexi@cibr.ac.cn">suzexi@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/QianqianZhang-PhDstudent.jpg" />
      <div class="person-info">
        <h3>Qianqian Zhang (张倩倩), M.S.</h3>
        <p class="person-title">2022-present Ph.D. Student</p>
        <p>China Agricultural University & CIBR</p>
        <p><a href="mailto:zhangqianqian@cibr.ac.cn">zhangqianqian@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Liuyu-PhDstudent.jpg" />
      <div class="person-info">
          <h3>Yu Liu (刘煜), M.S.</h3>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p>Peking Union Medical College & CIBR</p>
          <p><a href="mailto:liuyu@cibr.ac.cn">liuyu@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Yating Liu-PhDstudent.jpg" />
      <div class="person-info">
          <h3>Yating Liu (刘雅婷), B.S.</h3>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p>China Agricultural University & CIBR</p>
          <p><a href="mailto:liuyating@cibr.ac.cn">liuyating@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Zhanghanyue-PhDstudent.jpg" />
      <div class="person-info">
          <h3>Hanyue Zhang (张含玥), B.S.</h3>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p>Peking University & CIBR</p>
          <p><a href="mailto:zhanghanyue@cibr.ac.cn">zhanghanyue@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Lisiqi-PhDstudent.png" />
      <div class="person-info">
          <h3>Siqi Li (李思齐), B.S.</h3>
          <p class="person-title">2024-present Ph.D. Student</p>
          <p>Peking University & CIBR</p>
          <p><a href="mailto:lisiqi@cibr.ac.cn">lisiqi@cibr.ac.cn</a></p>
      </div>
    </div>
    
    <div class="person-entry">
      <img class="person-photo" src="/people/Ningsiyu-PhDstudent.jpg" />
      <div class="person-info">
          <h3>Siyu Ning (宁思宇), B.S.</h3>
          <p class="person-title">2024-present Ph.D. Student</p>
          <p>China Agricultural University & CIBR</p>
          <p><a href="mailto:ningsiyu@cibr.ac.cn">ningsiyu@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Litianhe-PhDstudent.png" />
      <div class="person-info">
          <h3>Tianhe Li (李天赫), M.S.</h3>
          <p class="person-title">2025-present Ph.D. Student</p>
          <p>Peking Union Medical College & CIBR</p>
          <p><a href="mailto:litianhe@cibr.ac.cn">litianhe@cibr.ac.cn</a></p>
      </div>
    </div>
  </div>


  <!-- ============================ Lab Staff ============================ -->
  <h2 class="people-section-title"><i class="fas fa-users"></i>Lab Staff</h2>
  <div class="people-grid">
    <div class="person-entry">
      <img class="person-photo" src="/people/Wangjunjie-Engineer.png" />
      <div class="person-info">
        <h3>Junjie Wang (王俊杰), M.S.</h3>
        <p class="person-title">Deep Learning Engineer</p>
        <p><a href="mailto:wangjunjie@cibr.ac.cn">wangjunjie@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Chaogao-Engineer.png" />
      <div class="person-info">
        <h3>Chao Gao (高超), M.S.</h3>
        <p class="person-title">Deep Learning Engineer</p>
        <p><a href="mailto:gaochao@cibr.ac.cn">gaochao@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/fanyu-Reinforcement Learning Engineer.png" />
      <div class="person-info">
        <h3>Fanyu Zhu (朱璠宇), M.S.</h3>
        <p class="person-title">Reinforcement Learning Engineer</p>
        <p><a href="mailto:zhufanyu@cibr.ac.cn">zhufanyu@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/Hujiewen-researchasssistant.png" />
      <div class="person-info">
        <h3>Jiewen Hu (胡洁雯), B.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:hujiewen@cibr.ac.cn">hujiewen@cibr.ac.cn</a></p>
      </div>
    </div>

     <div class="person-entry">
      <img class="person-photo" src="/people/Yaoyaqian-researchasssistant.png" />
      <div class="person-info">
        <h3>Yaqian Yao (要雅倩), M.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:yaoyaqian@cibr.ac.cn">yaoyaqian@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="/people/JiahuiAn-researchasssistant.png" />
      <div class="person-info">
        <h3>Jiahui An (安佳晖), M.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:anjiahui@cibr.ac.cn">anjiahui@cibr.ac.cn</a></p>
      </div>
    </div>
  </div>


  <!-- ============================ Lab Alumni ============================ -->
  <h2 class="people-section-title"><i class="fas fa-history"></i>Lab Alumni</h2>
  <p>Information about our past lab members can be found on the <a href="{% link alumni.md %}">Alumni page</a>.</p>

</div>
