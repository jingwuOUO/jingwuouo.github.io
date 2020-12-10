---
layout: page
title: Visual SLAM on Unmanned Aerial Vehicle
description: Extended Semi-direct Visual Odometry (SVO) by combining direct method and feature-based method in pose estimation and implemented Extended Kalman Filter (EKF) to improve the accuracy of pose estimation.
img: /assets/img/projects/vo.jpg
importance: 1
---

### Introduction

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded mx-auto d-block" src="{{ '/assets/img/projects/optical_flow.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Visualization of optical flow during initialization.
</div>

I extended a classic monocular visual odometry called semi-direct visual odometry. The initial idea to extend this algorithm is to make it more robust in indoor environments. It is sometime hard to achieve localization in indoor and textureless environment. So I optimized this algorithm based on this setting by utilizing direct method and added sensor like lidar information in an extended kalman filter implemented by myself. 


### Demo

<div class="row center">
        <iframe src="https://www.youtube.com/embed/hWU_P3U6o9g" width="800" height="480" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
</div>
<div class="caption">
    Extended SVO Demo
</div>