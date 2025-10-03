---
layout: page
title: Research
permalink: /research/
---

<style>
/* 全局页面字体和背景 */
.wrapper {
    max-width: 1700px;
    padding-left: 20px;
    padding-right: 20px;
  }

.research-container {
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
line-height: 1.6;
}

/* 顶部全宽背景 */
/* 顶部全宽背景 */
.hero-section-full-width {
    color: white;
    padding: 80px 25px;
    text-align: center;
    /* --- 用户修改 ---: 图片路径已更新为本地图片 */
    background-image: url("{{ '/research/background.png' | relative_url }}");
    background-size: cover;
    background-position: center;
}

/* 这个容器让内部的文字内容保持居中，不会延伸到屏幕边缘 */
.hero-content-centered {
/* --- 修改点: 增加了最大宽度以减少两侧空白 --- */
max-width: 1700px;
margin: 0 auto;
}

.hero-content-centered h2 {
font-size: 3em;
font-weight: 600;
margin-top:-30px;
/* margin-bottom: 30px; */
}

.hero-content-centered .intro-text {
max-width: 1550px;
margin: 0 auto 50px auto;
font-size: 1.5em;
}

/* 三大研究方向模块 */
.pillars-container {
display: flex;
justify-content: center;
align-items: flex-start;
flex-wrap: wrap;
gap: 20px;
}

.pillar {
flex: 1;
min-width: 280px;
padding: 0 25px;
text-align: center;
position: relative;
}

/* 模块之间的分割线 */
@media (min-width: 992px) {
.pillar:not(:last-child)::after {
content: '';
position: absolute;
top: 15%;
right: 0;
height: 70%;
width: 1px;
background-color: rgba(255, 255, 255, 0.4);
}
}

.pillar .icon {
width: 65px;
height: 65px;
margin-bottom: 20px;
}

.pillar h3 {
font-size: 2em;
margin-bottom: 10px;
}

.pillar p {
font-size: 1.05em;
}

/* 主要内容区域 */
.main-content-section {
padding: 60px 25px;
text-align: center;
background-color: #ffffff;
/* --- 修改点: 增加了最大宽度以减少两侧空白 --- */
max-width: 2320px;
margin: 0 auto;
}

.main-content-section .section-title {
font-size: 2.1em;
color: #0d5f6f;
max-width: 900px;
margin: 0 auto 30px auto;
line-height: 1.4;
font-weight: 500;
}

.main-content-section .details-text {
max-width: 900px;
margin: 0 auto;
text-align: justify;
color: #558;
font-size: 1.2em;
}

/* 媒体展示区域 */
.media-grid {
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 35px;
padding: 20px;
/* --- 修改点: 增加了最大宽度以减少两侧空白 --- */
max-width: 1820px;
margin: 30px auto 50px auto;
}

.media-item {
flex: 1;
min-width: 300px;
max-width: 350px;
text-align: center;
}

/* 媒体文件样式 (图片和视频) */
.media-item img, .media-item video {
width: 100%;
height: auto;
border-radius: 8px;
box-shadow: 0 4px 12px rgba(0,0,0,0.1);
background-color: #f0f0f0;
margin-bottom: 15px;
}

.media-item .caption {
font-size: 1em;
color: #666;
font-weight: 500;
}

</style>
<!-- ======================= 顶部介绍区域 (现在是全宽背景) ======================= -->
<div class="hero-section-full-width">
<div class="hero-content-centered">
<h2>Research</h2>
<p class="intro-text">
Gaining insight into the navigational algorithms of organisms and their neural network-level regulatory mechanisms not only deepens our understanding of biological navigational decision-making but also offers novel perspectives for developing artificial intelligence (AI) navigation control systems. Our laboratory uses animal navigational behaviors as a model to explore the neural computational principles of the animal brain in complex environments, with a focus on three key aspects: (1) multimodal sensory integration; (2) behavioral decision-making; and (3) memory and learning. We integrate interdisciplinary approaches—including whole-brain imaging, quantitative behavioral analysis, machine learning, and theoretical modeling—to uncover the computational principles that make biological neural networks advantageous compared to existing artificial neural networks.
</p>
<div class="pillars-container">
  <div class="pillar">
    <!-- --- 用户修改 ---: 请将这里的图标路径换成您自己的图标文件 -->
    <!-- <img src="/assets/icon_modeling.svg" alt="Modeling Icon" class="icon"> -->
    <h3>Modeling</h3>
    <p>Modeling navigation behavior to decode biological algorithms.</p>
  </div>
  <div class="pillar">
    <!-- --- 用户修改 ---: 请将这里的图标路径换成您自己的图标文件 -->
    <!-- <img src="/assets/icon_dynamics.svg" alt="Dynamics Icon" class="icon"> -->
    <h3>Dynamics</h3>
    <p>Imaging brain-wide circuits and analyzing computational dynamics.</p>
  </div>
  <div class="pillar">
    <!-- --- 用户修改 ---: 请将这里的图标路径换成您自己的图标文件 -->
    <!-- <img src="/assets/icon_comparison.svg" alt="Comparison Icon" class="icon"> -->
    <h3>Comparison</h3>
    <p>Comparing species and AI agents to uncover core neural principles.</p>
  </div>
</div>
<!-- ======================= 核心内容区域 ======================= -->
</div>
</div>
<div class="research-container">
<!-- ======================= 核心内容区域1 ======================= -->
<div class="main-content-section">
<h3 class="section-title">
Quantitative Experiments + ML/Statistical Modeling: Describe, Simulate Animal Navigation & Explain Algorithmic Mechanisms
</h3>
<p class="details-text">
We employs the Caenorhabditis elegans (C. elegans), as a model system to decipher the neural computational mechanisms underlying its navigational behaviors in complex environments. Capitalizing on its fully mapped connectome, we focus on understanding how the worm optimizes survival strategies through integrated processes of sensation, learning, and decision-making. Our research is organized around three primary directions: (1) Adaptive foraging in C. elegans, where we quantify the dynamic transitions between "roaming" and "dwelling" behavioral states to uncover foraging algorithms across different environmental contexts; (2) Probabilistic associative learning in C. elegans, investigating how the worm performs probabilistic associative learning in noisy settings and elucidating the neural substrates that support Bayesian-like inference; and (3) Olfaction-based (food) object recognition, examining how C. elegans utilizes olfactory cues to distinguish among different bacterial (food) types from a distance, and clarifying the neural mechanisms by which it integrates multisensory information to approach beneficial substances and avoid harmful ones. To support these investigations, we have established a freely moving whole-brain imaging platform, which enables us to monitor and analyze neural activity across the entire brain at cellular resolution during behavior, thereby providing direct insights into the circuit-level mechanisms governing these adaptive processes.
</p>
</div>

<!-- ======================= 媒体展示区域1 ======================= -->
<div class="media-grid">
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/C.elegans.png"| relative_url }}" alt="Navigational behavior visualization">
<p class="caption">C.elegans</p>
</div>
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/WBI.gif"| relative_url }}" alt="Behaivor">
<p class="caption">Behaivor</p>
</div>

<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/WBI-platform.png"| relative_url }}" alt="C. elegans worm">
<p class="caption">Whole-Brain Imaging Platform</p>
</div>

</div>
<!-- ======================= 核心内容区域2 ======================= -->
<div class="main-content-section">
<h3 class="section-title">
Analysis of RNNs that can learn one or more motor tasks
</h3>
<p class="details-text">
 Predictive motor control is a fundamental feature of everyday behavior. A quintessential example is the game of table tennis: how does the brain predict the ball's trajectory to initiate arm movement at the precise moment, ensuring accurate contact between the racket and the ball? To address this, we employ Recurrent Neural Networks (RNNs) to model the neural mechanisms underlying this complex sensorimotor transformation. We train RNNs on large-scale neural population data—specifically, spike recordings obtained via invasive electrodes implanted in the common marmoset. The dynamics and outputs of the trained RNNs are then meticulously analyzed to identify potential neural correlates of anticipation, such as predictive activity and dynamical primitives, and to uncover the fundamental computational principles the brain uses to perform fast, accurate motor interception in a dynamic world.
</p>
</div>

<!-- ======================= 媒体展示区域2 ======================= -->
<div class="media-grid">
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/motor.jpg"| relative_url }}" alt="Interception in Daily Life
">
<p class="caption">Interception in Daily Life</p>
</div>
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/interception new paradigm .gif"| relative_url }}" alt="Interception Behaivor">
<p class="caption">Interception Behaivor</p>
</div>

<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/interception paradigm.gif"| relative_url }}" alt="Interception Behaivor">
<p class="caption">Interception Behaivor</p>
</div>

</div>
<!-- ======================= 核心内容区域3 ======================= -->
<div class="main-content-section">
<h3 class="section-title">
Human exploration & function learning in high dimensions
</h3>
<p class="details-text">
Humans and animals need to use environmental context to guide their learning and decision-making. How they actively sample a high dimensional environment, and efficiently learn the low-dimensional mapping between environmental features and task-specific values is unclear. What we do know is that humans and animals are constantly faced with a high-dimensional sensory world and they are indeed efficient learners compared to some of today’s AI models. The goal of this study is to record and analyze human exploratory behavior while they learn a contextual bandit task where the “context” resides in a high-dimensional space. Past studies suggest that human exploration in contextual bandit tasks can be approximated by the non-parametric algorithm, Gaussian process regression. However, those tasks are relatively low-dimensional and the task-relevant dimensions are explicitly told to the participants, thereby overriding the need for active exploration and dimensionality reduction. We hope our study can leverage a more naturalistic task setting to truly uncover the active learning potential in humans.
</p>
</div>

<!-- ======================= 媒体展示区域 ======================= -->
<div class="media-grid">
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/Topic 3 .png"| relative_url }}" alt="How to Choose a Restaurant" style="width: 300px; height: 300px;">
<p class="caption">How to Choose a Restaurant?</p>
</div>
<div class="media-item">
<!-- --- 用户修改 ---: 请将这里的图片或GIF文件路径换成您自己的文件 -->
<img src="{{"/research/Topic 3-2.png"| relative_url }}" alt="Possible Behavior" style="width: 500px;">
<p class="caption">Possible Behavior</p>
</div>

</div>


<br clear="left" />
<hr style="height:2px; border:0; background-image: linear-gradient(to right, rgba(255, 94, 19, 0), rgba(255, 94, 19, 0.6), rgba(255, 94, 19, 0))" />
<br>

