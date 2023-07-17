### Wine quality Prediction based on physicochemical properties

This is the course project from my Master's program Data Science course. 

Project Proposal:

Context and Dataset
This project is based on Wine Quality Data Set(https://archive.ics.uci.edu/ml/datasets/wine+quality)  from UCI Machine Learning Repository. 2 data set are provided which relate to red and white variants of the Portuguese "Vinho Verde" wine. 
The data set includes 4898 instances and 12 attributes. The attributes are the results based on  physicochemical tests. Output variable is the rating/graded quality based on sensory data.
Input variables:
1 - fixed acidity
2 - volatile acidity
3 - citric acid
4 - residual sugar
5 - chlorides
6 - free sulfur dioxide
7 - total sulfur dioxide
8 - density
9 - pH
10 - sulphates
11 - alcohol 
 Output variable (based on sensory data):
12 - quality (score between 0 and 10) 

Problem and Why
What problem did you decide to address?
The goal of the study is to generate a prediction model of wine quality. Wine plays a very important role in human history. However, it is hard for common people to adjust the wine without experience. Thus, having a data set of wines that have already been graded by the experts with their physicochemical features will help us build a model to predict other wines’ quality in the future. 

Why do you think it is important and why you do you think data science is a good tool to tackle this problem?
The quality of a wine is based on human sensory data but also highly related to its physicochemical features, since the difference among these features leads to a various teases. This project is based on this idea: If the  physicochemical features of the wine, which can be tested from the lab, have strong correlation with wine’s quality, then we can build model based on data science to replace human(wine expert) resource with cheaper lab and computing resources. Since everything in this process can be quantified, this area might be a usage of data science with enormous economic benefit.

Use of Data and Models
What dataset did you chose for that (highlight any interesting aspects of your data with visualizations, statistics, etc)?
The data set is Portuguese "Vinho Verde" wine quality data set from UCI Machine learning Repository. It provided 11 physicochemical test features like acidity and dioxide, which can represents a comprehensive test result from a lab. The predict variable is quality, which is between 0-10. it is a subjective numeric variable based on human sensory.  By separating wine instances into different quality levels, we might find out the distribution and statistics of some features are different for different levels of wine.
What models did you train and how did they perform?
This model can be treated as a regression solution since the input and output variables are all numeric and can be regraded as continuous. However, it can also be treated as a classification problem if transfer the quality variable into “low quality”, “medium quality” and “high quality” based on its numeric value. So we could use classification models like KNN or Decision Tree. I could build models based on the two ideas and evaluate several models to find out which one has the best performance. It will also provide me an opportunity to transfer my problem with flexibility in machine learning.

User Interface
How did you design your service and how would a user interact with it? (give us a quick demo of your service)
For user to interact with this model, I could develop a UI for inputs of physicochemical features and return a predicted wine quality based on the training data.  

Future Leverage
What benefits do you think your solution provides?
This model serves as a bridge between lab-testable result and human subjective feelings. It is potentially enables machine algorithm the power to predict human behaviors/feelings. Manufacturer could save a fortune after they reduced their wine expert and use more computing resources. It is also an instance to compare regression/classification in a certain situation, demonstrating their advantages and disadvantages.
Any final thoughts
Some features might mot be relevant, so we can calculate correlation/mutual information to filter down some feature. 
In some cases the input features might be too much, so PCA method might be used.
