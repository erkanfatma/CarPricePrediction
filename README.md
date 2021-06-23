# CarPricePrediction

## Introduction
Specifying if the listed price of a car is a difficult task due to the many features that drive a used vehicle’s price on the market. The main point of this homework is to develop a machine learning model that can predict the price of a used var based on the factors of it to make informed purchases. I implement code statements that contains decision trees model and I used a dataset which consist of some features called Model, Year, Price, Transmission, Mileage, Fuel Type, Tax, Mpg, Engine Size to train and I evaluated the results. 

When looking at the online lists, it is difficult to decide if a used car is worth the posted price. Many features such as model, year, engine size and others can influence the real worth of a car. A dilemma also occurs to define a price for a used car by a car seller. Depending on the training data, the main goal is to use decision tree which is a machine learning model to implement models to predict car prices.

## Dataset
To train model, “train.csv” dataset is used to train and “test.csv” file is used to test it. Available attributes in the dataset are Model, Year, Price, Transmission, Mileage, Fuel Type, Tax, Mpg and Engine Size. 

## Decision Trees
Decision tree is a modelling approaches which used in machine learning and data mining. Decision trees identify ways to separate dataset depend on different conditions. This approach is most popular method for supervised learning. It is used for classification and regression tasks. The goal pf decision trees are to find the optimum value of a variable via extract rules from features of dataset. When creating decision tree, each node has different type of question. Depend on the question, information will be calculated to correspond to it. This information is used to make a decision which attribute to separate on each step to build a tree. As always, simplicity is best so that the tree will be small enough. For that, in each point choose the split that results in the purest children nodes. 

The first node on the tree separates the data depend on most effective attribute. For this, there are 2 important property occurs. The first one is Entropy and the second one is Gini Impurity.

1. Entropy
It is a measurement of uncertainty of the data. In decision tree, data will be divided into parts depend on minimizing entropy value. If entropy value close to 0, result of the algorithm will be better than others. 

If elements in a set is the same value, then the value of Entropy is 0. On the other hand, if elements separated into parts with equal values, then the Entropy value is 1. As shown entropy have a value between 0 and 1. 

2.	Gini Impurity
 This method calculates the inequality. If all elements are homogeneous, then the Gini value will be 0. If inequality value is maximum, then the Gini value is 1. 

Gini impurity is the measurement of possibility of incorrect classification of the instance of random variable in the data set. 


## Results

Decision trees were implemented in python to predict car prices. Decision trees can be used both classification and regression. It can catch the non-linear relationship between attributes and the target value. It also does not require rescaling of features.

![alt text](https://github.com/erkanfatma/CarPricePrediction/blob/main/img/Picture1.png)

Figure in the above shows that the test data which is used to test. There are over 3000 data in the document. This dataset provides information about Cars and its features to predict price of the car. As seen, I used Model, Year, Price, Transmission, Mileage, Fuel Type, Tax, Mpg and Engine Size to predict car price. I needed to convert string values to integer values, and I controlled the drop any rows that include missing values. 

![alt text](https://github.com/erkanfatma/CarPricePrediction/blob/main/img/Picture2.png)

In this assignment, first the data will be used to train the algorithm and prepared to analyze it. Using Scikit-Learn library the predicted property assigned as ‘Price’. Remained features were assigned to separate variables to train and test the model. X and Y used to assign variables that X is a matrix of features to predict the price and Y is a vector made up of the data to find best prediction.  I changed model, transmission and fuel type data to integer data as seen in the code above. To get this integer value method that is called LabelEncoder used. A method named ‘pairplot’ was implemented to generate scatterplot matrix. Their histograms are shown in the below figure. 

The figure contains some graphics that shows the changing of features to other features. For instance, the second graph that is located in first row and second column shows that the model changing depend on year. 

![alt text](https://github.com/erkanfatma/CarPricePrediction/blob/main/img/Picture3.png)

I was used my datasets as train and test. It means I have 4 different sets called as X_train, X_test, Y_train and Y_test. Fit method was implemented to train the algorithm using dataset inside of ‘train.csv’. To test the model dataset is used inside of ‘test.csv’. 

The successful rate of the test data nearly 84%. The output as shown in figure below. Originals are shown by red color and predictions are shown as green color.

![alt text](https://github.com/erkanfatma/CarPricePrediction/blob/main/img/Picture4.png)

Decision tree model of the algorithm is shown in the figure below. The graph of the dataset is too large so that the small part of the graph is seen. 

![alt text](https://github.com/erkanfatma/CarPricePrediction/blob/main/img/Picture5.png)

