## Lab Activity 4.2 — Analyzing Customer Satisfaction Levels
Objective
To develop and test null and alternative hypotheses to examine customer satisfaction differences across service sectors, and determine whether order accuracy significantly affects customer satisfaction.

Dataset
Customer Satisfaction (10k) dataset from Kaggle:
🔗 Kaggle Dataset Link

Requirements

Computer with Python and Jupyter Notebook installed
Python Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels


Prerequisites

Basic Python programming knowledge
Understanding of statistics, especially hypothesis testing
Familiarity with pandas for data manipulation
Understanding of data visualization using matplotlib and seaborn


Problem Statement
Analyze customer satisfaction levels across different service factors — delivery experience, food quality, and delivery speed — and test whether order accuracy has a statistically significant effect on customer satisfaction.

Steps
StepTask1Import required libraries (pandas, numpy, matplotlib, seaborn, scipy)2Load the dataset (customer-satisfaction.csv)3Rename columns for easier access4Clean missing values using dropna()5Convert Order_Accuracy from categorical (Yes/No) to numerical (1/0)6Print summary statistics using df.describe()7Perform Independent t-test (ttest_ind) on delivery satisfaction by order accuracy8Visualize results using a boxplot

Hypothesis
HypothesisStatementH₀ (Null)Order accuracy does not impact delivery satisfactionH₁ (Alternate)Order accuracy does impact delivery satisfaction

Key Concept — Decision Rule
ResultConclusionp-value < 0.05Reject H₀ — order accuracy significantly affects customer satisfactionp-value ≥ 0.05Fail to reject H₀ — no significant relationship found

Visualization

Boxplot — Order_Accuracy (x-axis) vs Delivery_Satisfaction (y-axis) to visually compare satisfaction levels between accurate and inaccurate orders


Tech Stack
LibraryUsagepandasData loading and manipulationnumpyNumerical operationsmatplotlibPlottingseabornBoxplot visualizationscipyIndependent t-test (ttest_ind)statsmodelsAdditional statistical analysis

File Structure
Lab4_2/
├── Lab4_2.ipynb                  # Main notebook
├── customer-satisfaction.csv     # Dataset
└── README.md                     # This file

Conclusion
If the p-value < 0.05, order accuracy significantly impacts delivery satisfaction — reject H₀. If the p-value ≥ 0.05, there is no significant relationship — fail to reject H₀. This analysis helps businesses understand which service factors most influence customer satisfaction and where improvements should be focused.
