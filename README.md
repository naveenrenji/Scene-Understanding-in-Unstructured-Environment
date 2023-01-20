## Solving-Scene-Understanding-for-Autonomous-Navigation-in-Unstructured-Environments
FINAL YEAR PROJECT 2021

### INTRODUCTION
Autonomous vehicles are the next big thing in the automobile industry and they are expected to revolutionize the future of transportation. Understanding the scenario in which the autonomous vehicle will operate is critical for its competent functioning. Deep Learning has played a massive role in the progress that has been made till date. Semantic Segmentation, the process of annotating every pixel of an image with an object class, is one crucial part of this scene comprehension using Deep Learning. It is especially useful in Autonomous Driving Research as it requires comprehension of drivable and non-drivable areas, roadside objects and the like. In this paper we perform semantic segmentation on Indian Driving Dataset which has been recently compiled on the urban and rural roads of Bengaluru and Hyderabad. This dataset is more challenging compared to other datasets like Cityscapes, since it is based on unstructured driving environments. It has a four level hierarchy and in this paper we perform segmentation on the first level. Five different models have been trained and their performance has been compared using the Mean Intersection over Union. These are UNET, UNET+RESNET50, DeepLabsV3, PSPNet and SegNet. The highest MIOU of 0.6496 has been achieved. The paper discusses the dataset, exploratory data analysis, preparation, implementation of the five models and studies the performance and compares the results achieved in the process.

### PROBLEM STATEMENT
Semantic Segmentation: The segmentation challenge involves pixel level predictions for all the 26 classes at level 3 of the label hierarchy.

This project will be using the mean Intersection over Union metric. For each class (except 26), the  True positives (TP), False Negatives (FN) and False positives (FP) are computed and all the prediction maps and ground truths will be resized to 720p using nearest neighbour algorithm over the entire test split of the dataset. Intersection over Union (IoU) will be computed for each class by the formula TP/(TP+FN+FP) and the mean value is taken as the metric (commonly known as mIoU) for the segmentation challenge.


### DATASET
INDIAN DRIVING DATASET
https://idd.insaan.iiit.ac.in/dataset/download/
