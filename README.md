# Twitter-Sentiment-Analysis
## 🔰 Introduction

Sentiment analysis refers to identifying as well as classifying the sentiments that are expressed in the text source. Tweets are often useful in generating a vast amount of sentiment data upon analysis. These data are useful in understanding the opinion of the people about a variety of topics.

Therefore, we need to develop an **Automated Machine Learning Sentiment Analysis Model** in order to compute the customer perception. Due to the presence of non-useful characters (collectively termed as *noise*) along with useful data, it becomes difficult to implement models on them.

## 🎯 Objective

We aim to analyze the sentiment of the tweets provided from the **Sentiment140** dataset by developing a Machine Learning model involving the use of three classifiers:

- **Logistic Regression (LR)**
- **Bernoulli Naive Bayes (BNB)**
- **Support Vector Machine (SVM)**

Along with using **Term Frequency-Inverse Document Frequency (TF-IDF)**.

The performance of these classifiers is then evaluated using:

- **Accuracy**
- **ROC-AUC Curve**
- **F1 Scores**
## DataSet Used  <a href="https://www.kaggle.com/datasets/kazanova/sentiment140?resource=download">Click Here</a>

## 📚 Project Pipeline

The various steps involved in the Machine Learning Pipeline are:

1️⃣ **Import Necessary Dependencies**  
2️⃣ **Read and Load the Dataset**  
3️⃣ **Exploratory Data Analysis**  
4️⃣ **Data Visualization of Target Variables**  
5️⃣ **Data Preprocessing**  
6️⃣ **Splitting our Data into Train and Test Subset**  
7️⃣ **Transforming Dataset using TF-IDF Vectorizer**  
8️⃣ **Function for Model Evaluation**  
9️⃣ **Model Building**  
🔟 **Conclusion**

## 🏗️ Model Building

In this project, we have used three different classification models:

- **Bernoulli Naive Bayes (BNB)**
- **Support Vector Machine (SVM)**
- **Logistic Regression (LR)**

### 💡 Rationale Behind Model Selection

The idea behind choosing these models is to experiment with a range of classifiers — from **simple** to **complex** — and evaluate their performance on the sentiment analysis task.

This helps us identify the model that performs the best in terms of accuracy, robustness, and generalization on unseen data.


## Model Evaluation

After training the model, we then apply evaluation measures to check how the model is performing. We use the following evaluation parameters to assess the performance of the models:

### 📌 Accuracy Score
- Typically, the accuracy of a predictive model is considered good if it achieves above **90% accuracy**.

### 📌 ROC-AUC Curve
- The **Area Under the Curve (AUC)** measures the ability of a classifier to distinguish between classes.
- It serves as a summary of the ROC curve.
- The **higher the AUC**, the better the model performs at distinguishing between the positive and negative classes.

### 📌 Confusion Matrix with Plot
- A **Confusion Matrix** is an *N x N* matrix used to evaluate the performance of a classification model, where **N** is the number of target classes.
- The matrix compares the **actual target values** with those **predicted** by the model.

#### Matrix Layout:
|               | Actual Positive | Actual Negative |
|---------------|------------------|------------------|
| **Predicted Positive** | True Positive (TP) | False Positive (FP) |
| **Predicted Negative** | False Negative (FN) | True Negative (TN) |

- **Rows** represent **predicted values**.
- **Columns** represent **actual values**.


## ✅ Conclusion

We therefore conclude that **Logistic Regression** is the best-performing model for the given dataset, although it took significantly longer to run compared to the other models.

In our problem statement, **Logistic Regression** adheres to **Occam's Razor principle**, which states that *among competing models that perform similarly, the simplest one should be preferred*. 

Since our dataset makes no strong assumptions and Logistic Regression is a relatively simple and interpretable model, this principle holds true for the sentiment analysis task based on the Sentiment140 dataset.
