# END-TO-END-ML-House-prediction

A complete machine learning pipeline for predicting house prices using various features and algorithms.

## Project Overview

This project implements an end-to-end machine learning solution for predicting house prices. It includes data extraction, preprocessing, feature engineering, model training, evaluation, and deployment capabilities.

## Table of Contents

- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Model Pipeline](#model-pipeline)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

```
├── analysis/          # Exploratory data analysis notebooks and reports
├── explanations/      # Model explanation documents and visualizations
├── extracted_data/    # Raw and processed datasets
├── mlruns/            # MLflow experiment tracking artifacts
├── pipelines/         # Modular pipeline components
├── README.md          # Project documentation
└── config.yaml        # Configuration parameters
```

## Installation

### Prerequisites

- Python 3.8+
- pip or conda

### Setup

Clone the repository:

```bash
git clone https://github.com/lakshyaog/END-TO-END-ML-House-prediction.git
cd END-TO-END-ML-House-prediction
```

Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Configuration

Modify the `config.yaml` file to adjust parameters for data processing, feature engineering, and model training.

### Running the Pipeline

To execute the complete pipeline:

```bash
python -m pipelines.main
```

For individual pipeline steps:

```bash
python -m pipelines.data_processing
python -m pipelines.feature_engineering
python -m pipelines.model_training
python -m pipelines.model_evaluation
```

### Tracking Experiments

This project uses MLflow for experiment tracking. View the experiment dashboard:

```bash
mlflow ui
```

Then navigate to http://localhost:5000 in your browser.

## Data

The dataset contains various features of houses including:
- Location attributes
- Size measurements
- Number of rooms and bathrooms
- Age of property
- Neighborhood characteristics
- Historical sale prices

Data preprocessing steps include:
- Handling missing values
- Outlier detection and treatment
- Feature normalization
- Categorical encoding

## Model Pipeline

The prediction system implements several machine learning algorithms:
- Linear Regression
- Random Forest
- Gradient Boosting
- XGBoost
- Neural Networks

Features are selected using:
- Correlation analysis
- Feature importance ranking
- Dimensionality reduction techniques

## Results

Model performance is evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Cross-validation results

Visualizations in the `analysis` directory demonstrate:
- Feature importance
- Prediction vs. actual plots
- Residual analysis
- Learning curves

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
