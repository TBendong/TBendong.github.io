---
layout: page
permalink: /Research/
title: Research
nav: true
nav_order: 3
---
<div>
    <p>Modern power systems are experiencing unprecedented levels of uncertainty, arising from several sources: incomplete knowledge of power system physics, sensor measurement errors, as well as the increasing integration of renewable energy resources and flexible loads. As these uncertainties propagate through the grid, they affect both steady-state operations and dynamic performance, posing significant challenges to system reliability and security. My long-term goal is to advance power system resilience against uncertainties. My research has developed an efficient, scalable, and high-fidelity uncertainty quantification framework for power system modeling and risk analysis. The developed power system uncertainty quantification framework consists of two main modules: 
<ul>
    <li><b>Inverse Problem: Dynamic Modeling of System Components</b>: This module models loads and inverter-based resources (IBRs) using sensor measurements. It involves parameter estimation for these components, which is fundamental for operators to conduct accurate power system analysis.</li>
    <li><b>Forward Problem:  Risk Assessment</b>: Built upon the modeled power system, this module quantifies the probability of key operational metrics, such as voltage magnitudes, exceeding normal ranges due to stochastic variations in renewable generation, load demands, and contingencies.</li>
 </ul>
Through broad collaborations with industry and national laboratories, including <b>NREL, LLNL, PNNL, ANL, and ISO New England</b>, my research bridges theory and real-world applications. Some of these modules have been validated in practice, such as the load modeling technique, successfully applied to fault measurements from a utility company in the southern United States.</p>
<ul> </ul>
    
  <h4>Research Topic I: High-Dimension WECC Composite Load Modeling</h4>
  <p>
<div style="text-align: center;">
  <img src="/assets/img/myimage.png" alt="" width="300">
</div>
    The Western Electricity Coordinating Council (WECC) composite load model comprises various load components, such as different types of motors, distributed energy resources, and electric loads. This structure provides it with the capacity to emulate the dynamic characteristics of loads. Accurate dynamic load modeling is therefore essential for power system dynamic stability analysis, particularly for voltage stability. The goal of load modeling is to estimate the parameters of the WECC composite load model to replicate the measured dynamic response of actual loads. However, with over 100 parameters involved, this high-dimensional estimation task poses a significant challenge. My contributions to this topic are:
 <ul>
    <li> Proposed a global sensitivity analysis method based on sparse polynomial chaos expansion for identifying critical parameters. This mitigates the issue of "curse of high dimensionality". </li>
    <li> Achieved significant improvements in modeling efficiency by developing differentiable surrogate models, which eliminate the need for time-consuming load model simulations and prevent unconverged results.</li>
    <li> My research was the first in the dynamic load modeling field to provide both point estimates and confidence intervals for load parameters, enabling the quantification of uncertainties from learning or measurement errors and improving the reliability of power system models. </li>
 </ul>
  </p>

  <h4>Research Topic II: Time-Varying Inertia Estimation for IBRs</h4>
  <p>
    Inertia is an index that quantifies a power system's capability to mitigate frequency deviations. Accurate inertia estimation is therefore crucial for assessing power system frequency stability. However, certain devices in the power system, particularly IBRs such as renewable energies, are equipped with time-adaptive virtual inertia control strategies to enhance frequency deviation mitigation. While these strategies are beneficial for maintaining frequency stability, they pose significant challenges for parameter estimation. The difficulty arises because this time-varying inertia can undergo rapid and substantial changes within a matter of seconds, making it challenging for existing methods to track accurately. My contributions to this topic are:
       <ul>
    <li>Formulated the dynamic equations of virtual inertia into a Bayesian Kalman filter framework, enabling real-time estimation of time-varying inertia from IBRs.</li>
    <li>Designed an adaptive noise covariance update mechanism, allowing the filter to quantify estimation uncertainty and accurately track changes in inertia.</li>
    <li>Introduced an adaptive model-switching mechanism to maintain robust inertia estimation even when control switches, such as current limiter activation, occur.</li>
</ul>

  </p>

  <h4>Research Topic III: Scalable Power System Risk Assessment</h4>
  <p>
    Due to the penetration of various uncertain sources, such as flexible loads, solar, and wind generation, power system operations exhibit stochastic behavior, making it challenging to maintain the system within its normal operating range. Additionally, the power system is subject to contingencies, such as scheduled branch maintenance or unexpected branch outages caused by extreme weather. These uncertainties propagate through the system, increasing the likelihood that operational metrics may exceed safe thresholds. This necessitates accurate quantification of the risks posed by these uncertainties to prevent power system failures. However, existing data-driven methods either cannot handle a large number of contingencies simultaneously, fail to address the high-dimensional inputs caused by numerous uncertain sources, or struggle with the high-dimensional outputs required to model power system operational metrics. My contributions to this topic are: 
  </p>
    <ul>
    <li>Developed transfer learning-based surrogate models for pre-contingency load margin (static voltage stability) risk assessment, enabling rapid adaptation to network topology changes caused by scheduled branch maintenance.</li>
    <li>Proposed topology embeddings and multi-fidelity surrogate modeling techniques to evaluate voltage under numerous potential contingencies caused by rare events, significantly enhancing the accuracy and computational efficiency of pre-contingency voltage risk assessment.</li>
    <li>Designed instability-aware surrogate models to handle high-dimensional outputs for post-contingency scenarios, enabling immediate prediction of dynamic trajectories with quantified uncertainties using only a few real-time measurements.</li>
</ul>


</div>
