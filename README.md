# Statistical Theory Final Project 📊

This project was developed as part of a university course on **Statistical Theory**.

## Project Objective
The aim of this study was to examine whether personality profiles explain variance in overall life happiness.
We constructed and analyzed two types of profiles:
- Intuitive (theory-driven) profiles – created by selecting conceptually related survey items based on theoretical reasoning, and calculating the mean score across these items for each respondent.
- Empirical (EFA-derived) profiles – created using exploratory factor analysis with oblimin rotation, allowing the statistical structure of the data to determine the grouping of items. Mean scores were then computed for the items loading on each factor

The analysis included:
- Scale construction and reliability checks (Cronbach’s α)
- Screening of background variables
- Ordinary Least Squares (OLS) regression with robust (HC3) standard errors
- Benjamini–Hochberg False Discovery Rate (FDR) correction
- Evaluation of incremental explanatory power (ΔR², effect sizes)
---

## How to Run

1. Make sure you have the dataset files: (The files in the repository)
   - responses.csv – original survey data (one row per respondent, columns = survey items)
   - columns.csv – mapping of survey item codes to full question text and variable type
     
 You can also download the original dataset file from Kaggle:  
 👉 https://www.kaggle.com/datasets/miroslavsabo/young-people-survey 

2. Place both files in the root directory of the project.

3. Run the main notebook: (`Statistical_Theory.ipynb`) or script (`.py`) to:
   - performs data loading, preprocessing, profile construction, regression modeling, and result         generation.  


👉 **Important:** Before running the notebook, execute the initial import cell to ensure all required libraries are loaded and the environment is prepared.

---
## Working with Data Files
-.csv files can be opened in Excel, Google Sheets, or loaded into Python using pandas.read_csv().
- The notebook produces:
  - Profile score tables
  - Regression coefficient tables
  - Model diagnostics and visualizations

---
## Key Files

- Statistical_Theory.ipynb – Main analysis notebook:
  - Data loading & cleaning
  - Profile construction (intuitive & EFA)
  - Reliability checks (Cronbach’s α)
  - OLS regression with robust inference
  - Multiple testing control (BH–FDR)
  - Visualizations & summary tables

- Statistical_Theory_Final_Project.pdf – Final written report including:
  - Abstract
  - Methodology
  - Results & Evaluation
  - Conclusions
  - Discussion: Interpretation of findings, theoretical implications, and limitations


