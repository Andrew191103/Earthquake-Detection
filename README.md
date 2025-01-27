# Advanced Machine Learning Techniques for Accurate Earthquake Prediction and Preparedness

## Overview
This repository contains the implementation and analysis of advanced machine learning models for predicting earthquakes. The project leverages various supervised and unsupervised learning techniques to enhance the accuracy of earthquake forecasting and provide actionable insights for preparedness.

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Models and Techniques](#models-and-techniques)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Visualization](#visualization)
- [Installation and Usage](#installation-and-usage)
- [Contributors](#contributors)
- [License](#license)

---

## Introduction
Earthquakes are among the most devastating natural disasters, and predicting them accurately remains a significant challenge. This project explores the potential of machine learning techniques to improve earthquake forecasting by analyzing seismic data from 1965 to 2016.

## Problem Statement
Despite advancements in geosciences, traditional methods fall short in accurately predicting earthquakes. By integrating machine learning models, this project aims to:
- Identify patterns in seismic data.
- Classify earthquake types (tectonic, volcanic, anthropogenic).
- Provide actionable insights for disaster preparedness.

## Dataset
The dataset used in this project was sourced from Kaggle's National Earthquake Information Center (NEIC) data, containing 23,412 earthquake records with 21 attributes. It includes critical features such as:
- Date and Time
- Latitude and Longitude
- Depth and Magnitude
- Location Type (Oceanic/Continental)

**Dataset Link**: [Earthquake Dataset on Kaggle](https://www.kaggle.com/datasets/usgs/earthquake-database/data)

### Preprocessing
Key preprocessing steps included:
1. Data cleaning and feature selection.
2. Creation of derived attributes like `Location Type`, `Magnitude Type`, and `Earthquake Type`.
3. Encoding categorical variables.

## Models and Techniques
The project employs the following algorithms:
1. **Decision Tree**
2. **Random Forest**
3. **Support Vector Machine (SVM)**
4. **XGBoost**
5. **LightGBM**
6. **K-Means Clustering** (Unsupervised)

Each model was tuned using hyperparameter optimization to maximize accuracy and minimize error.

## Evaluation Metrics
Models were evaluated based on:
- **Accuracy**: Overall correctness of predictions.
- **Precision, Recall, and F1-Score**: For imbalanced class distributions.
- **SHAP Values**: For feature importance interpretation.

## Results
The LightGBM algorithm outperformed others with an accuracy of **92%**, demonstrating robust classification capabilities across all earthquake types.

| Algorithm        | Accuracy | Micro F1 | Macro F1 |
|------------------|----------|----------|----------|
| SVM              | 0.92     | 0.92     | 0.61     |
| XGBoost          | 0.88     | 0.88     | 0.68     |
| LightGBM         | 0.92     | 0.92     | 0.65     |
| Decision Tree    | 0.87     | 0.88     | 0.66     |
| Random Forest    | 0.90     | 0.90     | 0.68     |

## Visualization
Visualizations provide a comprehensive understanding of seismic patterns:

### Key Visualizations
1. **All Affected Areas**
   - Highlights global earthquake distribution.
   - Image placeholder: `images/location_classification.png`
2. **Location Classification (Oceanic vs Continental)**
   - Differentiates events by their tectonic context.
   - Image placeholder: `images/location_classification.png`
3. **Earthquake Occurrences Heatmap**
   - Displays density of earthquake events using hexagonal bins.
   - Image placeholder: `images/heatmap.png`
4. **Earthquake Data Distribution Maps**
   - Scatter plots for magnitude and depth distributions.
   - Image placeholder: `images/data_distribution.png`
5. **Interactive Visualization Map**
   - Folium-based interactive map for seismic data exploration.
   - GIF placeholder: `images/interactive_map.gif`
6. **Geographical Network Graph**
   - Displays connectivity of earthquake events.
   - Image placeholder: `images/network_graph.png`
7. **Distribution of Earthquake Types**
   - Pie chart illustrating the proportions of tectonic, volcanic, and anthropogenic events.
   - Image placeholder: `images/earthquake_types.png`
8. **Distribution of Earthquakes by Time of Day**
   - Pie chart showing temporal spread of seismic events.
   - Image placeholder: `images/time_distribution.png`

## Installation and Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/Andrew191103/earthquake-ml-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook for analysis:
   ```bash
   jupyter notebook EarthquakePredictionFinal.ipynb
   ```
4. Add visualization images to the `images/` folder and update the README accordingly.

## Contributors
- **Andrew Sebastian Sibuea**  
  [andrew.sibuea@binus.ac.id](mailto:andrew.sibuea@binus.ac.id)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
