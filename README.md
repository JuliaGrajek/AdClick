# AdClick

This project is a slight modification of the task for the second track of the KDD CUP 2012, as presented here: https://www.kaggle.com/c/kddcup2012-track2.
The aim was to predict the click-through rate (pCTR) of ads given some tabular data about the user and the ad itself. The training set consisted of 80 million records.
The features consist of categorical variables, more preciselythe user's age and gender, and the ad's position and depth (as explained in the link) as well as token lists, corresponding to the query, keyword, ad title, and ad description.

Hence, I have built a multi-input neural network to deal with the two types of features. Categorical variables are one hot encoded or hashed/bucketized, while tokenized variables are preprocessed via embedding layers. Dropout was used for regularization. I obtained an AUC of 0.73 on the test set training for just 4 epochs (due to time constraints). This project is from 2021 and tensorflow 2.3 was used.



