# 📧 Spam Mail Prediction Project

Welcome to the **Spam Mail Prediction Project**! This repository contains the code to classify emails as either **Spam** or **Ham** (non-spam) using a Logistic Regression model and TF-IDF vectorization. 📨

## 📋 Project Overview

Spam emails are a nuisance and pose security risks. The goal of this project is to build a machine learning model that can automatically detect spam emails from their content. Using the [Spam Mails Dataset](https://www.kaggle.com/datasets/venky73/spam-mails-dataset), we train a classification model to differentiate between spam and ham emails.

## 📂 Dataset

The dataset contains the following:
- `text`: The email content
- `label`: Label of the email (Spam or Ham)
- `label_num`: Numeric representation of the label (0 for Ham, 1 for Spam)

You can download the dataset [here](https://www.kaggle.com/datasets/venky73/spam-mails-dataset).

## 🛠️ Features

- **TF-IDF Vectorization**: Converts the email text into numerical format by weighting the importance of words.
- **Logistic Regression**: A simple yet effective binary classification model.
- **Accuracy Evaluation**: Measures the model's performance on both training and testing datasets.

## 🚀 Installation

To run the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/smebad/spam-mail-prediction.git
   ```
2. Navigate to the project directory:
  ``` cd spam-mail-prediction ```

## 📊 Model Performance
The Logistic Regression model achieves the following accuracy:

* Training Accuracy: 95%
* Test Accuracy: 93%

 ## 💡 Usage
You can use the trained model to predict whether new emails are spam or ham. Example usage:
``` test_data = ['Subject: hpl nom for january 9 , 2001 ( see attached file : hplnol 09 . xls )']
test_data_tfidf = tfidf.transform(test_data)

if lr.predict(test_data_tfidf) == 0:
    print("Ham e-mail")
else:
    print("Spam e-mail")
```
## 📈 Conclusion
This project provides a simple yet effective solution for detecting spam emails using machine learning. Future improvements could include:

* Trying more advanced models (e.g., SVM, Random Forest)
* Adding more text preprocessing steps to handle complex text patterns.

### ⭐ Don't forget to star the repo if you found this project useful!

