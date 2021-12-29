CSE6250-project
Team 11 Project - Predicting ICU Readmission Using NLP
Authors: Caroline Dickey, Ben Fan, Michael Mow, and Eliza Tadley

Overview
Machine Learning techniques like Natural Language Processing (NLP) can be used to draw insights from large amounts of unstructured data including medical records. The benefits of analyzing electronic health records (EHR) for patterns are numerous, but the process of extracting meaningful results requires extensive pre-processing and text transformation prior to introducing traditional machine learning models. In this project, we create a systematic approach to predicting hospital readmission using a SQL/BigQuery pipeline, feature tokenization and vectorization, and multiple classification models.

Data
The data set for this project is the MIMIC-III (Medical Information Mart for Intensive Care) data set maintained by MIT. The data contains de-identified ICU data and access to the data much be requested and a data use agreement signed before use. The data can be downloaded directly or access on the AWS of GCP cloud. For easy integration with Google Colab, this project uses the data hosted by GCP. A google account is necessary to acces the data. Access the data by:

Create an account at https://physionet.org/register/ and complete any necessary training.
Sign the data use agreement
Link your physionet account to your google account by following the instructions at https://mimic.mit.edu/docs/gettingstarted/cloud/link/
Request access to the data on Google BigQuery from https://physionet.org/content/mimiciii/1.4/
Follow the steps at https://mimic.mit.edu/docs/gettingstarted/cloud/bigquery/ to access the data via the BigQuery console
Usage
The entire project pipeline is contained within a single python notebook that is destined to be run on Google Colab. All the necessary libraries are installed within the notebook

Download model.ipynb from Github
Navigate to https://colab.research.google.com/
Upload the notebook into Colab
Select "Run All" which executes all the cells in the notebook including data analysis, data preprocessing, model building, and evaluation. The second cell in the notebook authenticates access to the MIMIC dataset. Follow the link in the output cell to complete the verification and the rest of the notebook will execute.
Note: running the entire notebook at once can take up to an hour
