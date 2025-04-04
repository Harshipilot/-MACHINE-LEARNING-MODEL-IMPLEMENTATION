# -MACHINE-LEARNING-MODEL-IMPLEMENTATION

*COMPANY*: CODETECH IT SOLUTIONS

*NAME*: HARSHITH

*INTERN ID*: CT04WU173

*DOMAIN*: PYHTON PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

**Spam Email Detection: Machine Learning Model Implementation
The objective of this project is to build a machine learning model capable of detecting spam emails (or SMS messages) from legitimate (ham) ones. Spam email detection is a crucial task for email services to help users filter out unwanted content and protect against potential security threats, such as phishing and malicious attachments. In this project, we utilize the Scikit-learn library, a powerful tool for machine learning in Python, to create a spam classifier using a popular dataset known as the SMS Spam Collection.

Dataset Overview
The dataset used in this project is the SMS Spam Collection, which contains a set of SMS messages labeled as either "spam" or "ham" (legitimate). The dataset includes over 5,000 messages, where each message is categorized based on its content. The primary challenge is to develop a machine learning model that can distinguish between these two classes accurately. The dataset contains two columns: Label (indicating whether a message is spam or ham) and Message (the content of the SMS). The goal is to train a model that predicts the label (spam or ham) of a new, unseen message based on its content.

Data Preprocessing
The raw data is text-based, which requires preprocessing before it can be fed into the machine learning model. First, the dataset is loaded, and the labels are converted from categorical strings ('spam' and 'ham') into binary numerical values (1 for spam, 0 for ham). The text data in the Message column must also be converted into numerical features. This is achieved through the CountVectorizer from Scikit-learn, which converts each message into a vector of word counts, essentially creating a Bag of Words representation. Additionally, common stop words (like "the", "a", "is") are removed to ensure that only the most relevant words contribute to the model.

Model Selection
For this project, the Multinomial Naive Bayes (NB) algorithm is chosen. Naive Bayes is a simple but effective algorithm for text classification tasks, particularly when the features are conditionally independent given the class, which holds in many text-based problems. It calculates the probability of a message belonging to each class (spam or ham) and assigns the label with the highest probability. The Multinomial Naive Bayes classifier is well-suited for text classification problems as it handles discrete feature sets (like word counts) effectively.

Model Training and Evaluation
The data is split into a training set (80%) and a testing set (20%) using train_test_split from Scikit-learn. The training set is used to train the Naive Bayes model, while the testing set serves to evaluate its performance. After training the model, predictions are made on the test data, and its performance is evaluated using several key metrics:
**

*output*

![Image](https://github.com/user-attachments/assets/4c4d12d7-2745-4916-b65d-3e66aa94af2d)
