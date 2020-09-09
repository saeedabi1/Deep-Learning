
Semisupervised learning combines the benefits of both supervised and unsupervised learning, taking advantage of the few labels that are available to uncover structure in a dataset and help label the rest.

Approach:
1.	Take the representation(features) learned by the unsupervised learning, here is autoencoder (the hidden layer)
2.	Combine this representation(features) with the original training set features
3.	Feed this new set of combined features into the supervised model. 


Dataset “credit cards” is used in this program.  By dropping 90% of the fraudulent credit card transactions from the training set, we simulate how to work with partially labeled datasets.

