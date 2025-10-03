---
layout: page
# title: JI LAB
---

<style>
  /* 减少页面两侧空白 */
  .wrapper {
    max-width: 1100px;
    padding-left: 20px;
    padding-right: 20px;
  }

  /* 第一张大图的样式 */
  .image-first {
    width: 800px;
    margin: 0 auto 30px;
    display: block;
    border-radius: 8px;
  }

  /* --- 新增：用于排列一行图片的 Flexbox 容器 --- */
  .image-row {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    margin-bottom: 30px;
  }

  /* --- 新增：行内图片的样式 --- */
  .image-in-row {
    width: 300px;
    height: auto;
    border-radius: 8px;
    transition: all 0.3s ease-in-out; 
  }

  /* --- 新增：让中间的图片向上突出显示 --- */
  .image-row .image-in-row:nth-child(2) {
    transform: translateX(22px) scale(1.05); /* 向上移动20px并放大5% */
    /* box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2); 添加阴影增加立体感 */
    /* z-index: 1; 确保它叠在其他图片之上 */
  }

  /* --- 新增：鼠标悬停在整行上时，让未悬停的图片变暗、缩小 --- */
  /* .image-row:hover .image-in-row:not(:hover) {
    opacity: 0.8;
    transform: scale(0.98);
  } */

  /* 第一段文字样式 */
  .text-first {
    font-size: 28px;
    text-align: center;
    margin-bottom: 20px;
  }

  /* 第二段文字样式 */
  .text-second {
    font-size: 18px;
    line-height: 1.6;
  }




</style>

<p class="text-first">
  <font size="6">Welcome to <strong>Ji Lab</strong> at the <a href="http://cibr.ac.cn/#/">Chinese Institute for Brain Research (CIBR), Beijing</a>.</font>
</p>

<!-- 第一张大图 -->
<img class="image-first" src="{{ "/assets/lab_pic.jpg" | relative_url }}" alt="lab-show">

<!-- 新增的图片行容器 -->
<div class="image-row">
  <img class="image-in-row" src="{{ "/assets/fluorescence.png" | relative_url }}" alt="lab-show">
  <img class="image-in-row" src="{{ "/assets/index_show1.png" | relative_url }}" alt="lab-show">
  <img class="image-in-row" src="{{ "/assets/topic2.png" | relative_url }}" alt="lab-show">
</div>



<!-- 第二段文字 -->
<p class="text-second">
  <font size="6">Our research focuses on the <strong>computational neural mechanisms of perception, decision-making, and learning in animal navigation behavior.</strong>  <br>On this website, you can get to know <a href="{{ '/people/' | relative_url }}">who we are</a> and <a href="{{ '/research/' | relative_url }}">what we do</a>, check out the <a href="{{ '/publications/' | relative_url }}">publications</a> and <a href="{{ '/news/' | relative_url }}">news</a> for the latest updates 
  <!--or explore useful <a href="{% link Resources.md %}">resources</a>, <a href="{% link Fun.md %}">fun stuff</a>, -->and possible <a href="{{ '/join/' | relative_url }}">positions</a> in the lab.</font>
</p>
 
<!-- The navigation ability of organisms is crucial to their survival needs such as foraging, finding mates, harm avoidance and shelter hunting. Through evolution and natural selection, many species (from bacteria to mammals) have gained the powerful ability to effectively navigate through complex and uncertain natural environments. Previous studies have found that the navigation behavior of different species often points to similar principles at the algorithmic level (e. g., the movement of bacteria and nematodes in heterogeneous environments can be explained by the random walk model). At the same time, different species also develop perceptual and decision-making mechanisms specific to their own environment through evolution or acquired learning. Understanding the navigation algorithm of organisms and its neural control mechanism, on the one hand, can reveal the neural principle of biological brain control navigation behavior, on the other hand, can provide a new idea for the development of artificial intelligence navigation control system. -->
