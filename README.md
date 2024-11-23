# Music Popularity Prediction

This project focuses on analyzing a dataset of song tracks and predicting their popularity based on various features. The dataset undergoes extensive preprocessing, including cleaning and feature engineering, followed by the application of machine learning models for both regression and classification tasks. Using Python libraries like pandas, scikit-learn, and pycaret, the project employs algorithms such as Gradient Boosting, Random Forest, Decision Trees, XGBoost, and K-Nearest Neighbors to predict popularity scores.
The analysis begins with the removal of irrelevant columns and label encoding of categorical features like track_genre. Following this, a regression model (RandomForestRegressor) is trained to predict the continuous popularity score. To enhance performance, feature selection is done using mutual information, and various models are evaluated using R² scores.
Subsequently, the target variable, popularity, is binned into categories (e.g., 'Top 30', 'Below 30') for classification tasks. The classification models, including RandomForestClassifier, DecisionTreeClassifier, XGBClassifier, and KNeighborsClassifier, are trained and evaluated based on accuracy and F1 scores. The project aims to determine which factors most influence a song's popularity and create accurate predictions using these machine learning models.

### Requirements:
- Python 3.12.4
- Jupyter Notebook 7.1
- Libraries: pandas, matplotlib, numpy, scikit-learn, pycaret

### Exploratory Data Analysis (EDA)
**Data Cleaning:**
- **Data Loading:** Imports the dataset from a CSV file hosted on Google Sheets for further analysis.
- **Column Removal:** Drops irrelevant columns (e.g., track_id, track_name, Unnamed: 0, and artists) to simplify the dataset and focus on the most important features.
- **Missing Value Handling:** Fills missing values in the album_name column with the most frequent value (mode) to ensure no missing data.
- **Categorical Data Transformation:** Uses Label Encoding to convert categorical features (e.g., track_genre) into numeric values suitable for machine learning algorithms.
- **Target Variable Binning:** Converts the continuous popularity into categorical bins (e.g., 0-20, 20-40) to prepare the dataset for classification tasks.
  
### Machine Learning Algorithms
**Random Forest Classifier:**
- Purpose: This classifier predicts the popularity category of songs after binning the popularity values (e.g., "Top 30" vs "Below 30"). It uses an ensemble of decision trees to make predictions by averaging the outputs of multiple trees to improve accuracy.

**Decision Tree Classifier:**
- Purpose: A decision tree is used to classify songs into popularity categories based on their features. It recursively splits the data based on feature values to create decision nodes and make predictions.

**XGBoost Classifier:**
- Purpose: XGBoost is a powerful gradient boosting algorithm that combines multiple weak classifiers into a strong one, improving prediction accuracy for the popularity categories.

**K-Nearest Neighbors (KNN) Classifier:**
- Purpose: KNN is a simple, non-parametric algorithm that classifies songs based on the majority class of the 'K' nearest neighbors in the feature space.
  
### Feature Selection:
- **SelectKBest:** Identifies the most important features based on their relationship with the target variable to improve model performance.
- **Mutual Information:** Measures feature dependencies with the target variable, aiding in the selection of relevant features for classification models.

### Model Evaluation:
- **Regression Model Evaluation:** Evaluates the Random Forest Regressor and Gradient Boosting Regressor models using R² score, measuring how well the model captures the variance in song popularity.
- **Classification Model Evaluation:** After transforming popularity into bins, evaluates the Random Forest Classifier using accuracy and F1 score to determine how well it classifies songs into popularity categories.

### Project Screenshot
![Alt text](https://github.com/brianwpiano/Music-Popularity-Prediction/blob/main/Screenshot%202024-11-22%20201135.png)
![Alt text](https://github.com/brianwpiano/Music-Popularity-Prediction/blob/main/Screenshot%202024-11-22%20201159.png)
![Alt text](https://github.com/brianwpiano/Music-Popularity-Prediction/blob/main/Screenshot%202024-11-22%20204232.png)


## Run the app

Clone this repo then `cd Music-Popularity-Prediction`.

Assuming you have Python3 installed on a Windows 10 or 11 or on MacOS, run this commands:

``` bash
Music-Popularity-Prediction.ipynb
```

---
