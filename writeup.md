
### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

In a nutshell I followed following steps
1. Converted image to greyscale
2. Applied Gaussian blur with kernel value 7
3. Applied edge detection function on blurred image to detect lane marks on the road
4. Removed/ Cropped down unwanted part of the image 
5. Applied HoughLinesP function to get coordinates of detected lines
6. Extended line coordinates by finding out slope 
7. Drawing lane lines on original image by passing extended line corordinates


### 2. Identify potential shortcomings with your current pipeline

Current pipeline may fail to identify lines if colour of the road changes or if the road is 
slightly curved

### 3. Suggest possible improvements to your pipeline

In my opinion, pipeline can be improved to detect slope of  stripped lines for curvature
or by detecting slope of lines at periodic interavals
