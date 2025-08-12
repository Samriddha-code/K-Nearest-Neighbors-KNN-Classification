# K-Nearest Neighbors (KNN) Classification on the Iris Dataset

## Overview
This project implements a K-Nearest Neighbors (KNN) classification model using the Iris flower dataset. The goal is to classify iris species based on four features: Sepal Length, Sepal Width, Petal Length, and Petal Width. The project includes data preprocessing, model training, evaluation, parameter tuning, and visualization.

## Project Structure
- **iris.csv**: The original Iris dataset containing 150 samples with features and species labels.
- **knn_iris.ipynb**: Jupyter Notebook implementing the KNN classification pipeline with detailed steps and visualizations.
- **README.md**: This file, describing the project.

## Steps Performed

1. **Data Loading and Exploration**
   - Loaded Iris dataset.
   - Checked for missing values and data types.
   - Verified that the dataset contains no missing values and only one categorical target column.

2. **Data Preprocessing**
   - Separated features and target labels.
   - Split data into 70% training and 30% testing sets with stratified sampling.
   - Normalized numeric features using StandardScaler to ensure fair distance calculations in KNN.

3. **KNN Model Training and Evaluation**
   - Trained initial KNN model with K=3 neighbors.
   - Evaluated on test data using accuracy, confusion matrix, and classification report.
   - Achieved high accuracy (~95.5%) on test data.

4. **Optimal K Selection**
   - Tested K values from 1 to 20.
   - Found the best K based on test accuracy.
   - Visualized accuracy versus K to understand the effect of neighborhood size.

5. **Visualization**
   - Plotted the accuracy against different K values.
   - Visualized decision boundaries for the model using two features (Petal Length and Petal Width).

## Summary of Findings

- The KNN classifier performs well on the Iris dataset with normalized features.
- The best K value was found to be 3, which yielded the highest accuracy.
- Normalization of features is crucial because KNN is a distance-based algorithm.
- Visualization of decision boundaries helps in understanding the model’s behavior.

