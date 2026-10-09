# Biomedical Data Analysis Pipeline

### Exploring Biomedical Data Using Python

## About This Project

This project is being developed as part of my independent learning alongside my MSc in Computer Science at the University of Birmingham.

With a background in Biomedical Science and experience using RStudio for experimental data analysis, I am expanding my programming skills by developing a reproducible Python-based biomedical data analysis pipeline.

The project will explore the Breast Cancer Wisconsin Diagnostic dataset, using statistical analysis, data visualisation and machine learning techniques.

## Project Objectives

- Import and explore a real biomedical dataset.
- Identify missing values and assess data quality.
- Perform exploratory data analysis using Python.
- Create scientific visualisations to investigate patterns.
- Apply appropriate statistical analysis techniques.
- Develop and evaluate a machine learning classification model.
- Document the workflow to support reproducibility.

## Technologies

**Planned tools:**
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- SciPy
- Scikit-learn
- Jupyter Notebook
- GitHub

## Dataset

**Breast Cancer Wisconsin Diagnostic Dataset**

A publicly available dataset containing numerical features derived from digitised images of breast cell nuclei, alongside benign and malignant diagnostic labels.

The dataset is available through the scikit-learn Python library.

## Project Progress

- [x] Create GitHub repository
- [x] Write initial project README
- [x] Import the dataset into Python
- [x] Explore and clean the dataset
- [x] Create scientific visualisations
- [x] Perform statistical analysis
- [x] Train and evaluate a classification model
- [x] Document findings and limitations

## Project Status

**In progress** — this repository will be updated as the analysis and implementation develop.

## Disclaimer

This is an educational programming and data analysis project. It is not intended for clinical diagnosis or medical decision-making.
## Machine Learning Results

### Classification Models

Two supervised machine-learning algorithms were implemented to classify benign and malignant observations from the Breast Cancer Wisconsin Diagnostic dataset:

- **Logistic Regression:** A linear classification model using standardised numerical features.
- **Random Forest:** An ensemble learning algorithm combining multiple decision trees.

The dataset was divided into 80% training and 20% testing data using a stratified split with a fixed random state for reproducibility.

### Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Test Accuracy | 96.49% | 97.37% |
| Correct Predictions | 110 | 111 |
| Incorrect Predictions | 4 | 3 |
| False Negatives | 3 | 3 |
| Malignant Recall | 92.86% | 92.86% |

Logistic Regression also achieved a mean five-fold cross-validation accuracy of 97.36% on the training data.

### Key Findings

Both models achieved high classification accuracy on the held-out test set. Random Forest produced one additional correct prediction compared with Logistic Regression.

However, both models incorrectly classified three malignant observations as benign. Consequently, their malignant recall was approximately 92.9%.

This highlights the importance of considering class-specific recall and false-negative errors rather than evaluating a classification model using overall accuracy alone.

### Limitations

- The dataset contains 569 observations and may not represent the diversity of real-world clinical populations.
- The reported test results come from one held-out split, so small differences between models should be interpreted cautiously.
- Further cross-validation, model selection and external validation would be required to assess generalisability.
- These models are educational demonstrations and are not suitable for clinical diagnosis.

### Future Improvements

- Compare both algorithms using stratified cross-validation.
- Investigate precision-recall trade-offs and classification thresholds.
- Explore feature importance and model interpretability.
- Evaluate additional models using appropriate validation procedures.
