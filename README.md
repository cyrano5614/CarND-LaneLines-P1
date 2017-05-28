# P1 - Finding Lane Lines on the Road
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

## Overview

In this project, we will explore and develop a pipeline to find a lane line on the road in a given image and video.  The goals / steps of this project are the following:

* Develop pipeline to find lane lines on the road.
* Apply the pipeline to images and videos provided.

---
[//]: # (Image References)
[image1]: ./test_images_output/solidwhite.jpg
[image2]: ./test_images_output/solidyellow.jpg
[image3]: ./test_images_output/solidWhiteCurve_process.jpg
---

## Video Results

![solidWhiteRight.mp4 Output][image1]
(https://www.youtube.com/watch?v=_60zb0sT8uo)

![solidYellowLeft.mp4 Output][image2]
(https://www.youtube.com/watch?v=WHLfEyUmsfU)

## Reflection

The pipeline consists of 6 steps.

* Grayscale Conversion
* Apply Gaussian Blur
* Detect Canny Edges
* Mask Region of Interest
* Apply Hough Transform and draw lane lines
* Combine original image and line image

Each step is defined in P1.ipynb in 'Helper Functions' section.  Below is an example of pipeline steps.

![alt text][image3]

The pipeline is not robust enough to handle various lighting conditions.  The robustness could be improved using various color masking technique to further distinguish the lane lines.
