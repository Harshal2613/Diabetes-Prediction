# Diabetes Prediction Model

## Overview
This project implements a machine learning model to predict diabetes using patient health metrics. The model is built with Python and scikit-learn, utilizing a Support Vector Machine (SVM) classifier.

## Features
- **Data Preprocessing**: Handles missing values and standardizes features
- **Machine Learning Model**: SVM classifier with linear kernel
- **Evaluation Metrics**: Accuracy scores for training and test sets
- **Prediction Function**: Ready-to-use function for new patient data

## Dataset
The model uses the Pima Indians Diabetes Dataset containing:
- 768 patient records
- 8 health metrics (e.g., glucose levels, BMI)
- Binary outcome (diabetes/no diabetes)

## Requirements
- Python 3.6+
- Required packages:
  ```
  numpy
  pandas
  scikit-learn
  ```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Harshal2613/Diabetes-Prediction.git
   cd diabetes-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Diabetes.ipynb
   ```

2. For predictions:
   ```python
   from predict import predict_diabetes
   
   # Example patient data
   patient_data = [6, 148, 72, 35, 0, 33.6, 0.627, 50]
   result = predict_diabetes(patient_data)
   print("Diabetes Prediction:", "Positive" if result else "Negative")
   ```

## Results
| Metric        | Score  |
|---------------|--------|
| Training Accuracy | 78.66% |
| Test Accuracy | 77.27% |

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.
