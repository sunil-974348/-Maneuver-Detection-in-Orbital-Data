# -Maneuver-Detection-in-Orbital-Data

## Overview

This repository contains code for detecting maneuvers in orbital data using machine learning techniques. The goal is to identify potential maneuvers, such as engine burns or orientation adjustments, using only the variation in the semi-major axis (SMA) over time.

## Project Structure

- `data/`: Contains the raw data file used for analysis.
- `notebooks/`: Jupyter notebooks for exploratory data analysis, feature engineering, and model training.
- `scripts/`: Python scripts for data preprocessing, feature extraction, model training, and evaluation.
- `requirements.txt`: Python dependencies required for the project.
- `README.md`: This file.

## Data

The data used in this project is available [here](https://drive.google.com/uc?export=download&id=1BvQRvWXdbpXpOaSahEMovATmKQuQilQa). It includes SMA and Datetime data used to identify maneuvers.

## Features

- `SMA`: Semi-major axis.
- `SMA_Change`: Absolute change in SMA.
- `SMA_Change_Rate`: Rate of change in SMA.
- `SMA_Moving_Avg`: Moving average of SMA.
- `SMA_Variance`: Rolling variance of SMA.
- `SMA_Change_Acceleration`: Acceleration of SMA change.
- `Time_Delta`: Time difference between consecutive entries.
- `SMA_Gradient`: Gradient of SMA with respect to time.
- `SMA_Rolling_Std`: Rolling standard deviation of SMA.
- `SMA_EMA`: Exponential moving average of SMA.
- `SMA_Cum_Sum`: Cumulative sum of SMA changes.
- `SMA_Rate_of_Change`: Percentage rate of change in SMA.
- `SMA_FFT_Real`: Real part of the Fourier Transform of SMA.
- `SMA_FFT_Imag`: Imaginary part of the Fourier Transform of SMA.

## Installation

Clone the repository and install the required dependencies using `pip`:

```bash
git clone https://github.com/yourusername/maneuver-detection.git
cd maneuver-detection
pip install -r requirements.txt


Usage
Data Preparation: Place the raw data file in the data/ directory.

Feature Extraction and Model Training:

Open and run the Jupyter notebooks in notebooks/ or the Python scripts in scripts/ for data preprocessing, feature extraction, and model training.
Ensure that the correct file paths are set in the scripts or notebooks.
Evaluation: The trained model is evaluated using accuracy and other metrics. Feature importance is visualized to understand the contribution of each feature.

Visualization: Visualizations of the SMA, true maneuvers, and predicted maneuvers are generated to assess the model's performance.

Requirements
Python 3.x
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn

