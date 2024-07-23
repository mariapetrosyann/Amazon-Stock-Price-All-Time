# Amazon Stock Price Prediction

This repository contains a machine learning project to predict Amazon's stock prices using historical data. The project leverages Long Short-Term Memory (LSTM) networks to forecast future stock prices based on historical data.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project aims to build a predictive model for Amazon's stock prices using historical data. The model uses an LSTM network, a type of Recurrent Neural Network (RNN) suitable for time series forecasting. The goal is to provide accurate predictions of future stock prices based on historical trends.

## Features

- **Data Preprocessing:** Normalization and creation of time series data suitable for LSTM input.
- **Model Building:** LSTM-based model architecture for predicting stock prices.
- **Evaluation:** Metrics including Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to evaluate model performance.
- **Visualization:** (Optional) Visualization of predicted vs. actual stock prices (if implemented).

## Setup

To get started with this project, you need to set up your environment and install the necessary dependencies.

### Prerequisites

- Python 3.x
- Google Colab or a similar environment (optional)
- Basic knowledge of machine learning and time series forecasting

### Installing Dependencies

Create a virtual environment and install the required packages:

```bash
pip install numpy pandas keras scikit-learn matplotlib
```

## Usage

Follow these steps to run the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/Amazon-Stock-Price-All-Time.git
   cd Amazon_Stock_Price_All_Time
   ```

2. **Prepare the Dataset:**

   Place your dataset file (e.g., `Amazon.csv`) in the project directory. This dataset should contain historical stock price data with at least a "Close" column.

3. **Run the Code:**

   Open the `Amazon_Stock_Price_All_Time.ipynb` notebook (if using Google Colab) 

4. **Evaluate the Model:**

   The model will be trained and evaluated. The performance metrics, including MAE and RMSE, will be printed to the console.

## Model Architecture

The LSTM model is built with the following architecture:

- **Bidirectional LSTM Layer:** 100 units, return sequences.
- **Dropout Layer:** 30% dropout rate.
- **Bidirectional LSTM Layer:** 100 units, without return sequences.
- **Dropout Layer:** 30% dropout rate.
- **Dense Layer:** 50 units.
- **Output Dense Layer:** 1 unit for the predicted stock price.

**Compile Configuration:**

- **Optimizer:** Adam with a learning rate of 0.0001.
- **Loss Function:** Mean Absolute Error (MAE).

## Results

The model's performance metrics are as follows:

- **Mean Absolute Error (MAE):** 493.90
- **Root Mean Squared Error (RMSE):** 955.60

These metrics reflect the accuracy of the model's predictions compared to actual stock prices.

## Contributing

Contributions are welcome! If you have suggestions for improvements or fixes, please open an issue or submit a pull request.
