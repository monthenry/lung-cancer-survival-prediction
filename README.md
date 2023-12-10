# Lung Cancer Survival Prediction with Synthetic Data

## Supervisor
Markus Haug, University of Tartu  

## Authors
- Henry Marie MONT
- Jean-Côme CARISSAN

## Motivation and Goal
This project aims to predict 5-year survival post-lung cancer diagnosis using synthetic medical data. The primary objectives are to identify key features for lung cancer treatment and find the most suitable models to predict 5-year survival so as to get the best AUC-ROC score possible when trying to predict with our model.

## Project Overview
The project is organized into several notebooks:

- **final-workflow.ipynb:** The main notebook that brings together data cleaning, feature engineering, feature selection, and model training using an ensemble of Gradient Boosting, XGBoost, Random Forest, and SVM. Every other notebook has mostly been used for exploration and testing purposes.
- **data-exploration.ipynb:** Explore the structure and characteristics of the provided data and proceeded to some very rudimentary training and predictions.
- **data-preprocessing.ipynb:** Preprocess the data, handle missing values, and prepare it for further analysis.
- **feature-selection.ipynb:** Experiment with feature selection techniques, including PCA and Stepwise Selection.
- **model-selection.ipynb:** Test and evaluate different machine learning models.
- **random_forest.ipynb:** Different tests and analysis with the Random Forest model.

## How to Replicate the Analysis
1. **Clone the Repository:**
```bash
git clone https://github.com/your-username/lung-cancer-survival-prediction.git
cd lung-cancer-survival-prediction
```

2. **Install Dependencies:**
```bash
pip install -r requirements.txt
```

3. **Run the Notebook:**  
The main file is **final-workflow.ipynb**. Simply run it with jupyter notebook on your set of data by replacing the path to your own csv file.

## Disclaimer  
You will find a lot of commented code in those notebooks. We have tried several things that didn't work out due to computational power limitation.  
As an example, we wanted to bin 'TIME' down to the year of the procedure and then merge it to the 'DEFINITION_ID' column so as to be able to one-hot encode the whole thing later and give some more valuable information to our model. But it resulted in too many features and our own laptops couldn't handle that.  
