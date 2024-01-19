---
layout: archive
permalink: /research/
author_profile: true
---
{% include base_path %}
Bendong has dedicated himself to advancing techniques related to uncertainty in modern power systems. His work is pivotal in enhancing the efficiency and accuracy of power system operation. It also plays a critical role in the holistic and secure management of power systems with highly penetrated inverter-based resources (IBRs).
<center>
    <h2>Research Framework</h2>
</center>
<div>
    <img src='/images/Uncertainty Quantification.png' alt="network" style="width: 40%; float: left; margin-right: 2px;">
    <p>I concentrate on both practical applications within the system and the development of underlying algorithms. A comprehensive framework has been established to address a broad spectrum of uncertainty-related issues in power systems. This framework encompasses both forward and inverse uncertainty quantification methodologies.</p>
</div>
<center>
    <h2>Forward Uncertainty Quantification</h2>
</center>
<div>
    <img src='/images/Forward problem.png' alt="network" style="width: 40%; float: left; margin-right: 2px;">
    <p>Forward problem primarily addresses the propagation of input uncertainties through computational models to ascertain their consequent effects on the outputs. This process involves evaluating the sensitivity of the system’s responses to variations in inputs. The application of forward UQ is fundamental in appraising system behavior under variable scenarios, thereby serving as an invaluable tool in risk analysis and probabilistic stability assessment in power systems.</p>
</div>




{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
