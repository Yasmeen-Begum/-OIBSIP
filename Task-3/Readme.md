# SMS Spam Detection using Naive Bayes and Gradio

## Project Overview

This project builds a Machine Learning model to classify SMS messages as **Spam** or **Ham (Not Spam)** using the SMS Spam Collection Dataset. The project includes data preprocessing, exploratory data analysis (EDA), text cleaning, TF-IDF feature extraction, model training using Multinomial Naive Bayes, and deployment with Gradio.

The final model achieves approximately **97% accuracy** and is deployed through a simple web interface where users can enter SMS messages and receive instant predictions.

---

## Dataset

Dataset Source:

https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

The dataset contains over 5,500 SMS messages labeled as:

* Ham (Legitimate Message)
* Spam (Unwanted Promotional/Fraudulent Message)

### Dataset Features

| Column | Description                 |
| ------ | --------------------------- |
| v1     | Message Category (Ham/Spam) |
| v2     | SMS Message Text            |

---

## Project Workflow

### 1. Data Collection

* Load SMS Spam Collection Dataset
* Inspect dataset structure
* Understand feature distributions

### 2. Data Cleaning

* Remove unnecessary columns
* Rename columns
* Handle duplicates
* Check missing values

### 3. Exploratory Data Analysis (EDA)

* Dataset statistics
* Message distribution
* Character count analysis
* Word count analysis
* Spam vs Ham comparison
* WordCloud visualization

### 4. Text Preprocessing

* Convert text to lowercase
* Tokenization
* Remove punctuation
* Remove stopwords
* Apply stemming using Porter Stemmer

### 5. Feature Engineering

* TF-IDF Vectorization
* Unigram and Bigram extraction

### 6. Model Training

* Train-Test Split
* Multinomial Naive Bayes Classifier

### 7. Model Evaluation

* Accuracy Score
* Precision Score
* Confusion Matrix
* Classification Report

### 8. Model Deployment

* Save trained model using Pickle
* Create Gradio Interface
* Predict Spam or Ham in real time

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* NLTK
* WordCloud
* Scikit-Learn
* Gradio
* Pickle

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/sms-spam-detection.git

cd sms-spam-detection
```

Install required libraries:

```bash
pip install -r requirements.txt
```

---

## Required Libraries

```text
pandas
numpy
matplotlib
seaborn
nltk
wordcloud
scikit-learn
gradio
```

---

## Project Structure

```text
SMS-Spam-Detection/
│
├── spam.csv
├── notebook.ipynb
├── model.pkl
├── vectorizer.pkl
├── requirements.txt
├── README.md

```

---

## Exploratory Data Analysis

The following analyses were performed:

* Dataset Shape Analysis
* Missing Value Detection
* Duplicate Record Detection
* Spam vs Ham Distribution
* Character Count Analysis
* Word Count Analysis
* Message Length Distribution
* Word Frequency Analysis
* Correlation Analysis
* WordCloud Visualization

---

## Text Preprocessing Pipeline

The preprocessing function performs:

1. Lowercase conversion
2. Tokenization
3. Removal of special characters
4. Removal of stopwords
5. Stemming using Porter Stemmer

Example:

Input:

```text
Congratulations! You won a FREE iPhone.
```

Processed Output:

```text
congratul free iphon
```

---

## Feature Extraction

TF-IDF Vectorizer Configuration:

```python
TfidfVectorizer(
    max_features=3000,
    ngram_range=(1,2),
    min_df=2,
    max_df=0.95
)
```

This converts SMS text into numerical vectors suitable for machine learning algorithms.

---

## Machine Learning Model

### Multinomial Naive Bayes

The model was trained using:

```python
MultinomialNB()
```

Reasons for choosing Naive Bayes:

* Fast training
* Excellent performance on text classification
* High precision for spam detection
* Efficient with TF-IDF features

---

## Model Performance

### Accuracy

```text
97%+
```

### Precision

```text
100%
```

### Confusion Matrix

```text
[[896   0]
 [ 27 111]]
```

### Classification Report

```text
Precision : 1.00
Recall    : 0.78
F1 Score  : 0.88
Accuracy  : 0.97
```

---

## Saving the Model

Vectorizer:

```python
pickle.dump(tfidf, open("vectorizer.pkl","wb"))
```

Model:

```python
pickle.dump(model, open("model.pkl","wb"))
```

---

## Gradio Web Application

The project includes a Gradio interface for real-time SMS classification.

Features:

* User-friendly interface
* Instant prediction
* Spam/Ham classification
* Lightweight deployment


## Example Predictions

### Example 1

Input:

```text
Congratulations! You have won a $1000 Amazon Gift Card. Click the link below to claim your prize now.
```

Output:

Spam Message


<img width="870" height="312" alt="Image" src="https://github.com/user-attachments/assets/88d4957f-82dd-4446-843b-c4308453e062" />


### Example 2

Input:

```text
The meetings has been resheduled to 3pm.Please check your email. 
```

Output:

Ham Message

<img width="893" height="311" alt="Image" src="https://github.com/user-attachments/assets/a1da41b7-ce98-4120-afb9-6d7570afde00" />



## Learning Outcomes

Through this project, the following concepts were explored:

* Natural Language Processing (NLP)
* Text Cleaning
* Feature Engineering
* TF-IDF Vectorization
* Machine Learning Classification
* Model Evaluation
* Pickle Serialization
* Gradio Deployment

---

## Author

Yasmeen Begum

Machine Learning | Data Science | NLP Enthusiast

