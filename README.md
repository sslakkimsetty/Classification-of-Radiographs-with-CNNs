# Classification-of-Radiographs-with-CNNs
Classification of Radiographs using Convolutional Neural Networks

The objective of the project is to classify X-rays (images) of various upper body extremities on Stanford's MURA dataset to be either positive (shows a disease) or negative (free of disease). The dataset consists of six different types of X-rays (elbow, finger, forearm, hand, humerus, and shoulder). 
Given an image, we want to correctly classify if the body part shown (we do not know which kind of body part) is positive or negative. This is not a trivial problem because, we have to first identify which body part it is and then classify if it is positive or negative. 
We approached the problem with an stacked ensamble CNN model. Broadly speaking, we use one convolutional neural network (CNN) to first classify the image one of six upper body extremities. 
Then we use another CNN that corresponds to the body part prediction by the first model. That means we train one model to predict the type of body part and then six CNN models to classify if the predicted body part shows a disease or not. 

We have achieved 91.2% accuracy for the classification of the body part with ~36K tunable parameters. The six CNN models are 160-layered models to classify healthy-disease conditions with an accuracy of 80% with ~4K parameters. 
