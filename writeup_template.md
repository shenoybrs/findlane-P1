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

My pipeline consisted of 5 steps. First, I converted the images to grayscale, by taking a combination of yellow and white part of the image . combining them and getting the edges detected with the canny edge detection algorithm , which is again passed through the region of interest after which the pipeline finds lines through hough line transform.I have modified the hough_line function to get the lines detection corrected , to in turn get a better result.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


###2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when there is not lane lines at all , in india lot of roads dont have lane lines how will we manuer the vehicle with out lane lines , when lane lines are not seen .




###3. Suggest possible improvements to your pipeline

Need to learn more to understand how stanley went through terrain where there were no lane lines