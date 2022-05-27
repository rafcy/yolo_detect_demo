# yolo_detect_demo
Basic video object detection using OpenCV and a tiny yolo network.

## Packages Requirements
- Numpy 
- OpenCV

## Installation
 ```
 pip install numpy opencv-python
 ```

## Run the detector 
 ```
 python3 Monitoring.py -i ./video_file.mp4 -s 
 or
  python3 Monitoring.py -i ./video_file.mp4 -s -c ./cfg/tiny-yolov4.cfg -w ./cfg/yolov4-tiny.weights -o video_det 
 ```
 Options:
 - -i : input file or stream eg. "video_file.mp4" or "192.1.20.4/live"
 - -s : display opencv window with detections/tracks
 - -w : yolo weights file path eg. ./cfg/tiny-yolov4.cfg
 - -c : yolo configs file path eg. ./cfg/yolov4-tiny.weights
 - -o : video output filename, saves the file to ./output folder

 Class names can be found in './cfg/coco.names'
