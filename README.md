# Effect-of-Dimensionality-Reduction-on-Generative-and-Discriminative-Classifiers


### Results comparison:
Case 1:  Classifiers trained on Singular Value Decomposition(SVD) reduced test data<br />
Case 2: Classifiers trained on raw (scaled) test data<br />

![image](https://user-images.githubusercontent.com/24207916/140415842-f1c39133-6f59-431a-979e-b96c83189cc6.png)


### Inference:
o	KNN and Multinomial Logistic regression(MLR) performed better than Naïve Bayes in both Case 1 & Case 2.<br />
o	Naïve Bayes accuracy improved significantly after using dimensionality reduction(SVD). This is because after SVD all the features are independent of each other which is the main assumption of Naïve Bayes. But Naïve Bayes accuracy is still low compared to other classifiers because features might not necessarily be Gaussian distributed and discrimination between likelihoods might not be clear.<br />
o	KNN’s accuracy is almost same in both cases because KNN makes no prior assumption of the data and performs the same way both the time. Only difference was in the computation time. KNN without dimensionality reduction took longer time to run compared to KNN with dimensionality reduction.<br />
o	MLR trained on raw test data have high variance(Over-fit)  as compared to MLR trained on SVD test data. Because SVD aided in creating more stable model by avoiding overfitting.<br />
o	KNN is the best classifier among the three classifiers in both case 1 and case 2.<br />



Note: See iPython notebook for implementation of all the above results

