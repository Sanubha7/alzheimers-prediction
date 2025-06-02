# alzheimers-prediction
KNN-based classification model to predict Alzheimer's from clinical data

## Dataset:
- **Source**: [Kaggle Alzheimer's Dataset](https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset)

## Files:
1) knn.py: Unoptimized knn model which gives an accuracy of 0.54
2) optimized_knn.py: Optimized knn model which gives an accuracy of 0.86

## Optimization steps:
### Data Preprocessing
- Used ANOVA F-scores to select the top 10 most relevant features from the dataset.

- Removed irrelevant and low-impact features to reduce noise and improve model performance.

- Applied standardization to selected features using StandardScaler, ensuring all features contribute equally in distance-based KNN computations.

### Algorithm & Model Training
- Split the dataset into 75% training and 25% testing subsets.

- Performed hyperparameter tuning using GridSearchCV with 4-fold cross-validation to find the optimal value of K.

- Trained the final model using the best k value identified.

- Evaluated model performance on the test set and generated a detailed classification report.

