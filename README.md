# F1-Car-classification
This project aims to develop a deep learning image classification solution to identify teams during live races. The solution includes collecting and labeling car images, training and evaluating CNN-based neural networks, and deploying the highest accuracy model to provide real-time team and driver information to audiences.
A total 8 different classes of F1 car images were scraped from the web and labelled. These images were then used to train and test 3 pre-trained ImageNet models: RESNET-18, VGG-16 and MOBILENET_V2. 

## Results
![image](https://github.com/j0519740/F1-Car-classification/assets/99134168/7932cfd3-9a79-4129-a710-eb8d2e0305e2)
The MOBILENET_V2 pre-trained model gave the best accuracy of 96.7% when classifying using the test data.

![image](https://github.com/j0519740/F1-Car-classification/assets/99134168/017d9304-46be-418a-8bc1-ae35973c655b)
![image](https://github.com/j0519740/F1-Car-classification/assets/99134168/396519dd-c923-4587-b49f-6ac7a22b6e2e)


## Conclusion
In this project, we attempt Formula 1 cars image classification using different deep learning architectures. This can help new fans understand the teams and their origins and have a smoother experience while watching the race. We approach the problem using a labeled dataset containing 8 distinct car classes (teams) within Formula 1 racing. It is concluded that MobileNet_V2 with full fine-tuning leads to faster convergence and better prediction results compared to the other models. Significantly, the above conclusion is not final, as some other models could also be
tested. Better results could be achieved by using proper resources and overcoming limitations.

Nonetheless, the deduction obtained from this research is very substantial, and proper inferences can be obtained to decide upon the best model. In the future, traditional models and other deep convolutional neural networks can be implemented and
compared. In addition, other large-scale vehicle datasets (Boxcars, BRCars, etc.) can be utilized to evaluate the diversity of models for the fine-grained classification of vehicles. Another approach that can be explored is to use a bounding box object detector. Specifically, PASCAL VOC file format (an XML file format used by Image Net) can be used to annotate the images. After converting the PASCAL VOC primitive dataset to a TFRecord file (format optimized for tensorflow), an object detector model such as MobileNet SSD can be used to detect the cars and label them.
