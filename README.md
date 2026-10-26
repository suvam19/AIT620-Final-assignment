AI4I 2020 Machine Failure Classification — Final Project
This repository contains an executed Jupyter Notebook investigating whether machine operating measurements can classify recorded machine-failure events in the synthetic AI4I 2020 dataset.
Files to upload
- AI4I_Predictive_Maintenance_Final.ipynb — fully executed, annotated notebook
- ai4i2020.csv — dataset needed to rerun the notebook
- AI4I_Predictive_Maintenance_Final.pdf — PDF printout for course submission
Requirements
Python 3 with pandas, numpy, matplotlib, scikit-learn (and seaborn, although the submitted charts use Matplotlib).
Run
Keep the CSV and notebook in the same folder. Open the notebook in Jupyter and choose Run All. Charts, summary tables, and metrics will appear inline. It has already been executed and contains saved outputs.
Study design
- 10,000 records, 339 machine-failure examples
- 7 exploratory charts plus evaluation visualizations
- Train/test stratified 80/20 split, seed 42
- Logistic Regression, Decision Tree, Random Forest
- Evaluate accuracy, precision, recall, F1, and ROC-AUC
- Exclude TWF, HDF, PWF, OSF, and RNF from predictors to prevent leakage
Limitations
Synthetic data. The observed failure status is not a guaranteed advance-warning target. No time-to-failure evaluation. Model comparisons are exploratory and should not be deployed without further validation.

Data source: UCI Machine Learning Repository, AI4I 2020 Predictive Maintenance Dataset (https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset)
