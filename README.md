# Autonomous_Driving_Car_Detection_YOLO
Autonomous Driving Car Detection Application using YOLO algorithm


## How I generated yolo.h5 from YAD2K repository
YAD2K repo: https://github.com/allanzelener/YAD2K

Creating env from environment.yml did not work for me. I created a new env locally and installed necessary packages from scratch. 

1. Clone the YAD2K repo
2. Download the yolo.weights file from here: http://pjreddie.com/media/files/yolo.weights
3. Download the v2 config from here: https://github.com/pjreddie/darknet/blob/master/cfg/yolov2.cfg
4. Create the YAD2K env locally. (conda env create -f environment.yml) 
If step 4 does not work, install packages manually using instructions in YAD2K repo
5. To generate the yolo.h5 file, run the command: `python yad2k.py yolo.cfg yolo.weights model_data/yolo.h5`

## Additional references and Notes

NOTES:

* YAD2K repository: https://github.com/allanzelener/YAD2K
* yolov2 official website: https://pjreddie.com/darknet/yolov2/
* yolov3 official website: https://pjreddie.com/darknet/yolo/
* darknet repository - will all configs: https://github.com/pjreddie/darknet/tree/master/cfg

opensourse threads related to this:

https://github.com/JudasDie/deeplearning.ai/issues/2
https://github.com/allanzelener/YAD2K/issues/57 