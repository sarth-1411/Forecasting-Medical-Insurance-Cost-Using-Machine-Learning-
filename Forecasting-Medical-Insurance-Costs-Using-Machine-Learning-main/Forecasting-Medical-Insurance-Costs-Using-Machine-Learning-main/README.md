# Forecasting-Medical-Insurance-Costs-Using-Machine-Learning


## Overview

This project aims to develop a machine learning model to predict individual medical insurance costs based on demographic and health-related factors such as age, BMI, smoking status, and geographical region. Using a Gradient Boosting Machine (GBM) model, this project explores how machine learning can help insurers and healthcare providers predict costs more accurately, allowing for personalized care and optimized resource allocation.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Dataset

The dataset used in this project was sourced from Kaggle. It contains data on individual medical insurance costs along with features such as:
- **age**: Age of the person.
- **sex**: Gender of the insurance contractor.
- **bmi**: Body mass index, a measure of body fat.
- **children**: Number of children/dependents covered by the insurance.
- **smoker**: Whether the person smokes.
- **region**: Residential area in the US.
- **charges**: Final medical insurance costs.

[Dataset link](https://www.kaggle.com/datasets/mirichoi0218/insurance)

## Methodology

### 1. Data Preprocessing
- **Data Cleaning**: Checked for missing values and inconsistencies. All missing values were addressed to ensure a complete dataset for analysis.
- **Encoding**: Used one-hot encoding for categorical variables (sex, smoker, region).
- **Scaling**: StandardScaler was applied to numerical features such as age, BMI, and number of children.

### 2. Model Development
- **Gradient Boosting Machine (GBM)**: The main model used for predicting medical insurance costs. GBM is effective for regression tasks, providing high accuracy.
- **Pipeline**: Preprocessing steps and model training were integrated into a pipeline to ensure consistent and efficient data handling.
- **Train-Test Split**: The data was split into training and testing sets to evaluate model performance.

### 3. Model Evaluation
- **Metrics**: The performance of the model was evaluated using the following metrics:
  - **Mean Squared Error (MSE)**
  - **Root Mean Squared Error (RMSE)**
  - **R-squared (R²)**

## Results

The model accurately predicted medical insurance costs with the following performance:
- **MSE**: {Include result}
- **RMSE**: {Include result}
- **R² Score**: {Include result}

Key factors influencing the predictions were:
1. **Age**
2. **BMI**
3. **Smoker status**
4. **Region**

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
```bash
git clone https://github.com/BalaElangovan/Forecasting-Medical-Insurance-Costs-Using-Machine-Learning
```

2. Navigate to the project directory:
```bash
cd Medical_Insurance_Cost_Prediction
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage
To run the model training and evaluation process:

```bash
python scripts/model_training.py
```
Alternatively, you can explore the analysis by running the Jupyter notebooks in the notebooks/ directory.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request for any enhancements or bug fixes.
