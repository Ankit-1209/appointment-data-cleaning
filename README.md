# 🩺 Medical Appointment No-Show — Data Cleaning
This repository documents the data cleaning and preprocessing of the "Medical Appointment No-Show" dataset from Kaggle. The aim was to clean the raw healthcare data to prepare it for analysis.

## 📂 Dataset Overview
This dataset contains 100k+ medical appointments from Brazil, including details such as appointment dates, patient demographics, health conditions, and whether the patient showed up.

📊 [Original Dataset on Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

## 🧹 Cleaning Summary
### ✅ Basic Cleaning Steps
1. Handled missing values 
2. Removed duplicate rows
3. Fixed inconsistent column names (lowercase, no spaces)
4. Converted date columns (`scheduledday`, `appointmentday`) to datetime format
5. Removed extra spaces from text fields 
6. Ensured correct data types 
7. Filtered out logically invalid rows (e.g., negative ages)
8. Validated and cleaned categorical fields (`gender`, `neighbourhood`, etc.)
9. Removed scientific notation for large IDs
10. Exported the cleaned dataset to `.csv` for future analysis

### ✅ Advanced Cleaning Performed
 **Step 1: Logical Consistency**  
  - Removed rows where the `scheduledday` was after the `appointmentday`.

- **Step 2: Outlier Detection & Removal**  
  - Checked and handled outliers in age and other numeric columns.

- **Step 5: Class Imbalance Analysis**  
  - Analyzed proportions of `no_show` values to detect imbalance (about 71% showed up, 29% did not).

## 📁 Files

| File Name                    | Description                                  |
|------------------------------|----------------------------------------------|
| `cleaned_medical_dataset.csv`| Final cleaned dataset                        |
| `DA_TASK1.ipynb`             | Code notebook with detailed cleaning steps   |
| `README.md`                  | Project overview and documentation           |

## 🛠️ Tools Used

- Python
- Pandas
- Google Colab

## 🙋‍♂️ About

This project was completed as a part of a data cleaning task using real-world healthcare data. Focus was on building strong fundamentals in **Pandas-based cleaning**.

## 📜 License

This work is for learning and educational purposes. The dataset is publicly available on Kaggle under its own license.
