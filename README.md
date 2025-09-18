Obesity Level Prediction Project


Overview
This project aims to predict obesity levels using a dataset with various demographic, lifestyle, and health-related features. Our model leverages machine learning techniques to classify individuals into different obesity categories, providing a powerful tool for health insights.

Data Preprocessing
Data Exploration and Initial Cleaning

Inspected data for missing values and performed initial cleaning to prepare the dataset for analysis.
Descriptive Statistics and Visualization

Conducted univariate and bivariate analysis to understand feature distributions and correlations using histograms, boxplots, and pair plots.
Utilized heatmaps for visual correlation analysis to inform feature selection.
Feature Encoding and Scaling

Categorical features were transformed using one-hot encoding for compatibility with machine learning algorithms.
Applied feature scaling using StandardScaler or MinMaxScaler to ensure all features were on a similar scale, enhancing model convergence.
Feature Selection
Features chosen based on correlation analysis and domain knowledge include age, family_history_with_overweight_sometimes, snacks_sometimes, physical_activity, and vegetables_per_meal.
Model Development
Model Selection and Training
Utilized several machine learning algorithms, including Random Forests and Logistic Regression, to build predictive models.
Split dataset into training and test sets using train_test_split.
Hyperparameter Tuning
Applied GridSearchCV to fine-tune hyperparameters for the Random Forest model. Best parameters identified as:
max_depth: None
max_features: 'sqrt'
min_samples_leaf: 2
min_samples_split: 5
n_estimators: 200
Evaluation Metrics
Classification Report: Evaluated model performance using precision, recall, and F1-score for each class.
Confusion Matrix: Visualized predictions to assess model accuracy and identify areas for improvement.
ROC and PR Curves: Utilized RocCurveDisplay and PrecisionRecallDisplay to further analyze model performance across thresholds.
Addressing Class Imbalance
Implemented techniques like:
SMOTE for synthetic over-sampling of minority classes.
Adjusting class_weight to handle class imbalance in Random Forest.
Results and Next Steps
Achieved a weighted F1 Score of approximately 0.57 in the current model configuration.
Considerations for further enhancement include fine-tuning model parameters, exploring additional features, and trying ensemble methods.
Continuous integration of domain knowledge and advanced techniques, like anomaly detection and ensemble learning, is recommended to refine the model's accuracy and robustness.
Conclusion
This project establishes a foundation for predictive analysis of obesity levels using machine learning, setting the groundwork for future improvements and expansions. The insights gained can assist in targeted health interventions and policy-making.
