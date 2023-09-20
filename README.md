# Income_Classification
The aim of the project is to employ several supervised algorithms to accurately model individuals' income, whether he makes more than 50,000 or not, using data collected from the 1994 U.S. Census.
# The project poses some questions about this experiment:

1. Does an individual make more than 50k income or not?

2. What are the most important features that help to define the income of an individual?

# PROBLEM DEFINITION
The income classification and prediction problem is a supervised learning task that involves predicting whether an individual's income exceeds a certain threshold based on their demographic, education, and employment information. The goal is to develop a machine learning model that can accurately predict an individual's income level given their personal information.
# DATASET
The dataset used for this task  was extracted from the machine learning repository (UCI), which contains about 32561 rows and 15 features will include various features of individuals, such as age, education level, occupation, marital status, and sex, along with their corresponding income level. The dataset also include missing values, categorical variables, and outliers, which will need to be handled appropriately during data preprocessing.
# ARTIFICIAL INTELLIGENCE/MACHINE LEARNING MODEL IMPLIMENTED
In this task, we used three different machine learning classification model to test the best algorithm model. Once we have prepared the dataset, we can train and test different models using various performance metrics, such as accuracy and F1-score. Once we have trained and tested different models, we can compare their performance on the test set using accuracy and F1-score and select the algorithm that performs the best. 
The classification models used for this work are as follows;

•	Random Forest
•	Ada boost classifier
•	Logistic Regression
# EVALUATION
The data was split into training and testing parts of the features and the label with a test size of 20%, with a random state to get the same randomness with the next runs. Cross-validation was applied between the models to select the most suitable ones. This was done using the cross validate function with 5 folds splitting and outputs the train and test score of the model.
The metrics used for evaluation include;
•	Accuracy
•	F1-score 
In this task, Random-forest gave the best accuracy and F1-score metric than AdaBoost and logistic regression.
# ANALYSIS
We imported the necessary library used for this particular task into our environment, analyzed our data to get the information and structure of the data. Next, we cleaned our data by checking for null and duplicate values, we figured out there were duplicate values in our data so we dropped these values. After cleaning our data, we can say our data is ready for exploration. We checked the statistic of our data and realized that people with education classes of 9 & 10 make up the highest portion in the dataset. Also, we notice that people with education class of 14 to 16 proportionally usually make >50k as income in the statistics we have in the dataset, unlike lesser education classes where they usually make <=50k as income. We checked the average age of sex relative to income and realized that people with >50K has a higher average age than the ones with <=50K. And in both cases of income, we see that the male category has a little bit greater age average than the female category. We checked the average hours per week relative to income and notice that the income grows directly with the average of work hours per week, which is a pretty reasonable and logical result, now our data is ready to be pre-processed and ready for our models. The data has been scaled to MinMaxScalling for numerical features, which converts the data to have a range between 0 and 1. That would help to make the data well-prepared for the model. We converted the categorical data into numerical data using the one-hot encoding for better understanding of our result and to get a more numerical representation. From our evaluation using skewed data, random forest gave the highest accuracy score of 0.99% and an F1 score of 0.99% compared to logistic regression and adaboost. We used the random oversampling technique to balance our data and train our model. From our analysis random forest gave us a very good result when our data is balanced. We removed the least important feature to speed up the process of fitting the model.
From my observation, random forest performed better on both skewed and balanced data. We can confidently say random forest is the best model for this particular task.
![image](https://github.com/dannielabutu/Income_Classification/assets/94900548/821e6c61-1772-4f63-925e-4fd53d716898)
