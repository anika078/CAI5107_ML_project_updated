# Parkinson's Disease Analysis using Decision Trees

This repository contains code and analysis for classifying Parkinson's Disease (PD) status and staging (Early vs. Advanced) using Decision Trees based on data collected from tablet-based assessments.

## Project Structure

The repository includes the following key files:

- `Parkinsons_vs_Control_Dataset.csv`: The main dataset containing DeviceMetric features and diagnosis/stage information.
- `feature_description_modified.csv`: A file describing the DeviceMetric features and their categories.
- Google Colab Notebook (e.g., `ML_DT_Project.ipynb`): The notebook containing the Python code for data loading, preprocessing, model training, evaluation, and visualization.

## How to Run the Code in Google Colab

1.  **Upload Files to Colab:**
    *   Download the `Parkinsons_vs_Control_Dataset.csv` and `feature_description_modified.csv` files from this repository.
    *   Open google colab Notebook 
    *   Upload the two CSV files to your Colab environment. 

2.  **Install Dependencies:**
    The code uses standard libraries like `pandas`, `numpy`, `matplotlib`, and `scikit-learn`. These are pre-installed in Google Colab.

3.  **Execute the Notebook Cells:**
    *   Run each cell in the notebook sequentially. The notebook is structured to perform the following steps:
        *   Load and preprocess the main dataset (`Parkinsons_vs_Control_Dataset.csv`).
        *   Perform classification of PD vs. Control using a Decision Tree.
        *   Evaluate the model using various metrics (Accuracy, Precision, Recall, F1, AUROC) and visualize results (Confusion Matrix, ROC, PR curves, Decision Tree plot).
        *   Perform K-Fold Cross-Validation and paired t-tests to compare model variations 
        *   Perform category-wise analysis for PD vs. Control, evaluating models trained on subsets of features (Motor, Memory, Speech, Executive Function).
        *   Perform PD staging (Early vs. Advanced) classification.
        *   Perform K-Fold Cross-Validation and paired t-tests to compare model variations for staging 
        *   Perform category-wise analysis for PD staging.

4.  **View Results:**
    *   The notebook will display printed output of metrics, classification reports, and confusion matrices.
    *   Plots (Decision Trees, Confusion Matrices, ROC curves, PR curves) will be generated and displayed within the notebook. Image files are also included in the code compilation.

## Dataset

The `Parkinsons_vs_Control_Dataset.csv` contains data from tablet-based assessments. The relevant columns for this analysis include:

- `UniqueID`: Unique identifier for each participant.
- `Stage`: Diagnosis/Stage of Parkinson's Disease (0 for Control, >0 for PD).
- `DeviceMetric_1` through `DeviceMetric_57`: Numerical features extracted from the tablet assessments.

The `feature_description_modified.csv` provides a mapping of `DeviceMetric` features to cognitive categories (e.g., Motor, Memory, Speech, Executive Function).

## Analysis Highlights

*   The notebook demonstrates how to build and evaluate Decision Tree models for both PD vs. Control classification and Early vs. Advanced PD staging.
*   Category-wise analysis helps understand which groups of features are most predictive of PD status and stage.
*   Cross-validation and paired t-tests provide a more robust evaluation of model performance and comparisons.



