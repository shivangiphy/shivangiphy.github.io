---
layout: post
title: Image Transformations in C++
---

1. TOC
{:toc}

## Introduction

This project was a part of the final week assignment of an online course on Coursera on [Object-Oriented Data Structures in C++](https://www.coursera.org/learn/cs-fundamentals-1) taught by Prof. Ulmschneider from department of computer science at UIUC. It is such a well designed course for people from all background who are interested in understanding the essential components of a C++ code. The goal of this project was to transform the given image by changing the Hue, Saturation or Luminance of the pixel.

## Illinify
The first part of the assignment was to 'Illinify' the image, which is explained as follows. Hue itself refers to the color of the pixel. The color range is defined in between 0 and 360. The hue of each pixel should be set to either 'Illini orange' which has a hue of 11 or 'Illini Blue' which has a hue of 216, depending on which hue value the original hue of the pixel is closer to.
                                                                    
<img src="./assets/alma.png" width="400"> <img src="./assets/out-illinify.png" width="400">

## Spotlight
The second part of the project was to put a spotlight on the image. What this means is to decrease the luminance (or brightness of the pixels) with increasing radial distance around a central pixel. In this case the luminance was decreased by 0.5% per pixel unit in euclidean distance with a maximum of 80% decrease.
<img src="./assets/out-spotlight.png" width="400">        

## Watermarking
The third part of the project required putting a watermark on the image. This requires the use of an overlay image as a stencil, to find out the pixels in the Alma image that intersects with overlay image where the luminance is 1. The luminance of such pixels in original image were increased by 0.2 (with a maximum allowed value upto 1)                                                       
<img src="./assets/overlay.png" width="400">|<img src="./assets/out-watermark.png" width="400">
