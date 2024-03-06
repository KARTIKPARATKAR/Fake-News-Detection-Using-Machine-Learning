# ******Fake News Detection using Machine Learing****** 
***

****Dataset**** Used is 
[here](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqazBGMjhPMllBdHRUd3ZBWWxoMDY1QXNFSG1zUXxBQ3Jtc0ttdUQ3elBhc01ybTBMMXhIcGtkdXBHQVpUd0JuaVR5dHRFZUtTVTc2NWJDQ01xeVByMUxia3I3VlhWeHFuR1VCVDFQT3hJZVhjTjF4eF9xdUJDZDlxU2pRM3lxN2JXeU1QRUR5QXVRcEhPWWZTNl8xRQ&q=https%3A%2F%2Fwww.kaggle.com%2Fc%2Ffake-news%2Fdata%3Fselect%3Dtrain.csv&v=nacLBdyG6jE)
***
## Problem Statement : 
We are living in a world of social media where lot of information is available. Those information/news have a capacity of changing the minds, making a wrong perspective or decision , being involved in a wrong things and disguduide the user. This work is done to detect those fake news and aware the social media user from such misinformation on the social media. So constructing a machine learning model which will tell the user whether the news is fake or not.
***
![fake news](https://github.com/KARTIKPARATKAR/Fake-News-Detection-Using-Machine-Learning/assets/100400207/f85dd273-231c-48a0-86ec-94d838a52ffe)
***
## **Steps involved in construction of the model are as follows:** ##

**1)Fake-News Dataset:**
Dataset is collected from Caggle: 
* Each news article has unique id

* Each news has its ows title

* Each news has text which might be wrong

* Each news has author

* Each news has label which make news whether it is true or false.

Zero(0) represents real news.

One(1) represents fake news.

**2)Importing Required Libraries:**
* re                  - re means regular expression which is a sequence of characters used to find text in a document or used as a search pattern.
* nltk                - natural language toolkit
* stopwords           - These are words which does not add much value to a paragraph or text.
* stemming            - Converting similar words to its stemmed word. Connect might be stemmed word of connects and connected.
* Tfidf Vectorizer    - Term Frequency and Inverse Document Frequency of a word. Tfidf counts the number of times the perticular word is occuring in a document.
* train_test_split    - Splitting dataset in training data and testing data.
* Logistic_regression - A ML model used to describe data and the relationship between dependant variable and one or more independant variable.
* Accuracy_score      - It ia a matrix that measures how often a machine learning model correctly predicts the output.

**2)Data Pre-Processing:**
* Loading of dataset in pandas dataframe.
* Finding null/missing values in each column of the dataset.
* Replacing null values with null strings using fillna function.
* Stemming is the process of reducing a word to its root word.Remove numeric values and characters present in the dataset.Convert the data in lower_case.
* Converting text data into feature vectors i.e. into equivalent numeric data with the help of Tfidf vectorizer.
* Splitting dataset into training data and testing data before feeding it to the machine learning model.

**3)Model Construction**
* As I have a problem of specifying whether a news is true or false , it is a predominantly a classification problem. Hence we will consider logistic regression model.
* Then I will train the model on training data and find the accuracy on training data.
* Similarly we will train the model on testing data and find the accuracy on tescting data.

**4)Model Evaluation:**
  I got a accuracy score of 0.98659 on training data and it is shown below.
  ![trainingData](https://github.com/KARTIKPARATKAR/Fake-News-Detection-Using-Machine-Learning/assets/100400207/68725337-2f4e-45a1-8cd7-43c8ed09c6e4)
  
  
  I got a accuracy score of 0.9790 on testing data and it is shown below.
  ![testData](https://github.com/KARTIKPARATKAR/Fake-News-Detection-Using-Machine-Learning/assets/100400207/29598724-4701-4678-9b8d-286146b00ed4)


  I have made a predictive system which will print the output as whether a news is fake or real and it is shown below.
  ![predictive system](https://github.com/KARTIKPARATKAR/Fake-News-Detection-Using-Machine-Learning/assets/100400207/f0bf10e2-7ddb-4f7d-aaf0-e9ef0bc2ca65)

  
  
  

