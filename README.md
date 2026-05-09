# Car Price Prediction

A machine learning project that predicts car prices using regression models and exploratory data analysis techniques.

## 📋 Table of Contents
- [About](#about)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Models & Results](#models--results)
- [Contributing](#contributing)
- [License](#license)

## About

This project develops predictive models to estimate car prices based on various features such as brand, model, mileage, age, and other specifications. The analysis includes data preprocessing, feature engineering, exploratory data analysis (EDA), and model comparison using various machine learning algorithms.

## Dataset

Describe your dataset here:
- **Source**: [Kaggle]
- **Number of records**: [Number of rows :1610 , Number of columns:17]
- **Features**: [List key features - e.g., brand, model, year, mileage, engine size, etc.]
- **Target variable**: Car price

## Project Structure

```
Car-Price-Prediction/
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_preprocessing.ipynb
│   ├── 03_feature_engineering.ipynb
│   └── 04_model_training.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── models/
├── README.md
└── requirements.txt
```

## Installation

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/pravinhase6-eng/Car-Price-Prediction.git
   cd Car-Price-Prediction
   ```

2. **Create a virtual environment** (optional but recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

## Usage

1. **Explore the notebooks** in the `notebooks/` directory in order:
   - Start with `01_data_exploration.ipynb` to understand the dataset
   - Follow through `02_data_preprocessing.ipynb` for data cleaning
   - Review `03_feature_engineering.ipynb` for feature creation
   - Check `04_model_training.ipynb` for model development and results

2. **Make predictions** (if a trained model is saved):
   ```python
   import pickle
   
   # Load the model
   with open('models/best_model.pkl', 'rb') as f:
       model = pickle.load(f)
   
   # Make predictions
   predictions = model.predict(new_data)
   ```

## Models & Results

### Algorithms Tested
- Linear Regression

### Best Performing Model
- **Model**: [LinearRegression]
- **R² Score**: [0.89]
- **RMSE**: [16534.59]


## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request


## Author

**Pravin Hase**
- GitHub: [@pravinhase6-eng](https://github.com/pravinhase6-eng)
- Email: [pravinhase6@gmail.com]

---

**Note**: This project is for educational and analytical purposes. Actual car pricing depends on many external factors not captured in this model.
