# Database Normalization: Assignment-4

This repository contains the resources and documentation for the database normalization assignment, focusing on the transition of a given dataset through the First Normal Form (1NF), Second Normal Form (2NF), and Third Normal Form (3NF).

## Overview

The purpose of this assignment is to demonstrate the process of normalizing a database. Starting with an unnormalized dataset, we incrementally apply normalization rules to remove redundancies, reduce anomalies, and improve data integrity.

## Contents

- `Assignment 4.pdf`: The assignment brief and requirements.
- `Database Normalization.ipynb`: A Jupyter notebook detailing the normalization process step by step.
- `patients.csv`: Initial unnormalized dataset containing patient information.
- `treatments.csv`: Initial unnormalized dataset containing treatment records.
- `patient_clean.csv`, `treatments_clean.csv`: Intermediate datasets representing various normalization stages.
- `treatments_clean_data.csv`: Final dataset in 3NF.

## Normalization Stages

- **1NF (First Normal Form)**: Ensures that the table has no repeating groups or arrays. We transform the data into a tabular format with each column containing atomic values, and each record being unique.
- **2NF (Second Normal Form)**: Builds on the first normal form, removing partial dependencies of any column on the primary key. It requires that each table has a single primary key and that all non-key columns are fully functionally dependent on the entire primary key.
- **3NF (Third Normal Form)**: Removes transitive dependencies from tables, ensuring that non-key columns are not dependent on other non-key columns.

The Jupyter notebook `Database Normalization.ipynb` contains detailed explanations and SQL queries used to transform the datasets through these normalization stages.

## Installation and Usage

To run the Jupyter notebook:

1. Ensure you have Jupyter installed; if not, install it via `pip install jupyter`.
2. Clone this repository.
3. Navigate to the repository directory in your terminal.
4. Run `jupyter notebook` and open `Database Normalization.ipynb`.
