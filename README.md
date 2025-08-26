# Customer Churn Prediction | [LINK](https://customer-churn-prediction-aaenxktg5czumermmnbxhx.streamlit.app/)

This project provides a comprehensive solution for predicting customer churn using a neural network model. It includes data analysis, model training, and a user-friendly web application built with Streamlit for both single and batch predictions.

---

## Project Structure

- **`1.Data_Analysis.ipynb`**  
  Jupyter Notebook for exploratory data analysis (EDA), data cleaning, and preprocessing. Visualizes and prepares data for model training.

- **`2.Prediction.ipynb`**  
  Jupyter Notebook for model training and predictions. Loads the trained model and pre-trained scalers/encoders to make predictions on new data.

- **`app.py`**  
  Streamlit web application for predicting customer churn. Supports single and batch predictions.

- **`Customer_Churn.csv`**  
  Dataset used for training and testing the model.

- **`model.keras`**  
  Trained neural network model.

- **`scaler.pkl`**  
  Serialized `StandardScaler` object for scaling numerical features.

- **`encoders.pkl`**  
  Serialized dictionary containing `LabelEncoder` and `OneHotEncoder` objects for encoding categorical features.

---

## Prerequisites

Install Python and the following libraries:

- pandas  
- numpy  
- tensorflow  
- scikit-learn  
- streamlit  
- plotly  

Install dependencies with:

```
pip install pandas numpy tensorflow scikit-learn streamlit plotly
```

---

## How to Run the Project

### 1. Data Analysis and Model Training

- Use **1.Data_Analysis.ipynb** for data processing and visualization.
- Use **2.Prediction.ipynb** to train and save `model.keras`, `scaler.pkl`, and `encoders.pkl`.

### 2. Running the Web Application

- Run the Streamlit app from your terminal:

```
streamlit run app.py
```

- This will start a local web server and open the app in your browser.

---

## Features of the Web Application

- **Single Prediction:**  
  Input a customer's details through a form and get an instant churn probability prediction, visualized with a gauge chart.

- **Batch Prediction:**  
  Upload a CSV file with multiple customer records. The app processes all records, adds "Churn Probability" and "Prediction" columns, and allows you to download the updated CSV.

---

## Acknowledgements

- **Dataset:** Derived from a public source for customer churn prediction.
- **Libraries:** Built with pandas, numpy, tensorflow, scikit-learn, streamlit,
