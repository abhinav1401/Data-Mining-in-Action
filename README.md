# Data Mining in Action
This project involves building KNN, Decision Tree Learner, and Random Forest Learner classifiers to predict the Qualified status of the housing property. The dataset is present on Kaggle at this link -- 

https://www.kaggle.com/c/2018s-uts-data-analytics-assignment-3/overview

Two data sets used are, ‘TrainingSet.csv’ and ‘TestingSet.csv’. ‘TrainingSet’ is the dataset that will be fed to the classifier to build a predictive model and ‘TestingSet’ is the dataset for which the class attribute value (QUALIFIED) is predicted. The ‘TrainingSet’ contains 75008 rows and 39 attributes. The ‘TestingSet’ contains 32148 rows and 38 attributes. The additional attribute that the ‘TrainingSet’ has is the class attribute, which is utilized to build the classifier model and estimate the classifier’s accuracy. The knime workflow I designed for this project is as follow:

![alt text](https://github.com/abhinav1401/Data-Mining-in-Action/blob/main/Knime_Workflow.png)


The final result includes data cleaning and pre-processing using Knime and Excel on a Kaggle dataset to test multiple classification models to predict the house qualification for sale with an accuracy of 92%. The output with various parameters to test the model is in the table below.

<table style="width: 61px;">
<tbody>
<tr style="height: 43px;">
<td style="width: 15px; height: 43px;"><b>Split Criterion&nbsp;</td>
<td style="width: 15px; height: 43px;">&nbsp;<b>Tree Depth</td>
<td style="width: 15px; height: 43px;">&nbsp;<b>Number Models</td>
<td style="width: 15px; height: 43px;">&nbsp;<b>Accuracy</td>
</tr>
<tr style="height: 43px;">
<td style="width: 15px; height: 43px;">&nbsp;Information Gain</td>
<td style="width: 15px; height: 43px;">15</td>
<td style="width: 15px; height: 43px;">300</td>
<td style="width: 15px; height: 43px;">89.976%</td>
</tr>
<tr style="height: 43px;">
<td style="width: 15px; height: 43px;">&nbsp;Information Gain</td>
<td style="width: 15px; height: 43px;">&nbsp;15</td>
<td style="width: 15px; height: 43px;">&nbsp;200</td>
<td style="width: 15px; height: 43px;">&nbsp;89.455%</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 23px;">&nbsp;Gini Index</td>
<td style="width: 15px; height: 23px;">&nbsp;15</td>
<td style="width: 15px; height: 23px;">&nbsp;300</td>
<td style="width: 15px; height: 23px;">&nbsp;<b>92.541%</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 23px;">Gini Index&nbsp;</td>
<td style="width: 15px; height: 23px;">20&nbsp;</td>
<td style="width: 15px; height: 23px;">200&nbsp;</td>
<td style="width: 15px; height: 23px;">&nbsp;89.535%</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 23px;">&nbsp;Information Gain Ratio</td>
<td style="width: 15px; height: 23px;">15&nbsp;</td>
<td style="width: 15px; height: 23px;">300&nbsp;</td>
<td style="width: 15px; height: 23px;">&nbsp;89.535%</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 23px;">Information Gain Ratio</td>
<td style="width: 15px; height: 23px;">20</td>
<td style="width: 15px; height: 23px;">200</td>
<td style="width: 15px; height: 23px;">89.561%</td>
</tr>
</tbody>
</table>
<!-- DivTable.com -->

