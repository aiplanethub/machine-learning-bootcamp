## Learning Objectives

* Accuracy vs Interpretability Trade-off
* Existing techniques to evaluate models
* Feature Importance
* LIME


## Accuracy vs Interpretability Trade-off

There exists a typical Trade-oﬀ between Model Performance and Interpretability just like we have our standard Bias vs. Variance Trade-oﬀ in machine learning.

In the industry, you will often hear that **business stakeholders tend to prefer models which are more interpretable**, like **linear models (linear\logistic regression) and trees** which are intuitive, easy to validate and can be explained to a non-expert in data science.

This increases the trust of people in these models since its decision policies are easier to understand.

However, if you talk to data scientists solving real-world problems in the industry, they will tell you that **due to the inherent high-dimensional and complex nature of real-world datasets, they often have to leverage machine learning models which might be non-linear and more complex in nature**, which are often impossible to explain using traditional methods (ensembles, neural networks).

Thus, data scientists spend a lot of their time trying to improve model performance but in the process trying to strike a balance between model performance and interpretability.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_19087bd6162740729673237b9de6e312.png)




## Existing techniques to evaluate models

* If you’ve been building some Machine Learning models, you might’ve used the **model performance evaluation metrics** like precision, recall, accuracy, ROC curve and the AUC (for classification models) and the coefficient of determination (R-squared or R2), root mean-square error (RMSE) and mean absolute error (for regression models) as the ultimate truth for how good your model is, right?
* But that score doesn’t really take into account how interpretable or easy to understand the model is.
* Let's talk about **Exploratory Data Analysis and visualization techniques.** Some of these techniques can help us in identifying key features and meaningful representations from our data which can give an indication of what might be influential for a model to take decisions in a human-interpretable form. But that still isn’t enough since in the real-world, a model’s performance often decreases and plateaus over time after deployment due to variability in data features, added constraints and noise.
* Thus, we need to constantly check for how important features are in deciding model predictions and how well they might be working on new data points.

## Feature Importance

Feature importance is a generic term for the degree to which a predictive model relies on a particular feature, or how much the prediction is impacted by the value of a specific feature.

Typically, a feature’s importance is the increase in the model’s prediction error after we permuted/removed the feature’s values.










![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_6272d32b8abe4978868c4980801d15e0.png)






For example, we can see that X1 is the most important feature here - if we don’t use X1 to build our model, we might get more errors than if we use it to build our model.

## LIME - An Advanced Model Interpretation Technique

Lime (Local Interpretable Model-agnostic Explanations) helps to illuminate a machine learning model and to make its predictions individually comprehensible. The method explains the classifier for a specific single instance and is therefore suitable for local consideration.

Model-agnostic means it is applicable to any model in order to produce explanations for predictions.








<iframe width="560" height="315" src="https://www.youtube.com/embed/hUnRCxnydCc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>







A lot of the major state-of-the-art model interpretation frameworks out there are extensions of LIME — the original framework and approach proposed for model interpretation.

We’ll have a look at one such framework in detail - known as SHAP - in the next module.