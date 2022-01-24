# Recommendation-IBM
Recommendations for Article in IBM Watson in collaboration with IBM Watson and UDACITY


Installation and Library Used
1. Python
2. Pandas
3. Numpy
4. Matplotlib
5. Pickle

These libraries can be installed using simple pip command or conda (if you are using Jupyter).

Project Motivation:

This project is a part of my course curriculum in UDACITY DataScientist NanoDegree.

File Description

This project consists of following files:
1. Data: It consists of the data required to do the analysis. This data is provided by IBM Watson in collaboration with UDACITY
2. Tests: This tests files are used to check the working of the code at various places.
3. Python File consists of the working of the Recommendation Engine 

How to Interact with the project:

This project is divided into following tasks:

1.Exploratory Data Analysis
2.Rank Based Recommendations
3.User-User Based Collaborative Filtering
4.Matrix factorisation

All the above task is completed using Python functions and its libraries as mentioned above.

Summary:

Articles are recommended to a user based on three parameters as below:
1. Rank based recommendations for the user new to the IBM Watson, based on the best articles selected on the basis of no. of interactions an article received.
2. User-user collaborative model based recommendations for the old user based on the type of articles read by the users who shares the same interest.
3. Matrix Based recommendations using SVD model.

We noted that if we were given a new user, Rank Based Function will be most suitable for recommendation. Only after we have information about the user, we can use a mix of rank based, collaborative and content based method for recommendation.

Also,after applying the SVD we found that Accuracy for Train data increase with increase in number of Latent Features, however Accuracy for Test data decreses. This is mainly due to Overfitting which is needed to be avoided in all possible circumstances. We also note that accuracy for test data is very high (~99.10%) which is mainly due to the sparse matrix for test data. Further addition of data sets in test data is needed to get the better picture of the resulting accuracy. As can be observed from above, nearly 80 Latent Features are required for function to perform optimally under the given conditions. In order to check for the results to the new users, to avoid cold start problem, we can do the A/B testing with our Recommendation system. If the click-through rate improves then we can recommend our model to the new users.

Licensing, Authors, Acknowledgements, etc.

Thanks to UDACITY for providing various starter codes as well as tests.

