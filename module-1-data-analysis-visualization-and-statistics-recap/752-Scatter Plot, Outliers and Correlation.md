## Learning Objectives

* Scatter Plot
* Outliers
* Correlation in Data Science

## Scatter Plot

Scatter plots are used for interpreting trends in data. Below is an example of a scatter plot between temperature and ice cream sales in dollars. What is the trend in this scatter plot? Roughly we can say that as temperature increases, ice cream sales increase.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_042d0e9f8c6f4eeb8510c6bec6297562.png)







## Outlier

In statistics, an outlier is a data point that differs significantly from other observations.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_699037b84a2f4c82bf213daace320a3f.png)






## Correlation

Correlation is a statistical measure.

It measures the strength of a linear relationship between two quantitative variables.

Now you may ask, what is a variable? - If we go back to the scatter plot example: temperature and ice-cream sales are variables. Variable is often interchangeably used as features too.

Target variable - In data science, The "target variable" is the variable whose values are to be modeled and predicted by other variables in the dataset.

### Importance of Correlation

Every successful data science project revolves around finding accurate correlations between the input and target variables. However, more often than not, we oversee how crucial correlation analysis is.

It is recommended to perform correlation analysis before and after a data science project's data gathering and transformation phases.

### Positive Correlation

Two features (variables) can be positively correlated with each other. It means that when the value of one variable increases, the value of the other variable(s) also increases (also decreases when the other decreases).



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_43f8c653097e4a9095f32b87eb54ea79.png)





Real-life examples:

* The more time you spend running on a treadmill, the more calories you burn.
* As the temperature goes up, ice cream sales also go up.
* As the water level decreases in a fish tank, the fish's habitat volume decreases.

### Negative Correlation

Two features (variables) can be negatively correlated with each other. This occurs when the value of one variable increases and the value of the other variable(s) decreases (inversely proportional).






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_8274789faaae424f91340c5fefb0ff64.png)







Real-life examples:

* As the weather gets colder, air conditioning costs decrease.
* The more vitamins one takes, the less likely one is to have a deficiency.
* The more one works, the less free time one has.

### Zero/No Correlation

Two features might not have any relationship with each other. This happens when the value of a variable is changed, then the value of the other variable is not impacted.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_37216e529f474cdf9edecb95ca073928.png)







Real-life examples:

* There is no relationship between the amount of tea drunk and the level of intelligence.
* It was raining this morning, and the grocery store was out of bananas.
* The temperature on Mars and the stock market have an almost zero correlation because the stock market price will not depend on the temperature on Mars.

### Notebook and Dataset

* Next, we'll be looking at a pre-recorded session on Data
Visualization with Matplotlib and Pandas
* Link to the Notebook:  
https://dphi.tech/notebooks/853/manish_kc_06/day-4-notebook-data-visualization-in-python
* Link to the Dataset: https://github.com/dphi-official/Datasets/blob/master/Standard_Metropolitan_Areas_Data-data.csv
* Go through the dataset and try to understand what the columns represent.

### Dataset Description

It contains data from 99 standard metropolitan areas in the US. The data set provides information on ten variables for each area from 1976 to 1977. The areas have been divided into four geographic regions: 1=North- East, 2=North-Central, 3=South, 4=West. The variables provided are listed in the table below:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_6f49160e3cc34f618d6f1283b4f2ad41.png)




### Slide Download Link
You can download the slides for this topic from [here](https://docs.google.com/presentation/d/1GiYoMN9Zly4r12RR_0Iwd6IkzMwUYwMTeo4L5R9UA1A/edit?usp=sharing).