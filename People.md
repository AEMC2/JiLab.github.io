---
layout: page
title: People
permalink: /people/
---

<style>
  /* 寮曞叆 Font Awesome 鍥炬爣搴擄紝鐢ㄤ簬鏍囬鍥炬爣 */
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css');
 /* 鍑忓皯椤甸潰涓や晶绌虹櫧 */
  .wrapper {
    max-width: min(1480px, calc(100vw - 72px));
    padding-left: 36px;
    padding-right: 36px;
  }
  /* 鏁翠綋瀹瑰櫒 */
  .people-container {
    font-family: 'Lato', sans-serif; /* 浣跨敤鏇翠笓涓氱殑瀛椾綋 */
  }

  @media (max-width: 900px) {
    .wrapper {
      max-width: calc(100vw - 32px);
      padding-left: 16px;
      padding-right: 16px;
    }
  }

  /* 1. 鍒嗗尯鏍囬鏍峰紡 */
  .people-section-title {
    font-size: 28px;
    font-weight: 700;
    color: #2a7ae2; /* 閱掔洰鐨勮摑鑹?*/
    padding-bottom: 10px;
    border-bottom: 3px solid #2a7ae2;
    margin-top: 50px;
    margin-bottom: 30px;
  }
  .people-section-title .fas {
    margin-right: 15px;
  }
  /* 绗竴涓爣棰樹笉闇€瑕佷笂杈硅窛 */
  .people-section-title:first-of-type {
    margin-top: 20px;
  }

  /* 2. 鎴愬憳鍗＄墖甯冨眬 (Flexbox) - 淇濇寔 PI, Associate Investigator, Lab Manager 鐨勬牱寮?*/
  .person-entry {
    display: flex;
    align-items: flex-start; /* 椤堕儴瀵归綈 */
    gap: 25px; /* 鍥剧墖鍜屼俊鎭箣闂寸殑闂磋窛 */
    margin-bottom: 30px;
    padding: 20px;
    border-radius: 12px; /* 鍦嗚 */
    background-color: #fdfdfd;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease-in-out; /* 涓烘偓鍋滄晥鏋滄坊鍔犲钩婊戝姩鐢?*/
  }

  /* 3. 浜掑姩鏁堟灉锛氶紶鏍囨偓鍋滄椂 */
  .person-entry:hover {
    transform: translateY(-5px) scale(1.05); /* 鍚戜笂娴捣骞舵斁澶?*/
    box-shadow: 0 8px 20px rgba(42, 122, 226, 0.15); /* 钃濊壊杈夊厜闃村奖 */
  }

  /* 鎴愬憳鐓х墖鏍峰紡 */
  .person-photo {
    width: 150px;
    height: 150px;
    border-radius: 50%; /* 鍦嗗舰澶村儚 */
    object-fit: cover; /* 纭繚鍥剧墖涓嶅彉褰?*/
    border: 3px solid #fff;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  }

  /* 鎴愬憳淇℃伅鍖哄煙 */
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
  
  /* 鎴愬憳閾炬帴鏍峰紡锛堝 Google Scholar锛?/
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
  /* ========= 鏂板: 缃戞牸甯冨眬瀹瑰櫒 (Grid Layout) ======== */
  /* ================================================= */
  .people-grid {
    display: grid;
    /* 鍒涘缓鍝嶅簲寮忓垪锛氬睆骞曞搴﹁冻澶熸椂鏈€澶?鍒楋紝鍚﹀垯鍑忓皯涓?鍒楁垨1鍒?*/
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px; /* 缃戞牸椤逛箣闂寸殑闂磋窛 */
  }

  /* 璋冩暣缃戞牸甯冨眬鍐呯殑鍗＄墖鏍峰紡 */
  .people-grid .person-entry {
    flex-direction: column; /* 鍨傜洿鍫嗗彔鐓х墖鍜屼俊鎭?*/
    align-items: center; /* 灞呬腑瀵归綈 */
    text-align: center;
    margin-bottom: 0; /* 缃戞牸闂磋窛鐢眊ap鎺у埗锛屼笉鍐嶉渶瑕乵argin-bottom */
  }

  .people-grid .person-photo {
    width: 120px;
    height: 120px;
  }


  /* 鍝嶅簲寮忚璁★細鍦ㄦ墜鏈虹瓑灏忓睆骞曚笂鍨傜洿鍫嗗彔 (鍘熸湁鐨? */
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
      <h3>Ni Ji , Ph.D.</h3>
      <p class="person-title">Principal Investigator</p>
      <p>Ph.D. in Neuroscience, Massachusetts Institute of Technology</p>
      <p><a href="mailto:niji@cibr.ac.cn">niji@cibr.ac.cn</a><br>Room B319</p>
      <div class="person-links">
        <a href="https://scholar.google.com/citations?hl=zh-CN&user=phTqe74AAAAJ" target="_blank">Google Scholar</a>
        <a href="https://www.cibr.ac.cn/#/teamDetail/cibrTeamteam/7eaf96c5b298444b84328680fb1b7a15/Ni%20Ji?lang=en" target="_blank">Faculty Page</a>
        <a href="{{ '/CV/Niji.html' | relative_url }}">C.V.</a>
      </div>
    </div>
  </div>

  <!-- ============================ Associate Investigator ============================ -->
  <h2 class="people-section-title"><i class="fas fa-bookmark"></i>Associate Investigator</h2>
  <div class="person-entry">
    <img class="person-photo" src="{{"/people/jiachang.jpg"| relative_url }}" />
    <div class="person-info">
      <h3>Jiachang Hao , Ph.D.</h3>
      <p class="person-title">Associate Investigator</p>
      <p>Ph.D. in Computer science, Beijing University of Posts and Telecommunication</p>
      <p><a href="mailto:haojiachang@cibr.ac.cn">haojiachang@cibr.ac.cn</a><br>Floor A6</p>
      <div class="person-links">
        <a href="https://scholar.google.com/citations?user=XRR603kAAAAJ&hl=en" target="_blank">Google Scholar</a>
      </div>
    </div>
  </div>

  <!-- ============================ Lab Manager ============================ -->
  <h2 class="people-section-title"><i class="fas fa-list"></i>Lab Manager</h2>
  <div class="person-entry">
    <img class="person-photo" src="{{"/people/Songxiangyu.jpg"| relative_url }}" />
    <div class="person-info">
      <h3>Xiangyu Song , Ph.D.</h3>
      <p class="person-title">Lab Manager</p>
      <p>Ph.D. in Biochemistry,Texas A&M University</p>
      <p><a href="mailto:songxiangyu@cibr.ac.cn">songxiangyu@cibr.ac.cn</a>
      <br>Floor B3</p>
      <!-- <div class="person-links">
        <a href="https://scholar.google.com/citations?user=XRR603kAAAAJ&hl=en" target="_blank">Google Scholar</a>
      </div> -->
    </div>
  </div>


  <!-- ============================ Postdoc ============================ -->
  <h2 class="people-section-title"><i class="fas fa-microscope"></i>Postdoc</h2>
  <div class="person-entry">
    <img class="person-photo" src="{{"/people/Jiachunying.jpg"| relative_url }}" />
    <div class="person-info">
      <h3>Chunying Jia , Ph.D.</h3>
      <p class="person-title">Postdoc</p>
      <p>Ph.D. in Electronic Engineering, University of Maryland, Baltimore County</p>
      <p><a href="mailto:jiachunying@cibr.ac.cn">jiachunying@cibr.ac.cn</a><br>Floor A6</p>
      <div class="person-links">
        <a href="https://scholar.google.com/citations?user=QwNC_bQAAAAJ&hl=en" target="_blank">Google Scholar</a>
      </div>
    </div>
  </div>


  <!-- ============================ Students ============================ -->
  <h2 class="people-section-title"><i class="fas fa-user-graduate"></i>Students</h2>
  
  
  <div class="people-grid">
    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Zexi Su-PhDstudent.png"| relative_url }}" />
      <div class="person-info">
        <h3>Zexi Su <br>B.S.</h3>
        <p>Peking University<br>& CIBR</p>
        <p class="person-title">2022-present Ph.D. Student</p>
        <p><a href="mailto:suzexi@cibr.ac.cn">suzexi@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/QianqianZhang-PhDstudent.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Qianqian Zhang <br>M.S.</h3>
        <p>China Agricultural University<br>& CIBR</p>
        <p class="person-title">2022-present Ph.D. Student</p>
        <p><a href="mailto:zhangqianqian@cibr.ac.cn">zhangqianqian@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Yating Liu-PhDstudent.jpg"| relative_url }}" />
      <div class="person-info">
          <h3>Yating Liu <br>B.S.</h3>
          <p>China Agricultural University<br>& CIBR</p>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p><a href="mailto:liuyating@cibr.ac.cn">liuyating@cibr.ac.cn</a></p>
      </div>
    </div>


    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Liuyu-PhDstudent.jpg"| relative_url }}" />
      <div class="person-info">
          <h3>Yu Liu <br>M.S.</h3>
          <p>Peking Union Medical College<br>& CIBR</p>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p><a href="mailto:liuyu@cibr.ac.cn">liuyu@cibr.ac.cn</a></p>
      </div>
    </div>

    

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Zhanghanyue-PhDstudent.jpg"| relative_url }}" />
      <div class="person-info">
          <h3>Hanyue Zhang <br>B.S.</h3>
          <p>Peking University<br>& CIBR</p>
          <p class="person-title">2023-present Ph.D. Student</p>
          <p><a href="mailto:zhanghanyue@cibr.ac.cn">zhanghanyue@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Lisiqi-PhDstudent.png"| relative_url }}" />
      <div class="person-info">
          <h3>Siqi Li <br>B.S.</h3>
          <p>Peking University<br>& CIBR</p>
          <p class="person-title">2024-present Ph.D. Student</p>
          <p><a href="mailto:lisiqi@cibr.ac.cn">lisiqi@cibr.ac.cn</a></p>
      </div>
    </div>
    
    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Ningsiyu-PhDstudent.jpg"| relative_url }}" />
      <div class="person-info">
          <h3>Siyu Ning <br>B.S.</h3>
          <p>China Agricultural University<br>& CIBR</p>
          <p class="person-title">2024-present Ph.D. Student</p>
          <p><a href="mailto:ningsiyu@cibr.ac.cn">ningsiyu@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Litianhe-PhDstudent.png"| relative_url }}" />
      <div class="person-info">
          <h3>Tianhe Li <br>M.S.</h3>
          <p>Peking Union Medical College<br>& CIBR</p>
          <p class="person-title">2025-present Ph.D. Student</p>
          <p><a href="mailto:litianhe@cibr.ac.cn">litianhe@cibr.ac.cn</a></p>
      </div>
    </div>

     <div class="person-entry">
      <img class="person-photo" src="{{"/people/Liuchun.jpg"| relative_url }}" />
      <div class="person-info">
          <h3>Chun Liu <br>B.S.</h3>
          <p>Peking Union Medical College<br>& CIBR</p>
          <p class="person-title">2025-present M.S. Student</p>
          <p><a href="mailto:liuchun@cibr.ac.cn">liuchun@cibr.ac.cn</a></p>
      </div>
    </div>

  </div>


  <!-- ============================ Lab Staff ============================ -->
  <h2 class="people-section-title"><i class="fas fa-users"></i>Lab Staff</h2>
  <div class="people-grid">


    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Wangdegang-Engineer.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Degang Wang <br>M.S.</h3>
        <p class="person-title">Deep Learning Engineer</p>
        <p><a href="mailto:wangdegang@cibr.ac.cn">wangdegang@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Wangjunjie-Engineer.png"| relative_url }}" />
      <div class="person-info">
        <h3>Junjie Wang <br>M.S.</h3>
        <p class="person-title">Deep Learning Engineer</p>
        <p><a href="mailto:wangjunjie@cibr.ac.cn">wangjunjie@cibr.ac.cn</a></p>
      </div>
    </div>


    <div class="person-entry">
      <img class="person-photo" src="{{"/people/fanyu-Reinforcement Learning Engineer.png"| relative_url }}" />
      <div class="person-info">
        <h3>Fanyu Zhu <br>M.S.</h3>
        <p class="person-title">Reinforcement Learning Engineer</p>
        <p><a href="mailto:zhufanyu@cibr.ac.cn">zhufanyu@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/JiahuiAn-researchasssistant.png"| relative_url }}" />
      <div class="person-info">
        <h3>Jiahui An <br>M.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:anjiahui@cibr.ac.cn">anjiahui@cibr.ac.cn</a></p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Hujiewen-researchasssistant.png"| relative_url }}" />
      <div class="person-info">
        <h3>Jiewen Hu <br>B.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:hujiewen@cibr.ac.cn">hujiewen@cibr.ac.cn</a></p>
      </div>
    </div>

     <div class="person-entry">
      <img class="person-photo" src="{{"/people/Yaoyaqian-researchasssistant.png"| relative_url }}" />
      <div class="person-info">
        <h3>Yaqian Yao <br>M.S.</h3>
        <p class="person-title">Research Assistant</p>
        <p><a href="mailto:yaoyaqian@cibr.ac.cn">yaoyaqian@cibr.ac.cn</a></p>
      </div>
    </div>

    
  </div>


  <!-- ============================ Interns ============================ -->
  <h2 class="people-section-title"><i class="fas fa-seedling"></i>Interns</h2>
  <div class="people-grid">
    <div class="person-entry">
      <img class="person-photo" src="{{"/people/Panyuhang.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Yuhang Pan</h3>
        <p class="person-title">Intern</p>
        <p>Zhejiang University, Psychology</p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/intern/wuyilin.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Yilin Wu</h3>
        <p class="person-title">Intern</p>
        <p>Nanjing University, Psychology</p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/intern/Jiazixing.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Zixing Jia</h3>
        <p class="person-title">Intern</p>
        <p>Sun Yat-sen University, Physics</p>
      </div>
    </div>

    <div class="person-entry">
      <img class="person-photo" src="{{"/people/intern/renlinhao.jpg"| relative_url }}" />
      <div class="person-info">
        <h3>Linghao Ren</h3>
        <p class="person-title">Intern</p>
        <p>Guilin University of
Electronic Technology, Information and Computing Science</p>
      </div>
    </div>
  </div>


  <!-- ============================ Lab Alumni ============================ -->
  <h2 class="people-section-title"><i class="fas fa-history"></i>Lab Alumni</h2>
  <p>Information about our past lab members can be found on the <a href="{{ '/alumni/' | relative_url }}">Alumni page</a>.</p>

</div>



