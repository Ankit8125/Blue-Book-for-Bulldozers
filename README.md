# Bulldozer Price Prediction
This project aims to predict the auction sale price of heavy equipment (e.g., bulldozers) based on historical data. The notebook walks through the steps of loading the data, exploratory data analysis (EDA), building machine learning models, and evaluating their performance.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)

## Project Overview
The objective of this project is to predict the auction sale price of bulldozers and other heavy equipment using machine learning algorithms. The following approach is used:

1. **Problem Definition**: 
   - Given historical auction data for bulldozers and other heavy machinery, can we predict the sale price of a particular machine?
2. **Data**: 
   - Sourced from the Kaggle Bluebook for Bulldozers competition: [Kaggle Dataset](https://www.kaggle.com/competitions/bluebook-for-bulldozers/data).
3. **Evaluation**: 
   - Minimize the Root Mean Squared Log Error (RMSLE) between the predicted and actual auction prices.
   - RMSLE achieved on the validation set: **0.2467**, which ranks **32nd** out of 474 participants.

## Dataset
The dataset contains the following features:

- **YearMade**: The year the machine was manufactured.
- **MachineHoursCurrentMeter**: The number of hours the machine has been used.
- **UsageBand**: The usage range (Low, Medium, High).
- **fiModelDesc**: Full description of the machine model.
- **fiBaseModel**: Base model of the machine.
- **fiProductClassDesc**: Product class of the equipment.
- **DriveSystem**: The drive system used (e.g., 4WD).
- **Enclosure**: The type of enclosure (e.g., cab or canopy).
- **Hydraulics**: Whether the machine has hydraulics.
- **Tire_Size**: The tire size of the machine.
- **SaleDate**: The date of the auction sale.
- **SalePrice**: The auction sale price (target variable).
- And many more.

## Installation
To run this project, you will need to install the following libraries:

```bash
# Clone the repository
git clone https://github.com/yourusername/bulldozer-price-prediction.git

# Navigate to the project directory
cd bulldozer-price-prediction

# Install dependencies
pip install -r requirements.txt
```

## Dependencies:
- Pandas
- Numpy
- Matplotlib

## Exploratory Data Analysis (EDA)
The notebook explores the following aspects of the data:

- Handling missing values and outliers.
- Feature distributions and correlation analysis.
- Visualization of relationships between features like machine age, usage, and the target variable (SalePrice).

## Modeling
The following machine learning algorithms are used:
- Random Forest Regressor <br/><br/>
Hyperparameters are tuned using RandomizedSearchCV and GridSearchCV to find the optimal model configurations. The models are evaluated using the RMSLE score.

## Evaluation
Model performance is evaluated based on:
- Root Mean Squared Log Error (RMSLE).
- The final model achieved an RMSLE of 0.2467 on the validation set, which places the project at 32nd out of 474 participants in the Kaggle leaderboard.
