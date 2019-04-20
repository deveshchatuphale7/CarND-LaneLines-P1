# **Finding Lane Lines on the Road** 

### 1. Pipeline-

In a nutshell I followed following steps
1. Converted image to greyscale
2. Applied Gaussian blur with kernel value 7
3. Applied edge detection function on blurred image to detect lane marks on the road
4. Removed/ Cropped down unwanted part of the image 
5. Applied HoughLinesP function to get coordinates of detected lines
6. Extended line coordinates by finding out slope 
7. Drawing lane lines on original image by passing extended line corordinates


### 2. Potential shortcomings with current pipeline

Current pipeline may fail to identify lines if colour of the road changes or if the road is 
slightly curved

### 3.Possible improvements to  pipeline

In my opinion, pipeline can be improved to detect slope of  stripped lines for curvature
or by detecting slope of lines at periodic interavals
