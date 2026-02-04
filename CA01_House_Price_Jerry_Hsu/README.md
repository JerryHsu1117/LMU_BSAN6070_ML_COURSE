# CA01 – House Price Prediction (EDA & Data Preparation)

## 1. Project Overview
This project is part of BSAN 6070 – Machine Learning assignment

The purpose of this of assignment is to perform Exploratory Data Analysis (EDA) and data cleaning on the house price training dataset in order to produce a clean, well-understood, and analytics-ready dataset

This notebook Mainly covers: 

Part 1 (Data Understanding)

Part 2 (Data Cleaning) 

Part 3 Post Processing (Collinearity ONLY)

---

## 2. What This Program Does
This notebook performs **Exploratory Data Analysis (EDA)** and **data preparation** on a housing dataset.

The main tasks include:
- Reviewing the dataset and understanding each variable  
- Identifying the target variable (`SalePrice`)  
- Exploring data distributions and relationships  
- Handling missing values  
- Detecting outliers  
- Checking correlations between numeric variables  

The final result is a dataset that is suitable for future machine learning modeling.

---

## 3. Libraries Used
The following Python libraries are required to run the notebook:

- pandas  
- numpy  
- matplotlib  
- seaborn  

These libraries are commonly available in Anaconda and Google Colab.

---

## 4. Software and Environment
- Python 3  
- Jupyter Notebook  
- Google Colab or Anaconda Navigator  

No special setup or paid software is required.

---

## 5. Dataset Overview
- **Dataset name:** House Prices – Training Dataset  
- **File name:** `house-price-train.csv`  
- **Source:** Provided by the instructor (originally based on the Kaggle House Prices dataset)
- Dataset Link: https://github.com/ArinB/MSBA-CA-Data/blob/main/CA01/house-price-train.csv
- Dataset Description Link: https://github.com/ArinB/MSBA-CA-Data/blob/main/CA01/data_description.txt

After reviewing the dataset and the data description, each row represents a single house sale and each column describes a characteristic of the house or the sale.

The main target column: "SalePrice"

It represents the house sale price and also represents y for the machine learning model.

Important feature columns: "OverallQual", "GrLivArea", "TotalBsmtSF", "GarageArea".

Because these variables describe key aspects of house quality and size, which are commonly strong drivers of house prices. Higher overall quality, larger living area, more basement space, and larger garage area generally indicate higher property value and show clear relationships with the target variable SalePrice.

Other feature columns: location-related, structural, condition, and sale-related variables that provide additional information about the property.

---

## 6. How to Run the Code

### Option 1: Google Colab
1. Upload the notebook file (`.ipynb`) to Google Colab  
2. Upload the dataset file  
3. Run the notebook cells from top to bottom  

### Option 2: Local Computer
1. Open Jupyter Notebook  
2. Place the notebook and dataset in the same folder  
3. Run all cells in order  

---

## 7. Files in This Folder
- `CA01_House_Price_Jerry_Hsu.ipynb` – Main analysis notebook  
- `README.md` – Project documentation

---

## 8. Acknowledgements
- Course materials and guidance provided by **Professor Arin Brahma**, Loyola Marymount University  
- Dataset structure inspired by the Kaggle House Prices competition  

All analysis was completed independently for this assignment.

---

## 9. Notes for Peer Reviewers
This README is written to be clear, readable, and easy to understand for both technical and non-technical readers.  
Feedback on clarity and organization is appreciated.
My GitHub link: https://github.com/JerryHsu1117/LMU_BSAN6070_ML_COURSE/tree/main/CA01_House_Price_Jerry_Hsu




