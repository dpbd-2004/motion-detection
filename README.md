**Motion Detection using OpenCV**

This project implements motion detection by comparing a static background frame with either a test image or video stream. It highlights areas of motion by drawing bounding boxes around moving objects. This can be used for basic surveillance or object detection tasks.

**🧠 Features**
Load and preprocess static images

Image subtraction to detect changes

Thresholding and dilation to highlight moving regions

Contour detection for bounding box drawing

Real-time motion detection from video files or webcam

**🛠️ Technologies Used**
Python

OpenCV

NumPy

Matplotlib

imutils

**📸 Image-based Detection**
The script compares two images (static.png and test.png) to find differences (i.e., motion or object change) and visualizes them.

Steps:
Load and resize images.

Convert them to grayscale.

Subtract the grayscale images.

Apply thresholding and dilation.

Find contours and draw bounding boxes.

Output:
Displays:

Original static image

Test image

Difference image

Thresholded binary image

Bounding boxes around detected changes

**🎥 Video-based Detection**
You can also use a video file (or webcam) to detect motion in real time.

Steps:
Read frames from a video or webcam.

Set the first frame as the static background.

For every next frame:

Convert to grayscale.

Subtract from the static background.

Apply thresholding and dilation.

Detect and draw bounding boxes around moving objects.
