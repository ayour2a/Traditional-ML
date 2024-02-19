# Traditional-ML
Abstract
This report aims to highlight the steps required to train a model and to predict the CO2 
emission of the vehicles and to classify the vehicles based on the categorical variables. 

Introduction:
Climate change is on the front burner of the whole world hence, being able to reduce and 
manage Co2 emission from vehicle is of paramount importance to the Government of all
Countries. To achieve our desired goal, we tried to build a model that can accurately predict 
Co2 emissions of vehicles.

1. The steps required to train a model:
The following are the steps required to train a model:
1. Gathering data. For us to have a good model, we must have quality and enough data sets.
2. Data Wrangling: This includes data cleaning, removing duplicates, taking care of missing 
data, normalizing our dataset. Also, carry out data pre-processing and exploratory data 
analysis, visualization to enable us see the relationships between variables in our dataset. 
3. Split our datasets into Train and test sets. A lot of time, I see 70/30, 80/20, 90/10 split. 
Although this depends on what you are trying to achieve, peculiarity of dataset etc.
4. After doing the above, we can now decide model to choose as there are different model for 
different task. We want ensure we choose the correct model otherwise, it will be sheer waste 
time.
5. This is the point we train our model with the train dataset to enable is make accurate 
prediction on our test dataset.
6. Performance Measure and evaluation of our model: Here we use our fit our model on our 
test dataset which our model has not seen before to evaluate it. There are other metrics used 
in measuring performance such accuracy, f1-score, recall etc.
7. There are sometimes need to carry out hyperparameter tuning for optimal performance.
8. Also, we may need to further feed our model more test data which was withheld initially to 
evaluate performance before deploying it.

Attempt to use all the numerical continuous variables in the dataset provided to build a 
model to predict the CO2 emission. Perform exploratory data analysis to select a subset of 
the variables and repeat the procedure. Compare your models and report if there are any 
differences in the models’ performances? Explain your findings.

The following models Linear Regression, Random Forest Regressor, Bagging Regressor, 
ExtraTrees Regressor and Decision Tree Regressor were explored. The R2 score which is one 
of statistical measure that shows how well our model is performing on a scale of 0 to 1. All 
the model explored shows 97% except for linear regression which was 87%
Determine whether there were any noticeable improvements in the CO2 emission from 
year 2010 to year 2014? Explain your findings.

From the chart above, we can see that cars made in year 2010 has the highest Co2 emission 
when compared with others. 2014 shows the lowest Co2 emission.
Using each categorical variable as the target variable at each instance, determine which of 
the variables performed best in classifying the dataset. Explain your findings.
From the findings after using the categorical variable Fuel type and Model, the following 
models were explored Random Forest Classifier, Extra Trees Classifier and K-Neighbors
Classifier. From the classification report, Random Forest Classifier performed best with 
weighted average of precision, recall and f1-score of 94% for fuel type while with Model’s 
classification report shows 35%, 34% and 33% respectively.

How did you check whether your models did not overfit?
This was achieved by splitting the dataset into Train, test and validation. The model was fit to 
the validation dataset to enable us see performance and also to check whether or not there is 
an overfitting.

State the performance measure(s) you were most interested in and the reason(s).
The F1 score and the R-squared. The F1 score is a popular performance measure for 
classification and often preferred over, for example, accuracy when data is unbalanced, such 
as when the quantity of examples belonging to one class significantly outnumbers those 
found in the other class like in the case of Model. Although the R-squared will give you an 
estimate of the relationship between movements of a dependent variable based on an 
independent variable's movements. It doesn't tell you whether your chosen model is good 
or bad, nor will it tell you whether the data and predictions are biased.(C3. AI)
Can your models be deployed based on their performances? Explain

Yes. According to investopedia : What qualifies as a “good” R-Squared value will depend on 
the context. In some fields, such as the social sciences, even a relatively low R-Squared such 
as 0.5 could be considered relatively strong. In other fields, the standards for a good RSquared reading can be much higher, 
such as 0.9 or above. In finance, an R-Squared above 
0.7 would generally be seen as showing a high level of correlation, whereas a measure below 
0.4 would show a low correlation. This is not a hard rule, however, and will depend on the 
specific analysis.

Use only the non-categorical variables to form groups. Using internal and external 
evaluation metrics, determine which categorical variable best describes the groups formed.

The categorical variable that best describes the groups is the vehicle class.
Reference:
1. C3 AI Glossary: https://c3.ai/glossary/data-science/f1-
score/#:~:text=Why%20is%20the%20F1%20Score,found%20in%20the%20other%20class.
2. Investopedia : https://www.investopedia.com/terms/r/rsquared.asp#:~:text=R%2Dsquared%20will%20give%20you,data%20and%20predictions%2
0are%20biased
