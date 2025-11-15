
#  Electricity Theft Detection

This project detects **electricity theft** using **Isolation Forest**, an anomaly detection machine learning model.
The model analyzes electricity consumption patterns and identifies abnormal or suspicious usage.


##  What This Project Contains

* **Main Notebook**:
  `Final_Electricity_theft.ipynb`
  (This is where all preprocessing, training, and anomaly detection happens)

* **Dataset**:
  `sgcc_filled_zero.csv`

* **Model**:
  Isolation Forest (trained inside the notebook)


## 🛠 Requirements

Install these packages:

numpy
pandas
scikit-learn
matplotlib
seaborn
joblib

Or simply:

```bash
pip install -r requirements.txt
```


##  How to Run

1. Open the Jupyter Notebook:

   
   Final_Electricity_theft.ipynb
   
2. Run all cells from top to bottom.
3. The model will:

   * Clean the data
   * Scale features
   * Train Isolation Forest
   * Detect anomalies
   * Plot anomaly scores



##  Predicting New Data

Example code inside the notebook:

```python
new_data = np.array([[5.1, 6.0, 7.2, 6.3, 8.1, 9.0]])
scaled = scaler.transform(new_data)
prediction = iso.predict(scaled)[0]
score = iso.decision_function(scaled)[0]
```

## Output

* **Anomaly Score Plot**
* **Normal vs Anomalous consumers**
* **Predictions for new consumption values**



##  Author

Roopasree G
Electricity Theft Detection Project
