# Smart Regional Inclusion Analysis System using Artificial Immune System (AIS)   

## Overview

The **Smart Regional Inclusion Analysis System** is an intelligent machine learning project designed to analyze and predict **district-wise Scheduled Caste (SC) population inclusion patterns** using historical demographic data and engineered regional growth indicators. The project applies the **Artificial Immune System (AIS)** optimization algorithm to improve the performance of a **Random Forest Regressor** for predicting the **2011 total Scheduled Caste population percentage**.

The system analyzes district-level Scheduled Caste population percentages across **rural, urban, and total population segments** for the years **2001 and 2011**. It also derives intelligent demographic indicators such as **population growth, rural-urban disparity, average inclusion percentage, and priority score** to identify districts requiring higher regional inclusion attention.

In addition to regression-based prediction, the project categorizes districts into **Low**, **Medium**, and **High Priority** regional inclusion groups using a calculated **Priority Score**, enabling data-driven social welfare planning and demographic intelligence.

---

# Objectives

- Predict district-wise **2011 total Scheduled Caste population percentage**.
- Optimize Random Forest using **Artificial Immune System (AIS)**.
- Estimate a **regional inclusion priority score** for each district.
- Analyze rural, urban, and total SC population growth patterns.
- Generate complete analytics, prediction outputs, and visualizations.
- Save trained models for future deployment and research use.
- Support intelligent regional inclusion planning and demographic policy analysis.

---

# Dataset

Dataset used:

```text
Percentage_of_Scheduled_Caste_Population_to_Total_Population.csv

Dataset Location:

Regional Inclusion Analysis System/
Machine Learning Workflow
Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
District Encoding
      │
      ▼
Feature Scaling
      │
      ▼
Train-Test Split
      │
      ▼
AIS Feature Weight Optimization
      │
      ▼
Optimized Random Forest Regressor
      │
      ▼
Deep Learning Model
      │
      ▼
Prediction
      │
      ▼
Evaluation
      │
      ▼
Visualization
      │
      ▼
Save Models and Outputs
Feature Engineering

The following intelligent demographic features are generated automatically.

Rural Growth
Urban Growth
Total Growth
Rural-Urban Gap (2001)
Rural-Urban Gap (2011)
Average SC Percentage
Priority Score
AIS Priority Category
Artificial Immune System (AIS)

AIS is a bio-inspired optimization algorithm based on the working principles of the human immune system.

It performs:

Antibody generation
Candidate selection
Cloning
Mutation
Affinity evaluation using R² score
Selection of the best antibody

The optimized antibody represents the best feature weight combination for the Random Forest model.

Optimized Parameters / Outputs include:

Best Feature Weight Vector
Best R² Score
AIS Convergence History
Machine Learning Models

The project uses and compares the following models.

AIS Optimized Random Forest Regressor
Artificial Neural Network (ANN)
Regression Model

The primary prediction target is:

2011 Total Scheduled Caste Population Percentage

Regression Metrics:

MAE
MSE
RMSE
R² Score
Accuracy Percentage
Performance Metrics

Regression Metrics:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score
Accuracy Percentage
Dataset Columns

The original dataset contains the following district-level demographic fields:

District
Percentage of Scheduled Caste Population _2001_Rural
Percentage of Scheduled Caste Population _2001_Urban
Percentage of Scheduled Caste Population _2001_Total
Percentage of Scheduled Caste Population _2011_Rural
Percentage of Scheduled Caste Population _2011_Urban
Percentage of Scheduled Caste Population _2011_Total
Engineered Features

The project automatically creates the following derived features:

Rural_Growth = Rural SC % in 2011 − Rural SC % in 2001
Urban_Growth = Urban SC % in 2011 − Urban SC % in 2001
Total_Growth = Total SC % in 2011 − Total SC % in 2001
Rural_Urban_Gap_2001 = Rural SC % in 2001 − Urban SC % in 2001
Rural_Urban_Gap_2011 = Rural SC % in 2011 − Urban SC % in 2011
Average_SC_Percentage = Mean of all SC percentage values across 2001 and 2011
Priority_Score = Weighted demographic inclusion priority score
AIS_Priority_Category = Low / Medium / High priority label
Priority Score Formula

The system calculates a regional inclusion priority score using the following formula:

Priority_Score = (
    Total_2011 * 0.6 +
    Total_Growth * 0.3 +
    abs(Rural_Urban_Gap_2011) * 0.1
)

This score is used to classify districts into:

Low Priority
Medium Priority
High Priority
Input Features Used for Modeling

The following columns are used as input features:

District_Encoded
Percentage of Scheduled Caste Population _2001_Rural
Percentage of Scheduled Caste Population _2001_Urban
Percentage of Scheduled Caste Population _2001_Total
Percentage of Scheduled Caste Population _2011_Rural
Percentage of Scheduled Caste Population _2011_Urban
Rural_Growth
Urban_Growth
Total_Growth
Rural_Urban_Gap_2001
Rural_Urban_Gap_2011
Average_SC_Percentage
Priority_Score
Target Variable

The regression target used in this project is:

Percentage of Scheduled Caste Population _2011_Total
Project Structure
Regional Inclusion Analysis System/
│
├── Percentage_of_Scheduled_Caste_Population_to_Total_Population.csv
│
├── ais_model.h5
├── ais_model.pkl
├── ais_config.yaml
├── ais_results.json
│
├── ais_result.csv
├── ais_prediction.csv
├── ais_full_dataset_result.csv
│
├── ais_accuracy_graph.png
├── ais_heatmap.png
├── ais_comparison_graph.png
├── ais_result_graph.png
├── ais_prediction_graph.png
├── ais_convergence_graph.png
├── ais_growth_graph.png
├── ais_training_graph.png
│
└── README.md
Generated Outputs
Models
H5 Model
PKL Model
Configuration Files
YAML Configuration
JSON Metadata
CSV Files
Result CSV
Prediction CSV
Full Dataset Result CSV
Graphs
Accuracy Graph
Heatmap
Comparison Graph
Result Graph
Prediction Graph
AIS Convergence Graph
Growth Graph
Deep Learning Training Graph
Visualization
Growth Visualization

The AIS Growth Graph highlights the top districts by Scheduled Caste population growth between 2001 and 2011.

It helps in identifying districts that have experienced the strongest change in SC population percentage and therefore may require focused regional inclusion planning, welfare support, and demographic analysis.

Model Evaluation Metrics

The project evaluates the AIS-optimized model using the following metrics:

Metric	Description
MAE	Mean Absolute Error
MSE	Mean Squared Error
RMSE	Root Mean Squared Error
R² Score	Goodness-of-fit score for regression
Accuracy Percentage	R² score converted to percentage
Technologies Used
Python
Pandas
NumPy
Scikit-learn
TensorFlow / Keras
Matplotlib
YAML
Pickle
JSON
Installation

Install dependencies:

pip install pandas
pip install numpy
pip install matplotlib
pip install scikit-learn
pip install tensorflow
pip install pyyaml

or

pip install pandas numpy matplotlib scikit-learn tensorflow pyyaml
Running the Project

Execute the AIS project file:

python ais_regional_inclusion.py

or run the Jupyter Notebook cells sequentially.

Results

The system automatically:

Loads the district-wise SC population dataset
Cleans and preprocesses the data
Performs demographic feature engineering
Encodes district names
Scales numerical features
Applies AIS-based feature weight optimization
Trains Random Forest and Deep Learning models
Predicts 2011 total SC population percentage
Calculates district inclusion priority score
Categorizes districts into priority groups
Evaluates model performance
Generates visualizations
Saves trained models and output files
Applications

The project can be used for:

Regional Inclusion Planning
Scheduled Caste Population Analysis
District-level Welfare Planning
Rural vs Urban Demographic Comparison
Government Resource Allocation
Social Equity and Inclusion Research
Educational and Scholarship Planning
Public Policy Support Systems
Demographic Intelligence Dashboards
Future Enhancements
GIS-based district mapping
Future SC percentage forecasting for 2021 and beyond
Streamlit / Flask dashboard integration
Inclusion of literacy, income, healthcare, and education indicators
Multi-state comparative regional inclusion analysis
Explainable AI for demographic prediction
Cloud deployment for real-time policy dashboards
Author

Sagnik Patra

M.Tech (Computer Science & Engineering)

Machine Learning | Artificial Intelligence | Data Science | Bio-inspired Optimization

License

This project is developed for educational and research purposes.
