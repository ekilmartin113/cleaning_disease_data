# MDSS Disease Surveillance Processing

This repository contains an R-based data-processing pipeline designed to clean, standardize, and combine disease export files from the Michigan Disease Surveillance System (MDSS). The script automates the ingestion of multiple MDSS “Disease Export” files, extracts key case data, applies consistent demographic transformations, and outputs a dataset for downstream reporting and upload into data dashboards (e.g., Power BI).

Features

Bulk ingestion of MDSS exports Automatically loads all “Disease Export – ” CSV files in a folder and merges them into a single standardized dataset.

Automatic disease detection Extracts the disease name directly from each filename

Date cleaning & validation Handles irregular MDSS date formats and converts them into proper Date class fields.

Age & age-range calculation Computes case age at referral and assigns categorical age ranges (e.g., <1, 1–9, 10–19, …, >80).

Key field standardization Keeps only essential fields for analysis

Referral year/month extraction Adds Referral_Year and Referral_Month variables for trend analysis.

Output ready for dashboards Generates a clean dataset ideal for Power BI dashboards (monthly case trends, demographic breakdowns, suppression logic, etc.).
