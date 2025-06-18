# 🏡 House Size Prediction Project


This project uses a machine learning pipeline to predict missing house_size values in a real estate dataset of over 2,200,000 entries. It employs feature engineering, outlier detection, and a LightGBM regression model to fill in missing values with a mean error of approximately ±300 sq ft—about the size of a small personal office.

📂 Data Sources
Due to GitHub's 25MB file upload limit, the full CSV files are hosted externally:

🔗 [View genhousedata.csv here](https://drive.google.com/file/d/1T0XZzCm0TsEVoMyUK4v75oMk6dFIUT0o/view?usp=sharing) – Original dataset containing missing house_size entries.

🔗 [View genhousedata_filled.csv here](https://drive.google.com/file/d/1bqhySJn2t658kAxBMl0J2Up9lcmkWr1D/view?usp=sharing) – Dataset after filling in missing values using the trained model.

🧠 Highlights
Identified and excluded outliers using the IQR method.

Trained a LightGBM regression model on "normal" entries.

Filled all 568,484 missing house_size entries.

Created a size_label column to flag outliers and a house_size_predicted flag for imputed values.

Evaluated model performance using MAE, RMSE, and R² on a validation split.
