---
layout: page
permalink: /Research/
title: Research
nav: true
nav_order: 3
---

<div class="research-statement">

  <p>
    Modern power systems are experiencing unprecedented levels of uncertainty, arising from two primary sources: incomplete knowledge of power system physics and sensor measurement errors, as well as the increasing integration of renewable energy resources and flexible loads such as electric vehicles. As these uncertainties propagate through the grid, they affect both steady-state operations and dynamic performance, posing significant challenges to system reliability and security. Effectively and efficiently quantifying these uncertainties and their impacts is the cornerstone of risk and insecurity mitigation in power system operations. However, existing uncertainty quantification research often struggles to handle complex, time-varying, and high-dimensional power system analyses, limiting their applicability to large-scale, real-world systems. 
    <b>In light of these challenges, my ambition is to establish aims to develop an efficient, scalable, and high-fidelity uncertainty quantification framework for power system modeling and risk analysis.</b>
    This framework is able to provide a deeper understanding of uncertainty propagation in power systems and support the reliable and resilient operation of renewable energy-integrated grids—ultimately contributing to global decarbonization efforts.
  </p>

  <div style="float:right; width:55%; text-align:center; margin:10px;">
    <img src="framework.pdf" alt="Power system uncertainty quantification framework" style="width:100%;">
    <p style="font-size:small;">Power system uncertainty quantification framework.</p>
  </div>

  <h3>My Past and Current Research</h3>
  <p>
    As shown in Figure above, the developed power system uncertainty quantification framework consists of two main modules: 
  </p>
  <ul>
    <li><b>Bayesian Dynamic modeling of system components</b>: This module models loads and inverter-based resources (IBRs) using sensor measurements. It involves parameter estimation for these components, which is fundamental for operators to conduct accurate power system analysis.</li>
    <li><b>Risk assessment</b>: Built upon the modeled power system, this module quantifies the probability of key operational metrics, such as voltage magnitudes, exceeding normal ranges due to stochastic variations in renewable generation, load demands, and contingencies.</li>
  </ul>

  <p>
    My research focuses on two core questions:<br>
    <i>1) How can we accurately estimate high-dimensional and time-varying system parameters, while also quantifying the uncertainties of these estimates, to achieve reliable dynamic modeling of power systems?<br>
    2) How can we efficiently and accurately quantify power system risks in the presence of large-scale integration of renewable energies, varying load demands, and potential contingencies?</i>
  </p>

  <p>
    I have developed various <u><i>computationally efficient data-driven techniques</i></u> to answer these questions, focusing on three key research directions:
  </p>
  <ul>
    <li>Developing high-dimensional constant parameter modeling methods for composite loads, aiding system operators in constructing accurate dynamic power system models and ensuring reliable system analysis.</li>
    <li>Proposing time-varying inertia estimation approaches for IBRs, which support online frequency stability analysis.</li>
    <li>Constructing scalable risk assessment methods for power systems across different time scales, ensuring the stability and reliability of power system operations.</li>
  </ul>

  <p>
    These efforts advance power system uncertainty quantification in terms of efficiency, scalability, and accuracy, leading to more than ten publications in top-tier journals (e.g., IEEE Transactions on Power Systems). Furthermore, through <b>broad collaborations with industry and national laboratories</b>, including <b>NREL, LLNL, PNNL, ANL, and ISO New England</b>, my research bridges theory and real-world applications. Some of these methods have been validated in practice, such as composite load modeling technique, successfully applied to fault measurements from a utility company in the southern United States.
  </p>


</div>
