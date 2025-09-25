LA_Crime

A data analysis & machine learning project focused on crime trends in Los Angeles. This repository includes data preprocessing, exploratory data analysis (EDA), visualizations, and predictive modeling efforts.

Table of Contents

Project Overview

Data

Getting Started

Prerequisites

Installation

Usage

Notebook / Workflow

Results & Visualizations

Modeling

Contributing

License

Contact

Project Overview

The goal of this project is to explore and analyze crime data from Los Angeles to uncover patterns and, where possible, build a predictive model to forecast crime occurrences. The project covers:

Data cleaning and preprocessing

Exploratory Data Analysis (EDA) to understand crime trends by category, location, and time

Visualization of temporal and spatial patterns

Regression / predictive modeling to estimate crime occurrence or trends

Data

LA_Crime_dataset.csv — the primary dataset used for analysis

regression dataset/ — contains derived/processed data used for modeling

The data includes (but may not be limited to) crime incident types, locations (e.g. neighborhoods or coordinates), timestamps, and related features.

Getting Started
Prerequisites

Python 3.7 or newer

Environment management tool (e.g. conda or venv)

Packages as specified in environment.yml

Installation

Clone the repository:

git clone https://github.com/smusab9152/LA_Crime.git
cd LA_Crime


Create and activate the environment:

conda env create -f environment.yml
conda activate LA_Crime


Or, if you prefer venv/pip, install dependencies from a requirements.txt (you may create one) or manually.

Usage

Launch Jupyter / JupyterLab:

jupyter notebook


Open Regression_Notebook.ipynb to follow through the analysis and modeling workflow.

You can also import scripts or modules (if you break the notebook into .py files) and generate visualizations or predictions programmatically.

Notebook / Workflow

The Regression_Notebook.ipynb is the core of your workflow:

Data Preprocessing — handling missing values, encoding, feature engineering

Exploratory Data Analysis (EDA) — inspect distributions, correlations, temporal trends

Visualization — maps, time-series plots, histograms, etc.

Modeling — training regression or classification models, evaluating performance

Interpretation & Insights — examining which features influence crime prediction

Results & Visualizations

Visual outputs include:

Crime counts over time (yearly, monthly, daily)

Distribution of crime types

Heatmaps or geospatial plots of crime across neighborhoods or geographic coordinates

Feature importance charts from the modeling stage

You may export figures or embed them in a final report or presentation.

Modeling

Models used may include linear regression, random forest, or other regression / classification algorithms (based on your notebook).

Performance metrics (e.g. RMSE, MAE, R²) are computed to evaluate predictive accuracy.

You may further experiment with hyperparameter tuning or additional models like XGBoost, etc.
