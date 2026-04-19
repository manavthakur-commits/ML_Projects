# Aqueous Solubility Prediction using Machine Learning

## Overview
This project builds machine learning models to predict the aqueous solubility (`logS`) of chemical compounds based on their structural and molecular properties. 

## Dataset
The model is trained on the **Delaney Solubility Dataset**, a well-known benchmark dataset in cheminformatics used for solubility prediction. 

## Features Used
The predictive models utilize the following four molecular descriptors:
1. **MolWt**: Molecular Weight
2. **MolLogP**: Octanol-water partition coefficient (a measure of hydrophobicity)
3. **NumRotatableBonds**: Number of rotatable bonds
4. **AromaticProportion**: Proportion of heavy atoms in the molecule that are in an aromatic ring

## Models Built
The notebook implements and compares the performance of two different regression algorithms:
* **Linear Regression:** Serves as a baseline model to capture direct linear relationships between the features and solubility.
* **Random Forest Regressor:** An ensemble learning method (configured with `max_depth=2`) used to capture non-linear relationships in the data while preventing overfitting.

## Evaluation Metrics
The models are evaluated on a 20% test split using:
* **Mean Squared Error (MSE):** Measures the average squared difference between the estimated and actual solubility values.
* **R-squared ($R^2$) Score:** Represents the proportion of the variance in solubility that is predictable from the molecular features.

## Requirements
To run this notebook locally or in a cloud environment, you will need the following standard Python libraries:
* `pandas`
* `scikit-learn`

## Usage
1. Upload the `ML_Project.ipynb` notebook to Google Colab, or open it locally using Jupyter Notebook.
2. Run the cells sequentially from top to bottom.
3. The notebook will automatically download the dataset, train the models, and output the comparative evaluation metrics.
