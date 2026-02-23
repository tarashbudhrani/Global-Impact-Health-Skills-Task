# Global Impact Health -- HIV 2013 Impact Score Replication

## Project Overview

This project reproduces the HIV 2013 Impact Score computation framework
for estimating DALYs (Disability-Adjusted Life Years) averted by
antiretroviral drugs. The original framework was implemented in Excel
(ORS template) and has been re-engineered and replicated in Python.

## Objective

-   Reverse-engineer the Excel-based ORS impact model
-   Implement the full drug-level impact computation in Python
-   Compute per-drug and overall treatment impact scores
-   Export clean, reproducible results

## Methodology

The model calculates impact using:

-   Country-level DALYs (Adults and Children)
-   Treatment Coverage
-   Regimen Usage Share
-   Drug Efficacy
-   Retention Rate Normalization

## Impact Formula

Impact = (DALYs × Coverage × Regimen Share × Efficacy) / (1 − (Coverage
× Regimen Share × Efficacy))

Final Impact = Total Impact / Treatment Length

Treatment Length = 100 / (100 − Retention Rate)

## Key Features Implemented

-   Entity mapping from Excel grid references
-   WHO Group A vs Group B logic
-   First-line and Second-line regimen attribution
-   Drug-level DALY allocation
-   Retention-based normalization

## Files Included

-   Hiv_2013_entity_map.ipynb -- Main computation notebook
-   updated_HIV2013_nb.csv -- Final computed dataset

## Skills Demonstrated

-   Health Data Analytics
-   Model Translation (Excel to Python)
-   Public Health Impact Modeling
-   Data Cleaning and Entity Mapping
-   Analytical Documentation

Author: Tarash Budhrani Program: MS Computer Science, Indiana University
