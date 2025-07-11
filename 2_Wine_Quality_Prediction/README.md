# Wine Quality Prediction using Random Forest Classifier

## Project Overview

This project focuses on predicting the quality of red wine using chemical properties as input features. A Random Forest Classifier was trained to classify wines as "Good" or "Bad" based on their quality scores. The model helps automate wine quality grading, which is useful for wineries, distributors, and quality control systems.

## Dataset

The dataset used is `winequality-red.csv`, which includes:
- 11 physiochemical features such as acidity, sugar, chlorides, and alcohol
- A `quality` score (integer between 0 and 10) representing expert ratings

The dataset was obtained from the UCI Machine Learning Repository.

## Key Tasks Performed

- Explored and visualized the dataset using Seaborn and Matplotlib
- Checked for missing data and reviewed statistical distributions
- Analyzed feature relationships using bar plots and correlation heatmaps
- Converted the quality score into binary labels:  
  - `1` for good quality (score ≥ 7)  
  - `0` for bad quality (score < 7)
- Trained a Random Forest Classifier on the processed dataset
- Evaluated model performance using accuracy score
- Built a predictive system to classify new input data

## Tools and Libraries Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- scikit-learn (RandomForestClassifier, accuracy_score, train_test_split)

## Results

- The model achieved high accuracy in distinguishing good and bad quality wines.
- Visual analysis confirmed strong correlations between quality and factors like alcohol and volatile acidity.
- The prediction system correctly classified custom wine samples.

## Conclusion

This project demonstrates the practical use of machine learning for quality control in the wine industry. By leveraging ensemble learning techniques, we achieved robust classification performance. The approach is scalable and adaptable to similar classification tasks in food and beverage analytics.
