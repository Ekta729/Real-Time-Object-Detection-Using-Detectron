# Real-Time-Object-Detection-using-DETECTRON
<img width="430" alt="detectron2-logo" src="https://user-images.githubusercontent.com/55136275/130313033-064eb833-151a-46a8-af7b-c229040355b5.png">


**Detectron2** is Facebook AI Research's next generation library that provides state-of-the-art detection and segmentation algorithms. It is the successor of Detectron and maskrcnn-benchmark. It supports a number of computer vision research projects and production applications in Facebook.

https://user-images.githubusercontent.com/55136275/130313574-78111d76-b34c-4927-b411-db899aeed3ba.mp4

## Getting Started

### >>PROBLEM STATEMENT

**Dataset information:** 

Dataset link : https://drive.google.com/file/d/1NKLt3_lPDIxGyiQ_m0QXTVygeC4V7TK7/view?usp=sharing

There are two folders within the dataset

1. test_videos - Contain videos on which your model needs to be tested

2. train - This dataset contains “Images” folder - which has images containing bat and ball. There is a CSV file “bat_ball.csv” which contains following columns “class (label)” “X axis (Top Left X-coordinate of the image )” “Y Axis (Top Left Y-coordinate of the image)” “width(width of the class (bat or ball))” , “height (height of the class (bat or ball))” , “name (Name of the image)”, “image_width”, “image_height”

 We have to detect and localize ball and bat In a given frame. 

Information about the training dataset:

There is a folder named “images” which has all the images containing bat and ball. These images are already annotated and the annotation file is a CSV file named “bat_ball” at the same level as the “images folder”

The columns of the CSV file are described above

Once we train the models test them on the videos given in the “test_videos” folder.

Detect bat and ball in each frame of test videos and draw a rectangular bounding box around bat and ball in each frame.


### >> APPROACH

We approached the problem statement  in two phases:
1) Any algorithm is of no use if data is not good. So very first we converted given dataset in one of the standard object detection dataset formats like COCO. Doing this made my dataset compatible with lot of open source algorithms and frameworks. We chose **COCO** format as it involved much more complexities in implementation.
2) We converted existing data set into coco format (ref: COCO Json Data.ipynb notebook)
3) 
