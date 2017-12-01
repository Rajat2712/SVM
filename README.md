# Support Vector Machine
"Support Vector Machine” (SVM) is a supervised machine learning algorithm which can be used for both classification or regression challenges. However,  it is mostly used in classification problems. In this algorithm, we plot each data item as a point in n-dimensional space (where n is number of features you have) with the value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiate the two classes very well
![svm_1](https://user-images.githubusercontent.com/23000971/33506650-de8f9ed0-d716-11e7-8310-56ef4dd15f82.png)

# Identify the right hyper-plane
## Scenario-1
![svm_21](https://user-images.githubusercontent.com/23000971/33506962-1f35d49e-d718-11e7-80e4-191abb7686ad.png)
Select the hyper-plane which segregates the two classes better”. In this scenario, hyper-plane “B” has excellently performed this job.
## Scenario-2
![svm_3](https://user-images.githubusercontent.com/23000971/33506957-1de601e0-d718-11e7-98e0-3de5e9a7852c.png)
maximizing the distances between nearest data point (either class) and hyper-plane will help us to decide the right hyper-plane. This distance is called as Margin. Let’s look at the below snapshot:
![svm_4](https://user-images.githubusercontent.com/23000971/33506958-1e2073de-d718-11e7-9e31-d3a7c9d9da18.png)
the margin for hyper-plane C is high as compared to both A and B. Hence, we name the right hyper-plane as C. Another lightning reason for selecting the hyper-plane with higher margin is robustness. If we select a hyper-plane having low margin then there is high chance of miss-classification.

## Scenario-3
![svm_5](https://user-images.githubusercontent.com/23000971/33506959-1e56f972-d718-11e7-8d37-ad59fe8cd84e.png)
SVM selects the hyper-plane which classifies the classes accurately prior to maximizing margin. Here, hyper-plane B has a classification error and A has classified all correctly. Therefore, the right hyper-plane is A.

## Scenario-4
![svm_61](https://user-images.githubusercontent.com/23000971/33506963-1f6c4740-d718-11e7-8e69-b376fbd28d94.png)
one star at other end is like an outlier for star class. SVM has a feature to ignore outliers and find the hyper-plane that has maximum margin. Hence, we can say, SVM is robust to outliers.
![svm_71](https://user-images.githubusercontent.com/23000971/33506964-1f9d78ec-d718-11e7-96a8-0bb22adfcc0a.png)

## Scenario-5
![svm_8](https://user-images.githubusercontent.com/23000971/33506960-1e8dd2f8-d718-11e7-98f0-639436ff4e4d.png)
SVM can solve this problem. Easily! It solves this problem by introducing additional feature. Here, we will add a new feature z=x^2+y^2. Now, let’s plot the data points on axis x and z:
![svm_9](https://user-images.githubusercontent.com/23000971/33506961-1ec4cf60-d718-11e7-93ad-c9560bed73fe.png)
