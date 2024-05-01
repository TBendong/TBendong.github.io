---
layout: archive
permalink: /research/
author_profile: true
---
{% include base_path %}
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 100%; text-align: left;">
        <p> Modern power systems face increasing levels of uncertainty from renewable generation, time-varying loads, modeling limitations and measurement errors. These uncertainties propagate through the system and impact analysis related to steady-state conditions and dynamic performance. Consequently, <b>my primary research interests lie in the uncertainty quantification framework for power systems</b>. This framework is dedicated to enhancing the efficiency and precision of power system planning. It also aims to ensure the secure operation of power systems, as well as to achieve precise estimation and identification for power system modeling.</p>
    </div>
</div>

<html lang="zh">
<head>
<meta charset="UTF-8">
<title>自定义直线示例</title>
<style>
  .line {
    width: 100%; /* 线条宽度为整个容器的宽度 */
    height: 10px; /* 线条的粗细 */
    background-color: black; /* 线条颜色 */
    border-top: 5px dashed red; /* 设置线条为虚线，颜色为红色，线宽为5px */
  }
</style>
</head>
<body>
<div class="line"></div> <!-- 这是自定义的直线 -->
</body>
</html>

<center>
    <h2><strong>Research Framework</strong></h2>
</center>
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 50%; text-align: left;">
        <p>I concentrate on both practical applications within the system and the development of underlying algorithms. A comprehensive framework has been established to address a broad spectrum of uncertainty-related issues in power systems. This framework includes both forward and inverse uncertainty quantification methodologies. The forward problems focus on risk assessment and stability analysis, which are crucial for proactive system management. Conversely, the inverse problems address parameter estimation, essential for system modeling and control. </p>
    </div>
    <div style="width: 50%;">
        <img src='/images/Uncertainty Quantification.png' alt="network" style="width: 100%; display: block; margin-left: auto; margin-right: auto;">
    </div>
</div>


<html lang="zh">
<head>
<meta charset="UTF-8">
<title>图文并排示例</title>
<style>
  .container {
    display: flex; /* 启用 flex 布局 */
    align-items: flex-start; /* 内容垂直对齐到顶部 */
    justify-content: space-between; /* 内容分散对齐 */
  }
  .text {
    width: 50%; /* 文本占容器的一半宽度 */
  }
  .image-container {
    width: 50%; /* 图片容器占容器的一半宽度 */
    text-align: center; /* 图片和说明文字居中显示 */
  }
  img {
    max-width: 100%; /* 图片最大宽度为其容器宽度 */
    height: auto; /* 图片高度自动 */
  }
</style>
</head>
<body>
<div class="container">
  <div class="text">
    <p>这里是文章的文本内容。此部分内容在左边占据了50%的空间，与右侧的图片和说明文字并排展示。</p>
  </div>
  <div class="image-container">
    <figure>
      <img src="/images/Uncertainty Quantification.png" alt="图片描述">
      <figcaption>这是图片的说明文字。</figcaption>
    </figure>
  </div>
</div>
</body>
</html>


<center>
    <h2>Forward Uncertainty Quantification</h2>
</center>
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 50%; text-align: left;">
        <p>Forward problem primarily addresses the propagation of input uncertainties through computational models to ascertain their consequent effects on the outputs. This process involves evaluating the sensitivity of the system’s responses to variations in inputs. The application of forward UQ is fundamental in appraising system behavior under variable scenarios, thereby serving as an invaluable tool in risk analysis and probabilistic stability assessment in power systems.</p>
    </div>
    <div style="width: 50%;">
        <img src='/images/Inverse problem.png' alt="network" style="width: 100%; display: block; margin-left: auto; margin-right: auto;">
    </div>
</div>

<center>
    <h2>Inverse Uncertainty Quantification</h2>
</center>
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 50%; text-align: left;">
        <p>Contrarily, the inverse problem is centered on deducing unknown model parameters or elucidating the nature of underlying uncertainties from power system observations. This modality is employed when direct measurement of certain system parameters is impractical, necessitating the inference of these parameters from observable data. Inverse UQ encompasses the calibration of model parameters to minimize the disparity between model simulation response and observed data, thereby bridging the gap between theoretical models and empirical reality. This approach is particularly pertinent in power system parameter estimation and data assimilation.</p>
    </div>
    <div style="width: 50%;">
        <img src='/images/Inverse problem.png' alt="network" style="width: 100%; display: block; margin-left: auto; margin-right: auto;">
    </div>
</div>







{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
