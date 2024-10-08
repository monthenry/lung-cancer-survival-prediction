# Lung Cancer Survival Prediction with Synthetic Data

## Overview
This project aims to predict 5-year survival rates following a lung cancer diagnosis using synthetic medical data. By identifying key features from patient treatment trajectories and evaluating various machine learning models, we strive to achieve an optimal AUC-ROC score for our predictions.

### Authors
- **Henry Marie MONT**
- **Jean-Côme CARISSAN**

### Supervisor
- **Markus Haug, University of Tartu**

## Motivation and Goals
Lung cancer remains one of the leading causes of cancer-related deaths worldwide. This project focuses on developing a predictive model that assists in understanding patient outcomes and improving treatment strategies by leveraging synthetic data. Our main goals are:
- Identify crucial features impacting lung cancer survival.
- Compare and select the most effective machine learning models for accurate survival predictions.

## Project Structure
The project is organized into several Jupyter notebooks, each serving a specific purpose in the data analysis workflow:

- **`final-workflow.ipynb`**: The primary notebook integrating data cleaning, feature engineering, and model training using an ensemble of Gradient Boosting, XGBoost, Random Forest, and SVM.

- **`data-exploration.ipynb`**: Explores the structure and characteristics of the provided data, including preliminary training and predictions.

- **`data-preprocessing.ipynb`**: Preprocesses the data by handling missing values and preparing it for analysis.

- **`feature-selection.ipynb`**: Experiments with feature selection techniques, such as PCA and Stepwise Selection.

- **`model-selection.ipynb`**: Tests and evaluates different machine learning models to identify the best performer.

- **`random_forest.ipynb`**: Conducts various tests and analyses using the Random Forest model.

## How to Replicate the Analysis

### Clone the Repository
```bash
git clone https://github.com/your-username/lung-cancer-survival-prediction.git
cd lung-cancer-survival-prediction
```

### Install Dependencies
Install the required packages using the following command:
```bash
pip install -r requirements.txt
```

### Run the Notebook
To run the analysis, open the main notebook:
```bash
jupyter notebook final-workflow.ipynb
```
Make sure to replace the file path in the notebook with the path to your own CSV file containing synthetic data.

## Disclaimer
Some notebooks contain commented-out code reflecting experiments that did not yield satisfactory results due to computational power limitations. For instance, attempts to bin the 'TIME' variable into yearly intervals resulted in too many features, which overwhelmed our local computational resources.

The synthetic medical data is not included in the repo as it is too big.

## Conclusion
This project not only aims to predict survival rates but also enhances understanding of the critical factors affecting lung cancer outcomes. We invite contributions and feedback from the community to improve our model further.

---

For questions or collaboration inquiries, please contact the authors via their respective emails.