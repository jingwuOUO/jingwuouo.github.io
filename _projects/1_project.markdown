---
layout: page
title: Visual SLAM on Unmanned Aerial Vehicle in indoor environment
description: Extended Semi-direct Visual Odometry (SVO)
img: /assets/img/vo.jpg
importance: 1
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded mx-auto d-block" src="{{ '/assets/img/optical_flow.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Visualization of optical flow during initialization.
</div>

I extended a classic monocular visual odometry called semi-direct visual odometry. The initial idea to extend this algorithm is to make it more robust in indoor environments. It is sometime hard to achieve localization in indoor and textureless environment. So I optimized this algorithm based on this setting by utilizing direct method and added sensor like lidar information in an extended kalman filter implemented by myself. 


<div class="row center">
    <div style="text-aligh:center;">
        <iframe class="mx-auto d-block" width="800" height="480" src="http://www.youtube.com/embed/hWU_P3U6o9g?autoplay=1&loop=1&autopause=0"  frameborder="0"></iframe>
    </div>
</div>
<div class="caption">
    Demo
</div>