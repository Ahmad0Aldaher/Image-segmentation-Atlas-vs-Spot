
# Image-segmentation-Atlas-vs-Spot
# Detection and segmentation for two of Boston Dynamics robots Atlas and Spot 
This project uses YOLOv8 and Mask RCNN model using Detectron2 to detect and do instance segmentation for two of Boston Dynamics robots Atlas and Spot in different images.

## Project steps:
### 1. **step1:** I collected 100 image for both robots (50 for each) 
### 2. **step2:** I annotated the images on Roboflow for segmentation. 
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/Roboflow.jpg)

### 3. **step3:** Train YOLOv8 model on this dataset 
#### confusion matrix
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/con_matrix.png)
#### traning  results
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/trainig.png)

#### Yolov8 results for Atlas and Spot
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/Atlas_yolo.jpg)
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/Spot_yolo.jpg)
### 4. **step4:** Train Mask RCNN model using Detectron2 on this dataset  on this dataset 
#### RCNN model using Detectron2 results for Atlas and Spot
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/Atlas_dec.png)
![alt text](https://github.com/Ahmad0Aldaher/Image-segmentation-Atlas-vs-Spot/blob/main/figs/Spot_dec.png)
### 5. **step5:** comparison between Yolov8 and Mask RCNN for this dataset:

|Weeks |YOLOv8                               | Mask RCNN
|---	|---	                            | ---
|   mAP	| 0.924   	        |  0.84710
|   Speed 	|15.9ms   	            | 109ms
|   Size	|27240806         	        |36229740
