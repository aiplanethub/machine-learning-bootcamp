## Learning Objectives
* What is Machine Learning?
* Machine Learning Categorization
* Classification and Regression
* Binary and Multiclass Classification



## What is Machine Learning?










<iframe width="560" height="315" src="https://www.youtube.com/embed/gmvvaobm7eQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>









## Machine Learning Categorization





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_098810bc3f584610b0fad6fc3cefe4ab.png)






### Supervised Learning Algorithms

Let's talk about the datasets that have both input and target variables (labels for the data)—ranging from predicting a person's survival rate in Titanic Dataset, where Survival Rate is already given, to predicting the House Price according to house characteristics where the house prices are provided.

The algorithms that work on such datasets are known as Supervised Learning Algorithms.

It is called supervised learning because the process of an algorithm learning from the training dataset can be thought of as a teacher supervising the learning process. We know the correct answers; the algorithm iteratively makes predictions on the training data and is corrected by the teacher. Learning stops when the algorithm achieves an acceptable level of performance.

### Unsupervised Learning Algorithms
Unsupervised learning is where you have unlabeled data (or no target variable) in the dataset.

Unsupervised Learning Algorithms aim to find some structure in the dataset.

These are called unsupervised learning because, unlike supervised learning, there are no correct answers and there is no teacher.
Algorithms are left on their own to discover and present the interesting structure in the data.

### Reinforcement Learning Algorithms

A robot takes a big step forward, then falls. The next time, it takes a smaller step and is able to hold its balance. The robot tries variations like this many times; eventually, it learns the right size of steps to take and walks steadily. It has succeeded.

What we see here is called reinforcement learning. The robot learns how to walk based on reward (staying on balance) and punishment (falling). This feedback is considered "reinforcement" for doing or not doing an action.

In simple terms, reinforcement learning is learning the best actions based on reward or punishment.

## Types of Supervised Learning Algorithms

Supervised learning can be further divided into two types:
1. Classification
2. Regression

### Classification vs Regression




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2f1a3fec2a5d41cab7699b1f259245eb.png)





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a37a46f393d94654a67e9f314152c45d.png)






To decide whether to use a regression or classification model, the first question you should ask yourself is:

Does your target variable have a continuous value, or is it discrete (binary or multi-class)?

### Regression

If your answer is continuous values, you're dealing with Regression.

If you're trying to predict quantities like height, income, price, or scores, you should use a model that will output a continuous number.

So if your objective is to determine tomorrow's temperature, you should use a regression model.

### Classification

Let's come to the second case, where you can see that the target variable is divided into classes. You'll be using Classification.

* When the number of classes is 2, it is known as Binary Classification. E.g. whether it will be hot or cold tomorrow is a binary classification problem with two categories: Hot and Cold.
* When it is more than 2, it is known as Multi-Class Classification. E.g., classifying movies as Good, Average, or Bad according to reviews.


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_4a520a2089eb4445a02030bc8ae5d1e0.png)



Understanding your target variable's characteristics is essential before you begin running models and forming predictions.

**In this course, we'll be focusing on Classification**.

## What is Classification?

Let's learn with some examples:

* In **Classification**, we classify the outcome
* **Examples:**
  * Predict whether a transaction is fraudulent or not
  * Predict whether to give a loan or not
  * Predict whether to give college admission or not
  * Predict the grade (Grade A, B, C, D)
  * Note: Classification can be more than two









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_31e1df95589141bab35c5ef370106723.png)







## What is Multi-Classification?

**It is as simple as dividing waste into four categories - plastic, glass, metal, and paper.**







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2a56408037994f92a50af1845ddb68c1.png)



### Slide Download Link

You can download the slides for this topic from [here](https://docs.google.com/presentation/d/1qsCHaAIR4ZNhsuqyc_sjxEE2Zik9hgdKij9QRZ1KsxE/edit?usp=sharing).