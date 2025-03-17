## ✈ Airfare Analytics: Machine Learning-Based Price Prediction

### 📌 Overview  
This project aims to predict flight ticket prices using machine learning techniques. The dataset includes airline, source, destination, stops, duration, and booking time. The workflow covers **data preprocessing, exploratory data analysis (EDA), feature engineering, model selection, hyperparameter tuning, and evaluation using key performance metrics**.

---

## 📂 Dataset  
The dataset contains various features affecting flight prices:  
- **Airline** – Name of the airline  
- **Source City & Destination City** – Departure and arrival locations  
- **Departure & Arrival Time** – Time of flight travel  
- **Stops** – Number of stops in the journey  
- **Class** – Flight class (Economy, Business)  
- **Duration** – Total travel duration  
- **Days Left** – Days left before departure when the booking was made  
- **Price** – Target variable  

---

## 🔍 Exploratory Data Analysis (EDA)  
- **Missing Values Handling** – Imputation with median for numerical variables  
- **Outlier Detection** – Identified using **box plots and IQR method**  
- **Feature Correlation Analysis** – Heatmap and correlation matrix to determine relationships  
- **Data Visualization** – Histograms, bar plots, and pair plots  

---

## 🔧 Feature Engineering  
- **One-Hot Encoding** – Applied to categorical features  
- **Label Encoding** – Used where necessary to convert categorical variables  
- **Log Transformation** – Addressing skewness in price distribution  

---

## 🏗 Model Building  
Several models were implemented and compared:  
1. **Linear Regression**  
2. **Random Forest Regressor**  
3. **Gradient Boosting Regressor**  
4. **XGBoost Regressor**  
5. **Neural Networks (ANN-based approach)**  

**Hyperparameter tuning** was performed using **GridSearchCV** to optimize model performance.

---

## 📊 Model Evaluation Metrics  
The models were evaluated using:  
- **R² Score (Coefficient of Determination)** – Measures the goodness of fit  
- **Mean Absolute Error (MAE)** – Measures absolute differences between actual and predicted values  
- **Mean Squared Error (MSE)** – Penalizes large errors  
- **Root Mean Squared Error (RMSE)** – Standard deviation of residuals  
- **Mean Absolute Percentage Error (MAPE)** – Percentage-based accuracy metric  

---

## 🚀 Results & Inferences  
- **XGBoost performed the best with the highest R² score and lowest RMSE.**  
- **Feature importance analysis** showed that "airline," "duration," and "days left" were the most influential factors in determining ticket prices.  
- **Booking earlier reduces prices significantly**, as evident from the "days left" feature.  

---

## 🛠 Tech Stack  
- **Python**  
- **Pandas, NumPy** (Data Processing)  
- **Matplotlib, Seaborn** (EDA & Visualization)  
- **Scikit-Learn, XGBoost** (Model Training & Evaluation)  

---

## 📌 Future Scope  
- Implement **deep learning models (LSTMs or Transformers)** for time-series forecasting.  
- Use **web scraping** to get real-time flight price updates.  
- Deploy the model as a **web app using Flask or Streamlit**.  

---

## 📎 How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/Flight-Price-Prediction.git
   cd Flight-Price-Prediction
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook or Python script to train the model.  

---

## 📜 License  
This project is open-source under the **MIT License**.  

---
