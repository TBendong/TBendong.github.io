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


<div id="globe-container" style="height: 600px;"></div>
<script src="https://cdn.jsdelivr.net/npm/three@0.126.0/build/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/three-globe@2.24.6/dist/three-globe.min.js"></script>
<script>
  const globeElement = document.getElementById('globe-container');
  const Globe = new ThreeGlobe()
    .globeImageUrl('//unpkg.com/three-globe/example/img/earth-blue-marble.jpg')
    .pointsData([
      { lat: 40.7128, lng: -74.0060, size: 0.5, color: 'red' }, // New York
      { lat: 37.7749, lng: -122.4194, size: 0.4, color: 'red' }, // San Francisco
      // Add more points as needed
    ])
    .pointAltitude('size')
    .pointColor('color');
    
  // Set up scene
  const scene = new THREE.Scene();
  scene.add(Globe);
  scene.add(new THREE.AmbientLight(0xbbbbbb));
  scene.add(new THREE.DirectionalLight(0xffffff, 0.6));
  
  // Set up camera
  const camera = new THREE.PerspectiveCamera();
  camera.aspect = globeElement.clientWidth / globeElement.clientHeight;
  camera.updateProjectionMatrix();
  camera.position.z = 500;
  
  // Set up renderer
  const renderer = new THREE.WebGLRenderer({ antialias: true });
  renderer.setSize(globeElement.clientWidth, globeElement.clientHeight);
  globeElement.appendChild(renderer.domElement);
  
  // Add controls
  const controls = new THREE.OrbitControls(camera, renderer.domElement);
  controls.enableDamping = true;
  controls.dampingFactor = 0.25;
  controls.enableZoom = true;
  
  // Animation loop
  (function animate() {
    controls.update();
    renderer.render(scene, camera);
    requestAnimationFrame(animate);
  })();
</script>

<div style="color: white;">
    这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际上存在于页面中。您可以在这里放置任何您想要添加的隐藏内容。这种技术有时用于搜索引擎优化(SEO)或特殊用途，但请注意滥用这种方法可能被一些搜索引擎视为不良做法。这是一段白色字体的内容，在网页白色背景下不可见，但实际
