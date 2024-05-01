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
    font-size: 20px; /* 字体大小 */
    border-radius: 10px; /* 圆角 */
  }
  .container {
    overflow: hidden; /* 清除浮动，保持布局整洁 */
  }
  .image-side {
    float: right; /* 图片浮动在右侧 */
    width: 50%; /* 图片占用容器的一半宽度 */
    text-align: center; /* 图片居中显示 */
    padding: 5px; /* 图片区域的内边距 */
  }
  img {
    width: 100%; /* 图片宽度调整为容器的100% */
    height: auto; /* 图片高度自动调整 */
  }
  figcaption {
    color: #666; /* 说明文字颜色 */
    font-size: 16px; /* 说明文字大小 */
  }
  .text-side {
    padding: 5px; /* 文字区域的内边距 */
  }
</style>
</head>
<body>
<div class="header">Research Framework</div>
<div class="container">
  <div class="image-side">
    <figure>
      <img src="/images/Uncertainty Quantification.png" alt="描述性文本">
      <figcaption>Research framework of uncertainty quantification for power system.</figcaption>
    </figure>
  </div>
  <div class="text-side">
    <p>I concentrate on both practical applications within the system and the development of underlying algorithms. A comprehensive framework has been established to address a broad spectrum of uncertainty-related issues in power systems. </p>
    <p><b>This framework includes both forward and inverse uncertainty quantification methodologies</b>. The forward problems focus on risk assessment and stability analysis, which are crucial for proactive system management. Conversely, the inverse problems address parameter estimation, essential for system modeling and control.</p>
  </div>
</div>
</body>
</html>




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
    font-size: 20px; /* 字体大小 */
    border-radius: 10px; /* 圆角 */
  }
  .container {
    overflow: hidden; /* 清除浮动，保持布局整洁 */
  }
  .image-side {
    float: right; /* 图片浮动在右侧 */
    width: 50%; /* 图片占用容器的一半宽度 */
    text-align: center; /* 图片居中显示 */
    padding: 5px; /* 图片区域的内边距 */
  }
  img {
    width: 100%; /* 图片宽度调整为容器的100% */
    height: auto; /* 图片高度自动调整 */
  }
  figcaption {
    color: #666; /* 说明文字颜色 */
    font-size: 16px; /* 说明文字大小 */
  }
  .text-side {
    padding: 20px; /* 文字区域的内边距 */
  }
</style>
</head>
<body>
<div class="header">Forward Uncertainty Quantification</div>
<div class="container">
  <div class="image-side">
    <figure>
      <img src="/images/Forward problem.png" alt="描述性文本">
      <figcaption>Forward uncertainty quantification for power system.</figcaption>
    </figure>
  </div>
  <div class="text-side">
    <p>Forward problem primarily addresses the propagation of input uncertainties through computational models to ascertain their consequent effects on the outputs. This process involves evaluating the sensitivity of the system’s responses to variations in inputs. The application of forward UQ is fundamental in appraising system behavior under variable scenarios, thereby serving as an invaluable tool in risk analysis and probabilistic stability assessment in power systems.</p>
  </div>
</div>
</body>
</html>


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
    font-size: 20px; /* 字体大小 */
    border-radius: 10px; /* 圆角 */
  }
  .container {
    overflow: hidden; /* 清除浮动，保持布局整洁 */
  }
  .image-side {
    float: right; /* 图片浮动在右侧 */
    width: 50%; /* 图片占用容器的一半宽度 */
    text-align: center; /* 图片居中显示 */
    padding: 5px; /* 图片区域的内边距 */
  }
  img {
    width: 100%; /* 图片宽度调整为容器的100% */
    height: auto; /* 图片高度自动调整 */
  }
  figcaption {
    color: #666; /* 说明文字颜色 */
    font-size: 16px; /* 说明文字大小 */
  }
  .text-side {
    padding: 5px; /* 文字区域的内边距 */
  }
  .container {
    overflow: visible; /* 确保内容不被截断 */
    padding-bottom: 20px; /* 增加底部内边距 */
  }
</style>
</head>
<body>
<div class="header">Inverse Uncertainty Quantification</div>
<div class="container">
  <div class="image-side">
    <figure>
      <img src="/images/Inverse problem.png" alt="描述性文本">
      <figcaption>Inverse uncertainty quantification for power system.</figcaption>
    </figure>
  </div>
  <div class="text-side">
    <p>Contrarily, the inverse problem is centered on deducing unknown model parameters or elucidating the nature of underlying uncertainties from power system observations. This modality is employed when direct measurement of certain system parameters is impractical, necessitating the inference of these parameters from observable data. Inverse UQ encompasses the calibration of model parameters to minimize the disparity between model simulation response and observed data, thereby bridging the gap between theoretical models and empirical reality. This approach is particularly pertinent in power system parameter estimation and data assimilation.</p>
  </div>
</div>
</body>
</html>


<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 100%; text-align: left;">
        <p> Modern power systems face increasing levels of uncertainty from renewable generation, time-varying loads, modeling limitations and measurement errors. These uncertainties propagate through the system and impact analysis related to steady-state conditions and dynamic performance. Consequently, <b>my primary research interests lie in the uncertainty quantification framework for power systems</b>. This framework is dedicated to enhancing the efficiency and precision of power system planning. It also aims to ensure the secure operation of power systems, as well as to achieve precise estimation and identification for power system modeling.</p>
    </div>
</div>



{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
