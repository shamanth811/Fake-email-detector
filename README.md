# Fake-email-detector
Developed a spam detection model using logistic regression, achieving high accuracy by leveraging TF-IDF vectorization and label encoding techniques. Phishing detection is critical in cybersecurity to identify and mitigate fraudulent activities.

Key Features
Dataset: Loaded using pandas. The dataset mail_data.csv contains email messages categorized as 'spam' or 'ham'.

Missing Values: Handled by replacing any missing values with empty strings.

Label Encoding: Converted the 'Category' column to numerical values, where 'spam' is 0 and 'ham' is 1.

Feature Extraction: Used TF-IDF vectorization to transform text data into numerical features.

Model Training: Trained a Logistic Regression model on the training data and evaluated its accuracy on both training and testing datasets.

Predictions: Capable of predicting the category of new email messages.

Usage
Load Dataset:

python
Copy code
import pandas as pd
df = pd.read_csv('mail_data.csv')
Handle Missing Values:

python
Copy code
data = df.where((pd.notnull(df)), '')
Label Encoding:

python
Copy code
data.loc[data['Category'] == 'spam', 'category'] = 0
data.loc[data['Category'] == 'ham', 'category'] = 1
Feature Extraction and Model Training:

python
Copy code
from sklearn.model_selection import train_test_split
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score

# Continue with data processing and model training...
Predict New Data:

python
Copy code
input_your_mail = ["Your input email message here"]
input_data_features = feature_extraction.transform(input_your_mail)
prediction = model.predict(input_data_features)
Requirements
Python 3.x
Libraries: pandas, scikit-learn
Contributing
Feel free to submit issues and pull requests to improve the project!
