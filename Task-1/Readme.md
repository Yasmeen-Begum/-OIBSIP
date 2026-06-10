# Iris Flower Classification using Random Forest Classifier

## Project Structure


Iris_Classification/

├── Iris.csv

├── Iris_classification.ipynb

├── model.pkl

├── README.md

└── Gradio Application

## Overview

This project uses the Iris Flower Dataset to classify iris flowers into three species:

* Iris Setosa
* Iris Versicolor
* Iris Virginica
  

The project covers the complete Machine Learning workflow, including:

* Data Loading
* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Model Training using Random Forest Classifier
* Model Evaluation
* Model Saving using Pickle/Joblib
* Gradio Web Application Deployment

---

## Dataset

The Iris dataset contains flower measurements and corresponding species labels.

### Features

| Feature      | Description                    |
| ------------ | ------------------------------ |
| Sepal Length | Length of sepal in centimeters |
| Sepal Width  | Width of sepal in centimeters  |
| Petal Length | Length of petal in centimeters |
| Petal Width  | Width of petal in centimeters  |

### Target Variable

Species

* Iris-setosa
* Iris-versicolor
* Iris-virginica

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib
* Gradio

---

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas.

```python
df = pd.read_csv("Iris.csv")
```

---

### 2. Data Cleaning

The following preprocessing steps were performed:

* Checked dataset dimensions
* Checked missing values
* Removed duplicate records
* Removed unnecessary ID column

---

### 3. Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset:

#### Species Distribution

* Pie Chart

#### Feature Distribution

* Histogram
* KDE Plot

#### Outlier Analysis

* Box Plot
* Violin Plot

#### Correlation Analysis

* Heatmap

#### Feature Relationships

* Pair Plot

---

### 4. Data Preprocessing

The species labels were converted into numerical values.

```python
target = {
    "Iris-versicolor": 0,
    "Iris-virginica": 1,
    "Iris-setosa": 2
}
```

Feature scaling was applied using StandardScaler.

```python
scaler = StandardScaler()
```

---

### 5. Train-Test Split

The dataset was split into:

* 80% Training Data
* 20% Testing Data

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

---

## Machine Learning Model

### Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple Decision Trees and makes predictions using majority voting.

```python
rf = RandomForestClassifier()
```

### Why Random Forest?

* High Accuracy
* Handles Non-Linear Data
* Reduces Overfitting
* Robust and Reliable
* Works Well on Small and Large Datasets

---

## Model Evaluation

The model was evaluated using:

### Accuracy Score

```python
accuracy_score(y_test, y_pred)
```

### Classification Report

Provides:

* Precision
* Recall
* F1 Score

### Confusion Matrix

Shows correct and incorrect predictions for each class.

---

## Model Saving

After training, the model is saved using Joblib.

```python
joblib.dump(rf, "model.pkl")
```

Saved file:

```text
model.pkl
```

---

## Gradio Web Application

The trained model is integrated into a Gradio interface.

### Input Features

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

### Output

Predicted Iris Species

Example:

```text
Input:
Sepal Length = 5.1
Sepal Width = 3.5
Petal Length = 1.4
Petal Width = 0.2

Output:
Iris-setosa
```

---

## Running the Project

### Install Dependencies

```bash
pip install gradio matplotlib numpy pandas seaborn scikit-learn joblib
```

### Run Notebook

Open:

```text
Iris_classification.ipynb
```

Execute all cells sequentially.

### Launch Gradio Application

Run the final cell:

```python
app.launch()
```

A local Gradio URL will be generated.

---


<img width="1366" height="685" alt="Image" src="https://github.com/user-attachments/assets/301c3820-1cc5-4c7c-9ab9-a5515a410a28" />

---

## Results

The Random Forest Classifier successfully classifies iris flowers based on their measurements and provides predictions through an interactive Gradio web interface.

---

## Author

Yasmeen Begum

Machine Learning & Artificial Intelligence 


