---
title: 'Detection Rate in Image Recognition'
date: 2017-10-11
permalink: /posts/2017/10/detection-rate-in-image-recognition/
tags:
  - Image Recognition
  - Detection
  - CV
---

Image recognition is very important technology and image recognition has an endless scope in every field. Image recognition techniques have been applied in different applications such as finding pedestrians on the streets, detecting moving vehicles, counting the people in public places. Application of image recognition in the medical field has also been proven significant.

Image recognition technology is usually evaluated with the detection rate which indicates how well the objects are detected. The detection rate is measured based on the test where the number of successfully detected images are counted among the images used as input for the detection algorithm.

For example, let's say we have 100 images with faces of people. Each image may have either only one face or many faces. So let's say that the total number of faces included in 100 test images is 200. If the number of faces detected by the face detection algorithm is 100, the detection rate of this algorithm 50%.  Generally speaking, the detection rate of 50 percent doesn't sound appealing but it is not always the case. For example, let's say we have a CCTV camera that detects the faces of the people passing by. Let's assume that this camera takes footage at 10 frames/second and use it for face detection. So whenever a face appears in front of the camera, the same algorithm with 50% detection rate will detect it with 99% chance of detecting it.

Although detection rate is a reasonable measure for evaluating the performance on still images, for evaluating the performance of the real-time video, detection rate per unit time is more appropriate metric.
