# Obesity Risk Research - USC CSCI461 Final Project

**Med Minds Team**: James Simon, Shashank Joshi, Emma Yue, Phani Yalamanchili

## Live Website

The project website is hosted on GitHub Pages:
https://jamescsimon.github.io/Obesity-Risk-Research-USC/

## Overview

This repository hosts the GitHub Pages website for our machine learning research on predicting Body Mass Index (BMI) using survey-based data from the Behavioral Risk Factor Surveillance System (BRFSS) 2024 dataset.

We developed and evaluated seven machine learning models for BMI prediction, identifying 16 optimal predictors from 302 available variables. Our Stacking Ensemble achieves strong performance with R² = 0.8858, MAE = 2.26 BMI points, and 96.3% within-1-category accuracy, demonstrating the feasibility of survey-based obesity prediction at population scales.

## Research Highlights

Our work addresses the challenge of scalable population-level obesity screening by enabling BMI prediction using easily accessible survey features rather than requiring clinical visits. Key findings include:

- Feature selection reduced dimensionality from 302 variables to 16 optimal predictors (94.7% reduction)
- Evaluation of seven ML models: Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting, Voting Ensemble, and Stacking Ensemble
- Best performing model: Stacking Ensemble with R² = 0.8858 and MAE = 2.26 BMI points
- Comprehensive fairness analysis across demographic groups (race, sex, income, age)
- 96.3% within-1-category accuracy for BMI classification

## Repository Contents

This repository contains only the files necessary for the GitHub Pages website:

```
.
├── website/
│   ├── index.html          # Main website (single-page application)
│   └── .nojekyll           # GitHub Pages configuration
├── final_report/
│   └── latex_report/
│       └── Med_Minds_James_Simon_ProjectFinalReport_fall2025.pdf
├── index.html              # Root redirect to website
├── README.md               # This file
└── .gitignore              # Excludes large files from repository
```

Note: Large data files, Jupyter notebooks, and model files are excluded from this repository to keep it manageable. The full research code and datasets are stored separately.

## Website Features

The website includes three main sections:

**Overview**: Project introduction, research objectives, dataset information, and key results.

**Paper**: Embedded PDF viewer for the complete research paper, which includes detailed methodology, feature selection, model evaluation, fairness analysis, and comprehensive results.

**Interactive Tool**: BMI prediction interface where users can input demographic information and health features to receive predicted BMI category classifications, along with relevant health resources based on predicted categories.

## Project Structure

The complete research implementation includes:
- Data preprocessing and balancing pipeline
- Feature selection from 302 BRFSS variables to 16 optimal features
- Model training and evaluation across seven algorithms
- Fairness analysis across demographic dimensions
- Comprehensive visualization generation

The main Jupyter notebook (`final_notebook/Med_Minds/Med-Minds-Final-Project.ipynb`) contains the complete implementation. Due to repository size constraints, the full codebase is stored separately.

## Methodology Summary

Our approach follows three main stages:

1. **Data Preparation**: Load BRFSS 2024 dataset, preprocess missing values, create balanced dataset of 100,000 samples with equal representation across BMI categories.

2. **Model Development**: Perform feature selection on training data (80,000 samples), train seven ML models, evaluate on test set (20,000 samples).

3. **Evaluation and Analysis**: Comprehensive evaluation using regression, classification, and fairness metrics. Systematic subgroup analysis across demographic groups to identify disparities.

## Key Results

**Regression Performance**: Stacking Ensemble achieves RMSE = 3.32, MAE = 2.26 BMI points, R² = 0.8858

**Classification Performance**: Accuracy = 0.8879, Precision = 0.8881, Recall = 0.8875, F1 = 0.8878, AUC-ROC = 0.9588

**Category Accuracy**: Exact match = 65.1%, Within-1-category = 96.3%

**Fairness Analysis**: Identified disparities across race/ethnicity (Δ MAE = 0.86), income (Δ MAE = 0.79), sex (Δ MAE = 0.42), and age (Δ MAE = 0.12)

## Team Contributions

- **James Simon**: Project conceptualization, literature review, paper writing, fairness analysis, feature selection
- **Shashank Joshi**: Project conceptualization, model training and evaluation, feature selection, paper writing
- **Emma Yue**: Visualizations, presentation, data preprocessing, risk estimation
- **Phani Yalamanchili**: Presentation, flowcharts, feature selection, data preprocessing

## Citation

If you use this work, please cite:

```
Med Minds Team. (2024). Obesity Risk Prediction Using Machine Learning 
on BRFSS Survey Data. USC CSCI461 Final Project.
```

## License

This project is part of USC's CSCI461 course work.

## Contact

For questions about the research, please refer to the contact information in the research paper or reach out through the project repository.
