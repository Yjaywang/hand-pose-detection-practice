# Hand pose detection 

This is my first object detection practice project, the final model will be converted to TensorFlow.js model and used by my video conferece website project ([Meeting](https://github.com/Yjaywang/Meeting)).

In this practice, some goals need to be achieved for my end application:
* Light-weighted
* Low computation consumption
* Low latency
* Acceptable accuracy

Based on these requirements, I choose MobileNet-SSD to train the model.

## MobileNet Single Shot Detection (MobileNet-SSD)
![](https://i.imgur.com/L9FQt3T.png)

## Training data preparation
### Image Class
* 9 classes

![](https://i.imgur.com/s32Cgie.png)
### Labeling

* use [LabelImg](https://github.com/heartexlabs/labelImg)

### Train/test ratio
* train: 90%; test: 10%

## Training result
![](https://i.imgur.com/rotWyse.png)



## Reference
* https://www.researchgate.net/publication/343223517_A_Mobile-Based_Framework_for_Detecting_Objects_Using_SSD-MobileNet_in_Indoor_Environment
* https://www.analyticsvidhya.com/blog/2022/09/object-detection-using-yolo-and-mobilenet-ssd/
* https://www.researchgate.net/figure/MobileNet-SSD-AF-architecture-we-use-MobileNet-as-the-feature-extractor-network-and-SSD_fig7_324584455
* https://www.youtube.com/watch?v=pDXdlXlaCco
* https://www.youtube.com/watch?v=ZTSRZt04JkY
* https://www.tensorflow.org/tutorials/images/transfer_learning