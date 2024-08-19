# Predicting-Breast-Cancer-using-SVM-with-GridSearchCV

This repository hosts a Python-based machine learning project aimed at predicting breast cancer through the application of Support Vector Machines (SVM), enhanced with GridSearchCV for optimal hyperparameter tuning. The project leverages the Breast Cancer Wisconsin (Diagnostic) dataset from the UCI Machine Learning Repository, featuring diagnostic measurements from digitized images of breast mass fine needle aspirates.

## File explanations

- data.csv - dataset used
- model.ipynb - code 

## Dataset
The Breast Cancer Wisconsin (Diagnostic) dataset features measurements from digitized images of breast mass fine needle aspirates, used to predict whether a breast mass is benign or malignant.

[Dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)

### Dataset Features

The dataset includes various features derived from the breast mass images, such as:
- Radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension of cell nuclei, presented in three forms: mean, standard error, and "worst" (mean of the three largest values).

### Project Structure

- **Data Preprocessing**:
  - Removal of non-essential columns such as 'id' and 'Unnamed: 32'.
  - Transformation of the 'diagnosis' column into a binary format where 'M' (malignant) is 1 and 'B' (benign) is 0.
  - Feature Reduction: eliminating highly correlated features like perimeter_mean, perimeter_se, perimeter_worst, area_mean, area_se, and area_worst to reduce multicollinearity and enhance model performance.

- **Exploratory Data Analysis (EDA)**:
  - Use of heatmaps to visualize the correlation among features, identifying highly correlated features that may distort the predictive model.
  - Detailed statistical analysis to understand the central tendencies and dispersion of the data.
    
- **Data Splitting**:
  - The dataset is split into a 80-20 ratio for training and testing, ensuring a balanced approach to model training and evaluation.
    
- **Feature Scaling**:
  - Application of `StandardScaler` to normalize the features, which enhances the predictive capability of the SVM model.
    
- **Model Training**:
  - Configuration of GridSearchCV with SVM to explore various hyperparameters like kernel type, C, gamma, and degree.
  - Utilization of cross-validation within GridSearchCV to ensure that the model is not overfitting and is generalized well.
    
### Model Evaluation

- **High Accuracy**:
  - The model demonstrated a high accuracy of 98.25%, indicating exceptional performance in correctly classifying breast cancer instances.

- **Confusion Matrix Analysis**:
  - The confusion matrix displayed 45 true positives and 67 true negatives, with no false positives and only 2 false negatives, highlighting the model's effectiveness in accurately predicting outcomes.

- **Perfect Precision**:
  - With a precision score of 100%, the model identified all cases it predicted as malignant correctly, with no false positives.
    
- **Impressive Recall**:
  - The recall rate of 95.74% indicates the model's strong ability to identify the majority of true positive cases.

- **Robust F1 Score**:
  - An F1 score of 97.83% illustrates the model's balanced capability in both precision and recall, ensuring it is reliable and effective in practical scenarios.

![Model Evaluation Image](https://github.com/user-attachments/assets/e540e481-42de-452f-b6a0-cde478b74e58)

### Conclusion

In conclusion, this project has demonstrated the applicability of machine learning, specifically through SVM and GridSearchCV, in predicting breast cancer.

### Contributions

Contributions are encouraged! Feel free to fork this repo, implement your changes, and submit a pull request.
  
