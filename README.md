# 🌱 CarbonCurve - Carbon Footprint Predictor using Machine Learning

**CarbonCurve** is a machine learning-powered web application built with **Streamlit** and **Polynomial Regression** to estimate an individual's carbon footprint based on their lifestyle choices.  
It not only predicts the footprint but also provides **personalized recommendations** to help reduce it.  

---

## 📌 Features

- **ML Model**: Polynomial Regression (outperformed Ridge, Lasso, Linear, and Random Forest)
- **Accurate Predictions**: Uses preprocessed dataset from Kaggle's *Individual Carbon Footprint Calculation*.
- **User-Friendly UI**: Nature-based, calm, and responsive design built in Streamlit.
- **Interactive Visuals**: Plotly charts & metrics for better insights.
- **Personalized Recommendations**: Lifestyle tips to reduce carbon footprint.
- **Profile & Data Saving**: Users can create profiles and save their past results.
- **Vehicle Type Handling**: Works even for users with walking/cycling habits (NaN handling in vehicle type).
  
---

## 📂 Project Structure
CarbonFootprint/

│

├── app/

     ├──app.py # Main Streamlit app

├── models/

     ├── model_train.py # Model training script
     
     ├── PolynomialRegression.joblib
     
     ├── LinearRegression.joblib
     
     ├── RidgeRegression.joblib
     
     ├── LassoRegression.joblib
     
     ├── RandomForestRegressor.joblib

├── preprocessing.py # Data preprocessing script

├── data/ # Dataset files
    ├── 

├── requirements.txt # Python dependencies

└── README.md # Project documentation


---

## 🛠️ Tech Stack

- **Programming Language**: Python
- **Libraries**:
  - `streamlit` - Web app framework
  - `scikit-learn` - Machine learning model training
  - `plotly` - Interactive data visualizations
  - `pandas`, `numpy` - Data processing
  - `joblib` - Model persistence
- **Dataset**: [Individual Carbon Footprint Calculation - Kaggle](https://www.kaggle.com/datasets/)

---

## 📊 Workflow

1. **Data Preprocessing**  
   - Label encoding, one-hot encoding, and multilabel binarization for categorical features.
   - Scaling numerical features.
   - Handling NaN values for users who walk or cycle.

2. **Model Training**  
   - Tested multiple regression models: Linear, Ridge, Lasso, Random Forest, and Polynomial Regression.
   - Polynomial Regression gave the **best performance**.

3. **Deployment**  
   - Built an interactive Streamlit app for user input & predictions.
   - Visualized results using Plotly.
   - Deployed to Streamlit Cloud.

---

## 🚀 How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Gurpreet0022/carboncurve.git
   cd carboncurve
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
4. **Run the app**
   ```bash
   streamlit run app.py

##🌍 How It Works

The user fills in lifestyle details (transport, energy usage, diet, etc.).

The app preprocesses these inputs using the same transformations applied during training.

The trained Polynomial Regression model predicts the carbon footprint.

The app displays:

Predicted Carbon Footprint (tons/year)

Impact Visualization

Personalized Recommendations

## 📸 Screenshots

<img width="1366" height="768" alt="Screenshot (467)" src="https://github.com/user-attachments/assets/ee429b84-3b48-4cad-be92-2ea7980a31be" />

<img width="1366" height="768" alt="Screenshot (468)" src="https://github.com/user-attachments/assets/c51e720d-c4cb-45aa-b865-67f78c72d030" />

<img width="1366" height="768" alt="Screenshot (469)" src="https://github.com/user-attachments/assets/27723b99-b36c-4171-b3aa-e1eafd09db3c" />

<img width="1366" height="768" alt="Screenshot (470)" src="https://github.com/user-attachments/assets/6ab3c59c-0f0b-4e3b-820a-f6a2f3ac7b1e" />

<img width="1366" height="768" alt="Screenshot (471)" src="https://github.com/user-attachments/assets/ec69771d-ac53-491a-aba3-a79b9608640e" />
