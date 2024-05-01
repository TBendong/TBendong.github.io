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
<title>复杂图文布局示例</title>
<style>
  body {
    font-family: Arial, sans-serif; /* 设置字体 */
    margin: 0; /* 移除默认边距 */
    padding: 0; /* 移除默认内边距 */
  }
  .header {
    background-color: #ccc; /* 灰色背景 */
    padding: 10px; /* 内边距 */
    text-align: center; /* 文本居中 */
    font-size: 24px; /* 字体大小 */
    border-radius: 10px; /* 圆角 */
  }
  .image-side {
    float: right; /* 让图片区域浮动在右侧 */
    width: 50%; /* 图片区域占一半宽度 */
    text-align: center; /* 图片和文字居中显示 */
    padding: 20px; /* 图片区域的内边距 */
  }
  img {
    width: 100%; /* 图片宽度调整为100%容器宽度 */
    height: auto; /* 图片高度自动调整 */
  }
  figcaption {
    color: #666; /* 说明文字颜色 */
    font-size: 18px; /* 说明文字大小 */
  }
  .text-side {
    padding: 10px; /* 文字区域的内边距 */
  }
</style>
</head>
<body>
<div class="header">Research Framework</div>
<div class="container">
  <div class="image-side">
    <figure>
      <img src="/images/Uncertainty Quantification.png" alt="描述性文本">
      <figcaption>This is a caption of the image.</figcaption>
    </figure>
  </div>
  <div class="text-side">
    <p>I concentrate on both practical applications within the system and the development of underlying algorithms. A comprehensive framework has been established to address a broad spectrum of uncertainty-related issues in power systems. This framework includes both forward and inverse uncertainty quantification methodologies.</p>
    <p>This framework includes both forward and inverse uncertainty quantification methodologies. The forward problems focus on risk assessment and stability analysis, which are crucial for proactive system management. Conversely, the inverse problems address parameter estimation, essential for system modeling and control.</p>
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
