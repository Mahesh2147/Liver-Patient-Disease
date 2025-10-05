# Liver-Patient-Disease

## 🎯 Project Objective
  * Goal: Build a predictive model using various classifiers to predict the likelihood of liver disease based 	on patient data.
	
  * Dataset: Indian Liver Patient Dataset (ILPD) containing 583 records with 11 attributes.

## 📚 Data Preprocessing & Handling
	
  * Initial Checks:

    * Checked for duplicate entries and removed them.
		
    * Handled missing values by filling Albumin-Globulin Ratio using the median.
		
    * Label Encoding applied to the Gender column (Male = 1, Female = 0).
	
  * Data Distribution:
		
    * Target variable (Selector): Imbalanced data.
		
    * Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes.
	
  * Feature Scaling:
	  
     * Applied MinMaxScaler to normalize numerical features.

## 📊 Exploratory Data Analysis (EDA)
	
  * Univariate Analysis:
		
    * Distribution of numerical and categorical columns analyzed.
		
    * Identified outliers using boxplots and scatter plots.
	
  * Bivariate & Multivariate Analysis:
		
    * Visualized relationships between features and target variable.
		
    * Correlation heatmap identified highly correlated features.

## 🧠 Model Building & Comparison
	
  * Models Evaluated:
		
    * Logistic Regression
		
    * Support Vector Classifier (SVC)
		
    * SVM with Hyperparameter Tuning
		
    * Random Forest Classifier
		
    * Random Forest with Hyperparameter Tuning
		
    * Gradient Boosting Classifier
		
    * XGBoost Classifier with Hyperparameter Tuning
	
  * Hyperparameter Tuning Techniques:

    * Applied GridSearchCV to optimize models like SVM, Random Forest, and XGBoost.

    * Found optimal parameters that improved performance.

## 📈 Model Performance Summary
	
  * Best Performing Model:

    * Random Forest with Hyperparameter Tuning
		
    * Training Accuracy: 98%
		
    * Test Accuracy: 79%
		
    * Best Hyperparameters:
		
      * max_depth: None

      * min_samples_leaf: 2
		
      * min_samples_split: 5

      * n_estimators: 50
	
  * Overall Model Comparison:
		
    * Most models achieved a test accuracy between 75% to 79%.
		
    * Hyperparameter tuning improved performance in SVM, Random Forest, and XGBoost.

## 📊 Model Comparison Report
```
Model			                Training Accuracy	        Test Accuracy

Logistic Regression		            72%		                  76%

SVM				                    70%	                	  75%

SVM (Hyperparameter Tuned)	        70%	              	      75%

Random Forest			            100%	                  75%

Random Forest (Tuned)		        98%       	              79%

Gradient Boosting Classifier        96%		                  69%

XGBoost (Hyperparameter Tuned)	    70%		                  75%
```
## ⚡ Challenges Faced	
	
  * Class Imbalance:
    Addressed with SMOTE to balance the minority class.

  * Overfitting in Random Forest:
		Mitigated by tuning hyperparameters to reduce complexity.
	
  * Handling Outliers:
		Detected and visualized using boxplots, but minimal impact after processing.

## ✅ Conclusion
	
  * Random Forest with hyperparameter tuning achieved the best performance with 79% test accuracy.
	
