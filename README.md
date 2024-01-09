# Image-Based-Weather-Classification


DESCRIPTION
=================================================================================================================================
This computer vision-based project is made to predict weathers' condition based on the sky's current appearance. The model used in this dataset was obtained from kaggle dataset. In this project, we compared multiple pre-trained model and thus can we deduce which model perform the best in this weather classification project. Through training and testing process, it was hoped that the model produced to provide sustainable and valid classification prediction.


RELATED FIELDS
=================================================================================================================================
Data Analysis | Data Visualization | Data preprocessing | Computer Vision
<br>Machine Learning | Classification | Deep learning | Pre-trained model

DATASETS
=================================================================================================================================
The dataset was obtained from the following link:
[<br>https://archive.ics.uci.edu/dataset/186/wine+quality](https://www.kaggle.com/datasets/lethanhnghia/wheatherclassfication)

<br>There are 1125 images in the dataset which image type is PNG, with 4 classes as listed below:
- 300 image has label Cloudy
- 215 image has label Rain
- 253 image has label Shine
- 357 image has label Sunrise


IMAGE PREPROCESSING
=================================================================================================================================
In this project, I used ImageDataGenerator in order to bring variety to the dataset. By performing multiple types of image alteration, such as rotation, brightness adjusment, flipping, and zooming, the variety of images is hoped to increase the models' performances.


MODELLING EVALUATION
=================================================================================================================================
After comparing multiple pre-trained and non-pre-trained models, here are the result obtained:
No | Model | Accuracy | Precision | Recall | F1-score |
--- | --- | --- | --- |--- |--- |
1	|VGG-19 + Adam	|0.92	|0.93	|0.92	|0.92
2	|LeNet	|0.84	|0.86	|0.84	|0.84
3	|ResNet-50	|0.90	|0.92	|0.90	|0.90
4	|ResNet-18	|0.88	|0.88	|0.88	|0.88

From the table, it is evident that VGG-19 outperforms other models. Although it has fewer layers than ResNet-50, it manages to obtain a higher score in every single evaluation metric.

CONCLUSION
=================================================================================================================================
The charts plotted from the training process show a high level of oscillation. However, the models manage to perform well during testing, and thus, with less than 50 epochs, the previously pre-trained models such as the VGG and ResNet manage to adapt their parameters to be able to classify well in this weather classification project.
