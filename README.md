# Autonomous Driving Car Detection Application using YOLO algorithm (Tensorflow/Keras)

<center>
<video width="400" height="200" src="nb_images/pred_video_compressed2.mp4" type="video/mp4" controls>
</video>
</center>

YOLO (You Look Only Once) is the state of the art fast and accurate object dection algorithm, which is used here for the Autonomous driving car detection application. YOLO uses bounding boxes and class probabilities to detect  objects. The Deep CNN is trained using 608 x 608 x 3 images to identify 80 classes and uses 5 Anchor boxes.

This project was completed for "Convolutional Neural Networks" course by Coursera and deeplearning.ai (part of Deep Learning Specialization taught by Prof. Andrew Ng)

# How does YOLO work? 

* It uses Depp CNN that takes an input image of mX608X608X3 and returns 19x19x5x85 volume

<img src="nb_images/architecture.png" style="width:700px;height:400;">
<caption><center> <u> **Figure 2** </u>: **Encoding architecture for YOLO**<br> </center></caption>

test 

![architecture](nb_images/architecture.png)

## How I generated yolo.h5 from YAD2K repository
YAD2K repo: https://github.com/allanzelener/YAD2K

Creating env from environment.yml did not work for me. I created a new env locally and installed necessary packages from scratch. 

1. Clone the YAD2K repo
2. Download the yolo.weights file from here: http://pjreddie.com/media/files/yolo.weights
3. Download the v2 config from here: https://github.com/pjreddie/darknet/blob/master/cfg/yolov2.cfg
4. Create the YAD2K env locally. (conda env create -f environment.yml) 
If step 4 does not work, install packages manually using instructions in YAD2K repo
5. To generate the yolo.h5 file, run the command: `python yad2k.py yolo.cfg yolo.weights model_data/yolo.h5`

## References 



## NOTES:

* YAD2K repository: https://github.com/allanzelener/YAD2K
* yolov2 official website: https://pjreddie.com/darknet/yolov2/
* yolov3 official website: https://pjreddie.com/darknet/yolo/
* darknet repository - will all configs: https://github.com/pjreddie/darknet/tree/master/cfg

opensource threads related to this:
* https://github.com/JudasDie/deeplearning.ai/issues/2
* https://github.com/allanzelener/YAD2K/issues/57 