# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/write_image.png "Image Convert per Step"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I used Gaussian_blur function for reduce noise. After then i converted to Canny Edge as you see below, then i set interest rigion of image for sure detect for line. 4step is hough transform so i need to adjust several parameter(min_line_length, max_line_gap ..). the last step is image weighted that is compound both image which i converted and original image. finally i can see line detection on original image.

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what the path image environment like brightness, damaged image can be changed so that i have to change my parameter but it is not good for real driving.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to apply machine learning skill. i expect the machine learning argorithm can change my parameter that i set theirself. 
