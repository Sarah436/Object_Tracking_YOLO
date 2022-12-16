# Object_Tracking_YOLO
****IMPORTANT LINKS****
YOLO weights: https://github.com/AlexeyAB/darknet/releases/download/darknet_yolo_v3_optimal/yolov4.weights


YOLO-4 for object Detection and tracking
In this project, we design a very simple tracking program using Open CV detection, to track the motion trajectory of multiple objects in a video.

Object Detection
YOLO-You Only Look Once
The input given is an image along with ground truth values of the bounding boxes.The entire input image is divided into a square grid, 
the grid cell containing the center of the object is responsible for detecting that object. 
Each grid cell will predict B bounding boxes and the confidence scores associated with those boxes. 
This score indicates the accuracy of the box and how confident the model is that the box contains the object. 
Confidence score is IoU of predicted values and the ground truth values of the bounding box.

Object Tracking
Find the point and assign the ID
Initialize an array to keep track of the previous points and then we need to calculate the distance between the points 
to make sure they all belong to the same object. The closer the points are, the greater the probability that we are tracking the same object.


![image](https://user-images.githubusercontent.com/78144204/208061034-ff7c44dd-4f88-4872-b609-285d17044e37.png)

