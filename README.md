# Exoplanet Habitual Zone Analysis

This repository contains a comprehensive analysis of the exoplanet dataset to determine which planets are within the habitual zone. The analysis utilizes various machine learning techniques like Logistic Regression, Random Forest, and Lasso Regression.

## Project Overview

- **Objective:** To identify exoplanets within the habitual zone using statistical and machine learning models.
- **Dataset:** A publicly available exoplanet dataset is used for this analysis.

## Workflow and Steps

1. **Data Loading and Preprocessing:**
    - Load the dataset and clean up by handling missing values.
    - Apply transformations to certain variables and create new features, such as the binary `in_habitual_zone`.

2. **Exploratory Data Analysis:**
    - Use visualization techniques such as bar plots, scatter plots, and correlation matrices to understand the distribution and relationships in the data.

3. **Model Training:**

    - **Logistic Regression (Full and Reduced Models):**
        - Create a full logistic regression model to identify the importance of various features.
        - Reduce the model based on the correlation matrix and VIF values to eliminate collinear features.

    - **Random Forest Classifier:**
        - Implement a Random Forest classifier to compare the results and variable importance.

    - **Lasso Regression:**
        - Use cross-validated Lasso Regression to select optimal features while avoiding overfitting.

4. **Model Evaluation:**
    - **Confusion Matrix:** Generate confusion matrices for all models to evaluate accuracy, specificity, and sensitivity.
    - **ROC Curve:** Plot the ROC curves and calculate AUC values to compare model performance.

5. **Cross-Validation:**
    - Apply cross-validation to validate the models and ensure generalizability.

## How to Use This Repository

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/Mrudula666/632-project.git
    ```
2. **Install Dependencies:**
    - Ensure you have R and required libraries installed.
    - Install the R packages mentioned in the R script.

3. **Run the Analysis:**
    - Open the `.Rmd` or `.R` file in RStudio or an R IDE.
    - Execute the code chunks sequentially or knit the file to generate reports.

## Results and Findings

- The reduced logistic regression model shows a high overall accuracy of 96.4% and an AUC of 0.95, with specific sensitivity and specificity metrics reported.
- Random Forest provides an alternative method with significant feature importance insights.
- Lasso Regression helps refine the model by avoiding overfitting through feature selection.

## License

This repository is licensed under the MIT License.


