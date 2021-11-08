# beans_mlops_project
An end-to-end image classification model with deployment in GCP along with CI/CD

### ABOUT THE ML MODEL:
Beans is a dataset of images of beans taken in the field using smartphone cameras. It consists of 3 classes: 2 disease classes and the healthy class. Diseases depicted include Angular Leaf Spot and Bean Rust. 

![alt text](https://github.com/AI-Lab-Makerere/ibean/blob/master/bean-example-data.png)
Data was annotated by experts from the National Crops Resources Research Institute (NaCRRI) in Uganda and collected by the Makerere AI research lab.

The goal is to build a robust machine learning model that is able to distinguish between diseases in the Bean plants. Beans are an important cereal food crop for Africa grown by many small-holder farmers - they are a significant source of proteins for school-age going children in East Africa.

The data is of leaf images representing 3 classes: the healthy class of images, and two disease classes including Angular Leaf Spot and Bean Rust diseases. The model should be able to distinguish between these 3 classes with high accuracy. The end goal is to build a robust, model that can be deployed on a mobile device and used in the field by a farmer.

The data includes leaf images taken in the field. The figure above depicts examples of the types of images per class. Images were taken from the field/garden a basic smartphone.

The images were then annotated by experts from NaCRRI who determined for each image which disease was manifested. The experts were part of the data collection team and images were annotated directly during the data collection process in the field.

Class	            Examples
Healthy class	        428
Angular Leaf Spot	    432
Bean Rust	            436
Total:	              1,296
Data can be downloaded from here: https://github.com/AI-Lab-Makerere/ibean/
