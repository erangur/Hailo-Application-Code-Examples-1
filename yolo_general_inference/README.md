This is a general YOLO architecture Hailo inference example.  

The example takes one or more images, performs inference using the input HEF file and draws the detection boxes, claas type and confidence on the resized image.  
The example works with .jpg, .png and .bmp image files.   

The example was tested with the following Hailo Models Zoo networks:  
yolov3, yolov3_gluon, yolov4_leaky, yolov5m_wo_spp, yolox_l_leaky, yolov6n, yolov7

## Prerequesities:  
numpy  
zenlog  
PIL  
hailo_platform (installed from the HailoRT .whl)  
Hailo Model Zoo prerequesities (installed from the Hailo Model Zoo requierments.txt)  


## Running the example:
```./yolo_inference.py [--class-num NUM_OF_CLASSES] [--labels LABELS_PATH] HEF_PATH IMAGES_PATH YOLO_ARCH```
for example:  
```./yolo_inference.py --labels coco2017.txt yolov7.hef images yolo_v7```

For more information, run ```./yolo_inference.py --help```