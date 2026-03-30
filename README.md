**Crop Prediction using Multi-Class Logistic Regression**

This project implements a multi-class machine learning model to predict the most suitable crop based on soil characteristics, helping farmers make informed decisions and optimize yield.

**Project Overview**

- Goal: Predict the optimal crop for given soil conditions using nutrient content and pH levels.
- Dataset: 2,200 soil samples across 22 crop categories.
- Features: Nitrogen (N), Phosphorus (P), Potassium (K), pH
- Target: Crop type

**Key Insights**

- pH is the dominant predictor, significantly influencing crop selection.
- Nutrients (N, P, K) contribute but are less decisive individually.
- Model errors are concentrated among agriculturally similar crops, such as legumes and fruits, reflecting real-world overlaps in soil requirements.

**Methodology**

1. Data Preprocessing
    - Standardization (feature scaling)
    - Train-test split

2. Modeling
    - Baseline: Logistic Regression
    - Accuracy improved from 63% → 68% after scaling

3. Analysis

    - Feature importance analysis
    - Confusion matrix to identify systematic misclassifications

**Recommendations**

- Use nonlinear models such as Random Forests or Gradient Boosting for higher accuracy
- Incorporate environmental features like temperature, rainfall, and humidity for better differentiation between similar crops

**Results**

| Feature | Accuracy     |
| ------- | ------------ |
| Accuracy (unscaled)  | 63% |
| Accuracy (scaled)   | 68%  |
| Dominant Feature   | pH |

The confusion matrix revealed logical misclassifications primarily among crops with similar soil requirements, highlighting feature limitations and opportunities for model improvement.

**Project Impact**

- Helps farmers select crops suited to their soil
- Supports evidence-based agricultural decisions
- Demonstrates practical use of machine learning in agriculture

**Future Improvements**

- Expand feature set with climate data
- Explore hierarchical classification to first predict crop category, then specific crop