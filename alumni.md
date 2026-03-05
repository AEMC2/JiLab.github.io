---
layout: page
title: Alumni
permalink: /alumni/
---

<style>
  /* 引入 Font Awesome 图标库，用于标题图标 */
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css');

  .alumni-container {
    font-family: 'Lato', sans-serif;
    max-width: 1000px;
    margin: 0 auto;
  }

  .alumni-year-title {
    font-size: 24px;
    font-weight: 700;
    color: #2a7ae2;
    padding-bottom: 10px;
    border-bottom: 2px solid #ddd;
    margin-top: 40px;
    margin-bottom: 30px;
  }
  
  .alumni-year-title .fas {
    margin-right: 10px;
    color: #6495ED;
  }

  .alumni-grid {
    display: grid;
    /* 响应式网格：最多排3列，屏幕太小自动折行或变为2列/1列 */
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px;
  }

  .alumni-entry {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 20px;
    border-radius: 12px;
    background-color: #fdfdfd;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease-in-out;
  }

  .alumni-entry:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(42, 122, 226, 0.15);
  }

  .alumni-photo {
    width: 130px;
    height: 130px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid #fff;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    margin-bottom: 15px;
  }

  .alumni-info h3 {
    margin-top: 0;
    margin-bottom: 5px;
    font-size: 20px;
    color: #333;
  }

  .alumni-info .alumni-title {
    font-style: italic;
    color: #555;
    margin-bottom: 10px;
    font-size: 15px;
  }

  .alumni-info p {
    margin: 0;
    font-size: 14px;
    color: #666;
    line-height: 1.5;
  }
</style>

<div class="alumni-container">

  <!-- ============================ 2025 ============================ -->
  <h2 class="alumni-year-title"><i class="fas fa-calendar-alt"></i> 2025 Alumni</h2>
  <div class="alumni-grid">
    
    <div class="alumni-entry">
      <img class="alumni-photo" src="{{ '/people/Zhangwendi-LabManager5.png' | relative_url }}" />
      <div class="alumni-info">
        <h3>Wendi Zhang (张文迪), M.S.</h3>
        <p class="alumni-title">Lab Manager, 2024-2025</p>
      </div>
    </div>

    <div class="alumni-entry">
      <img class="alumni-photo" src="{{ '/people/gaochao.8454409e.jpg' | relative_url }}" />
      <div class="alumni-info">
        <h3>Chao Gao (高超), M.S.</h3>
        <p class="alumni-title">Deeplearning Engineer, 2023-2025</p>
      </div>
    </div>

    <div class="alumni-entry">
      <img class="alumni-photo" src="{{ '/people/Chizhang-alumni.png' | relative_url }}" />
      <div class="alumni-info">
        <h3>Chi Zhang (张弛), M.S.</h3>
        <p class="alumni-title">Research Assistant, 2023-2025</p>
        <p>M.S. Optical Engineering<br>National University of Defense Technology</p>
      </div>
    </div>

  </div>

  <!-- ============================ 2024 ============================ -->
  <h2 class="alumni-year-title"><i class="fas fa-calendar-alt"></i> 2024 Alumni</h2>
  <div class="alumni-grid">

    <div class="alumni-entry">
      <img class="alumni-photo" src="{{ '/people/Pengzhenghong-alumni.png' | relative_url }}" />
      <div class="alumni-info">
        <h3>Zhenghong Peng (彭正虹), M.S.</h3>
        <p class="alumni-title">Lab Manager, 2022-2024</p>
      </div>
    </div>

    <div class="alumni-entry">
      <img class="alumni-photo" src="{{ '/people/ChenJiang.jpg' | relative_url }}" />
      <div class="alumni-info">
        <h3>Chen Jiang (姜晨), B.S.</h3>
        <p class="alumni-title">Research Assistant, 2022-2024</p>
        <p>Now: PhD student at McGill University</p>
      </div>
    </div>

  </div>

</div>
