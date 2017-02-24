#**Finding Lane Lines on the Road** 

##Writeup Template

###You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

###1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I applied  Gaussian blur to image. Then I used Canny edges detection. After that, I croped the region of interest.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function. Then finally

blending original image and image with lines.


###2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the video is rolling and the pipeline cannot sustain the lines accurately. 

Another shortcoming could be frame dropping. 


###3. Suggest possible improvements to your pipeline

A possible improvement would be to have different processing of white and yellow lines

Another potential improvement could be to try a kalman filter. 
