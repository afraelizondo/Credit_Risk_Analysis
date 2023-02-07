# Credit Risk Analysis


## Overview of the project

Over the last years, FinTech has been using Machine Learning to perform analysis and get to know predictions about credit risk of their potential users. Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. 

One of the main reasons to use this powerful tool, is that machine learning provides a quicker and more reliable loan experience; also, the election of candidates for the credit loans, can be more accurate. To choose which model is the adequate, many evaluations have to be performed, in order to select the one that fits better with the specific data. 

In this specific project, we were working with a real-world challenge: credit card risk; this with the help of a dataset from LendingClub, a peer-to-peer lending services company. This kind of risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  


## Results 

In order to select the correct model, we performed 6 of them to determine which algorithm results in the best performance, as described below: 

### Naive Random Oversampling

- A technique that involves randomly duplicating examples from the minority class in the training dataset. 

- With this kind of oversampling, we got an accuracy of 62%, which is not a good number when the credit risk is implicated. 

<img width="750" alt="Screen Shot 2023-02-06 at 6 20 35 PM" src="https://user-images.githubusercontent.com/113856917/217116665-4fa767a8-02f8-4c0e-a065-5f74d4f6659e.png">

### SMOTE Oversampling

- An acronym for Synthetic Minority Oversampling Technique. The most popular oversampling method, it works by selecting examples that are close in the feature space, drawing a line between the examples in the feature space and drawing a new sample as a point along that line.

- The result for accuracy this time was 65%, which again, is not a good model for finances. 

<img width="732" alt="Screen Shot 2023-02-06 at 6 26 30 PM" src="https://user-images.githubusercontent.com/113856917/217117279-077af4f6-5b92-43ba-a6a3-2129f4ed3501.png">

### Undersampling 

- A technique to balance uneven datasets by keeping all of the data in the minority class and decreasing the size of the majority class.

- With an accuracy score of 65%, same as the SMOTE Oversampling. 

<img width="731" alt="Screen Shot 2023-02-06 at 6 29 07 PM" src="https://user-images.githubusercontent.com/113856917/217117585-6014547d-717e-41c8-bcb5-6a17f0241890.png">

### Combination (Over and Under) Sampling

- This time, the accuracy score was lower compared with the previous ones, 63%.

<img width="768" alt="Screen Shot 2023-02-06 at 6 31 38 PM" src="https://user-images.githubusercontent.com/113856917/217117907-2c2e0d4d-5e49-47b7-81be-aae3d9f98adb.png">

### Balanced Random Forest Classifier

- Technique that randomly under-samples each boostrap sample to balance it.

- Accuracy of 67%, this Ensemble Learner performed a little bit better than the other models; however from FinTech perspective is not good enough. 

<img width="727" alt="Screen Shot 2023-02-06 at 6 35 21 PM" src="https://user-images.githubusercontent.com/113856917/217118538-2a868c50-f453-4b29-85f3-693ed3cdc4c1.png">

### Easy Ensemble AdaBoost Classifier

- A meta-estimator that begins by fitting a classifier on the original dataset and then fits additional copies of the classifier on the same dataset but where the weights of incorrectly classified instances are adjusted such that subsequent classifiers focus more on difficult cases.

- Getting a result of 92% of accuracy. 

<img width="587" alt="Screen Shot 2023-02-06 at 6 38 27 PM" src="https://user-images.githubusercontent.com/113856917/217118776-8695c26f-3a66-4d59-99bc-6d6abf42ae59.png">


## Summary 

With an accuracy score of 92%, the best performance was of the Easy Ensemble AdaBoost Classifier. 

With the training and test dataset, it threw these results, that in my opinion are so much better than the results from the other training models. 

<img width="391" alt="Screen Shot 2023-02-06 at 6 43 09 PM" src="https://user-images.githubusercontent.com/113856917/217119283-1f32422f-0cac-4c75-8b8a-b657b8c4ecb5.png">

Even though is not perfect, it only predicted 8 as low risk, being an actual high risk. 

So, I would definitely choose this algorithm over the others.  
