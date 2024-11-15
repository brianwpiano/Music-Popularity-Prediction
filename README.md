# Music Popularity Prediction

This project is focused on analyzing the dataset of song tracks, exploring their features, and building predictive models to understand the factors influencing their popularity. We use machine learning techniques for both regression and classification tasks, and data manipulation is done using Python libraries like pandas, scikit-learn, and pycaret. The project involves data preprocessing, feature selection, model training, and evaluation, followed by the creation of classification bins to predict the song popularity as a category.

### Requirements:
- Python 3.12.4
- Jupyter Notebook 7.1
- Libraries: pandas, matplotlib, numpy, scikit-learn, pycaret

### Features
Data Cleaning:
- Data Loading: Imports the dataset from a CSV file hosted on Google Sheets for further analysis.
- Column Removal: Drops irrelevant columns (e.g., track_id, track_name, Unnamed: 0, and artists) to simplify the dataset and focus on the most important features.
- Missing Value Handling: Fills missing values in the album_name column with the most frequent value (mode) to ensure no missing data.
- Categorical Data Transformation: Uses Label Encoding to convert categorical features (e.g., track_genre) into numeric values suitable for machine learning algorithms.
- Target Variable Binning: Converts the continuous popularity into categorical bins (e.g., 0-20, 20-40) to prepare the dataset for classification tasks.
Machine Learning Algorithms:
- Gradient Boosting Regressor: Predicts the continuous popularity of songs based on their features. Evaluates model performance using R² score to measure variance explained.
- Random Forest Regressor: Another regression method used to predict popularity, focusing on robustness and handling complex datasets.
- Random Forest Classifier: After binning the popularity into categories, this classifier predicts the popularity bin. Evaluates performance with accuracy and F1 score.
Feature Selection:
- SelectKBest: Identifies the most important features based on their relationship with the target variable to improve model performance.
- Mutual Information: Measures feature dependencies with the target variable, aiding in the selection of relevant features for classification models.
Visualizations:
- R² Score vs. Number of Features: Generates bar plots to show how the number of selected features affects the R² score (for regression tasks) or F1 score (for classification tasks).
- Feature Importance: Creates visualizations to highlight the relative importance of each feature in predicting song popularity, helping to understand which features matter most.
Model Evaluation:
- Regression Model Evaluation: Evaluates the Random Forest Regressor and Gradient Boosting Regressor models using R² score, measuring how well the model captures the variance in song popularity.
- Classification Model Evaluation: After transforming popularity into bins, evaluates the Random Forest Classifier using accuracy and F1 score to determine how well it classifies songs into popularity categories.
Database Management:
- Data is effectively managed and manipulated using pandas for efficient retrieval and transformation, ensuring clean data for analysis and model training.

### Project Screenshot
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220651.png)
![Alt text](https://github.com/brianwpiano/Billboard-Hot100-Analysis/blob/main/Screenshot%202024-10-14%20120449.png)
![Alt text](https://github.com/brianwpiano/Billboard-Hot100-Analysis/blob/main/Screenshot%202024-10-14%20121207.png)
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220435.png)
![Alt text](https://github.com/brianwpiano/Billboard-Hot100-Analysis/blob/main/Screenshot%202024-10-14%20120823.png)
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220523.png)
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220548.png)
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220601.png)
![Alt text](https://github.com/brianwpiano/billboard-hot100-analysis/blob/main/Screenshot%202024-10-02%20220617.png)

## Run the app

Clone this repo then `cd Music-Popularity-Prediction`.

Assuming you have Python3 installed on a Windows 10 or 11 or on MacOS, run this commands:

``` bash
Music-Popularity-Prediction.ipynb
```

---
