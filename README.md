# yolo-heatmap

Sample code for creating a heat map using the results of object detection, based on [YOLOv5](https://github.com/ultralytics/yolov5).

# How to use

The usage is the same as the original Yolo5.
The added features and files from the original are as follows.
- features
    - Define multiple polygon regions and determine if the object detected by yolo is inside the polygon region.
    - Performs a projective transformation at a specified point.
        - image size is only 1920x1080.
- config file
    - basepoint_config.json
        - contains the coordinates of the points used to define the polygon.
    - map_config.json
        - defines how to use the polygon coordinates defined in basepoint_config.json to create a polygon.
