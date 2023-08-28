# Spam Email Detection using Support Vector Machine (Machine Learning)
---
## Overview
This repository contains a machine learning model for detecting spam emails using the **_Support Vector Machine (SVM)_** algorithm. The model is built using the Python programming language and popular libraries such as *_pandas, scikit-learn, and CountVectorizer._*

## Table of Contents
- Introduction
- Problem Statement 
- Installation
- Usage
- Dataset
- Methodology
- Results
- Conclusion

## Introduction
Spam emails, also known as junk emails, are unwanted or unsolicited emails that are sent in bulk to a large number of recipients. These emails often contain advertisements, scams, or malicious content. This project aims to develop a machine learning model that can automatically classify emails as spam or non-spam based on their content.

## Problem Statement

- In today's digital landscape, the menace of spam emails has emerged as a critical concern, inundating inboxes with unsolicited and often malicious content.
- The ability to efficiently identify and segregate spam from legitimate emails has become imperative to ensure user experience, data security, and operational efficiency.
- Manual identification of spam is arduous and time-consuming, necessitating an automated solution that can swiftly and accurately classify emails.
- This project seeks to develop a robust machine learning model that can effectively discern between spam and non-spam emails, contributing to the mitigation of this pervasive issue and enhancing the overall email ecosystem.
- Through the utilization of advanced techniques and algorithms, the aim is to construct a solution that empowers users to confidently interact with their email platforms while mitigating the risks associated with spam content.

## Installation
To use the code provided in this repository, you need to have Python and the required libraries installed. You can install the necessary libraries using the following command:
```
pip install pandas scikit-learn
```
Use train-test split method to train our email spam detector to recognize and categorize spam emails.
We can use it for either classification or regression of any supervised learning algorithm.
- **Train dataset:** used to fit the machine learning model.
- **Test dataset:** used to evaluate the fit of the machine learning model.

## Usage
- Clone this repository to your local machine.
- Place the 'spam.csv' dataset file in the same directory as the project files.
- Open a terminal or command prompt.
- Navigate to the project directory.
- Run the following command to execute the spam email detection model:
```
python spam_detection.py
```
*_SVM, the support vector machine algorithm, is a linear model for classification and regression.
The idea of SVM is simple, the algorithm creates a line, or a hyperplane, which separates the data into classes. SVM can solve both linear and non-linear problems:_*


![image](https://github.com/nerkaratharva/Detection-of-Spam-Email-using-SVM-Machine-Learning-/assets/112231555/46bb94e8-62f2-49bd-9060-fa127bbdc7cf)

## Dataset
- The dataset used for training and testing the model is stored in the 'spam.csv' file. 
- This dataset contains two columns: 'v1' (label) and 'v2' (email content). 
- The 'v1' column contains labels indicating whether an email is spam or not, while the 'v2' column contains the email content.

## Methodology
- The dataset is loaded using the pandas library, and it is split into training and testing sets using the train_test_split function from scikit-learn.
- The email content from the training set is transformed into a numerical format using the CountVectorizer.
- This technique converts the text data into a matrix of word counts.
- A Support Vector Machine (SVM) model is initialized using the svm.SVC class from scikit-learn.
- The SVM model is trained on the transformed training data using the fit method.
- The email content from the testing set is also transformed using the same CountVectorizer instance.
- The model's accuracy is evaluated on the testing set using the model.score method.

## Results
Upon completion of training and testing, the spam email detection model yields its accuracy, prominently displayed in the console. This accuracy serves as a decisive metric, reflecting the proportion of accurately categorized emails within the testing dataset. It stands as a testament to the model's proficiency in distinguishing between spam and legitimate emails. This pivotal outcome underscores the model's efficacy in addressing the intricate challenge of email classification, with potential implications for bolstering email security and user experience.

## Conclusion
This project demonstrates the use of machine learning, specifically the Support Vector Machine algorithm, for detecting spam emails. By utilizing the CountVectorizer to transform text data into a suitable format, the model is able to achieve a certain level of accuracy in identifying spam emails. Further improvements could be made by exploring more advanced text processing techniques and experimenting with different machine learning algorithms.
