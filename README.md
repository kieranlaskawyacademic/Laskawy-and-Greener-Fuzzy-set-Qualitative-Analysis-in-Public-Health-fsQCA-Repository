fsQCA Tutorial Application: Social Determinants of Health in Dundee, Aberdeen, and Glasgow

This repository contains the reproducible analytical workflow and supplementary materials for the paper:

Laskawy, K. & Greener, I (2026).
Fuzzy-set Qualitative Comparative Analysis in Public Health: An illustrative application to social determinants of health in Dundee, Aberdeen, and Glasgow.

All analysis code in this repository was developed by Professor Ian Greener. The code constitutes his intellectual property and is shared here solely to support transparency, reproducibility, and methodological learning in connection with the accompanying publication.
Use, adaptation, or redistribution of the code for purposes beyond personal research or teaching should not occur without prior permission from Professor Greener.
For questions regarding reuse or licensing, please contact Professor Ian Greener: Ian.Greener@glasgow.ac.uk, https://orcid.org/0000-0003-4918-8019.

The repository is designed as a resource for researchers interested in applying fuzzy-set Qualitative Comparative Analysis (fsQCA) to public health and health policy data. It demonstrates how routinely available deprivation and health indicators can be transformed into calibrated fuzzy sets and analysed using set-theoretic logic to identify necessary conditions and multiple sufficient configurational pathways.

Repository contents

3_cities.Rmd
End-to-end R Markdown script that performs data preparation, calibration, fsQCA, and generation of all results reported in the manuscript and Online Supplement.

expanded_data.csv
Extended dataset produced by the workflow and used for fsQCA.

What the workflow does

Running 3_cities.Rmd will:

Import SIMD indicator data at the intermediate-zone level.

Reformat indicators so that higher values consistently represent greater deprivation.

Construct domain-level deprivation scores for:

Income

Employment

Education and training

Housing

Crime

Access to services

Construct a composite health outcome index from:

Alcohol-related admissions

Drug-related admissions

Standardised mortality ratio

Low birthweight

Comparative Illness Factor

Standardise all variables using z-scores.

Explore distributions and clustering to inform calibration thresholds.

Calibrate variables into fuzzy-set membership scores.

Conduct necessary-condition analysis.

Construct truth tables.

Perform minimisation and generate intermediate fsQCA solutions.

The outputs correspond to Tables 1–4 and Figure 1 in the manuscript and supplementary material.

Software requirements

R (≥ 4.0 recommended)

RStudio (recommended)

Key R packages:

QCA

tidyverse

readr

dplyr

ggplot2

cluster

(Exact package calls are contained in 3_cities.Rmd.)

How to run

Clone or download the repository.

Open 3_cities.Rmd in RStudio.

Ensure required packages are installed.

Knit the document or run chunks sequentially.

No manual intervention is required once the script is running.

Reproducibility notes

The code was developed and tested using the authors’ native RStudio environments. Differences in R or package versions may lead to warnings or minor compatibility issues. If problems arise, please open an issue in the repository or contact the lead author.

Underlying SIMD data are publicly available from the Scottish Government. This repository provides the processing pipeline and derived analytic dataset to facilitate replication.

Intended use

This repository is intended as:

A teaching example for fsQCA in public health.

A template that can be adapted for other datasets and contexts.

A reproducibility resource accompanying the published article.

It is not intended to provide definitive causal estimates for the cities analysed.

Citation

If you use this code or adapt the workflow, please cite:

Laskawy, K. & Greener, I. Fuzzy-set Qualitative Comparative Analysis in Public Health: An illustrative application to social determinants of health in Dundee, Aberdeen, and Glasgow.
