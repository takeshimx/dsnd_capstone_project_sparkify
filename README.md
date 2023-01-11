# DSND Capstone Project Sparkify

### Project Motivation
In this project, event data from Sparkify is analyzed to build a model for classifying existing and future users who are likely to churn, based on behaviors of two user groups who stayed and churned.
A web app is included, where an emergency worker can input a new message and get classification results in several categories.

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

5. Top 20 artists by play counts<br>
![newplot](https://user-images.githubusercontent.com/29317778/211536421-6e9ece59-7c19-4b57-aef4-efb92acbc0f5.png)

6. Distribution of song length<br>
![image](https://user-images.githubusercontent.com/29317778/211536559-d119b8ef-c519-4477-9d76-a11d731fb9c0.png)

7. Device and OS used<br>
As shown in the chart below, 86%+ of all access to the service came from desktop.<br>
![newplot (1)](https://user-images.githubusercontent.com/29317778/211536872-9a1f46a9-4f79-498d-9821-6a30e34eab24.png)

8. What browser did users access from?<br>
![newplot (2)](https://user-images.githubusercontent.com/29317778/211537058-277fc789-b0c3-4f60-b650-ae4abbd56399.png)


### File Descriptions
Below are files for this project.

- Sparkify.ipynb # Jupyter notebook for EDA, feature engineering, and modeling
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
