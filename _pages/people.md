---
layout: page
permalink: /People/
title: People
nav: true
nav_order: 7
---

<!-- ==================== CSS ==================== -->
<style>
/* -------------------- Section Titles -------------------- */
.section-title {
    padding-bottom: 0.4em; /* Reduce space between title text and underline */
    border-bottom: 3px solid #007BFF; /* Blue thick underline */
    margin-bottom: 0.4em; /* Reduce space between underline and content */
    display: block; 
}

/* -------------------- Blue line under h4 -------------------- */
h4 {
    border-bottom: 1.5px solid #007BFF; /* Blue thick underline */
    padding-bottom: 0.4em; /* Reduce space between title text and underline */
    margin-bottom: 0.4em; /* Reduce space between underline and content */
    width: 100%; 
    display: block; 
}

/* -------------------- Member Container Styling -------------------- */
.member-container {
    display: flex;
    margin-bottom: 2em;
    padding-bottom: 1em;
    align-items: flex-start;
}

.member-photo {
    width: 150px;
    height: 180px;
    object-fit: cover;
    background-color: #f8f9fa;
    margin-right: 25px;
    border-radius: 4px;
    border: 1px solid #ddd;
}

.member-info {
    flex: 1;
    color: #000; /* Force all text to black */
}

/* Name: Bold and slightly larger */
.name {
    font-size: 1.25rem;
    font-weight: bold;
    margin: 0 0 5px 0;
}

/* Title and Education: Normal weight */
.title-date, .edu {
    font-size: 1rem;
    font-weight: normal;
    margin: 2px 0;
}

/* Research Interests styling */
.interests {
    font-size: 1rem;
    margin-top: 10px;
    font-weight: normal;
}

/* Bold the specific label */
.interests-label {
    font-weight: bold;
}

/* -------------------- Responsive -------------------- */
@media (max-width: 600px) {
    .member-container { flex-direction: column; }
    .member-photo { margin-bottom: 15px; width: 130px; height: 160px; }
}
</style>


<h4>Postdoctoral Fellows</h4>
<div class="member-container">
    <img src="{{ '/assets/img/tao_xue.jpg' | relative_url }}" alt="Tao Xue" class="member-photo">
    <div class="member-info">
        <p class="name">Tao Xue</p>
        <p class="title-date">Postdoc, 12/2025–Present</p>
        <p class="edu">Ph.D., Electrical Engineering, The Hong Kong Polytechnic University, 2024</p>
        <div class="interests">
            <span class="interests-label">Research Interests:</span> 
            Inverter-penetrated power system stability analysis and control.
        </div>
    </div>
</div>

<h4>Ph.D. Students</h4>



    <h4>Ph.D. Students</h4>

   

