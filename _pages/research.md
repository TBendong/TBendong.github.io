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
    <img src='/images/Photo.jpg' alt="network" style="width: 20%; float: left; margin-right: 10px;">
    <p>这里是图片右侧的文字内容。你可以继续添加更多的文字，它们将自动排列在图片的右侧。</p>
</div>




{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
