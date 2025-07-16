
# ⚡ Household Energy Consumption Prediction

## 📌 Description
This project predicts hourly household energy consumption (`kWh`) using historical date-time data features such as year, month, day, and hour. A **Linear Regression model** is trained, evaluated, and visualized to understand consumption trends and provide forecasts. The project also includes preprocessing, feature engineering, outlier detection, and model performance evaluation.

> 🔁 *You can replace Linear Regression with alternative models (e.g., Decision Tree, Random Forest) for improved accuracy and robustness.*

---

## 🛠️ Technologies Used
- Python (Google Colab)
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Missingno (for missing value visualization)
- Isolation Forest (for outlier detection)

---

## 📂 Dataset
- The dataset is expected in `.xlsx` format and should contain at least a `Date` column and an `Hourly energy kWh` column.
- Sample features used for modeling:
  - `year`, `month`, `day`, `hour` (extracted from `Date`)
  - Target: `Hourly energy kWh`

---

## 🔄 Workflow
1. Upload Excel dataset through `files.upload()`
2. Clean data: remove duplicates, handle missing values
3. Extract date features (`year`, `month`, `day`, `hour`)
4. Scale features using `StandardScaler`
5. Train model using `LinearRegression`
6. Evaluate using MAE, MSE, and R²
7. Predict energy based on user-input date & time
8. Visualize actual vs. predicted energy values
9. Detect outliers using `IsolationForest`

---

## 📊 Model Evaluation Metrics
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R² Score (Coefficient of Determination)**

---

## 📈 Output Examples
- **Graph:** Actual vs. Predicted Energy Scatter Plot
- **Outlier Detection:** Printed list of outlier predictions using `IsolationForest`

---

## ▶️ How to Run
1. Upload your `.xlsx` file when prompted by `files.upload()`.
2. Ensure your file has a `Date` column in datetime format and a target column `Hourly energy kWh`.
3. Run the code in sequence to:
   - Preprocess the data
   - Train and evaluate the model
   - Enter a custom date/time to make predictions
   - Visualize results and outliers

---

## 💡 Future Improvements
- Experiment with models like **Decision Tree**, **Random Forest**, or **Gradient Boosting** for better performance.
- Implement hyperparameter tuning.
- Save the trained model using `joblib` or `pickle`.
- Create a Streamlit web app for real-time energy forecasting.

---

## 👩‍💻 Author
**Mahnoor Kokab**  
3rd Semester – BS Computer Science  
University of Management and Technology (UMT), Lahore  
Email: [Add your email here]
