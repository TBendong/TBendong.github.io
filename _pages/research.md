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
    <img src='/images/Uncertainty Quantification.png' alt="network" style="width: 70%; float: left; margin-right: 2px;">
    <p>In my research of uncertainty in power system, I not only focus on power system applications, but also its algorithm development.
Furthermore, I aim to build a systematic framework in solving a general uncertainty-related problems.
Now, the framework includes uncertainty modeling, forward uncertainty quantification (UQ), inverse uncertainty quantification and decision-making under uncertainty.</p>
</div>




{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
