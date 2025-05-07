---
layout: archive
permalink: /contact/
author_profile: true
---

{% include base_path %}


{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}

Contact information is below, including email and various web services.  This is to make it easy for people to find me when they search for things and get wrong pages on my site.  Here are some other places on the Internet where I reside.
* E-mail: bendong.tan@uconn.edu
* Chinese Quora: [This is the website where I answer interesting questions](https://www.zhihu.com/people/tan-ben-dong/activities)
* Chinese Blog: [This is the website where I record my thoughts about life and learning in Chinese](https://tanbendong.github.io/)
* Google Scholar: [This is the website where I record my papers](https://scholar.google.com/citations?user=FdEP8xgAAAAJ&hl=en)
* LinkedIn: [This is the website where I follow the academic information](https://www.linkedin.com/in/bendong-tan-453046182/)
* Researchgate: [This is the website where I share my research](https://www.researchgate.net/profile/Bendong_Tan)

# 🗺️ Visitor Map

**<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My GitHub Website</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            max-width: 800px;
            margin: 0 auto;
        }
        header {
            text-align: center;
            margin-bottom: 30px;
        }
        .visitor-stats {
            background-color: #f5f5f5;
            padding: 15px;
            border-radius: 5px;
            margin-top: 20px;
        }
        footer {
            margin-top: 30px;
            text-align: center;
            font-size: 0.9em;
            color: #666;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
    </header>
    
    <main>
        <p>This is the main content of my website...</p>
        
        <div class="visitor-stats">
            <h3>Visitor Statistics</h3>
            <!-- Flag Counter for visitor countries and count -->
            <div>
                <a href="https://flagcounter.com/">
                    <img src="https://s11.flagcounter.com/count2/XXXX/bg_FFFFFF/txt_000000/border_CCCCCC/columns_2/maxflags_10/viewers_0/labels_1/pageviews_1/flags_0/percent_0/" alt="Flag Counter">
                </a>
            </div>
            
            <!-- Simple visitor counter -->
            <div id="visitor-count">
                <p>Visits: <span id="count">Loading...</span></p>
            </div>
            
            <!-- Visitor location information -->
            <div id="visitor-location">
                <p>Your location: <span id="location">Loading...</span></p>
            </div>
        </div>
    </main>
    
    <footer>
        <p>© 2025 My GitHub Website</p>
    </footer>

    <!-- Script for visitor location and counting -->
    <script>
        // Simple visitor counter (using localStorage for demonstration)
        // In a real application, you should use a backend service or third-party API
        window.addEventListener('DOMContentLoaded', function() {
            // Visitor counter
            let count = localStorage.getItem('visitorCount') || 0;
            count = parseInt(count) + 1;
            localStorage.setItem('visitorCount', count);
            document.getElementById('count').textContent = count;
            
            // Get visitor location information
            fetch('https://ipapi.co/json/')
                .then(response => response.json())
                .then(data => {
                    const location = `${data.city}, ${data.country_name}`;
                    document.getElementById('location').textContent = location;
                })
                .catch(error => {
                    document.getElementById('location').textContent = 'Unable to retrieve location';
                    console.error('Failed to get location information:', error);
                });
        });
    </script>
</body>
</html>**


<div style="color: white;">
    这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际
