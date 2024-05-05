# **Parkinson's Disease Progression Prediction**

**Description:**

This repository contains the solution for a code competition aimed at predicting the progression of Parkinson's disease (PD) using protein abundance data. The competition's goal is to develop models that predict the Movement Disorder Society-Sponsored Revision of the Unified Parkinson's Disease Rating Scale (MDS-UPDRS) scores, which measure the progression of PD in patients.

**Goal of the Competition:**

The objective of this competition is to develop models trained on data of protein and peptide levels over time in subjects with Parkinson’s disease versus normal age-matched control subjects. The models should predict MDS-UPDRS scores for patients at various time intervals, aiding in the search for potential biomarkers or therapeutic targets for PD.

**Dataset Description:**

The dataset consists of several CSV files:

train_peptides.csv: Contains mass spectrometry data at the peptide level, including visit ID, visit month, patient ID, UniProt ID, peptide sequence, and peptide abundance.
train_proteins.csv: Provides aggregated protein expression frequencies derived from the peptide level data, with information on visit ID, visit month, patient ID, UniProt ID, and normalized protein expression (NPX).
train_clinical_data.csv: Includes clinical data such as visit ID, visit month, patient ID, UPDRS scores (parts 1-4), and information on the patient's clinical state regarding medication.
supplemental_clinical_data.csv: Contains additional clinical records without associated CSF samples, offering context about the typical progression of Parkinson's.

**Code:**

The code provided in this repository offers a solution to the competition task. It utilizes Python and various data science libraries to develop predictive models for Parkinson's disease progression. The code follows the competition's requirements, including the use of Kaggle's time-series API for making predictions.

**Evaluation:**

Submissions to the competition are evaluated based on Symmetric Mean Absolute Percentage Error (SMAPE) between forecasts and actual values. Predictions for patient visits 6, 12, and 24 months later are required, with ignored predictions for visits that didn't ultimately take place.

**How to Use:**

To run the code, follow these steps:

Clone this repository to your local machine.
Install the required dependencies listed in the requirements.txt file.
Execute the code in a suitable Python environment.
Ensure that the competition's API is integrated for making predictions and submissions.

**License:**

This project is licensed under the MIT License.

**Acknowledgments:**

Special thanks to the Accelerating Medicines Partnership® Parkinson’s Disease (AMP®PD) and the competition organizers for providing the dataset and hosting the competition.

For further details and to participate in the competition, visit the competition page.
