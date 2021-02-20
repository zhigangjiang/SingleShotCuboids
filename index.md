---
layout: default
---

![Single-Shot Cuboids](./assets/images/graphical_abstract.png "Single-Shot Cuboids")

# Abstract

> It has been shown that global scene understanding tasks like layout estimation can benefit from wider field of views, and specifically spherical panoramas. While much progress has been made recently, all previous approaches rely on intermediate representations and postprocessing to produce Manhattan-aligned estimates. In this work we show how to estimate full room layouts in a single-shot, eliminating the need for postprocessing. Our work is the first to directly infer Manhattan-aligned outputs. To achieve this, our data-driven model exploits direct coordinate regression and is supervised end-to-end. As a result, we can explicitly add quasi-Manhattan constraints, which set the necessary conditions for a homography-based Manhattan alignment module. Finally, we introduce the geodesic heatmaps and loss and a boundary-aware center of mass calculation that facilitate higher quality keypoint estimation in the spherical domain.
Our models and code are publicly available at [https://github.com/VCL3D/SingleShotCuboids](https://github.com/VCL3D/SingleShotCuboids).

# Highlights

- **Single-shot**, end-to-end, spherical panorama-based cuboid layout corner estimation.

- **Spherical Center of Mass** for boundary-aware keypoint estimation on the sphere. [code](https://github.com/VCL3D/SingleShotCuboids/blob/master/ssc/quasi_manhattan_center_of_mass.py)

- **Explicit layout constraints** via direct keypoint estimation. [code](https://github.com/VCL3D/SingleShotCuboids/blob/master/ssc/quasi_manhattan_center_of_mass.py)

- **Geodesic Distance Loss** for boundary-aware keypoint estimation on the sphere. [code](https://github.com/VCL3D/SingleShotCuboids/blob/master/ssc/geodesic_distance.py)

- **Geodesic Gaussian** spherical heatmap reconstruction in the equirectangular domain. [code](https://github.com/VCL3D/SingleShotCuboids/blob/master/ssc/geodesic_gaussian.py)

- **Homography-based Cuboid Fitting** that ensures end-to-end full Manhattan alignment. [code](https://github.com/VCL3D/SingleShotCuboids/blob/master/ssc/cuboid_fitting.py)

# Paper

[![Paper pages](./assets/images/paper_image.jpg)](https://arxiv.org/pdf/2102.03939.pdf)

# Results

## Sun360

<img width=350 src="./assets/images/sun3601.jpg"><img src="./assets/images/sun3601.gif">

<img width=350 src="./assets/images/sun3602.jpg"><img src="./assets/images/sun3602.gif">

<img width=350 src="./assets/images/sun3603.jpg"><img src="./assets/images/sun3603.gif">

<img width=350 src="./assets/images/sun3604.jpg"><img src="./assets/images/sun3604.gif">

## Stanford2D3D

<img width=350 src="./assets/images/s2d3d1.jpg"><img src="./assets/images/s2d3d1.gif">

<img width=350 src="./assets/images/s2d3d2.jpg"><img src="./assets/images/s2d3d2.gif">

<img width=350 src="./assets/images/s2d3d3.jpg"><img src="./assets/images/s2d3d3.gif">

<img width=350 src="./assets/images/s2d3d4.jpg"><img src="./assets/images/s2d3d4.gif">

## Structured3D

<img width=350 src="./assets/images/s3d1.jpg"/><img src="./assets/images/s3d1.gif"/>

<img width=350 src="./assets/images/s3d2.jpg"/><img src="./assets/images/s3d2.gif"/>

<img width=350 src="./assets/images/s3d3.jpg"/><img src="./assets/images/s3d3.gif"/>

<img width=350 src="./assets/images/s3d4.jpg"/><img src="./assets/images/s3d4.gif"/>

## Kujiale

<img width=350 src="./assets/images/kuj1.jpg"/><img src="./assets/images/kuj1.gif"/>

<img width=350 src="./assets/images/kuj2.jpg"/><img src="./assets/images/kuj2.gif"/>

<img width=350 src="./assets/images/kuj3.jpg"/><img src="./assets/images/kuj3.gif"/>

<img width=350 src="./assets/images/kuj4.jpg"/><img src="./assets/images/kuj4.gif"/>