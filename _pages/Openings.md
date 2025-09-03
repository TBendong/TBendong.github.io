---
layout: page
permalink: /Openings/
title: Openings
description: Materials for courses you taught. Replace this text with your description.
nav: true
nav_order: 8
---

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dr. Bendong Tan — Open Positions / 开放岗位</title>
  <style>
    :root{
      --bg:#ffffff;
      --fg:#111827;
      --muted:#6b7280;
      --card:#f8fafc;
      --accent:#0ea5e9;
    }
    *{box-sizing:border-box}
    html,body{
      margin:0;padding:0;
      font-family: system-ui, -apple-system, "Segoe UI", Roboto, "PingFang SC", "Noto Sans SC", "Microsoft YaHei", "Helvetica", Arial, sans-serif;
      color:var(--fg);
      background:var(--bg);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    /* Top-left language toggle button */
    #langToggle {
      position:fixed;
      top:14px;
      left:14px;
      z-index:1000;
      background:#fff;
      border:1px solid #e5e7eb;
      padding:8px 12px;
      border-radius:999px;
      cursor:pointer;
      box-shadow:0 6px 18px rgba(2,6,23,0.08);
      font-weight:600;
      font-size:0.95rem;
      display:inline-flex;
      align-items:center;
      gap:8px;
    }
    #langToggle:focus{outline:3px solid rgba(14,165,233,0.18)}

    /* Layout */
    .wrap{
      max-width:980px;
      margin:86px auto 60px;
      padding:20px;
    }
    h1{font-size:1.7rem;margin:0 0 0.6rem;}
    h2{font-size:1.15rem;margin:1.3rem 0 0.45rem;border-bottom:1px solid #eef2f7;padding-bottom:0.25rem;}
    p{margin:0.5rem 0;line-height:1.7;}
    ul{margin:0.4rem 0 1rem 1.2rem}
    li{margin:0.25rem 0}
    .muted{color:var(--muted)}
    .card{
      background:var(--card);
      border:1px solid #eef2f7;
      border-radius:12px;
      padding:14px;
      margin-top:10px;
    }
    a{color:var(--accent);text-decoration:none}
    a:hover{text-decoration:underline}
    code{background:#f3f4f6;padding:0.08rem 0.35rem;border-radius:6px;font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono", "Noto Mono", monospace}

    /* language blocks */
    .lang { display:none; }
    .lang.active { display:block; }

    /* small screens */
    @media (max-width:520px){
      .wrap{margin:76px 14px 40px;padding:12px}
      h1{font-size:1.3rem}
      #langToggle{padding:7px 10px;font-size:0.88rem}
    }
  </style>
</head>
<body>
  <!-- Language toggle in top-left -->
  <button id="langToggle" aria-pressed="false" title="切换语言 / Toggle language">
    <span id="toggleLabel">中文</span>
    <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" aria-hidden>
      <path d="M12 5v14M5 12h14" stroke="#0ea5e9" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </button>

  <div class="wrap">
    <!-- ENGLISH CONTENT -->
    <article id="en" class="lang" lang="en">
      <h1>Open Positions — <span class="muted">Dr. Bendong Tan, PolyU EEE</span></h1>

      <section class="card">
        <p>
          Dr. Bendong Tan will join the Department of Electrical and Electronic Engineering (EEE) at
          The Hong Kong Polytechnic University (PolyU) as an Assistant Professor in Fall 2025.
          He is now recruiting fully funded Ph.D. students (Spring/Fall 2026), visiting students,
          and postdoctoral researchers, with research focusing on the modeling, stability assessment,
          and control of the next-generation power systems. Undergraduate and Master’s students are also
          welcome to join the group for research internships.
        </p>
      </section>

      <h2>About the Advisor</h2>
      <p>
        Before joining PolyU, Dr. Tan was a Postdoctoral Research Fellow at the University of Connecticut
        and a Visiting Scientist at the Massachusetts Institute of Technology (MIT), working with Dr. Junbo
        Zhao and Dr. Deepjyoti Deka. He received his Ph.D. degree in Electrical Engineering from the
        University of Connecticut in 2024, advised by Dr. Junbo Zhao. Prior to that, he earned an M.S. (2020)
        and a B.Eng. (2017) in Electrical Engineering from Wuhan University.
      </p>

      <p>
        Dr. Tan’s research focuses on the modeling, stability assessment, and control of next-generation
        power systems, with related work published in leading journals such as <em>IEEE Transactions on Power Systems</em>.
        He has received the 2023 Chinese Government Award for Outstanding Self-financed Students Abroad,
        the GE Fellowship for Excellence at the University of Connecticut, and the Ezra Postdoctoral Associate
        Fellowship at Cornell University. He is also a recipient of multiple awards, including Best Paper Awards
        at the IEEE PES General Meetings in 2021, 2022, and 2024, the Best Journal Paper Award from the
        <em>International Journal of Electrical Power & Energy Systems</em> in 2022, and the Outstanding Reviewer Award
        from <em>IEEE Transactions on Power Systems</em> (2021–2023).
      </p>

      <h2>Research Interests</h2>
      <p>The group focuses on modeling/monitoring, stability assessment, and control of stochastic inverter-penetrated power systems. Research interests include but are not limited to:</p>
      <ul>
        <li>Dynamic power system modeling, including dynamic load and inverter-based resources</li>
        <li>Inertia estimation and tracking in inverter-penetrated power systems</li>
        <li>Static and dynamic power system risk assessment with high penetration of inverter-based resources</li>
        <li>Stochastic power system decision-making and control</li>
        <li>Applications of artificial intelligence and machine learning in power system analysis and control</li>
      </ul>
      <p class="muted">If you are interested in other promising new directions, you are very welcome to bring them up, and we can explore and develop them together.</p>

      <h2>Application Requirements</h2>
      <ul>
        <li>Self-motivated individuals with strong research curiosity and passion for learning</li>
        <li>Background in electrical engineering, optimization and control, signal processing, statistics, artificial intelligence, or related fields</li>
        <li>Proficiency in programming (Python/Matlab), with experience in professional power system software such as PowerFactory/PSSE/PowerWorld</li>
        <li>Strong English writing and communication skills (PolyU requires an IELTS score of 6.5 or above, or a TOEFL score of 80 or above for admission).</li>
      </ul>

      <h2>Application Timeline and Procedure</h2>
      <p>
        <strong>Ph.D. Applicants:</strong> Enrollment in Spring or Fall 2026. The application deadline for Spring 2026 admission is <strong>September 30, 2025</strong>.
        Outstanding candidates are encouraged and supported to apply for the Hong Kong PhD Fellowship Scheme (HKPFS).
      </p>
      <p>
        <strong>Postdoctoral Applicants:</strong> Start date is flexible, with competitive compensation offered.
      </p>
      <p>
        Interested candidates should email their CV and transcripts to
        <a href="mailto:bendong.tan@uconn.edu">bendong.tan@uconn.edu</a> with the subject line:
        <code>{Postdoc|PhD Application}-{Your Name}</code> (e.g., <code>PhD Application-San Zhang</code>).
      </p>
    </article>

    <!-- CHINESE CONTENT -->
    <article id="zh" class="lang" lang="zh-Hans">
      <h1>开放岗位 — <span class="muted">谭本东博士，PolyU EEE</span></h1>

      <section class="card">
        <p>
          谭博士将于 2025 年秋季加入香港理工大学（PolyU）电机及电子工程系（EEE）担任助理教授。现招聘多名全奖博士研究生（2026 年春/秋入学）、访问学生及博士后，研究方向聚焦于新型电力系统的建模、稳定性评估与控制。也欢迎本科生或硕士生加入组内开展科研实习。
        </p>
      </section>

      <h2>导师简介</h2>
      <p>
        在加入 PolyU 之前，谭博士曾任康涅狄格大学（University of Connecticut）博士后研究员，并在麻省理工学院（MIT）担任访问学者，师从赵俊博教授与 Deepjyoti Deka 研究员。他于 2024 年在康涅狄格大学获得电气工程博士学位，导师为赵俊博教授。在此之前，他分别于 2020 年和 2017 年在武汉大学获得电气工程硕士与学士学位。
      </p>

      <p>
        谭博士的研究聚焦于新型电力系统的建模、稳定性评估与控制，相关成果在 IEEE Transactions on Power Systems 等电力领域顶级期刊发表。他曾获 2023 年国家优秀自费留学生奖学金、康涅狄格大学 GE Fellowship for Excellence，以及康奈尔大学 Ezra 博士后奖学金。此外，他还获得多项荣誉，包括 IEEE PES 年会最佳论文奖（2021、2022、2024）、International Journal of Electrical Power & Energy Systems 最佳期刊论文奖（2022）、以及 IEEE Transactions on Power Systems 杰出审稿人奖（2021–2023）。
      </p>

      <h2>研究兴趣</h2>
      <p>目前研究组的重点方向为电力电子设备主导的随机电力系统的建模/监测、稳定性评估与控制。具体研究兴趣包括但不限于：</p>
      <ul>
        <li>电力系统动态建模（包括动态负荷与基于逆变器的资源）</li>
        <li>高比例新能源电力系统的惯量估计与追踪</li>
        <li>高比例逆变器接入下的电力系统静态与动态风险评估</li>
        <li>随机电力系统的决策与控制</li>
        <li>人工智能与机器学习在电力系统分析与控制中的应用</li>
      </ul>
      <p class="muted">如果您对其他具有前景的新方向感兴趣，也非常欢迎提出，我们可以共同探讨并开展研究。</p>

      <h2>申请要求</h2>
      <ul>
        <li>具备持续的自我驱动力，富有钻研精神与学习热情</li>
        <li>拥有电气工程、优化与控制、信号处理、数理统计、人工智能或相关领域背景</li>
        <li>熟练掌握编程（Python/Matlab），并具有 PowerFactory/PSSE/PowerWorld 等电力系统专业软件使用经验</li>
        <li>具备良好的英文写作与交流能力（香港理工大学录取要求雅思 6.5 分或托福 80 分以上）。</li>
      </ul>

      <h2>申请时间与方式</h2>
      <p>
        <strong>博士生申请者：</strong>入学时间为 2026 年春季或秋季。2026 年春季入学申请截止日期为 <strong>2025 年 9 月 30 日</strong>。
        我们鼓励并支持优秀申请者申请香港博士研究生奖学金计划（HKPFS）。
      </p>
      <p>
        <strong>博士后申请者：</strong>岗位入职时间灵活，待遇从优。
      </p>
      <p>
        有意申请者请将简历（CV）和成绩单发送至
        <a href="mailto:bendong.tan@uconn.edu">bendong.tan@uconn.edu</a>，邮件标题请注明：
        <code>{Postdoc|PhD Application}-{Your Name}</code>（例如：<code>PhD Application-San Zhang</code>）。
      </p>
    </article>
  </div>

  <script>
    (function(){
      const btn = document.getElementById('langToggle');
      const label = document.getElementById('toggleLabel');
      const en = document.getElementById('en');
      const zh = document.getElementById('zh');

      // default language: use saved setting or browser / fallback to English
      const saved = localStorage.getItem('siteLang');
      const preferred = saved || (navigator.language && navigator.language.startsWith('zh')) ? 'zh' : 'en';

      function show(lang){
        if(lang === 'zh'){
          zh.classList.add('active');
          en.classList.remove('active');
          label.textContent = 'English';
          btn.setAttribute('aria-pressed','true');
          localStorage.setItem('siteLang','zh');
          document.documentElement.lang = 'zh-Hans';
        } else {
          en.classList.add('active');
          zh.classList.remove('active');
          label.textContent = '中文';
          btn.setAttribute('aria-pressed','false');
          localStorage.setItem('siteLang','en');
          document.documentElement.lang = 'en';
        }
      }

      // initialize
      show(preferred === 'zh' ? 'zh' : 'en');

      // toggle on click
      btn.addEventListener('click', function(){
        const current = localStorage.getItem('siteLang') || 'en';
        show(current === 'en' ? 'zh' : 'en');
      });

      // keyboard shortcut: press "L" to toggle (accessible)
      window.addEventListener('keydown', function(e){
        // ignore when typing in inputs (if added later)
        const tag = document.activeElement && document.activeElement.tagName;
        if(tag === 'INPUT' || tag === 'TEXTAREA' || document.activeElement.isContentEditable) return;
        if(e.key === 'l' || e.key === 'L'){
          btn.click();
        }
      });
    })();
  </script>
</body>
</html>

