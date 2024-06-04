# SENTIMENT ANALYSIS MODEL FOR AMAZON PRODUCTS

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Model Selection](#model-selection)
- [Conclsion](#conclusion)
- [Limitations](#limitations)

### Project Overview

The objective of this project is to build a sentiment analysis model to clasify product reviews as psitive, negative, or neutral.
The goal is to automatically analyze and categorize customer feedback to help business understand customer sentiment and improve product offerings.

### Data Sources

Amazon Product Review: The primary dataset used for this project is the "Amazon-Product-Reviews - Amazon Product Review (1).csv" file, containing detailed information on reviews given by customers who have purchased products from the Amazon website.

  -[Download here](https://www.kaggle.com/datasets/miriamodeyianypeter/sentiment-analysis-amazon-product-reviews)

### Tools

- Jupyter Notebook - Data Cleaning and Preparation - Text Cleaning and Preprocessing  - Model Training and Evaluation

### Data Cleaning and Preparation

In the initial data preparation phase, i perform the following tasks:
1. Importation of all the neccessary libraries
2. Data loading and inspection
3. Selected important variables for the data processing
4. Handling missing and duplicate values
5. Data cleaning and formating
6. Text cleaning and preprocessing
7. Data splitting into Training and Testing 
8. Label encoding

### Model Selection

#### Model training and evaluation
- This is done using:
  1. Logistic Regression with Hyperparameter & Countvectorizer
  2. Naive-Bays Model with Hyperparameters & Countvectorizer
  3. Logistic Regression with Hyperparameter & TfidfVectorizer
  4. Naive-Bays Model with Hyperparameters & TfidfVectorizer

### Conclusion

- The best model chosen for the project is LogisticRegression with Hyperparameter(C=10) and Countvectorizer (with a train and test accuracy of 86% and 82% respectively

  ![Confusion Matrix](confusion_matrix.JPG)

  ![confusion_matrix](https://github.com/BABALOLAbasit/ingryd_capstone_project/assets/140013199/03ddc166-6ee0-4f59-8672-5f24aa819e79)


### Limitations

I had to resample to balance the data set, this is because the data was bias towards positive review significantly and that could have affected the accuracy of the model. This bias reduces the model's ability to generalize well to real-world data with a more balanced or different distribution.
  
