# 🏥 Hospital Readmission Reduction Analysis

## 📝 Description
This project aims to explore and analyze hospital readmission data under the **Hospital Readmissions Reduction Program (HRRP)**. The dataset includes information on readmissions, discharges, and readmission rate predictions across hospitals and states for various conditions. By combining statistical analysis and rich visualizations, the project identifies trends, outliers, and patterns that contribute to hospital readmission rates.

## 📂 Dataset

* **Source**: [Hospital Readmissions Reduction Dataset](https://github.com/Sanchitsingh05/Hospital_Readdmision_Reduction/blob/main/Hospital_Readmissions_Reduction_Program%20(3).csv)
* Columns include:

  * `Hospital Name`
  * `State`
  * `Measure Name` (e.g., Heart Failure, Pneumonia)
  * `Number of Readmissions`
  * `Number of Discharges`
  * `Predicted Readmission Rate`
  * `Expected Readmission Rate`

## 🎯 Objectives
* Clean and preprocess hospital data
* Identify top hospitals and states by readmission metrics
* Compare actual, predicted, and expected readmission rates
* Perform visual and statistical analysis
* Highlight insights that could reduce readmission rates

## 🧰 Tech Stack
* **Python**
* **Pandas, NumPy** – for data manipulation
* **Matplotlib, Seaborn** – for data visualization
* **SciPy** – for statistical testing
* **Scikit-learn** – for evaluation metrics

## ⚙️ Project Workflow
### 1. Data Preprocessing

* Handled missing values by replacing `"Not Available"` and `"Too Few to Report"` with 0
* Converted necessary columns to numeric types for analysis

### 2. Exploratory Data Analysis (EDA)

* Counted and visualized average readmissions per hospital
* Identified top hospitals and states with the highest readmission rates
* Explored how diseases affect readmission trends using `Measure Name`

### 3. Visualizations

* **Bar plots**: Top 10 hospitals and conditions by average readmissions
* **Pie charts**: Disease-wise distribution of readmissions and discharges
* **Scatter plots**: Relation between actual, predicted, and expected readmissions
* **Box plots**: Identified outliers in numerical columns
* **Heatmap**: Correlation among all numerical variables

### 4. Statistical Analysis

* **Mean Absolute Error (MAE)** used to measure prediction accuracy
* **T-test** performed to compare actual vs predicted readmission rates

  * Result: p-value < 0.05 → significant difference found

## 📊 Key Insights
* Some hospitals have significantly higher average readmission rates.
* Conditions like **Heart Failure** and **Pneumonia** contribute heavily to readmissions.
* Certain states show consistently higher readmission averages.
* Actual and predicted readmission rates differ statistically, as shown by t-test results.
* Visualizations reveal potential anomalies and outliers in the dataset.

## 📈 Results
| Metric                    | Result                                          |
| ------------------------- | ----------------------------------------------- |
| Mean Absolute Error (MAE) | Low to moderate                                 |
| p-value (T-test)          | < 0.05                                          |
| Conclusion                | Prediction errors are statistically significant |


## 💡 Future Improvements
* Build ML models (e.g., regression, ensemble methods) to better predict readmission rates
* Integrate patient-level or time-series data
* Create dashboards or web apps to monitor hospital performance
* Use clustering to group hospitals with similar readmission behaviors

## 👨‍💻 Owner
This project is created and maintained by **Sanchit Singh** as part of a real-world healthcare analytics initiative.

## 🚀 Final Note

This analysis provides critical insights into how hospital readmissions vary across the U.S. By identifying key patterns and comparing actual, predicted, and expected values, the project lays a strong foundation for policy improvements and better hospital management strategies. The combination of analytics, statistics, and visual storytelling helps drive data-driven decisions in the healthcare sector.
