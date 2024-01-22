
## Heart Disase
It is predicted that heart disease, one of the most common diseases in the world, will continue to
be the number one cause of death for a long time. The fact that many of the factors of heart disease
can be prevented or treated is an opportunity to decrease the loss of life as a result of the disease.
For this reason, many studies aimed at detecting the disease by applying algorithmic and statistical
methods to case data have been conducted. The aim of this study is to examine the relationship
between the characteristics determined and the diagnosis of heart attack and to predict the
diagnosis of a heart attack at the maximum level. The values in the data set with 12 qualities and
303 cases were cleared and then analyzes were made. It has been found that the characteristics of
chest pain type, exercise-induced angina, and exercise-induced ST depression have a high rate of
correlation with the diagnosis of a heart attack. Analysis results were visualized and added to the
study. For the diagnosis of heart attack, 4 different algorithms were applied, namely the C4.5
decision tree, k-nearest neighbor, random forest, and SVM, which were successful in other
studies, and their results were compared. The C4.5 decision tree algorithm has been the most
accurate algorithm for predicting heart attack diagnosis. According to World Health Organization (WHO) data,
deaths due to cardiovascular diseases take the first place among all deaths with 30 percent. In our country, 
this rate is around 47 percent . Myocardial infarction (MI), which is one of the coronary artery diseases and popularly called heart attack,
occurs as a result of disruption of blood supply or oxygenation of a part of the heart.
It is a disease. In other words, it is caused by the insufficient amount of blood and therefore oxygen reaching the heart.
When there is not enough oxygen, damage to the heart occurs, and when there is no oxygen for a long time, death occurs in the heart.


### Posing a risk of death or adversely affecting human health
The main causes of this disease, which affects
can be listed as follows :
- Obesity
- Hypertension
- Diabetes
- Cholesterol
- Gender
- Age
- Tobacco use
- Alcohol use
- Family history



      -«Aksi ispat edilene kadar göğüs ağrısı olan her hasta acildir ve mortalitesi yüksektir.»
       Araş. Gör. Dr. Havva ŞEN


The purpose of this study is to examine age, gender, type of chest pain,
resting blood pressure, cholesterol value, fasting blood
blood sugar, resting electrocardiographic result,
maximum heart rate, exercise-induced angina, exercise-induced
related ST depression, ST segment slope and defect type
To examine the relationship between heart attack characteristics and heart attack diagnosis
and diagnose heart attack with maximum accuracy.
is to guess. Data pre-processing within the scope of the study
was made and the data was organized and analyzed.
Analysis results are visualized and
has been added. Decision tree for diagnosis prediction, k-en
nearest neighbor, Naive Bayes, Logistic regression
machine algorithms were used. 

## Process 
Data cleansing
Data cleaning is a process that must be done before data analysis. It consists of processes such as completing missing data, eliminating inconsistencies, and removing noise to detect outliers. Missing
The following methods can be used to complete the data:
 Records containing missing values can be deleted.
 The mean can be used instead of missing values.
 Median can be used instead of missing values.
 The average of the class in which it is located can be used instead of missing values.
 Instead of missing values, the most appropriate value can be used using methods such as regression.

Our Dataset was clean that's why we didnt cleaning much.

# Decide which Machine Learning Algorithm is suitable for our dataset
I chosed Calassification algoritm because:
The Classification algorithm is a Supervised Learning technique that is used to identify the category of new observations on the basis of training data. In Classification, a program learns from the given dataset or observations and then classifies new observation into a number of classes or groups. Such as, Yes or No, 0 or 1, Spam or Not Spam, cat or dog, etc. Classes can be called as targets/labels or categories.
We have column name as Target and we are trying to predict it that s why I chosed that.

I wanted to make comparisons and gain experience by using more than one algorithm.
I wanna give short information about them ...




# What is a Decision Tree?


Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features. A tree can be seen as a piecewise constant approximation.

# Some advantages of decision trees are:

- Simple to understand and to interpret. Trees can be visualized.
- Requires little data preparation. Other techniques often require data normalization, dummy variables need to be created and blank values to be removed. Some tree and algorithm combinations support missing values.

# The disadvantages of decision trees include:

Decision-tree learners can create over-complex trees that do not generalize the data well. This is called overfitting. Mechanisms such as pruning, setting the minimum number of samples required at a leaf node or setting the maximum depth of the tree are necessary to avoid this problem.





# What is a Naive Bayes?
  Naive Bayes is a statistical classification technique based on Bayes Theorem. It is one of the simplest supervised learning algorithms. Naive Bayes classifier is the fast, accurate and reliable algorithm. Naive Bayes classifiers have high accuracy and speed on large datasets.

#  Advantages
- Less complex: Compared to other classifiers, Naïve Bayes is considered a simpler classifier since the parameters are easier to  estimate. As a result, it’s one of the first algorithms learned within data science and machine learning courses.   
- Scales well: Compared to logistic regression, Naïve Bayes is considered a fast and efficient classifier that is fairly accurate when the conditional independence assumption holds. It also has low storage requirements. 
- Can handle high-dimensional data: Use cases, such document classification, can have a high number of dimensions, which can be difficult for other classifiers to manage. 

 # Disadvantages:   
- Subject to Zero frequency: Zero frequency occurs when a categorical variable does not exist within the training set. For example, imagine that we’re trying to find the maximum likelihood estimator for the word, “sir” given class “spam”, but the word, “sir” doesn’t exist in the training data. The probability in this case would zero, and since this classifier multiplies all the conditional probabilities together, this also means that posterior probability will be zero. To avoid this issue, laplace smoothing can be leveraged. 
- Unrealistic core assumption: While the conditional independence assumption overall performs well, the assumption does not always hold, leading to incorrect classifications. 

# What is K-Nearest Neighbors?
K-Nearest Neighbors (KNN) is a supervised machine learning model that can be used for both regression and classification tasks.
The algorithm is non-parametric, which means that it doesn't make any assumption about the underlying distribution of the data.

The KNN algorithm predicts the labels of the test dataset by looking at the labels of its closest neighbors in the feature space of the training dataset. The “K” is the most important hyperparameter that can be tuned to optimize the performance of the model.
The KNN classification algorithm works by finding K neighbors (closest data points) in the training dataset to a new data point. Then, it assigns the label of the majority class among neighbors to new data points.

# Advantages
- Easy to implement: Given the algorithm’s simplicity and accuracy, it is one of the first classifiers that a new data scientist will learn.
- Adapts easily: As new training samples are added, the algorithm adjusts to account for any new data since all training data is stored into memory.

- Few hyperparameters: KNN only requires a k value and a distance metric, which is low when compared to other machine learning algorithms.

# Disadvantages
- Does not scale well: Since KNN is a lazy algorithm, it takes up more memory and data storage compared to other classifiers. This can be costly from both a time and money perspective. More memory and storage will drive up business expenses and more data can take longer to compute. While different data structures, such as Ball-Tree, have been created to address the computational inefficiencies, a different classifier may be ideal depending on the business problem.

- Curse of dimensionality: The KNN algorithm tends to fall victim to the curse of dimensionality, which means that it doesn’t perform well with high-dimensional data inputs. This is sometimes also referred to as the peaking phenomenon (link resides outside of ibm.com), where after the algorithm attains the optimal number of features, additional features increases the amount of classification errors, especially when the sample size is smaller.

- Prone to overfitting: Due to the “curse of dimensionality”, KNN is also more prone to overfitting. While feature selection and dimensionality reduction techniques are leveraged to prevent this from occurring, the value of k can also impact the model’s behavior. Lower values of k can overfit the data, whereas higher values of k tend to “smooth out” the prediction values since it is averaging the values over a greater area, or neighborhood. However, if the value of k is too high, then it can underfit the data. 



# What is logistic regression?
This type of statistical model (also known as logit model) is often used for classification and predictive analytics. Logistic regression estimates the probability of an event occurring, such as voted or didn’t vote, based on a given dataset of independent variables. Since the outcome is a probability, the dependent variable is bounded between 0 and 1. In logistic regression, a logit transformation is applied on the odds—that is, the probability of success divided by the probability of failure. This is also commonly known as the log odds, or the natural logarithm of odds, and this logistic function is represented by the following formulas: 

Logit(pi) = 1/(1+ exp(-pi))

ln(pi/(1-pi)) = Beta_0 + Beta_1*X_1 + … + B_k*K_k

In this logistic regression equation, logit(pi) is the dependent or response variable and x is the independent variable. The beta parameter, or coefficient, in this model is commonly estimated via maximum likelihood estimation (MLE). This method tests different values of beta through multiple iterations to optimize for the best fit of log odds. All of these iterations produce the log likelihood function, and logistic regression seeks to maximize this function to find the best parameter estimate. Once the optimal coefficient (or coefficients if there is more than one independent variable) is found, the conditional probabilities for each observation can be calculated, logged, and summed together to yield a predicted probability. For binary classification, a probability less than .5 will predict 0 while a probability greater than 0 will predict 1.  After the model has been computed, it’s best practice to evaluate the how well the model predicts the dependent variable, which is called goodness of fit. The Hosmer–Lemeshow test is a popular method to assess model fit.


### After apply our modul we need to control it s suitable for our dataset we need to use some metrics .Those are ...


# Accuracy
Accuracy is defined as the ratio of the number of correct predictions to the total number of predictions. This is the most fundamental metric used to evaluate the model. The formula is given by

Accuracy = (TP+TN)/(TP+TN+FP+FN)
However, Accuracy has a drawback. It cannot perform well on an imbalanced dataset. Suppose a model classifies that the majority of the data belongs to the major class label. It yields higher accuracy. But in general, the model cannot classify on minor class labels and has poor performance.

# Precision and Recall
Precision is the ratio of true positives to the summation of true positives and false positives. It basically analyses the positive predictions.
Precision = TP/(TP+FP)
The drawback of Precision is that it does not consider the True  Negatives and False Negatives.

Recall is the ratio of true positives to the summation of true positives and false negatives. It basically analyses the number of correct positive samples.

Recall = TP/(TP+FN)
The drawback of Recall is that often it leads to a higher false positive rate.

# F1 score
The F1 score is the harmonic mean of precision and recall. It is seen that during the precision-recall trade-off if we increase the precision, recall decreases and vice versa. The goal of the F1 score is to combine precision and recall. 

F1 score = (2×Precision×Recall)/(Precision+Recall)

## When we look at the evaluation modules of the models we apply, in my opinion, the algorithm that makes the most accurate decisions is the decision tree and then the KNN algorithm.

FOR MORE INFORMATION YOU CAN VISIT SOURCE LINK BELOW


# SOURCE 

- https://dergipark.org.tr/en/download/article-file/1461309
- https://www.ibm.com/
- https://scikit-learn.org/
- https://www.jeremyjordan.me/evaluating-a-machine-learning-model/
- https://www.geeksforgeeks.org/machine-learning-model-evaluation/r