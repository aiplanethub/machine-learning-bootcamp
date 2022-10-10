## Logistic Regression

* Logistic Regression is one of the basic and popular algorithms for solving binary classification problems
* For each input, logistic regression outputs a probability that this input belongs to one of the two classes
  * Set a probability threshold boundary that determines which class the input belongs to
* Binary classification problems (2 classes):
  * Emails (Spam / Not Spam)
  * Credit Card Transactions (Fraudulent / Not Fraudulent)
  * Loan Default (Yes / No)

Now, you may ask, why don't we use Linear Regression? Why do we need a new algorithm?

Well, you will find all the answers in the video below.

The video below is a must-watch. The instructor has
brilliantly explained about logistic regression!












<iframe width="560" height="315" src="https://www.youtube.com/embed/zM4VZR0px8E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>










## Linear vs. Logistic Regression

* Linear regression is used to solve regression problems with continuous values
* Logistic regression is used to solve classification problems with discrete categories
  * Binary classification (Classes 0 and 1)
  * Examples:
    * Emails (Spam / Not Spam)
    * Credit Card Transactions (Fraudulent / Not Fraudulent)
    * Loan Default (Yes / No)
* Let's say a data scientist named John wants to predict whether a customer will buy insurance or not
* Remember that linear regression is used to predict a continuous value where the output (y) may vary between +∞ (positive infinity) to -∞ (negative infinity). In contrast, in this case, the target variable (y) takes only two discrete values, 0 (No insurance) and 1 (Yes, got the insurance).
* John decides to extend the concepts of linear regression to fulfill his requirement. One approach is to take the linear regression output and map it between 0 and 1. If the resultant output is below a certain threshold (say 0.5), classify it as No (didn't buy the insurance), whereas if the resultant output is above a certain threshold, classify it as buying the insurance (yes)
* We then plot a simple linear regression line and set the threshold as 0.5
  * Negative class (Insurance = No)– Age on the left side
  * Positive class (Insurance = Yes) – Age on the right side


















![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1c4394f033b541af95568bdf12bbeb39.png)





**Imagine there is an outlier towards the right**





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_0373ee7e00e04ba7933946c6f976f057.png)




* As we can see, an outlier in the data will distort the whole linear regression line.
* Clearly, the line is unable to diﬀerentiate the classes with the linear line fit
* The line should have been at the vertical yellow line, which can divide the positive and negative classes, i.e., yes or no for insurance

**Well, life would be much simpler if we had an algorithm that would fit the points like below, right? It is a much better fit compared to the regression line!**







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_14f92535c46c4dab9a855e4180885625.png)





### Solution

* Solution – Transform linear regression to a logistic regression curve
* Logistic regression is a Sigmoid function
* Now, what does this sigmoid function do?
  * Sigmoid function takes in any real value and gives an output probability between 0 and 1








![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_ea7cee4fca594e6abf99126153496744.png)







### What are we doing in Logistic Regression?

* We will use the real-valued output obtained from a linear regression model between 0 and 1 and classify a new example based on a threshold value. The function used to perform this mapping is the **sigmoid function**
* The Sigmoid Function is represented by the formula:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_756f623aa7c640b28e5d1ac6be262fe4.png)



* There's no need to go into the depth of how we obtained this formula right now.

## Sigmoid Function (Logistic Function/ Logit)

* Take the linear regression function and put it into the Sigmoid function
* Sigmoid function outputs probability between 0 and 1







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_32449fe29f284ee9863b8cecc382bb7c.png)





* Sigmoid function outputs probability between 0 and 1 (y-axis)
* Default probability threshold is set at 0.5 typically&#x20;
  * Class 0 – Below 0.5
  * Class 1 – Above 0.5






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_79f1845e8b994253a9767895f349156e.png)




## Types of Logistic Regression

The logistic regression model can be classiﬁed into three groups based on the target variable categories:

* **Binary Logistic Regression**
  * The target variable has two possible categories.
  * Common examples : 0 or 1, yes or no, true or false, spam or no spam, pass or fail, Transactions (Fraudulent / Not Fraudulent), Medical Condition (Diseased/ Not diseased)
* **Multi-Class Logistic Regression**
  1. **Multinomial Logistic Regression**
    * The target variable has three or more categories that are not in any particular order. So, there are three or more nominal categories.
    * Examples: Fruits (apple, mango, orange, and banana), profession (e.g., with ﬁve groups: surgeon, doctor, nurse, dentist, therapist)
  2. **Ordinal Logistic Regression**
    * The target variable has three or more ordinal categories. So, there is intrinsic order involved with the categories.
    * Student performance can be categorized as poor, average, good, and excellent.

### Notebooks for practice

* https://dphi.tech/notebooks/899/manish_kc_06/basic_logistic_model
* https://dphi.tech/notebooks/861/manish_kc_06/logistic-regression-advertisement
* https://dphi.tech/notebooks/862/manish_kc_06/logistic-regression-heart-disease
* https://dphi.tech/notebooks/891/manish_kc_06/logistic_regression_insurance

### Slide Download Link

You can download the slides for this topic from [here](https://docs.google.com/presentation/d/15-VDhUWLY51U8eG9UvhyMeqOIrXejZQfTSSgmfBQxck/edit?usp=sharing).