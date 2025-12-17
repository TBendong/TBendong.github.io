---
layout: page
permalink: /People/
title: People
nav: true
nav_order: 7
---
---
layout: page
title: Members
permalink: /Members/
nav: true
nav_order: 3
---

<style>
/* -------------------- Section Titles (Same as Publications) -------------------- */
h2 {
    padding-bottom: 0.4em;
    border-bottom: 3px solid #007BFF; /* Blue thick underline */
    margin-bottom: 1em;
    margin-top: 1.5em;
    display: block;
    font-size: 1.5rem;
    color: #000;
}

/* Remove top margin for the first section to align with title */
section:first-of-type h2 {
    margin-top: 0;
}

/* -------------------- Member Container Styling -------------------- */
.member-container {
    display: flex;
    margin-bottom: 2em;
    padding-bottom: 1em;
    border-bottom: 1px solid #eee;
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

<section>
    <h2>Postdoctoral Fellows</h2>

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

    </section>

<section>
    <h2>Ph.D. Students</h2>

    <div class="member-container">
        <img src="{{ '/assets/img/placeholder.jpg' | relative_url }}" alt="Student Name" class="member-photo">
        <div class="member-info">
            <p class="name">Student Name</p>
            <p class="title-date">Ph.D. Student, 09/2024–Present</p>
            <p class="edu">B.S., Electrical Engineering, [University Name], 2024</p>
            <div class="interests">
                <span class="interests-label">Research Interests:</span> 
                Power system state estimation and cybersecurity.
            </div>
        </div>
    </div>
</section>
