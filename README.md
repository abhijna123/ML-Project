# Arrest Data Analysis and Crime Prediction using Machine Learning

## Project Overview
This project analyzes arrest data in Pittsburgh from 2020–2023, aiming to uncover patterns in violent vs. non-violent offenses, neighborhood-level disparities, and model-based predictions. It combines exploratory analysis, classification modeling, clustering, and fairness audits to inform data-driven policy decisions.

## Data Sources
- Pittsburgh Arrest Data: https://data.wprdc.org/dataset/arrest-data
- Pittsburgh Neighborhood Boundaries: https://catalog.data.gov/dataset/neighborhoods-57111


## Project Structure
- `EDA_Visualization.ipynb`: Explores the arrest dataset using charts, maps, and summary statistics.
- `Modeling.ipynb`: Contains full data preprocessing, classification, clustering, and fairness analysis.
- `requirements.txt`: Lists Python packages required to run this project.
- `Input CSV file (arrest_data_2020_2023_1.csv) and geo-boundary file (pittsburghpaneighborhoods.geojson)

## Notebooks Overview

### 1. `EDA_Visualization.ipynb`
- Exploratory data analysis on arrest trends
- Temporal and demographic breakdown

### 2. `modeling.ipynb`
- Data preprocessing (encoding, scaling)
- Binary classification (Logistic Regression, Random Forest, XGBoost)
- Fairness auditing (by race and gender)
- Feature importance analysis
- Clustering (DBSCAN)
- Geospatial mapping of offense intensity
- Interactive choropleth maps using Folium

## How to Run This Project

1. **Clone this repository**

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

2. **(Optional) Create a virtual environment**

```bash
python -m venv venv
source venv/Scripts/activate  # On Windows: venv\Scripts\activate
```

3. **Install the required packages**

```bash
pip install -r requirements.txt
```

4. **Run the Jupyter notebooks**

```bash
jupyter notebook
```

Then open:
- `EDA_Visualization.ipynb` for exploratory data analysis
- `modeling.ipynb` for classification, clustering, and fairness evaluation

## Dataset Notes
Make sure the following files are in your working directory before running the notebooks:
- `arrest_data_2020_2023_1.csv`
- `pittsburghpaneighborhoods.geojson`

## Output
- The clustering model outputs a map saved as `choropleth_avg_danger_map.html` which visualizes average neighborhood crime severity.

## Highlights
- ROC-AUC comparisons for model performance.
- Neighborhood-based geospatial clustering and risk scoring.
- Fairness audits across demographic groups.

---
*Developed for academic purposes — CMU Heinz College ML Project*
