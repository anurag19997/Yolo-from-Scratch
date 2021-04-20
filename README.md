# Yolo-from-Scratch

Yolo is trained from scratch on Vooc 2007 dataset: http://host.robots.ox.ac.uk/pascal/VOC/voc2007/

## Sample annotation file:
![image](https://user-images.githubusercontent.com/18333608/115339285-11d79300-a1c2-11eb-92fd-36d31d60b6a5.png)

## Yolo architecture
![image](https://user-images.githubusercontent.com/18333608/115339369-3df31400-a1c2-11eb-8fcc-e7bd4b47f3f8.png)

Basic architecuture remains same only the major difference is that we need the last layer to predict a grid matrix of shape 7X7X30 where last dimension is composed of 20 classes and two bounding boxes with object probablities.

The two main function are Yolo_reshape and yolo_loss. First one is to create customized last layer and second one is for customized loss function.

Note: The training was taking a lot of time. Need to update again once the model training is complete
