# Amazon Reviews Sentiment Analysis

## Improving Customer Satisfaction through Automated Review Sentiment Analysis

## Objective

The objective of this project is to build a machine learning-based sentiment
analysis system that automatically classifies Amazon customer reviews as
Positive or Negative.

The system can help businesses analyze large volumes of customer feedback,
identify negative reviews, and gain insights into customer satisfaction.

## Business Problem

E-commerce companies receive thousands of customer reviews every day. Although
customers provide ratings, ratings alone may not always accurately represent
the sentiment expressed in the review.

Automated sentiment analysis can help businesses:

- Monitor customer sentiment.
- Identify negative feedback quickly.
- Analyze product performance.
- Detect changes in customer satisfaction.
- Improve customer experience.

## Dataset

The dataset used in this project is `amazonreviews.csv`.

It contains 10,000 pre-labeled Amazon customer reviews.

### Dataset Features

| Column | Description |
|---|---|
| `label` | Sentiment of the review: `pos` or `neg` |
| `review` | Text of the customer review |

### Target Variable

The `label` column represents the sentiment:

- `pos` - Positive review
- `neg` - Negative review

## Project Workflow

### 1. Data Cleaning

The following text preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Checked the dataset structure and data types.
- Checked for missing reviews.
- Removed duplicate reviews.
- Converted text to lowercase.
- Removed unnecessary characters and punctuation.
- Removed stopwords where appropriate.
- Prepared the cleaned text for feature extraction.

### 2. Exploratory Data Analysis

Exploratory analysis was performed to understand the review dataset.

The analysis included:

- Sentiment distribution.
- Number of positive and negative reviews.
- Most frequently occurring words.
- Positive sentiment word analysis.
- Negative sentiment word analysis.
- Word clouds for positive and negative reviews.

Visualizations were used to identify common patterns in customer feedback.

### 3. Feature Extraction

Natural Language Processing techniques were used to convert textual reviews
into numerical features that machine learning models can process.

TF-IDF (Term Frequency-Inverse Document Frequency) was used to represent the
importance of words within the reviews.

### 4. Model Development

A machine learning classification model was trained to classify reviews as
positive or negative.

Possible classification algorithms include:

- Logistic Regression
- Support Vector Machine (SVM)
- Neural Networks

The selected model was trained using the extracted text features.

### 5. Model Validation

The dataset was divided into training and testing sets.

Cross-validation was used where appropriate to assess model robustness.

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 6. Sentiment Prediction

The trained model can be used to predict the sentiment of new customer
reviews.

For a given review, the system predicts whether the review is:

- Positive
- Negative

## TF-IDF

TF-IDF (Term Frequency-Inverse Document Frequency) is a technique used to
convert text into numerical vectors.

It assigns higher importance to words that are frequent in a particular
document but less common across the entire collection of documents.

This allows machine learning algorithms to work with textual data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn
- WordCloud
- Jupyter Notebook / Google Colab

## Project Structure

```text
Amazon-Reviews-Sentiment-Analysis/
│
├── Amazon_Reviews_Sentiment_Analysis.ipynb
├── amazonreviews.tsv
└── README.md
