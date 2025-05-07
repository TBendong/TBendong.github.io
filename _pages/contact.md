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



<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Globe Visitor Map - My GitHub Website</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            font-family: 'Arial', sans-serif;
        }
        #globe-container {
            position: relative;
            width: 100%;
            height: 100vh;
            background-color: #000;
        }
        #info-panel {
            position: absolute;
            top: 20px;
            left: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 15px;
            border-radius: 5px;
            max-width: 300px;
        }
        h1 {
            margin-top: 0;
            font-size: 1.5em;
        }
        #visitor-count {
            font-size: 1.2em;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div id="globe-container"></div>
    
    <div id="info-panel">
        <h1>Visitor Globe</h1>
        <div id="visitor-count">Total Visitors: <span id="count">Loading...</span></div>
        <div id="latest-visitor">Latest Visitor: <span id="location">Loading...</span></div>
    </div>

    <!-- Load Three.js library -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    
    <script>
        // Globe visualization with Three.js
        let scene, camera, renderer, globe;
        let visitorPoints = [];
        let totalVisitors = 0;
        
        // Sample visitor data (in production, this would come from your backend or analytics API)
        // Format: [latitude, longitude, magnitude (size of point)]
        const sampleVisitors = [
            [40.7128, -74.0060, 0.5], // New York
            [51.5074, -0.1278, 0.8],  // London
            [35.6762, 139.6503, 0.6], // Tokyo
            [22.3193, 114.1694, 0.7], // Hong Kong
            [1.3521, 103.8198, 0.4],  // Singapore
            [-33.8688, 151.2093, 0.5], // Sydney
            [55.7558, 37.6173, 0.6]   // Moscow
        ];
        
        function init() {
            // Create scene
            scene = new THREE.Scene();
            
            // Create camera
            camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
            camera.position.z = 1.8;
            
            // Create renderer
            renderer = new THREE.WebGLRenderer({ antialias: true });
            renderer.setSize(window.innerWidth, window.innerHeight);
            renderer.setPixelRatio(window.devicePixelRatio);
            document.getElementById('globe-container').appendChild(renderer.domElement);
            
            // Create Earth globe
            const earthGeometry = new THREE.SphereGeometry(1, 64, 64);
            const earthTexture = new THREE.TextureLoader().load('https://cdn.jsdelivr.net/npm/three-globe/example/img/earth-blue-marble.jpg');
            const earthMaterial = new THREE.MeshBasicMaterial({ map: earthTexture });
            globe = new THREE.Mesh(earthGeometry, earthMaterial);
            scene.add(globe);
            
            // Add ambient light
            const ambientLight = new THREE.AmbientLight(0xffffff, 0.5);
            scene.add(ambientLight);
            
            // Add point light (sun)
            const pointLight = new THREE.PointLight(0xffffff, 1);
            pointLight.position.set(5, 3, 5);
            scene.add(pointLight);
            
            // Add visitor markers
            addVisitorMarkers();
            
            // Update visitor count
            totalVisitors = sampleVisitors.length;
            document.getElementById('count').textContent = totalVisitors;
            document.getElementById('location').textContent = 'Hong Kong, China';
            
            // Handle window resize
            window.addEventListener('resize', onWindowResize);
            
            // Start animation loop
            animate();
            
            // Simulate new visitor every 5 seconds
            setInterval(addNewVisitor, 5000);
        }
        
        function addVisitorMarkers() {
            sampleVisitors.forEach(visitor => {
                addMarkerAtLocation(visitor[0], visitor[1], visitor[2]);
            });
        }
        
        function addMarkerAtLocation(lat, lng, magnitude) {
            // Convert lat/lng to 3D coordinates
            const phi = (90 - lat) * Math.PI / 180;
            const theta = (lng + 180) * Math.PI / 180;
            
            const x = -Math.sin(phi) * Math.cos(theta) * 1.02;
            const y = Math.cos(phi) * 1.02;
            const z = Math.sin(phi) * Math.sin(theta) * 1.02;
            
            // Create marker
            const markerGeometry = new THREE.SphereGeometry(0.02 * magnitude, 16, 16);
            const markerMaterial = new THREE.MeshBasicMaterial({ color: 0xff0000 });
            const marker = new THREE.Mesh(markerGeometry, markerMaterial);
            
            marker.position.set(x, y, z);
            scene.add(marker);
            visitorPoints.push(marker);
            
            // Create glow/pulse effect
            const glowGeometry = new THREE.SphereGeometry(0.03 * magnitude, 16, 16);
            const glowMaterial = new THREE.MeshBasicMaterial({ 
                color: 0xff8800, 
                transparent: true,
                opacity: 0.7
            });
            const glow = new THREE.Mesh(glowGeometry, glowMaterial);
            glow.position.set(x, y, z);
            scene.add(glow);
            
            // Animate the glow
            let scale = 1;
            let growing = true;
            setInterval(() => {
                if (growing) {
                    scale += 0.01;
                    if (scale >= 1.5) growing = false;
                } else {
                    scale -= 0.01;
                    if (scale <= 1) growing = true;
                }
                glow.scale.set(scale, scale, scale);
            }, 50);
        }
        
        function addNewVisitor() {
            // Generate random latitude and longitude
            const lat = Math.random() * 180 - 90;
            const lng = Math.random() * 360 - 180;
            const magnitude = Math.random() * 0.5 + 0.3;
            
            // Add marker
            addMarkerAtLocation(lat, lng, magnitude);
            
            // Update counter
            totalVisitors++;
            document.getElementById('count').textContent = totalVisitors;
            
            // Update latest visitor (in reality, this would use IP geolocation)
            fetch('https://ipapi.co/json/')
                .then(response => response.json())
                .then(data => {
                    document.getElementById('location').textContent = `${data.city}, ${data.country_name}`;
                })
                .catch(error => {
                    // Random location if API fails
                    const cities = ['Tokyo, Japan', 'Paris, France', 'Berlin, Germany', 'San Francisco, USA', 'Melbourne, Australia'];
                    const randomCity = cities[Math.floor(Math.random() * cities.length)];
                    document.getElementById('location').textContent = randomCity;
                });
        }
        
        function animate() {
            requestAnimationFrame(animate);
            
            // Rotate globe
            globe.rotation.y += 0.001;
            
            renderer.render(scene, camera);
        }
        
        function onWindowResize() {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        }
        
        // Initialize the globe
        init();
    </script>
</body>
</html>

<div style="color: white;">
    这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际
