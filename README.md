# Obesity Risk Research - USC CSCI461 Final Project

**Med Minds Team**: James Simon, Shashank Joshi, Emma Yue, Phani Yalamanchili

## 🌐 Live Website

**Visit our interactive website**: [https://jamescsimon.github.io/Obesity-Risk-Research-USC/](https://jamescsimon.github.io/Obesity-Risk-Research-USC/)

## Overview

This repository hosts the GitHub Pages website for our comprehensive machine learning research on predicting Body Mass Index (BMI) using survey-based data from the Behavioral Risk Factor Surveillance System (BRFSS) 2024 dataset.

### Key Research Highlights

- **16 optimal features** selected from 302 available BRFSS variables
- **Seven ML models** evaluated (Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting, Voting, Stacking)
- **Stacking Ensemble** achieves **R² = 0.8858**, **MAE = 2.26 BMI points**
- **96.3% within-1-category accuracy** for BMI classification
- **Comprehensive fairness analysis** across demographic groups

## Website Features

### 📄 Research Paper
- Complete PDF of the research paper embedded in the website
- Available for download

### 💻 Code Repository
- Links to Jupyter notebooks (stored in separate repository if needed)
- Complete implementation details

### 🎯 Interactive BMI Prediction Tool
- Input your demographic information and health features
- Get predicted BMI category
- Compare to demographic averages
- Access health resources based on your category

## Repository Contents

This repository contains only what's needed for the website:

```
.
├── website/                      # Main website files
│   ├── index.html               # Complete website (single page)
│   └── .nojekyll                # GitHub Pages config
├── final_report/
│   └── latex_report/
│       └── Med_Minds_James_Simon_ProjectFinalReport_fall2025.pdf
├── index.html                   # Root redirect to website
└── README.md                    # This file
```

**Note**: Large data files, notebooks, and model files are excluded from this repository. The full research code and data are available in a separate private repository or can be accessed via the links in the website.

## Quick Links

- **Website**: [https://jamescsimon.github.io/Obesity-Risk-Research-USC/](https://jamescsimon.github.io/Obesity-Risk-Research-USC/)
- **Research Paper**: View on website or download PDF

## License

This project is part of USC's CSCI461 course work.
