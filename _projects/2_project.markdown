---
layout: page
title: Shonan Rotation Averaging Global Optimality by Surfing SO(p)^n
description: A fast, simple, and elegant rotation averaging algorithm guaranteed to recover globally optimal solutions under mild assumptions on the measurement noise.
img: /assets/img/projects/shonan.jpg
github: https://github.com/borglab/gtsam
importance: 2
---

Shonan Rotation Averaging is a fast, simple, and elegant rotation averaging algorithm that is guaranteed to recover globally optimal solutions under mild assumptions on the measurement noise. Our method employs semidefinite relaxation in order to recover provably globally optimal solutions of the rotation averaging problem. In contrast to prior work, we show how to solve large-scale instances of these relaxations using manifold minimization on (only slightly) higher-dimensional rotation manifolds, re-using existing high-performance (but local) structure-from-motion pipelines. Our method thus preserves the speed and scalability of current SFM methods, while recovering globally optimal solutions. You can watch the ECCV 2020 spotlight video by <a href="https://dellaert.github.io/ShonanAveraging/">Frank Dellaert</a> and read our <a href="https://arxiv.org/abs/2008.02737">paper</a> to know more about Shonan.

### Experiment platform

In this project, I used <a href="https://www.comet.ml/site/">comet</a> platform to record all experiments I did with Shonan algorithm. It provides a self-hosted and could-based platform and makes it much easier for you or the team to track, compare, explain and optimize experiments.

<p>
After import Comet in python environment, I use it as the hook function in Pytorch so that it will automitically logs the data, parameter and anything you want and save the experiment on cloud. If the experiment view is set already, each time after the code stops running, you can already see the experiment results without any extra work. For Shonan algorithm, there are lots of parameters we want to study, thus this playform is extremely helpful to analyze the results. 
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded mx-auto d-block" src="{{ '/assets/img/shonan.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Comparison between Shonan, Block Descent and Levenberg-Marquardt algorithm
</div>

In the chart above, LM represents for Levenberg-Marquart method, BD represents block-coordinate descent method by <a href="https://openaccess.thecvf.com/content_cvpr_2018/papers/Eriksson_Rotation_Averaging_and_CVPR_2018_paper.pdf">Anders Eriksson</a>, SA, SK, SL represent Shonan with different parameters. All the methods are given the same randomly initialized estimation, Shonan is the fastest-converged method which also has the minimal error, and then BD method. LM is the slowest method.



