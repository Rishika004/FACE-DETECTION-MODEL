# FACE-DETECTION-MODEL
Detecting faces in images and videos using haar casacades
What are the requirements for running the scripts ?

The following Python packages are required to run the scripts.
a) imutils : A series of convenience functions to make basic image processing functions such as translation, rotation, resizing, skeletonization, displaying Matplotlib images, sorting contours, detecting edges, and much more easier with OpenCV and both Python 2.7 and Python 3.
b) opencv2 : OpenCV (Open Source Computer Vision Library: http://opencv.org) is an open-source BSD-licensed library that includes several hundreds of computer vision algorithms.
c) ffmepg : FFmpeg is a free software project, the product of which is a vast software suite of libraries and programs for handling video, audio, and other multimedia files and streams. At its core is the FFmpeg program itself, designed for command-line-based processing of video and audio files, widely used for format transcoding, basic editing (trimming and concatenation), video scaling, video post-production effects, and standards compliance (SMPTE, ITU).
How is the performance of the script ? Why did we use Gray-Scale ?

The performance of the script is strictly based upon the Hardware of the system on which it is run and the quality of files provided. For the webcam, the performance dependency on hardware is not much of a factor but for videos it is, as FFmpeg is decoding the video frame by frame as the script is run.

We converted the input into Gray-Scale to simplify the job of the Haar Cascade algorithm. It would be able to work faster to determine edges and give out positive or negative results on images or frames.
