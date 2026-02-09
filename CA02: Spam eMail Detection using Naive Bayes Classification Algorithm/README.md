CA02 – Spam Email Classification (Naive Bayes)
1. Project Overview

This project is part of BSAN 6070 – Machine Learning at Loyola Marymount University.

The purpose of this assignment is to build a spam email classification model using the Naive Bayes algorithm.
This project focuses on understanding text data, converting emails into numerical features, and evaluating model performance.

2. What This Program Does

This notebook performs text preprocessing, feature engineering, and classification on a collection of email files.

The main tasks include:

Reading email text files from folders

Cleaning and preprocessing email text

Building a word dictionary (vocabulary)

Converting emails into numeric feature vectors

Training a Naive Bayes classifier

Predicting spam vs non-spam emails

Evaluating model accuracy

The final result is a working spam classifier with measurable performance.

3. Libraries Used

The following Python libraries are required to run the notebook:

os

numpy

collections (Counter)

scikit-learn

These libraries are commonly available in Anaconda and Google Colab.

4. Software and Environment

Python 3

Jupyter Notebook

Google Colab or Anaconda Navigator

No special setup or paid software is required.

5. Dataset Information

Dataset type: Text-based email files

Structure: Folder-based (not CSV)

Folders:

train-mails/ – training emails

test-mails/ – testing emails

Each file represents one email.

Label Rules

There is no separate label file.
Labels are inferred from file names:

File name starts with spmsg → Spam (1)

Otherwise → Not Spam (0)

The folder structure and file names must remain unchanged.

6. How to Run the Code
Option 1: Google Colab

Upload the notebook file (.ipynb)

Upload the train-mails and test-mails folders

Run the notebook cells from top to bottom

Option 2: Local Computer

Open Jupyter Notebook

Place the notebook and data folders in the same directory

Run all cells in order

7. Files in This Folder

CA02_NB_assignment_note_improved.ipynb – Main notebook with code and Markdown explanations

README.md – Project documentation
