# Document-Classifier

Program can be run using following command :

./topics mode dataset-directory model-file [fraction]

Mode can be :
  1. train 
  2. test

Fraction - Optional Parameter to decide whether to train the model using fully supervised or semi supervised learning.
Every time a new document is fetched the program decides whether to look at the label of the document or not based on the fraction.

fully supervised = 1.0. (default)
semi supervised = 0.0 < fraction < 1.0

Train Mode - trains the dataset in dataset-directory and write the trained model to model-file.
Test Mode - Predicts the genre of the document based on the model created in the train mode.

This program with slight modification can be used in cases where some labeled and and some unlabled training data is present.
To create a useful model. For the purpose of the academic project I simulated the unlabled training data with use of fraction 
command line option
