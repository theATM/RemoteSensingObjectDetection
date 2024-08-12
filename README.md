![BannerAirDetection](https://github.com/theATM/AirDetection/assets/48883111/17015a60-20a0-45c6-abe4-7c7b17a89ee9)

# AirDetection

The Repository for the Master's Thesis in the Remote Sensing Object Detection. The AirDetection Project explores the fascinating field of object detection in satellite imagery.

- The project's main objective is to compare the effectiveness of modern neural network architectures on <a href="https://github.com/Dr-Zhuang/geospatial-object-detection">RSD-GOD</a>  remote sensing dataset
- Propose improvements that could strengthen the models' ability to correctly detect various objects of interest
- Analyse the challanges with the top-down object detection


Multiple different architectures (shown in the structure chart) are used to detect images on the <a href="https://github.com/Dr-Zhuang/geospatial-object-detection">RSD-GOD</a> dataset.


## Project Structure Chart

![repo_structv2](https://github.com/theATM/AirDetection/assets/48883111/c5d58974-52b9-44a5-b703-73c3816a8a1b)


## Gdańsk Bay Detections

Object Detected using a large YOLOv8 model. Images taken from Google Maps.


| Gdańsk Lech Wałęsa International Airport | „Błyskawica” Polish Museum Ship   | 
| :---:   | :---: | 
| ![airport_3_b](https://github.com/theATM/AirDetection/assets/48883111/fc29eefb-1b91-4a99-95f6-66f1be689579)  |  ![warship_1_b](https://github.com/theATM/AirDetection/assets/48883111/7ad746d7-29ca-4f7c-8335-fd92990f52c9) | 


## YOLOv8 COCO Results on RSD-GOD dataset


### Validation scores

<pre>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.675 <br/>
 Average Precision  (AP) @[ IoU=0.50      | area=   all | maxDets=100 ] = 0.972 <br/>
 Average Precision  (AP) @[ IoU=0.75      | area=   all | maxDets=100 ] = 0.794 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.359 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.602 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.722 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=  1 ] = 0.403 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets= 10 ] = 0.726 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.739 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.467 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.684 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.784 <br/>
</pre>
  
 ### Test scores
  
<pre> 
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.589 <br/>
 Average Precision  (AP) @[ IoU=0.50      | area=   all | maxDets=100 ] = 0.932 <br/>
 Average Precision  (AP) @[ IoU=0.75      | area=   all | maxDets=100 ] = 0.652 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.135 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.418 <br/>
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.640 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=  1 ] = 0.364 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets= 10 ] = 0.671 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.681 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.228 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.587 <br/>
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.728 <br/>
</pre>

### Model Zoo


| YOLOv8  | Yolov5 | Yolov3 | SSD | DETR | Faster R-CNN | RTMDet
| ------------- | ---- | ---- |  ---- | ---- | ---- | ---- |
| [Y28](https://drive.google.com/file/d/1ai4D---5uvQeoz2RzkisL5hlNCXDshSg/view?usp=sharing) [Y25](https://drive.google.com/file/d/1I4L0x9Hoo-8R9oGka45giOWHbq33AcEG/view?usp=sharing) <br> [Y9](https://drive.google.com/file/d/1bk0tnVXpOP7wc_9Pp2L16MuhuW1vxDG2/view?usp=sharing) [Y7](https://drive.google.com/file/d/1g9L0rVkM9B2IeH6rYLcdfWcCwUKSuw_5/view?usp=sharing) <br> [L6](https://drive.google.com/file/d/1PMvREHjc_NFcAvgTdImDsp0ooyG631kQ/view?usp=sharing) [L8](https://drive.google.com/file/d/1eKePU7NxfheCx19Yjb_ijPqgk5n-EY7G/view?usp=sharing)  | [F29](https://drive.google.com/file/d/1FSccHMgBY9TrLokY8GxcW_k-VhXIzbIr/view?usp=sharing) | [O2](https://drive.google.com/file/d/1XbCKVi2A16a5E_rcWITa9IeLb5F1SGnt/view?usp=sharing) | [S23](https://drive.google.com/file/d/1sAsoLrs2eh66HGHyVldOu1I2l1yBQCyV/view?usp=sharing) <br> [S21](https://drive.google.com/file/d/1TVtVp_qJ0GdEV0s-6AZsdF_A8kXXnT4U/view?usp=sharing) | [D5](https://drive.google.com/file/d/1G84ybh_JvDLgcF-1OWM2ge63e3fCoESb/view?usp=sharing) <br> [D2](https://drive.google.com/file/d/1nt5jr17RP7hYRSsYByOoxuIyvWosARdf/view?usp=sharing) | [R4](https://drive.google.com/file/d/10CBfGHrepi_bTf17anL6ZzJqo2L60I3P/view?usp=sharing) | [T3](https://drive.google.com/file/d/1HYP-lMsq8xlZ6qG7_MmAQi5Gc33HMU8x/view?usp=sharing) |

