# DSND Capstone Project Sparkify

### Project Motivation
In this project, event data from Sparkify is analyzed to build a model for classifying existing and future users who are likely to churn, based on behaviors of two user groups who stayed and churned.

### A summary of the results of the analysis
The highlights from the results of the analysis including insights from this dataset are shared below.

1. The total number of unique users is 225 and who churned is 52 of them. The chart below describes the trend for who churned in termed of active days in the service. The majority of them canceled within 100 days from registration.<br>
![image](https://user-images.githubusercontent.com/29317778/211535402-f3ae508b-f260-4a8d-a698-77980d87da01.png)

2. Gender count<br>
![image](https://user-images.githubusercontent.com/29317778/211786769-9ce7dc3d-24fa-42d2-a13e-c3deeeed9cdc.png)

3. Account type<br>
![image](https://user-images.githubusercontent.com/29317778/211786908-73946ed2-eeb5-4c95-886d-06777b1fc82c.png)

4. The charts below shows how users actions are distributed by users status who stayed vs. who canceled. 'NextSong' action is excluded due to its data skewness.<br>
![image](https://user-images.githubusercontent.com/29317778/211787558-48709009-90f5-4d4a-91f9-42e7eb3ea553.png)<br>
![image](https://user-images.githubusercontent.com/29317778/211787615-3edbec57-6ce6-4165-9632-ef75e1cde7ec.png)

5. Distribution of song length<br>
![image](https://user-images.githubusercontent.com/29317778/211536559-d119b8ef-c519-4477-9d76-a11d731fb9c0.png)

6. Device and OS used<br>
As shown in the chart below, 86%+ of all access to the service came from desktop.<br>
![newplot (1)](https://user-images.githubusercontent.com/29317778/211536872-9a1f46a9-4f79-498d-9821-6a30e34eab24.png)

7. What browser did users access from?<br>
![newplot (2)](https://user-images.githubusercontent.com/29317778/211537058-277fc789-b0c3-4f60-b650-ae4abbd56399.png)

### Feature engineering and modeling
Before modeling, we have to define a target variable and features as below.<br>
<br>
Target variable (label): churn
Features: please see below list of features used.<br>
<img width="495" alt="Screenshot 2023-01-12 at 21 05 06" src="https://user-images.githubusercontent.com/29317778/212062224-7b3cc8bf-aa93-469b-8a0f-56ff2565a34f.png"><br>

All the features above are converted to numerical variables for modeling.<br>

As this is classification model, so 3 estimators LogisticRegression, RandomForestClassifier, and GradientBoostingClassifier are used to train dataset for buidling ML models.<br>
Of these 3 models, a model with GradientBoostingClassifier is better than the other 2 models when we look at f1 score.<br>
<img width="312" alt="Screenshot 2023-01-21 at 21 04 46" src="https://user-images.githubusercontent.com/29317778/213866037-da28d6bf-0ac4-45f8-9e7f-4fe1f4c421e5.png">


### File Descriptions
Below are files for this project.

- Sparkify_pandas.ipynb # Jupyter notebook for EDA, feature engineering, and modeling
- README.md

### Libraris used
The following Python libraries were used in this project.

- pandas
- numopy
- matplotlib
- seaborn
- plotly
- sklearn
- pyspark

### Blog link
Please see the details of analysis, insights, modeling, and results from [here](https://medium.com/@inthemoshpit/customer-churn-at-sparkify-b9ce66720e13).

### Acknowledgements
References below
- [17 Strategies for Dealing with Data, Big Data, and Even Bigger Data](https://towardsdatascience.com/17-strategies-for-dealing-with-data-big-data-and-even-bigger-data-283426c7d260)
- [Hyperparameter tuning in Python](https://towardsdatascience.com/hyperparameter-tuning-in-python-21a76794a1f7)
- [Popular Classification Models for Machine Learning](https://www.analyticsvidhya.com/blog/2020/11/popular-classification-models-for-machine-learning/)
- [A Straightforward Guide to Cleaning and Preparing Data in Python](https://towardsdatascience.com/a-straightforward-guide-to-cleaning-and-preparing-data-in-python-8c82f209ae33)
- [Data Leakage And Its Effect On The Performance of An ML Model](https://www.analyticsvidhya.com/blog/2021/07/data-leakage-and-its-effect-on-the-performance-of-an-ml-model/)

