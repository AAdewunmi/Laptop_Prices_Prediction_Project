# 💻 Laptop Price Prediction

This project predicts laptop prices based on various features using supervised machine learning techniques. It covers the full data science workflow: data loading, exploratory data analysis (EDA), feature engineering, model building, hyperparameter tuning, and evaluation.

## Project Structure

```
├── Laptop_Price_Predictor.ipynb # Main Jupyter notebook with code and analysis
├── requirements.txt # Python dependencies
├── sample_data/
│
├── laptop_data.csv # Raw dataset
│ └── Trained_Model/
│
├── df.pkl # Preprocessed DataFrame (pickle)
│
├── pipe.pkl # Trained pipeline/model (pickle)
│ └── traineddata.csv # Processed training data
├── .vscode/
│ └── extensions.json # VSCode settings
├── LICENSE # MIT License
└── README.md # Project documentation
```

## Features Used

- Company
- TypeName
- Inches
- ScreenResolution
- Cpu (processed to CPU_name)
- Ram
- Memory (processed into storage types)
- Gpu (processed to Gpu brand)
- OpSys (standardized)
- Weight
- TouchScreen, IPS, PPI (engineered features)

## Workflow

1. **Data Loading:** Reads data from `sample_data/laptop_data.csv`.
2. **EDA:** Visualizes distributions, relationships, and categorical counts.
3. **Feature Engineering:** Extracts and transforms features (e.g., CPU type, storage, screen resolution).
4. **Model Building:** Trains multiple regression models (Linear, Ridge, Lasso, Decision Tree, Random Forest).
5. **Hyperparameter Tuning:** Uses `RandomizedSearchCV` for optimal model parameters.
6. **Evaluation:** Compares actual vs. predicted prices, visualizes results.
7. **Model Persistence:** Saves trained models and processed data for deployment.

## Getting Started

### Prerequisites

- Python 3.7+
- See `requirements.txt` for dependencies (e.g., pandas, numpy, scikit-learn, seaborn, matplotlib, xgboost)

### Installation

```sh
pip install -r [requirements.txt](http://_vscodecontentref_/4)
```

### Usage

- Open Laptop_Price_Predictor.ipynb in Jupyter or VSCode.
- Run cells sequentially to reproduce the analysis and model training.
- Trained models and processed data are saved in sample_data/Trained_Model/.

### Data

- The dataset is located at sample_data/laptop_data.csv.

### Results

- Multiple regression models are compared.
- The best-performing model is saved as pipe.pkl and laptoppricepredictor.pkl.
- Visualizations show feature importance and prediction accuracy.

### License

- This project is licensed under the MIT License. See LICENSE for details.

### Author
Adrian Adewunmi