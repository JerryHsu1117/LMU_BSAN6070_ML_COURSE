# CA02 – Spam Email Classification (Naive Bayes)

## 1. Project Overview
This project is part of **BSAN 6070 – Machine Learning** at Loyola Marymount University.

The purpose of this assignment is to build a **spam email classification model** using the **Naive Bayes** algorithm.  
This project focuses on understanding **text data**, converting emails into numerical features, and evaluating model performance.

---

## 2. What This Program Does
This notebook performs **text preprocessing, feature engineering, and classification** on a collection of email files.

The main tasks include:
- Reading email text files from folders  
- Cleaning and preprocessing email text  
- Building a word dictionary (vocabulary)  
- Converting emails into numeric feature vectors  
- Training a Naive Bayes classifier  
- Predicting spam vs non-spam emails  
- Evaluating model accuracy  

The final result is a working spam classifier with measurable performance.

---

## 3. Libraries Used
The following Python libraries are required to run the notebook:

- os  
- numpy  
- collections (Counter)  
- scikit-learn  

These libraries are commonly available in Anaconda and Google Colab.

---

## 4. Software and Environment
- Python 3  
- Jupyter Notebook  
- Google Colab or Anaconda Navigator  

No special setup or paid software is required.

---

## 5. Dataset Information
- **Dataset type:** Text-based email files  
- **Structure:** Folder-based (not CSV)  
- **Folders:**
  - `train-mails/` – training emails  
  - `test-mails/` – testing emails  

Each file represents **one email**.

### Label Rules
There is no separate label file.  
Labels are inferred from file names:
- File name starts with `spmsg` → **Spam (1)**
- Otherwise → **Not Spam (0)**

The folder structure and file names must remain unchanged.

---

## 6. How to Run the Code

### Option 1: Google Colab
1. Upload the notebook file (`.ipynb`)  
2. Upload the `train-mails` and `test-mails` folders  
3. Run the notebook cells from top to bottom  

### Option 2: Local Computer
1. Open Jupyter Notebook  
2. Place the notebook and data folders in the same directory  
3. Run all cells in order  

---

## 7. Files in This Folder
- `CA02_NB_assignment_note_improved.ipynb` – Main notebook with code and Markdown explanations  
- `README.md` – Project documentation  

---

## 8. Notes on Model Design
- Emails are converted into numeric vectors using a **Bag-of-Words** approach  
- The dictionary is limited to the **top 3000 most frequent words**  
- **Multinomial Naive Bayes** is used because it is suitable for word count data  
- The dictionary is built using both training and testing emails to follow assignment instructions  

---

## 9. Acknowledgements
- Course materials and guidance provided by **Professor Arin Brahma**, Loyola Marymount University  
- Dataset and assignment structure provided by the instructor  

All work was completed independently for this assignment.

---

## 10. Notes for Peer Reviewers
This README is written to be **clear, concise, and easy to understand**, including for non-technical readers.  
Feedback on clarity and organization is appreciated. 
Link:https:https://github.com/JerryHsu1117/LMU_BSAN6070_ML_COURSE/tree/main/CA02%3A%20Spam%20eMail%20Detection%20using%20Naive%20Bayes%20Classification%20Algorithm
