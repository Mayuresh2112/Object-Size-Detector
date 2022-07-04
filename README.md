 **Object-Size-Detector**


**Measure size of objects in an image using OpenCV **

The project offers a script to read an image and determine the size of additional objects in a scene using the measurements of a reference object. The scene's leftmost item must be the reference object. A box with the dimensions 2 cm by 2 cm is used as the reference object in the provided sample photos.


**Requirments**
- Python 3
- Pip
- OpenCV
- Numpy


**Algorithm**
1. Image pre-processing
  - Read a picture and make it black-and-white
  - Blur the image with a Gaussian Kernel to eliminate extraneous edges.
  - Use the Canny edge detector to detect edges
  - Close contours by performing morphological operations
2. Object Segmentation
  - Find contours
  - Remove small contours by calculating its area (threshold used here is 100)
  - Sort contours from left to right to find the reference object









 
