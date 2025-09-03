---
layout: page
permalink: /Research/
title: Research
nav: true
nav_order: 3
---

<div style="float:right; width:55%; text-align:center; margin:10px;">
  <img src="/assets/img/framework.svg" alt="Power system uncertainty quantification framework" style="width:100%;">
  <p style="font-size:small;">Power system uncertainty quantification framework.</p>
</div>

<div>
    Modern power systems are experiencing unprecedented levels of uncertainty, arising from several sources: incomplete knowledge of power system physics and sensor measurement errors, as well as the increasing integration of renewable energy resources and flexible loads such as electric vehicles. As these uncertainties propagate through the grid, they affect both steady-state operations and dynamic performance, posing significant challenges to system reliability and security. My long-term goal is to advance power system resilience against uncertainties. My research has developed an efficient, scalable, and high-fidelity uncertainty quantification framework for power system modeling and risk analysis. The developed power system uncertainty quantification framework consists of two main modules: 
<ul>
    <li><b>Inverse Problem: Dynamic Modeling of System Components</b>: This module models loads and inverter-based resources (IBRs) using sensor measurements. It involves parameter estimation for these components, which is fundamental for operators to conduct accurate power system analysis.</li>
    <li><b>Forward Problem:  Risk Assessment</b>: Built upon the modeled power system, this module quantifies the probability of key operational metrics, such as voltage magnitudes, exceeding normal ranges due to stochastic variations in renewable generation, load demands, and contingencies.</li>
  </ul>
  <p>
Through <b>broad collaborations with industry and national laboratories</b>, including <b>NREL, LLNL, PNNL, ANL, and ISO New England</b>, my research bridges theory and real-world applications. Some of these methods have been validated in practice, such as composite load modeling technique, successfully applied to fault measurements from a utility company in the southern United States.
  </p>

  <h4>High-Dimension WECC Composite Load Modeling</h4>
  <p>
    The Western Electricity Coordinating Council (WECC) composite load model comprises various load components, such as different types of motors, distributed energy resources, and electric loads. This structure provides it with the capacity to emulate the dynamic characteristics of loads. Accurate dynamic load modeling is therefore essential for power system dynamic stability analysis, particularly for voltage stability. The goal of load modeling is to estimate the parameters of the WECC composite load model to replicate the measured dynamic response of actual loads. However, with over 100 parameters involved, this high-dimensional estimation task poses a significant challenge.
  </p>
  <p>
    To address this challenge, I propose an amortized Bayesian inference learning method to identify a subset of critical parameters that significantly influence the dynamic load response <i>(Tan, 2024, Amortized)</i>. To further mitigate the impact of measurement errors, a differentiable surrogate model of the composite load is integrated into the Hamiltonian Monte Carlo framework. This approach enables accurate Bayesian parameter estimation under noisy measurements and outliers <i>(Tan, 2024, High-Dimension)</i>. These are the first works in the dynamic load modeling field to simultaneously provide both point estimates and estimation confidence for load parameters, thus quantifying uncertainties due to learning or measurement errors and enhancing the reliability of power system models.
  </p>

  <h4>Time-Varying Inertia Estimation for IBRs</h4>
  <p>
    Inertia is an index that quantifies a power system's capability to mitigate frequency deviations. Accurate inertia estimation is therefore crucial for assessing power system frequency stability. However, certain devices in the power system, particularly IBRs such as renewable energies, are equipped with time-adaptive virtual inertia control strategies to enhance frequency deviation mitigation. While these strategies are beneficial for maintaining frequency stability, they pose significant challenges for parameter estimation. The difficulty arises because this time-varying inertia can undergo rapid and substantial changes within a matter of seconds, making it challenging for existing methods to track accurately.
  </p>
  <p>
    My recent work <i>(Tan, 2023, Inertia; Tan, 2024, Adaptive)</i> bridged this gap by embedding the dynamic equations of inertia into a Bayesian Kalman filter framework. This approach enables real-time tracking of time-varying inertia and its associated uncertainties, even in scenarios where control switches occur <i>(Tan, 2024, Adaptive)</i>. Consequently, it provides a robust method for accurately quantifying inertia from IBRs.
  </p>

  <h4>Scalable Power System Risk Assessment</h4>
  <p>
    Due to the penetration of various uncertain sources, such as flexible loads, solar, and wind generation, power system operations exhibit stochastic behavior, making it challenging to maintain the system within its normal operating range. Additionally, the power system is subject to contingencies, such as scheduled branch maintenance or unexpected branch outages caused by extreme weather. These uncertainties propagate through the system, increasing the likelihood that operational metrics may exceed safe thresholds. This necessitates accurate quantification of the risks posed by these uncertainties to prevent power system failures.
  </p>
  <p>
    However, existing data-driven methods either cannot handle a large number of contingencies simultaneously, fail to address the high-dimensional inputs caused by numerous uncertain sources, or struggle with the high-dimensional outputs required to model power system operational metrics. To tackle these long-standing challenges, I have developed various surrogate models to address these issues effectively in two ways: 
  </p>
  <ol>
    <li>For pre-contingency load margin (static voltage stability) risk assessment, I leverage transfer learning to rapidly update the surrogate models, enabling efficient adaptation to changes in network topology due to scheduled branch maintenance <i>(Tan, 2023, Transferable)</i>. Regarding massive possible unexpected branch outages caused by extreme weather, I utilize topology embeddings to assess multiple contingencies simultaneously for voltage risk assessment <i>(Tan, 2024, Scalable)</i>.</li>
    <li>Once a contingency occurs, the surrogate model is extended to handle high-dimensional outputs, allowing for the immediate prediction of uncertainty-quantified post-contingency dynamic trajectories using a few real-time measurements <i>(Tan, 2024, Bayesian)</i>.</li>
  </ol>
  <p>
    These approaches significantly accelerate the speed of risk assessment, thereby enhancing the reliability and resilience of power system planning and operation.
  </p>


</div>
