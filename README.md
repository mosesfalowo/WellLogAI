# Adaptive Well Log Interpretation: A Hybrid Supervised and Sequential Modeling Framework for Extrapolation

**CIS 730/530: Artificial Intelligence**

**Moses Falowo & Charlie Bergdall**

## Project Description
This project investigates machine learning models for interpreting well log data from the Kansas Geological Survey (KGS) to predict geological properties: Lithology, Fluid Type, and Porosity. The primary focus is on evaluating and comparing the extrapolation capabilities of Random Forest, k-Nearest Neighbors, and Long Short-Term Memory (LSTM) networks.

The study includes:
- Data preprocessing and target variable derivation from raw well log measurements.
- Training and evaluation of models (ZeroR, Random Forest, k-NN, Initial LSTM) on a standard 80/20 randomized and stratified data split.
- A rigorous extrapolation analysis using a chronological data split (top 80% for training/validation, bottom 20% for testing deeper, unseen zones), for which Random Forest and a Deeper LSTM architecture were retrained and evaluated.
- Analysis of performance degradation with depth and visual assessment of geological plausibility for extrapolated predictions.

## Main Analysis Notebook
The detailed methodology, Python code, experimental results, and visualizations can be found in the Jupyter Notebook.

## Dataset
The primary dataset used is `log.csv` from the Kansas Geological Survey (KGS), located in the directory.

## How to Run
1. Ensure you have Python 3.x and the necessary libraries installed.
2. Clone this repository.
3. Place the `log.csv` file in the `data/` directory if not already present.
4. Open and run the Jupyter Notebook.
   - The notebook includes a cell for uploading the data if run in Google Colab. For local execution, ensure the file path in the data loading cell is correct or modify it to load from the `data/` directory.

## Key Technologies
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- TensorFlow/Keras
- Matplotlib, Seaborn
- Jupyter Notebook / Google Colab
