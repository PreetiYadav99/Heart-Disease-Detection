# Heart Disease Detection 💔

A machine learning web application for predicting heart disease risk using KNN (K-Nearest Neighbors) algorithm with Streamlit.

## Project Overview

This project uses a trained KNN model to predict the likelihood of heart disease based on various health parameters such as age, blood pressure, cholesterol levels, and other medical indicators.

## Features

- 🎯 Real-time heart disease prediction
- 📊 Interactive web interface using Streamlit
- 🔬 Pre-trained KNN model
- 📈 Data-driven predictions
- 🎨 User-friendly UI with health metrics

## Dataset

The model is trained on heart disease data with the following features:
- **Age**: Patient age
- **Sex**: Male (M) or Female (F)
- **Chest Pain Type**: ATA, NAP, TA, ASY
- **Resting Blood Pressure**: In mm Hg
- **Cholesterol**: In mg/dL
- **Fasting Blood Sugar**: > 120 mg/dL (Yes=1, No=0)
- **Resting ECG**: Normal, ST, LVH
- **Max Heart Rate**: Maximum heart rate achieved
- **Exercise-Induced Angina**: Yes (Y) or No (N)
- **Oldpeak**: ST Depression induced by exercise
- **ST Slope**: Up, Flat, Down

## Requirements

```
streamlit
pandas
joblib
scikit-learn
```

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/PreetiYadav99/Heart-Disease-Detection.git
   cd Heart-Disease-Detection
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   
   Or manually install:
   ```bash
   pip install streamlit pandas joblib scikit-learn
   ```

## Usage

1. **Run the Streamlit app:**
   ```bash
   streamlit run app.py
   ```

2. **Open your browser:**
   - Local URL: `http://localhost:8501`

3. **Input your health parameters:**
   - Fill in the sliders and dropdown menus with your health metrics
   - Click the "Predict" button

4. **Get your prediction:**
   - ⚠️ High Risk: Red warning if at risk
   - ✅ Low Risk: Green confirmation if not at risk

## Project Files

- `app.py` - Main Streamlit application
- `Heart.ipynb`, `Heart2.ipynb` - Exploratory Data Analysis notebooks
- `train.ipynb` - Model training notebook
- `KNN_heart.pkl` - Trained KNN model
- `scaler.pkl` - Data scaler for normalization
- `columns.pkl` - Feature column names
- `heart.csv` - Training data
- `train.csv`, `test.csv` - Dataset files
- `formulatedtest.csv` - Formulated test data

## Model Details

- **Algorithm**: K-Nearest Neighbors (KNN)
- **Training Data**: Heart disease dataset
- **Features**: 12 input features
- **Output**: Binary classification (0: Low Risk, 1: High Risk)

## How It Works

1. User inputs health parameters through the web interface
2. Input data is preprocessed using the trained scaler
3. Features are formatted according to the model's expected columns
4. KNN model predicts the risk level
5. Result is displayed with appropriate warning/confirmation

## Warning

⚠️ **Disclaimer**: This application is for educational and demonstration purposes only. It should NOT be used for actual medical diagnosis. Please consult with a qualified healthcare professional for medical advice.

## Author

Created by Preeti Yadav

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

## Issues

If you encounter any issues, please create an issue on the GitHub repository.

---

**Repository**: [Heart-Disease-Detection](https://github.com/PreetiYadav99/Heart-Disease-Detection)
