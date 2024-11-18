#### English Version | [Kaggle competition](https://www.kaggle.com/competitions/playground-series-s4e11)

# Mental Health and Depression Analysis

### Competition Description

This project is part of a Kaggle competition aimed at exploring factors influencing mental health and depression based on survey data. The dataset includes over 140,000 entries, covering attributes like academic and work pressure, CGPA, sleep duration, and dietary habits. The goal is to predict whether an individual is experiencing depression.

### Goal

The goal is to predict the presence of depression. For each `id` in the test set, the target variable to predict is `Depression` (1 - Yes, 0 - No).

### Approach

This project follows a structured approach to analyze mental health data and predict depression using machine learning. The key steps involved were:

1. **Data Exploration:**
   - The training and testing datasets were analyzed to identify missing values and understand the distribution of key features such as `Academic Pressure`, `Work Pressure`, and `Dietary Habits`.
   - Visualizations were created to examine the relationships between features like `Gender`, `Family History of Mental Illness`, and the target variable.

2. **Data Preprocessing:**
   - Missing values were filled with appropriate placeholders.
   - Categorical features such as `Gender` and `City` were identified for encoding and included in the modeling process.

3. **Model Selection and Training:**
   - The CatBoostClassifier model was selected for its efficiency with categorical features and robust performance.
   - Hyperparameters were configured for optimal results, and the model was trained on an 80-20 train-validation split.

4. **Model Evaluation:**
   - The model was evaluated using classification metrics such as precision, recall, F1-score, and ROC-AUC.
   - Achieved an accuracy of **94%** and a ROC-AUC score of **0.8903** on the validation set.

5. **Prediction and Submission:**
   - The trained model was used to predict depression for the test dataset.
   - Final predictions were saved in the required CSV format for Kaggle submission.

### Results

The model demonstrated strong predictive performance, achieving a high accuracy and a balanced evaluation across precision, recall, and F1-score.

### Files

- `MentalHealth.ipynb`: Jupyter Notebook containing the complete analysis and model implementation.
- `submission.csv`: File containing the predictions for the test dataset.
- `train.csv`: Training dataset used for model training and validation.
- `test.csv`: Test dataset used for final predictions.

### Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- catboost

### Acknowledgements

This project was completed as part of a Kaggle competition. Thanks to Kaggle and the competition organizers for providing the dataset and platform!
