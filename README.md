# Water-Quality-Prediction-AICTE


This project predicts pollution levels (O₂, NO₃, NO₂, SO₄, PO₄, CL) using historical station data. The model is trained using Random Forest with a multi-output regression approach.

**Dataset**
From 2000 to 2021

Columns include:

id (station ID), date, and pollutants like O2, NO3, etc.

Additional columns year and month were extracted from the date.

**Key Steps**

Data Cleaning

Converted date column to datetime.

Removed rows with missing pollutant values.

**Feature & Target Selection**

Features: id, year

Targets: O2, NO3, NO2, SO4, PO4, CL

**One-Hot Encoding**

Encoded id column using pd.get_dummies.

**Train-Test Split**

80% training, 20% testing using train_test_split.

**Model Training**

RandomForestRegressor wrapped in MultiOutputRegressor.

**Evaluation**

Evaluated using MSE and R² score for each pollutant.

Plotted Actual vs Predicted graphs.

**Prediction**

Predicted future pollution levels for given station id and year.

**Saving the Model**

Saved trained model (pollution_model.pkl) and column structure (model_columns.pkl) using joblib.

## Model Link

```https://drive.google.com/file/d/1wqhMvZYzvWedPVikvmFYwTh5_zogFjeh/view?usp=sharing```

**Requirements**
Python 3.x

- pandas, numpy

- matplotlib, seaborn

- scikit-learn

- joblib


