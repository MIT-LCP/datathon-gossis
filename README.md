# Pittsburgh GOSSIS Datathon (2024)

This repository contains resources for the Pittsburgh GOSSIS Datathon. GOSSIS is the [Global Open Source Severity of Illness Score](https://gossis.mit.edu/).

## Contents

1. Getting started
2. Documentation
3. Databases on BigQuery
4. Analysing data with Google Colab
5. An example in Python
6. An example in R

## 1. Getting started

The datasets are hosted on Google Cloud, which requires a Gmail account to manage permissions.

1. Create a [Gmail account](https://www.google.com/gmail/about/), if you don't already have one. It will be used to manage your access to the resources.
2. Give your gmail address to the session hosts via the form provided in the data access instructions.

## 2. Documentation

We will be working with two care datasets during the event:

- WIDS datathon data (GOSSIS subset): https://physionet.org/content/widsdatathon2020/
- GOSSIS-1 Dataset (eICU only): https://physionet.org/content/gossis-1-eicu

## 3. Databases on BigQuery

BigQuery is a database system that makes it easy to explore data with Structured Query Language ("SQL"). There are several datasets on BigQuery available for you to explore, including `widsdatathon2020` (the WIDS Datathon data) and `gossis_1_eicu` (the GOSSIS-1 eICU Dataset).

1. [Open BigQuery](https://console.cloud.google.com/bigquery?project=gossis-datathon).
2. At the top of the console, select `gossis-datathon` as the project. This indicates the account used for billing.
3. "Pin" a project to the resources menu to view available datasets. In the Resources menu on the left, click "Add data", "Pin a project", then add the following project names: `physionet-data`.
4. You should be able preview the data available on these projects using the graphical interface.
5. Now try running a query. For example, try counting the number of rows in the demo eICU patient table:

   ```SQL
   SELECT count(*)
   FROM `physionet-data.widsdatathon2020.training_v2` 
   ```

## 4. Analysing data with Google Colab

Python is an popular programming language for analysing data. We will explore the data using Python notebooks, which allow code and text to be combined into executable documents. First, try opening a blank document using the link below:

- [https://colab.research.google.com/](https://colab.research.google.com/)

## 5. An example in Python

Several tutorials are provided below. Requirements for these notebooks are: (1) you have a Gmail account and (2) your Gmail address has been added to the appropriate Google Group by the workshop hosts.

- Coming shortly...

## 6. An example in R

If you prefer working in R, then you can connect to Google Cloud from your code in a similar way:

- Coming shortly...

