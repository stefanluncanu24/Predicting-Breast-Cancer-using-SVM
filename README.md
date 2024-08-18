# Predicting-Breast-Cancer-using-SVM-with-GridSearchCV

This repository hosts a Python-based machine learning project aimed at predicting breast cancer through the application of Support Vector Machines (SVM), enhanced with GridSearchCV for optimal hyperparameter tuning. The project leverages the Breast Cancer Wisconsin (Diagnostic) dataset from the UCI Machine Learning Repository, featuring diagnostic measurements from digitized images of breast mass fine needle aspirates.

## Dataset
The Breast Cancer Wisconsin (Diagnostic) dataset features measurements from digitized images of breast mass fine needle aspirates, used to predict whether a breast mass is benign or malignant.
[Dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)

### Dataset Features

The dataset includes various features derived from the breast mass images, such as:
- Radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension of cell nuclei, presented in three forms: mean, standard error, and "worst" (mean of the three largest values).

### Project Structure

- **Data Preprocessing**: Initial data cleaning and preparation by removing irrelevant columns and standardizing the dataset.
- **Exploratory Data Analysis (EDA)**: Correlation analysis among features using heatmap visualizations to identify and eliminate multicollinear features.
- **Data Splitting**: Segregating the dataset into training and testing sets to ensure unbiased model evaluation.
- **Feature Scaling**: Application of StandardScaler to normalize feature scales, enhancing model predictability.
- **Model Training**: Deployment of GridSearchCV to systematically explore multiple combinations of SVM parameters to find the most effective model settings.
- **Model Evaluation**: Assessing the model performance using accuracy, F1 score, precision, recall, and a confusion matrix for detailed performance insights.

### Installation

Clone this repository and install the necessary Python packages:

```bash
git clone https://github.com/your-username/breast-cancer-prediction.git
cd breast-cancer-prediction
pip install -r requirements.txt
