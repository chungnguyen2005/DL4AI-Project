# DL4AI-Project
# CS313: Deep Learning for Artificial Intelligence
## Time-Series Data and Application to Stock Markets

This repository contains the end-to-end implementation of a deep learning pipeline for financial time-series analysis. The project focuses on stock price forecasting, trading signal identification, and portfolio optimization using data from both the Nasdaq and Vietnam stock markets.

---

## Project Structure
Your repository is organized as follows:

* **230158_project_notebook.ipynb**: The main Jupyter notebook containing all code for data preprocessing, model training, and evaluation.
* **230158_project_report.pdf**: A comprehensive technical report detailing the methodology and results.
* **datasets.zip**: Zipped folders containing the Nasdaq and Vietnam stock market data.
* **README.md**: This file, providing a project overview and setup instructions.

---

## Task Overview
The project is divided into four main technical tasks:

### Task 1: Nasdaq Stock Price Prediction
This task involves building a Bidirectional LSTM (BiLSTM) model to predict stock prices for 10 Nasdaq companies. It includes multi-feature extensions, k-th day forecasting, and consecutive day forecasting. Models are evaluated using a strict chronological 5-fold Time-Series Cross-Validation.

### Task 2: Vietnam Stock Price Prediction
Following the same architecture as Task 1, this section applies deep learning to 25 major HOSE-listed companies. It adapts the preprocessing pipeline to handle the specificities of the Vietnam market data.

### Task 3: Trading Signal Identification
This task transforms the forecasting problem into a binary classification challenge. It uses feature engineering to identify buy and sell signals, addressing class imbalances to improve the precision of trading actions.

### Task 4: Portfolio Optimization
The final task combines the predictive power of the DL models with Modern Portfolio Theory. It involves selecting profitable stocks, managing risk, and applying Markowitz mean-variance optimization to construct an efficient investment portfolio.

---

## Setup and Running Instructions
Follow these steps to reproduce the results in this project.

### 1. Prerequisites
Ensure you have a Python 3.10+ environment installed. It is recommended to use a virtual environment.

### 2. Data Preparation
Due to GitHub's file size restrictions, the zipped datasets are hosted on Google Drive. Please download them and place them in your project directory before running the notebook.

* **Nasdaq Dataset:** [Here](https://drive.google.com/drive/folders/1oxZOKsQtmCoLafu-HbsQpGzEqfH4S87X?usp=drive_link)
* **Vietnam Dataset:** [Here](https://drive.google.com/drive/folders/1STdVt0YOdUkoPnwVw_WX1pnfmMxRCqzX?usp=drive_link)

**Instructions:**
1. Download both `.zip` files from the links above.
2. Unzip the contents into the root directory of this repository.
3. Verify that the folder names match the paths expected in the notebook (e.g., `./nasdaq_data/` and `./vietnam_data/`).

### 3. Install Dependencies
Install the required libraries using pip:

```bash
pip install numpy pandas matplotlib tensorflow scikit-learn yfinance


