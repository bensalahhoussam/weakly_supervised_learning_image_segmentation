# General concept 

The foundation of every machine learning project is data, the one thing you cannot do without.
The more data you get the more the model learns useful features ,increases performance and gets confident for better decisions ,but it can be a tedious job for data collection and annotation. 

To address this problem , there is a method called weakly semi-supervised learning or pseudo-labeling.

The main idea is to first train the model on labeled data , then use the trained model to predict on unlabeled data (Transfer learning method) , thus creating pseudo-labels,and will have more labeled data and continue doing that until the mode converges to higher performance.


![alt text](https://github.com/bensalahhoussam/weakly_supervised_learning_image_segmentation/tree/main/images/image_1.png)


# Problem description 

The problem is an image segmentation for multi class , it classifies each pixel as foreground or background , but deep learning requires complete annotation for the mask during the training. .

In order to annotate more data  without taking too much time , the method will be based on annotating points , and based on that , the model should be able to identify the selected class by that specific points .

# Problem solution

1- train a fully supervised model with large labeled data in order to make the model understand the features of each class .

2- use a transfer learning method to transfer the knowledge with the help of a point label the model will be able to identify the object with less amount of information . 

![alt text](https://github.com/bensalahhoussam/weakly_supervised_learning_image_segmentation/tree/main/images/img.png)


# Dataset 

We choose a remote sensing dataset named UAVID dataset.
It contains 8 classes which are  “Building,Road,Static car,Tree,Low vegetation,Human,
Moving car,Background clutter“.

link to dataset https://www.kaggle.com/datasets/dasmehdixtr/uavid-v1

