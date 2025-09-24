LA Crime Data Analysis

A machine learning + exploratory data analysis project investigating crime in Los Angeles using a local crime dataset and Jupyter Notebook visualizations.

Table of contents

Repository structure

Getting started

Prerequisites

Install and activate environment

Run the notebook

What’s in this repo

Machine learning & analysis

Dataset

Future work

Contributing

License

Author

Repository structure
.
├── LA_Crime_Analysis.ipynb     # Main Jupyter Notebook (EDA, visualizations, ML experiments)
├── la_crime_data.csv           # Dataset of LA crime records used in the notebook
├── enviroment.yml              # Conda environment file with dependencies
└── README.md                   # This file

Getting started
Prerequisites

Conda (recommended)
 or Python 3.x and pip

Jupyter Notebook / Jupyter Lab

Typical libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, folium (for maps)

Install and activate environment

If you use the provided Conda environment file:

# create environment from file
conda env create -f enviroment.yml

# activate it
conda activate la_crime


Or install the essentials with pip:

pip install pandas numpy matplotlib seaborn scikit-learn folium jupyterlab


Note: The repo contains enviroment.yml (spelling matches repository). If you rename it, update the filename in the command above.

Run the notebook

Clone the repo:

git clone https://github.com/smusab9152/LA_Crime.git
cd LA_Crime


Start Jupyter:

jupyter notebook
# or
jupyter lab


Open LA_Crime_Analysis.ipynb and run the cells in order. The notebook is structured so EDA comes first, followed by feature engineering and ML experiments.

What’s in this repo

Exploratory Data Analysis (EDA): summary statistics, distribution plots, time-series of crime counts, and geospatial visualizations.

Data cleaning & preprocessing: parsing datetimes, handling missing values, geocoding/coordinate checks.

Visualizations: static charts and interactive maps to identify hotspots and patterns.

Machine learning experiments: classification/regression/clustering attempts to model crime patterns (see notebook for model details and evaluation).

Machine learning & analysis

The notebook documents the modeling workflow. Typical experiments included:

Clustering to detect spatial/temporal hotspots (e.g., KMeans / DBSCAN).

Classification / Regression attempts to predict crime category or incident counts using tree-based models (e.g., RandomForest) and standard evaluation (confusion matrix, accuracy, precision/recall, cross-validation).

Feature engineering: extracting hour/day/month features, aggregations by neighborhood, and encoding categorical variables.

Refer to LA_Crime_Analysis.ipynb for exact model types, hyperparameters, and results.

Dataset

la_crime_data.csv — CSV file containing crime incident records.

Typical columns (may vary): Date, Time, Crime Type, Description, Neighborhood, Latitude, Longitude, and additional contextual fields.

⚠️ Confirm the dataset's origin and licensing before sharing or publishing results derived from it.

Future work

Ideas to expand the project:

Interactive dashboards with Streamlit, Dash, or a Plotly-based UI.

Improved hotspot detection using spatial statistics and kernel density estimation.

Time-series forecasting of incident counts (ARIMA, Prophet, LSTM).

Integrate socio-economic/demographic data for richer analysis.

Productionize a map-based dashboard for public use.
