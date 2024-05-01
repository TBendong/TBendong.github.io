---
layout: archive
permalink: /research/
author_profile: true
---
{% include base_path %}
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 50%; text-align: left;">
        <p>Bendong has dedicated himself to advancing techniques related to uncertainty in modern power systems. His work is pivotal in enhancing the efficiency and accuracy of power system operation. It also plays a critical role in the holistic and secure management of power systems with highly penetrated inverter-based resources (IBRs).</p>
    </div>
    <div style="width: 50%;">
        <img src='/images/Uncertainty Quantification.png' alt="network" style="width: 100%; display: block; margin-left: auto; margin-right: auto;">
    </div>
</div>

<center>
    <h2><strong>Research Framework</strong></h2>
</center>
<div style="display: flex; align-items: center; justify-content: space-between;">
    <div style="width: 50%; text-align: left;">
        <p>I concentrate on both practical applications within the system and the development of underlying algorithms. A comprehensive framework has been established to address a broad spectrum of uncertainty-related issues in power systems. This framework encompasses both forward and inverse uncertainty quantification methodologies.</p>
    </div>
    <div style="width: 50%;">
        <img src='/images/Forward problem.png' alt="network" style="width: 100%; display: block; margin-left: auto; margin-right: auto;">
    </div>
</div>

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
