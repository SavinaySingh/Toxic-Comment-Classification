# Toxic Comment Classification
<img width="482" alt="image" src="https://github.com/SavinaySingh/Toxic-Comment-Classification/assets/21008903/d905d299-69d3-4a72-aac4-3f4699f96622">

This repository contains a Jupyter Notebook file (toxic-comment-classification-v01.ipynb) that involves analyzing text comments to determine whether they contain toxic or offensive language. The goal of this task is to develop a model that can accurately identify and flag such comments, with the aim of reducing the prevalence of online harassment, hate speech, and other forms of toxic behavior. This is achieved by employing a classification ML model that can accurately classify online comments as toxic or non-toxic based on their content. The extension to this project involves censoring or masking inappropriate language in the dataset by replacing toxic words with asterisks instead of entirely removing them. 

# Dataset
The dataset used for training and evaluation consists of comments from various online platforms, annotated with labels indicating whether they are toxic or not. The dataset is split into training, validation, and test sets to ensure the model's performance is robust across different data partitions.

Dataset Source: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data

# NLP Methods and Techniques
1. Data Pre-processing
Check for Missing Values: Handle missing data to ensure accurate statistical analysis.
Data Cleaning: Employ various methods, including abbreviation handling, lowercasing, apostrophe handling, numeric value removal, punctuation removal, Unicode removal, removal of non-English alphabets, lemmatization, and stopwords removal.
2. Vectorization
Utilize TF-IDF (Term Frequency-Inverse Document Frequency) for transforming text data into numerical feature vectors.
3. Class Resampling
Address imbalanced data using the Synthetic Minority Over-Sampling Technique (SMOTE) to improve classifier performance.
4. Classification Models
Employ XGBoost, Logistic Regression, and Random Forest classification models.
Select XGBoost as the final model based on model evaluation, with a focus on achieving high recall.
5. Model Evaluation
Assess model performance using accuracy scores.
Choose XGBoost as the final model, emphasizing high recall for identifying negative or hate words.
6. Text Filtering and Masking
Modify text by replacing toxic words with asterisks to prevent the spread of hate speech.
Hyperparameter tuning, including adjusting scale_pos_weight to control the impact of positive and negative classes on the model.

## Dependencies
- Python 3.8.2
- Required Python packages specified in requirements.txt.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

# Group Members
- Savinay Singh
- Divgun Singh
- Sagar Sudhir Bhagwatkar
- Somayeh Amraee
