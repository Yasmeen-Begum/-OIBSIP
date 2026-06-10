# Iris Flower Classification Using Machine Learning and Gradio

## Project Overview

This project focuses on classifying Iris flower species using Machine Learning algorithms. The Iris dataset is one of the most popular datasets for classification tasks and contains measurements of flower characteristics such as sepal length, sepal width, petal length, and petal width.

The project includes:

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* Data visualization
* Feature scaling
* Training multiple Machine Learning models
* Model performance comparison
* Selection of the best-performing model
* Saving the trained model using Pickle (.pkl)
* Deploying the model with Gradio for real-time predictions

---

## Dataset

The Iris dataset contains 150 samples belonging to three species:

* Iris-setosa
* Iris-versicolor
* Iris-virginica

### Features

| Feature      | Description          |
| ------------ | -------------------- |
| Sepal Length | Length of sepal (cm) |
| Sepal Width  | Width of sepal (cm)  |
| Petal Length | Length of petal (cm) |
| Petal Width  | Width of petal (cm)  |

### Target Variable

Species of Iris flower.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Pickle
* Gradio

---

## Machine Learning Models

The following classification algorithms were trained and evaluated:

1. Logistic Regression
2. Gaussian Naive Bayes
3. Support Vector Machine (SVM)
4. Decision Tree Classifier
5. Random Forest Classifier

---

## Project Workflow

### 1. Data Collection

* Load the Iris dataset from CSV file.
* Inspect dataset structure and contents.

### 2. Data Cleaning

* Check missing values.
* Detect duplicate records.
* Remove duplicates if present.

### 3. Exploratory Data Analysis (EDA)

Performed the following visualizations:

* Species Distribution Pie Chart
* Histograms
* KDE Plots
* Boxplots
* Violin Plots
* Correlation Heatmap
* Pair Plot

### 4. Data Preprocessing

* Convert categorical labels into numerical values.
* Remove unnecessary columns.
* Separate features and target variable.
* Split dataset into training and testing sets.
* Apply feature scaling using StandardScaler.

### 5. Model Training

Each model was trained using:

* Training Dataset
* 5-Fold Cross Validation

### 6. Model Evaluation

Performance was evaluated using:

* Accuracy Score
* Classification Report
* Confusion Matrix
* Cross Validation Accuracy

### 7. Model Comparison

All model accuracies were compared using a bar chart.

### 8. Best Model Selection

The model with the highest accuracy was automatically selected.

### 9. Model Saving

The best-performing model was saved as:

* iris_best_model.pkl
* scaler.pkl

### 10. Deployment

A Gradio web application was created to allow users to enter flower measurements and receive species predictions instantly.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/iris-classification.git
cd iris-classification
```

Install required libraries:

```bash
pip install gradio seaborn scikit-learn pandas numpy matplotlib
```

---

## Running the Project

Run the notebook or Python script:

```bash
python app.py
```

Launch the Gradio application:

```bash
python gradio_app.py
```

---

## Model Prediction Inputs

The Gradio application accepts:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Output:

* Predicted Iris Species

---

## Sample Prediction

Input:

```text
Sepal Length = 5.1
Sepal Width = 3.5
Petal Length = 1.4
Petal Width = 0.2
```

Output:

```text
Iris-setosa
```

---

## Results

The project compares multiple Machine Learning models and automatically selects the best-performing classifier based on test accuracy.

Typical accuracy achieved:

* Logistic Regression: ~95%+
* Gaussian Naive Bayes: ~95%+
* SVM: ~96–100%
* Decision Tree: ~93–100%
* Random Forest: ~96–100%

---

## Future Enhancements

* Hyperparameter tuning using GridSearchCV
* Deployment on Hugging Face Spaces
* Deployment on Streamlit Cloud
* Docker containerization
* Model explainability using SHAP
* Feature importance visualization

---

## Learning Outcomes

Through this project, the following concepts were explored:

* Data preprocessing
* Exploratory Data Analysis
* Machine Learning classification
* Model evaluation techniques
* Cross Validation
* Model comparison
* Model persistence using Pickle
* Web application deployment with Gradio

---

## Author

Yasmeen Begum

Machine Learning and Artificial Intelligence Enthusiast


<img width="1366" height="685" alt="Image" src="https://github.com/user-attachments/assets/301c3820-1cc5-4c7c-9ab9-a5515a410a28" />
