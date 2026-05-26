# Heart Disease Prediction Model

## Project Overview

This machine learning project builds and compares multiple classification models to predict the presence of heart disease in patients based on health metrics. The project demonstrates end-to-end machine learning workflow including data exploration, model training, evaluation, and comparison.

## Objective

Predict whether a patient has heart disease (binary classification: Yes/No) using clinical health indicators and demographic features.

## Dataset

**Dataset**: Heart_Disease_Prediction.csv

**Features Include**:
- Age
- Sex
- Cholesterol levels
- Blood pressure
- Heart rate
- Other clinical indicators

**Target Variable**: Heart Disease (0 = No, 1 = Yes)

## Project Workflow

### 1. **Data Exploration & Analysis**
- Load and examine dataset structure
- Analyze data distribution with histograms
- Check for missing values
- View target variable distribution
- Explore relationships between features (scatter plots)

### 2. **Data Preparation**
- Separate features (X) from target (y)
- Visualize class balance
- Prepare for modeling

### 3. **Train-Test Split**
- Split data: 80% training, 20% testing
- Maintain reproducibility with random_state=42

### 4. **Model Building & Training**

#### Model 1: Logistic Regression
- Simple linear classification model
- Fast training and predictions
- Interpretable coefficients

#### Model 2: Random Forest
- Ensemble method using multiple decision trees
- Captures non-linear relationships
- Provides feature importance scores

### 5. **Model Evaluation**
- **Accuracy**: Overall correctness of predictions
- **Classification Report**: Precision, recall, F1-score per class
- **Confusion Matrix**: True positives, false positives, true negatives, false negatives

### 6. **Model Comparison**
- Visual comparison of model accuracies
- Identify best performing model
- Analyze feature importance

## Results

Both models are evaluated and compared based on:
- Overall accuracy score
- Precision and recall for each class
- Feature importance rankings

The model with higher accuracy on the test set is recommended for predictions.

## Key Features of the Analysis

✅ **Data Exploration**: Comprehensive analysis of dataset characteristics
✅ **Multiple Models**: Comparison of different algorithms
✅ **Feature Importance**: Identifies most influential health factors
✅ **Model Metrics**: Detailed performance evaluation
✅ **Visualization**: Charts for results interpretation

## Installation

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

Or manually:
```bash
pip install pandas numpy scikit-learn matplotlib
```

### 2. Place Data File
Ensure `Heart_Disease_Prediction.csv` is in the same directory as the notebook

## Usage

### Run the Notebook
```bash
jupyter notebook Heart_Disease_Prediction_Model.ipynb
```

### Execute Cells
Run cells sequentially from top to bottom to:
1. Load and explore data
2. Train both models
3. Evaluate performance
4. Compare results
5. Analyze feature importance

## Model Performance

The notebook outputs:
- Accuracy scores for both models
- Classification reports with precision/recall
- Confusion matrices
- Feature importance rankings
- Visual comparisons

## Important Findings

- **Most Important Features**: Identified through Random Forest feature importance
- **Model Comparison**: Random Forest typically outperforms Logistic Regression for this dataset
- **Class Balance**: Evaluation of how well models handle both disease and non-disease cases

## Dependencies

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **scikit-learn**: Machine learning models and metrics
- **matplotlib**: Data visualization

## Limitations

1. **Model Accuracy**: Models achieve ~85-90% accuracy (not 100% perfect)
2. **Data Size**: Performance depends on dataset completeness and quality
3. **Generalization**: Model performance may vary on different populations
4. **Clinical Use**: This model is for educational purposes; real medical decisions require professional evaluation
5. **Feature Selection**: Uses only available features; additional clinical tests may improve predictions

## Future Enhancements

- Add feature scaling and normalization
- Implement cross-validation for robust evaluation
- Tune hyperparameters for better performance
- Add additional models (SVM, Gradient Boosting, Neural Networks)
- Perform feature selection to reduce dimensionality
- Generate ROC curves and AUC scores
- Create confusion matrix heatmaps
- Deploy model as web service

## Disclaimer

⚠️ **Important**: This model is for **educational and research purposes only**. It should NOT be used for actual medical diagnosis or treatment decisions. Always consult qualified healthcare professionals for medical advice.

## References

- [scikit-learn Documentation](https://scikit-learn.org/)
- [Classification Metrics](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [Random Forest](https://scikit-learn.org/stable/modules/ensemble.html#forest)
- [Logistic Regression](https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression)

---

**Project Status**: ✅ Complete

*Last Updated: May 2026*
