# WINE-QUALITY-PREDICTION-USING-RANDOM-FOREST-CLASSIFIER

This project implements a Wine Quality Prediction Model using the Random Forest Classifier. The model is trained on a red wine dataset to classify wine as either good quality (≥7) or bad quality (<7) based on its physicochemical properties.

**Dataset Overview**
The dataset consists of multiple physicochemical attributes that influence wine quality, including:

Fixed Acidity,
Volatile Acidity,
Citric Acid,
Residual Sugar,
Chlorides,
Free Sulfur Dioxide,
Total Sulfur Dioxide,
Density,
pH,
Sulphates,
Alcohol,
*Quality (Target Variable),
The quality scores range from 3 to 8. For classification purposes, wines with a quality score of 7 or higher are labeled as "Good Quality" (1), while others are labeled as "Bad Quality" (0).*

**Technologies Used**
* Python
* NumPy, Pandas
* Matplotlib, Seaborn
* Scikit-learn (RandomForestClassifier, Train-Test Split, Accuracy Score)
* 
**{Why Use Random Forest?**
* Handles Non-Linear Relationships – Since wine quality depends on complex interactions between features, Random Forest captures these relationships effectively.
* Reduces Overfitting – By averaging multiple decision trees, Random Forest reduces the risk of overfitting, ensuring better generalization on new data.
* Handles Missing and Noisy Data Well – Unlike some ML algorithms, Random Forest is robust to missing values and noisy data.
* Feature Importance – It helps in understanding which attributes contribute most to wine quality.**}**
  
**Project Workflow**
* Load the dataset and check for missing values.
* Perform exploratory data analysis (EDA) using:
* Count plot for wine quality distribution.
* Bar plots to analyze the relationship between acidity and citric acid with quality.
* Correlation heatmap to identify the most influential features.

**Prepare the dataset:**
* Drop the "quality" column from input features.
* Convert the target variable into a binary classification (good/bad quality) using a lambda function.
* Split data into training (80%) and testing (20%) sets.
* Train a Random Forest Classifier on the training data.
* Evaluate the model’s performance on the test data using accuracy score.
* Test the model with a sample input to predict wine quality.

**Model Performance**
* Test Accuracy: 93.12% 

**Example Prediction:**
For an input wine sample with the following properties:

* Fixed Acidity: 7.3
* Volatile Acidity: 0.65
* Citric Acid: 0.0
* Residual Sugar: 1.2
* Chlorides: 0.065
* Free Sulfur Dioxide: 15.0
* Total Sulfur Dioxide: 21.0
* Density: 0.9946
* pH: 3.39
* Sulphates: 0.47
* Alcohol: 10.0
  
* **The model predicts: Bad Quality Wine**

**Future Improvements**
* Tune hyperparameters (e.g., number of trees, depth) to optimize performance.
* Experiment with other classifiers like XGBoost or SVM.
* Deploy the model as a web application for real-time predictions.

**Author**
[Arman Ahmad -> Connect with me on LinkedIn: www.linkedin.com/in/armanahmad16]
