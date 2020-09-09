Multiple Instance Learning (MIL) is  a weakly supervised learning method that takes a set of labeled bags containing many samples instead of receiving a set of labeled samples.
By using it, we are able to save the labeling effort and leverage weakly labeled data.

Example: When we have pathology slides from patients and we want to predict if a large slide contains cancer cells or, zooming out if the patient has malignant cells, Multiple Instance Learning(MIL) is a good option because doctors don’t need to segment individual cells or label each tile. Only the whole slide needs a label.

Provided program is based on MNIST dataset.

Each instance xi in one bag has a label yi. 

Define the label of the bag as:
Y = 1, if there exists a yi such that yi ==1
Y = 0, if for every yi such that yi == 0

MIL process implemented:
1.	Pre-train the ResNet model on the instance-labeled dataset 
2.	Feed the bag-labeled dataset in the model and extract features. 
3.	Finally, we apply MIL on extracted features.


