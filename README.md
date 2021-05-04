# Cancer-Prediction Projct Overview
Machine Learning technique can dramatically improve the level of diagnosis in breast cancer.
I used SVM and Logistic Regression to build a model that detects cancer.

## Code and Resources Used
**Python Version:** `3.8.6`

**Packages:** `pandas, numpy, matplotlib, seaborn, sklearn`



## Data Cleaning
After loading the data, I did a basic cleaning making the following changes:
* removed redundant features,
* checked for any null values

## EDA
I used seaborn library to plot the relationship between our features. 
Because all of the plots are linearly separable I used binary linear classification models: a Support Vector Machine (SVM) Model and a Logistic Regression Model. SVM performed better as is well suited for classification of small/medium sized datasets.
I checked if the dataset needed to be balanced or not - even though the majority of people in our dataset has no cancer, the dataset it balanced.


## Model Building
First, I performed Feature Selection - dropping highly correlated features. I then did Feature Scaling for better performance using MinMaxScaler. I also split the data (to prevent overfitting) into train and test subsets with a test size of 20%.

I built two models: SVM and Ligistic Regression.

## Model performance
The accuracy score for SVM and Logistic Regression is around 99% and 96% respectively.
SVM model performs better in this case.
There is always a room for improvement. One could use Hyperparameter Tuning in order to further optimize the model.
