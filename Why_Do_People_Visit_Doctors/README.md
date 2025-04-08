# 🩺 Why Do People Visit Doctors?

## Overview

This project explores the factors that influence the number of outpatient doctor visits using the `DoctorContacts` dataset from the *Ecdat* R package. The goal is to understand how **demographic**, **health**, and **socioeconomic** characteristics impact healthcare utilization.

The dataset includes over **20,000 individual records** from a 1977–1978 cross-sectional study, originally used in Deb & Trivedi's research on the structure of medical care demand.

---

## 📌 Objectives

- Identify key factors driving outpatient doctor visits
- Analyze how variables like income, age, and health status affect visit frequency
- Create clear, insightful visualizations to support findings
- Demonstrate data wrangling, EDA, and visualization skills in R

---

## 🛠️ Tools & Techniques

- **Language**: R
- **Dataset**: `DoctorContacts` from the [`Ecdat`](https://cran.r-project.org/web/packages/Ecdat/index.html) package
- **Key Packages**: `ggplot2`, `dplyr`, `ggmosaic`
- **Visualization Types**:
  - Histogram (distribution of visits)
  - Faceted hex plots (age & sex)
  - Boxplots (self-rated health)
  - Scatter plots with LOESS smoothing (chronic diseases & physical limitations)
  - Mosaic plots (income vs. visit frequency)

---

## 🔍 Key Findings

- Individuals in **poorer health**, with **chronic diseases**, or **physical limitations** are significantly more likely to visit doctors frequently.
- **Income level** affects the likelihood of visiting a doctor at all—low-income individuals are less likely to seek outpatient care.
- **Age** and **sex** show minor influence on visit frequency, with only slight trends observed.

---

## 📈 Data Summary

- **Observations**: 20,186
- **Target Variable**: `mdu` – number of outpatient doctor visits
- **Selected Features**:
  - `age`, `sex`
  - `linc` (log of family income)
  - `health` (self-rated: excellent, good, fair, poor)
  - `ndisease` (number of chronic conditions)
  - `physlim` (physical limitations)

---

## 📚 References

- Deb, P. & Trivedi, P. K. (2002). *The Structure of Demand for Medical Care: Latent Class versus Two-Part Models*. Journal of Health Economics, 21(4), 601–625.
- Croissant, Y. (2023). *Ecdat: Data Sets for Econometrics*. [CRAN R Package](https://cran.r-project.org/web/packages/Ecdat/index.html)
