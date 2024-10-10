Fake Email Detector Using Machine Learning
Developed a spam detection model using logistic regression, achieving high accuracy by leveraging TF-IDF vectorization and label encoding techniques. Phishing detection is critical in cybersecurity to identify and mitigate fraudulent activities.

Key Features
Dataset: Loaded using pandas. The dataset mail_data.csv contains email messages categorized as 'spam' or 'ham'.

Missing Values: Handled by replacing any missing values with empty strings.

Label Encoding: Converted the 'Category' column to numerical values, where 'spam' is 0 and 'ham' is 1.

Feature Extraction: Used TF-IDF vectorization to transform text data into numerical features.

Model Training: Trained a Logistic Regression model on the training data and evaluated its accuracy on both training and testing datasets.

Predictions: Capable of predicting the category of new email messages
