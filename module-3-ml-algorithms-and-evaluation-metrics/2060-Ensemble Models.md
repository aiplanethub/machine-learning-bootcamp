## Real-life Analogy

* Andrew wants to decide where to go during a one-year vacation, so he asks the people who know him best for suggestions. The ﬁrst friend he seeks out asks him about the likes and dislikes of his past travels. Based on the answers, he will give Andrew some advice.
* This is a typical decision tree algorithm approach. Andrew's friend created rules to guide his decision about what he should recommend by using Andrew's answers.
* Afterwards, Andrew starts asking more and more of his friends to advise him, and they again ask him diﬀerent questions they can use to derive some recommendations for him. Finally, Andrew chooses the places that are recommended the most to him, which is the typical random forest algorithm approach.












![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_456e8d576016402896fd92904f1c337f.png)







## Ensemble Models - "The wisdom of crowds"

* Let's pause and think about what Andrew did. He took multiple opinions from a large enough bunch of people and then made an informed decision based on them. This is what Ensemble methods also do.
* You might have two models that each are good at predicting a certain (diﬀerent) portion of your dataset. Combining the two models seems like a good idea to increase performance
* “ensemble” = Combination of models
* Ensemble models in machine learning **combine the decisions from multiple models to improve the overall performance.**
* So basically, ensembling/combining two or more algorithms could improve or boost your performance. But there is a logic behind ensembling - you cannot just randomly combine two models and demand an increase in performance. There is math behind everything.
* So, let's dive into the several ensembling methods you can try.

## Simple Ensemble Techniques

* In this section, we will look at a few simple but powerful techniques, namely:
  * Max Voting/Mode
  * Averaging
  * Weighted Averaging

### Max Voting

* The max voting method is generally used for classification problems. This technique uses multiple models to make predictions for each data point. The predictions by each model are considered a 'vote'. The predictions that we get from the majority of the models are used as the final prediction.
* For example, when you asked 5 of your colleagues to rate your movie (out of 5), we'll assume three rated 4 while two gave a 5. Since the majority gave a rating of 4, the final rating will be 4. You can consider this as taking the mode of all the predictions.
















![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_bdbe03409ba6455b83de263affcb9649.png)







### Averaging

* In this technique, we take an average of predictions from all the models and use it to make the ﬁnal prediction.
* Averaging can be used to make predictions in regression problems or calculate probabilities for classiﬁcation problems.
* For example, in the below case, the averaging method would take the average of all the values. i.e. (5+4+5+4+4)/5 = 4.4



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_447ba42698f845d8a116bb3923276b71.png)


### Weighted Average

* This is an extension of the averaging method. All models are assigned diﬀerent weights, deﬁning the importance of each model for prediction.
* For instance, if two of your colleagues are critics, while others have no prior experience in this ﬁeld, then the answers by these two friends are given more importance than the other people.
* The result is calculated as \[(5\*0.23) + (4\*0.23) + (5\*0.18) + (4\*0.18) + (4\*0.18)] = 4.41.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f4e9af57aa894fc7b262d5966c5a1f23.png)


## Advanced Ensemble Techniques

* Now that we have covered the basic ensemble techniques, we can move on to understanding the advanced techniques, namely:
  * Stacking
  * Blending
  * Bagging Eg: Random forest
  * Boosting Eg: Adaboost, Gradient Boost, Extreme Gradient Boost
* We'll learn about Bagging and Boosting techniques. There is nothing to worry about; they are just like any other algorithms like linear, logistic, and decision trees.

### Bagging (Bootstrap AGGregatING)

* The idea behind bagging is combining the results of multiple models (for instance, all decision trees) to get a generalized result.
* Here's a question: If you create all the models on the same training data and combine it, will it be useful? There is a high chance that these models will give the same result since they are getting the same input. So how can we solve this problem? A technique called bootstrapping helps us with that.
* Aggregating = Summing or Combining
* Bagging combines the diﬀerent models created by bootstrapping on diﬀerent sets of training data, hence the name Bootstrap Aggregating.
* Random forest is a famous bagging model which uses variations of multiple trees. If the same trees are used, it's a bagged decision tree.

### Boosting

* Here's another question: If the ﬁrst model incorrectly predicts a data point and then the next (probably all models), will combining the predictions provide better results? Such situations are taken care of by boosting.
* Intuitively, each new model focuses its eﬀorts on the most diﬃcult observations to ﬁt till now and attempts to correct the errors of the previous model. So at the end of the process, we obtain a strong learner.
* Boosting, like bagging, can be used for regression and classiﬁcation problems.
* There are various types of Boosting algorithms that we'll study about soon.

### Summary of differences between Bagging and Boosting












![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_dda5eb7f9da3401bb173d352dc0f8a02.png)








### Reading Material

* MUST READ - Simple guide for ensemble learning methods: https://towardsdatascience.com/simple-guide-for-ensemble-learning-methods-d87cc68705a2

### Slides Download Link

You can download the slides for this topic from [here](https://docs.google.com/presentation/d/1Rhx2QvlEzdl7g_TXb5wv32E9WTQczbIi1oxcfY0EeTA/edit?usp=sharing).