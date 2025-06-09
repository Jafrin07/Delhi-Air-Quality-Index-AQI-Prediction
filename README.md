# Delhi-Air-Quality-Index-AQI-Prediction
---

## Project Overview

Air Quality Index (AQI) is a crucial measure to understand the level of air pollution and its impact on human health. This project aims to predict the AQI for Delhi using machine learning techniques based on air pollutant data, primarily focusing on PM2.5 concentrations. The AQI values are calculated using the CPCB (Central Pollution Control Board) formula.

The project demonstrates the complete pipeline from data loading, cleaning, feature engineering, modeling, evaluation, and visualization.

---

## Dataset

* **Name:** Delhi AQI Dataset (`delhi_aqi.csv`)
* **Description:** Contains air quality measurements for various pollutants including PM2.5, PM10, NO2, SO2, CO, O3, etc. The dataset is processed to calculate AQI values from PM2.5.

---

## Technologies Used

* Python 3.x
* Pandas, NumPy
* Matplotlib, Seaborn (for visualizations)
* Scikit-learn (for machine learning)
* Jupyter Notebook / Google Colab

---

## Project Structure

* `delhi_aqi_prediction.ipynb` — Jupyter Notebook containing all code for data processing, modeling, and visualization.
* `requirements.txt` — List of Python packages needed.
* `README.md` — This file.

---

## Steps in the Project

### 1. Data Loading and Preprocessing

* Load the dataset and standardize column names.
* Drop irrelevant columns such as `location`, `date`, and `station`.
* Handle missing values.

### 2. AQI Calculation

* Compute AQI from PM2.5 concentrations using CPCB’s official breakpoints and formulas.

### 3. Exploratory Data Analysis (EDA)

* Generate correlation heatmaps.
* Visualize the distribution of AQI.
* Explore relationships between PM2.5 and AQI with scatter plots.

### 4. Feature Selection and Data Splitting

* Prepare features (`X`) and target variable (`y` = AQI).
* Split data into training and testing sets.

### 5. Model Training and Evaluation

* Train and evaluate three regression models:

  * Random Forest Regressor
  * Gradient Boosting Regressor
  * Linear Regression
    
* Evaluate models using:

  * Mean Absolute Error (MAE)
  * Mean Squared Error (MSE)
  * Root Mean Squared Error (RMSE)
  * R² Score (Coefficient of Determination)

---

## Performance Summary

*Random Forest model tends to give the best balance of accuracy and interpretability.*

---

## How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/Delhi-AQI-Prediction.git
   cd Delhi-AQI-Prediction
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Upload the `delhi_aqi.csv` dataset to your working directory or Google Drive (if using Colab).

4. Open and run the notebook:

   * In Jupyter Notebook:

     ```
     jupyter notebook delhi_aqi_prediction.ipynb
     ```
   * In Google Colab:

     * Upload the notebook.
     * Mount Google Drive if dataset is stored there.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

**Thank you for checking out the Delhi AQI Prediction project!**
Your feedback and contributions are welcome.
