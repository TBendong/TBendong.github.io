---
layout: page
title: Publications
permalink: /Publications/
nav: true
nav_order: 2
---

<!-- ==================== CSS ==================== -->
<style>
/* -------------------- Section Titles -------------------- */
.section-title {
    color: inherit; /* Use default text color */
    font-weight: normal; /* Remove bold */
    padding: 0; /* Remove background padding */
    border-radius: 0; /* Remove rounded corners */
    display: inline; /* Inline display */
    margin-bottom: 0.8em; /* Space below the title */
}

/* -------------------- Blue line under h4 -------------------- */
h4 {
    border-bottom: 3px solid #007BFF; /* Blue thick line */
    padding-bottom: 0.3em; /* Space between title and line */
    margin-bottom: 0.8em; /* Space below line before content */
    width: 100%; /* Line spans full width */
    display: block; /* Ensure block behavior */
}

/* -------------------- General publication list styling -------------------- */
.publications {
    list-style: none; /* Remove default bullets */
    padding-left: 0; /* Remove default padding */
    margin-bottom: 1.5em; /* Space below the list */
}

/* -------------------- Highlight author's name -------------------- */
.author-highlight {
    font-weight: normal; /* Remove bold */
    text-decoration: underline; /* Underline the name */
}

/* -------------------- Journal Papers Auto-numbering [J*] -------------------- */
.journal-publications {
    counter-reset: journal-counter;
}
.journal-publications li::before {
    counter-increment: journal-counter;
    content: "[J" counter(journal-counter) "] ";
    font-weight: bold;
}

/* -------------------- Conference Papers Auto-numbering [C*] -------------------- */
.conference-publications {
    counter-reset: conf-counter;
}
.conference-publications li::before {
    counter-increment: conf-counter;
    content: "[C" counter(conf-counter) "] ";
    font-weight: bold;
}

/* -------------------- Spacing between publication entries -------------------- */
.publications li {
    margin-bottom: 0.8em;
}

/* -------------------- Highlight Best Paper Award -------------------- */
.highlight {
    background-color: #FFFFE0; /* Light yellow background */
    color: #D32F2F; /* Red text */
    font-weight: bold;
    padding: 0.1em 0.3em; /* Padding around text */
    border-radius: 3px; /* Rounded corners */
}
</style>

<!-- ==================== HTML ==================== -->

For a complete list of publications, please refer to 
<a href="https://scholar.google.com/citations?user=FdEP8xgAAAAJ&hl=en">Google Scholar</a>.

<!-- -------------------- In-Progress Papers -------------------- -->
<h3 class="section-title">📝In-Progress Papers</h3>
<div class="journal-publications publications">
    <li>
        <span class="author-highlight">Bendong Tan</span>, Deepjyoti Deka and Junbo Zhao, 
        "Spatial-temporal global sensitivity analysis for probabilistic transient stability assessment", 
        <span class="journal-name">IEEE Transactions on Power Systems</span>, 2025. (Under revision)
    </li>
    <li>
        <span class="author-highlight">Bendong Tan</span>, Tong Su, Yu Weng, Ketian Ye, Parikshit Pareek, 
        Petr Vorobev, Hung Nguyen, Junbo Zhao and Deepjyoti Deka, 
        "<a href="https://arxiv.org/abs/2505.15950">Gaussian processes in power systems: Techniques, applications, and future Works</a>", 
        <span class="journal-name">Applied Energy</span>, 2025. (Under revision)
    </li>
    <li>
        <span class="author-highlight">Bendong Tan</span>, Ketian Ye, Junbo Zhao, Mingguo Hong, Slava Maslennikov and Xiaochuan Luo, 
        "Tail distribution-aware power system overloading risk assessment", 
        <span class="journal-name">Nature Communications</span>, 2025. (Under revision)
    </li>
    <li>
        <span class="author-highlight">Bendong Tan</span>, Junbo Zhao, 
        "Stochastic dynamic stability assessment with high penetration of uncertain sources: Uncertainty modeling, solutions and applications", 
        <span class="journal-name">Cyber-Physical Energy Systems</span>, 2025. (Under revision)
    </li>
    <li>
        Tong Su, Junbo Zhao, <span class="author-highlight">Bendong Tan</span>, Daniel Adrian Maldonado, Xiaodong Liu and Xiaochuan Luo, 
        "Analytic input convex neural networks enabled transient stability predictive control with wind generators", 
        <span class="journal-name">IEEE Transactions on Sustainable Energy</span>, 2025. (Under review)
    </li>
</div>

<!-- -------------------- Journal Papers -------------------- -->
<h3 class="section-title">📝Journal Papers</h3>
<div class="journal-publications publications">
    <li>
        <span class="author-highlight">Bendong Tan</span>, Junbo Zhao, Naiyuan Chiang and Nan Duan, 
        "<a href="https://ieeexplore.ieee.org/document/10892022">High-dimension Bayesian parameter estimation for WECC composite load model using realistic event measurements</a>", 
        <span class="journal-name">IEEE Transactions on Power Systems</span>, vol. 40, no. 5, pp. 3979-3992, Sept. 2025.
    </li>
    <!-- … more papers … -->
    <li>
        <span class="author-highlight">Bendong Tan</span>, Junbo Zhao, Marcos Netto, Venkat Krishnan, Vladimir Terzija and Yingchen Zhang, 
        "<a href="https://www.sciencedirect.com/science/article/pii/S0142061521006013">Power system inertia estimation: review of methods and the impacts of converter-interfaced generations</a>", 
        <span class="journal-name">International Journal of Electrical Power & Energy Systems</span>, Jan 2022. 
        <span class="highlight">Best Journal Paper Award</span>
    </li>
</div>

<!-- -------------------- Conference Papers -------------------- -->
<h3 class="section-title">📝Conference Papers</h3>
<div class="conference-publications publications">
    <li>
        Ketian Ye, Junbo Zhao, Mingguo Hong and Slava Maslennikov, <span class="author-highlight">Bendong Tan</span> and Xiaochuan Luo, 
        "<a href="https://ieeexplore.ieee.org/document/10688568">Power system overloading risk assessment considering topology and renewable uncertainties</a>", 
        in <span class="journal-name">2024 IEEE Power & Energy Society General Meeting (PESGM)</span>, pp. 1-5, 2024. 
        <span class="highlight">Best Paper Award</span>
    </li>
    <!-- … more papers … -->
</div>




