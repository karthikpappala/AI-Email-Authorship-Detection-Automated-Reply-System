AI Email Authorship Detection & Automated Reply System
📌 Overview

This project builds an AI-based system that identifies the likely author of an email and generates an automated reply. The system leverages Natural Language Processing (NLP), stylometric analysis, and machine learning classifiers to detect authorship patterns in emails and assist in automated response generation.

The project demonstrates an end-to-end data science pipeline including:

Data preprocessing

Exploratory Data Analysis (EDA)

Feature engineering (stylometric features)

Model training and evaluation

Deployment-ready ML pipeline

🎯 Objectives

Detect the authorship of an email using text-based features

Analyze writing style using stylometric features

Train multiple ML models and compare performance

Build a final deployable pipeline

Save the trained model for real-world usage

📂 Dataset

The project uses an email dataset containing:

Email text

Author labels

Intent categories

(If you have a specific dataset name, you can add it here.)

🔍 Methodology
1️⃣ Data Preprocessing

Text cleaning (removal of punctuation, special characters, etc.)

Handling missing values

Creating a full_text field for modeling

2️⃣ Exploratory Data Analysis (EDA)

Visualizations performed:

Distribution of authorship labels

Distribution of email intent

Histograms of stylometric features

Box plots comparing writing styles across authors

3️⃣ Feature Engineering (Stylometry)

Extracted features such as:

Text length

Average word length

Sentence count

Repetition percentage

Passive voice ratio

These features help capture unique writing styles of different authors.

4️⃣ Model Training

Multiple classifiers were trained and compared:

Logistic Regression

Decision Tree

Random Forest

Multinomial Naïve Bayes

TF-IDF vectorization was used to convert text into numerical features.

5️⃣ Hyperparameter Tuning

Grid Search was applied to improve Logistic Regression performance.

6️⃣ Final Deployable Pipeline

A final ML pipeline was created using:

TF-IDF Vectorizer + Logistic Regression


The trained model was saved using joblib for future inference.

🧠 Results

The Random Forest and Logistic Regression models performed best in authorship detection.

Stylometric features significantly improved model interpretability.

The final model is ready for deployment.

🚀 How to Run the Project
Install dependencies:
pip install pandas numpy scikit-learn nltk spacy matplotlib seaborn joblib

Run the Jupyter Notebook:
jupyter notebook "project (3).ipynb"

📁 Project Structure
📂 AI-Email-Authorship-Detection-Automated-Reply-System
│── project (3).ipynb   # Main notebook
│── trained_model.pkl   # Saved ML model (if generated)
│── dataset.csv         # Email dataset (if included)
│── README.md           # Project documentation

🔮 Future Improvements

Add deep learning models (LSTM / Transformers)

Implement real-time email classification

Integrate with Gmail/Outlook API

Improve automated reply generation using Generative AI
