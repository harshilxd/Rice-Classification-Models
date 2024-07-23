# Rice Classification

This project aims to classify rice grains into two types: Cammeo and Osmancik. The dataset contains various features extracted from images of rice grains. The project explores different machine learning algorithms to achieve accurate classification.

## Techniques and Methods Used

### Data Import and Preprocessing
- Imported the dataset using pandas to analyze and preprocess the data.
- Checked for null values and confirmed that there were no missing entries in the dataset.
- Used descriptive statistics to understand the distribution and summary of the data features.

### Data Visualization
- Generated a correlation matrix and pair plots using seaborn to visualize relationships between features and understand feature importance.
- Visualized the distribution of the target class to ensure balanced classes for model training.

### Encoding Categorical Variables
- Encoded the categorical target variable 'Class' using LabelEncoder from sklearn to convert it into a numerical format suitable for machine learning models.

### Model 1: Logistic Regression
- Chose Logistic Regression as the first model due to its simplicity and effectiveness for binary classification problems.
- Observed high accuracy, precision, and recall, indicating that Logistic Regression performs well on this dataset.

### Model 2: Random Forest
- Used Random Forest to capture non-linear relationships and interactions between features.
- Performed hyperparameter tuning using RandomizedSearchCV to find the best combination of hyperparameters.
- Achieved high accuracy and noted feature importance, providing insights into which features contribute most to the classification.

### Model 3: Gaussian Mixture
- Applied Gaussian Mixture for probabilistic clustering, which assumes data is generated from a mixture of several Gaussian distributions.
- Observed reasonable performance, but not as high as Random Forest, indicating it might not be the best fit for this dataset.

### Model 4: Birch Clustering
- Tested Birch clustering to identify hierarchical data structure and cluster the data.
- Noted that Birch did not perform well in terms of classification accuracy, indicating that I have definetely messed up the algorithm and have made a mistake.

## Observations

- Logistic Regression and Random Forest models achieved high accuracy, making them suitable for this classification problem.
- The Random Forest model provided valuable insights into feature importance, with features like Major Axis Length and Eccentricity being significant for distinguishing between Cammeo and Osmancik rice grains.
- Gaussian Mixture did not perform as well as the supervised learning models, highlighting the importance of choosing the right algorithm based on the nature of the dataset and the problem at hand.
- Hyperparameter tuning significantly improved the performance of the Random Forest model, demonstrating the importance of optimizing model parameters.

## Conclusion

This project explored different machine learning algorithms to classify rice grains into Cammeo and Osmancik types. The Random Forest classifier emerged as the best-performing model, achieving an accuracy of approximately 93%. Future work could include further hyperparameter tuning, feature engineering, and exploring more advanced models to enhance classification performance.
