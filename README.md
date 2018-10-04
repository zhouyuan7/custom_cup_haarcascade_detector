# custom_cup_haarcascade_detector

<p align="center">
<img src="https://github.com/zhouyuan7/custom_cup_haarcascade_detector/blob/master/readme_source/video3_gif.gif"/>
</p>

This a cup detector using haarcascade created by myself. It can detect an upside-down party cup. The haar-cascade cups.xml was trained using 1693 images of the cups (960 x 540 pixels), which capture by myself using kinectV2 RGB camera and manually set rectangular box. The window size is 20x25.

![alt text](https://github.com/zhouyuan7/custom_cup_haarcascade_detector/blob/master/readme_source/performance.jpeg)

## Introduction

The motivation of creating this detector is from my last baxter project. In last project, I loaded a state-of-the-art CNN model to detect the cup, however, I think that if the target is a particular cup, an individual detector would be better, and I choose the classical haar cascade method first.

<p align="center">
<img src="https://github.com/zhouyuan7/custom_cup_haarcascade_detector/blob/master/readme_source/video3_gif.gif"/>
</p>

The first tutorial I followed is this website [Creating your own Haar Cascade OpenCV Python Tutorial](https://pythonprogramming.net/haar-cascade-object-detection-python-opencv-tutorial/).  Although I have to admit that this is a good start, positive images set created by its ways cannot support a good performance. Too much positive false appears, and it turns out that for a target not unique like ‘company logo’, a good way is to manually capture positive inside the test environment from different view angles, illumination levels and distances and then box the target manually too. I have to say this is a time-consuming job, but the performance is good. 

