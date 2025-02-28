## Overview
Fake news detection is a crucial task in today's digital world, where misinformation spreads rapidly. This project focuses on classifying news headlines as real or fake using Natural Language Processing (NLP) techniques and machine learning models. By processing text data, extracting meaningful features, and applying classification algorithms, we aim to build an efficient model for detecting fake news.

## Dataset
The dataset used in this project contains 72,134 rows and includes four columns: id, title, text, and label. The title column contains the news headlines, while text holds the complete article content. The label column indicates whether the news is real or fake. To clean the dataset, we handled missing values by dropping rows with null text fields and replacing other missing values with empty strings where necessary.

## Data Preprocessing
To prepare the text data for machine learning models, we applied multiple preprocessing steps. We used the Natural Language Toolkit (NLTK) to remove stopwords, reducing noise in the dataset. Additionally, stemming was performed using the PorterStemmer algorithm to normalize words to their root forms. Regular expressions were employed to eliminate special characters and ensure consistent formatting. Finally, we applied Term Frequency-Inverse Document Frequency (TF-IDF) vectorization to convert text into numerical features, allowing machine learning models to process the data effectively.

## Model Selection and Training
Two classification models were implemented to evaluate their effectiveness in fake news detection: Logistic Regression and Decision Tree Classifier. The dataset was split into training and testing sets to assess model performance. Logistic Regression achieved an accuracy of approximately 89.95%, while the Decision Tree Classifier reached 87.05%. Based on these results, Logistic Regression was selected as the preferred model due to its higher accuracy. Future improvements could include hyperparameter tuning and experimenting with additional algorithms to further enhance performance.

## Conclusion
This project demonstrates the application of NLP and machine learning techniques in detecting fake news. By utilizing text preprocessing methods and classification models, we achieved a strong baseline for identifying misinformation. Further enhancements, such as hyperparameter optimization and deep learning approaches, could improve accuracy and robustness. This work contributes to the growing field of automated misinformation detection, offering potential real-world applications in media and journalism.
