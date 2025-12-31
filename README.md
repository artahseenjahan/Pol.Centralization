# Centralization of Power and Economic Outcomes in Parliamentary Democracies

This repository contains the empirical analysis and replication code for an undergraduate thesis examining how **political centralization through party dominance** affects **investment and inequality** in parliamentary democracies using a long-run panel dataset (1960–2022).

---

## Overview

This project analyzes whether **centralization of power**, measured by the **share of parliamentary seats held by the governing party**, influences key economic outcomes. Using panel data from **31 parliamentary democracies** across Europe and Asia, the study evaluates how political power concentration affects:

- **Investment** (Gross Capital Formation)
- **Well-being** (Income inequality)

The analysis combines **political data from election commissions** with **macroeconomic indicators from the World Bank (WDI)** and applies panel econometric techniques in **Stata**.

---

## Research Motivation

Existing literature provides mixed evidence on whether political centralization improves or harms economic performance. Most studies rely on abstract governance indices.

This project contributes by:
- Introducing a **new, transparent measure of centralization** based on **party dominance**
- Applying **long-horizon panel analysis (1960–2022)**
- Examining both **investment outcomes** and **distributional consequences**

---

## Key Research Questions

- Does higher political centralization reduce investment potential?
- Does centralization increase inequality and lower societal well-being?
- How do these effects vary across countries and over time?

---

## Data

### Sources
- **World Development Indicators (World Bank)**  
- **National Election Commission websites** (parliamentary seat data)

### Coverage
- **Countries:** 31 parliamentary democracies  
- **Period:** 1960–2022  
- **Structure:** Unbalanced panel dataset

### Key Variables
- **Degree of Centralization**  
  Ratio of governing party seats to total parliamentary seats  
- **Investment Indicator**  
  Log of Gross Capital Formation  
- **Well-Being Indicator**  
  Gini Index (income inequality)

---

## Methodology

The analysis uses panel econometric techniques:

- **Fixed Effects Models** (country-level controls)
- **Hausman Test** (model selection)
- **Two-Stage Least Squares (2SLS)** to address endogeneity
- Robust standard errors throughout

The models estimate how changes in political centralization affect economic outcomes **within countries over time**.

---

## Key Findings

### Investment Outcomes
- Higher political centralization is **negatively associated with investment**
- A rise in party dominance significantly reduces gross capital formation
- Results remain robust after controlling for savings and government expenditure

### Well-Being Outcomes
- Greater centralization is associated with **higher income inequality**
- Inequality increases as power becomes more concentrated in ruling parties
- Effects persist after accounting for income distribution and poverty controls

---

## Interpretation

The findings suggest that while centralized power may allow faster decision-making, **long-term economic performance deteriorates** when political authority becomes overly concentrated. Investment declines and inequality rises as dominant parties accumulate power and resources.

---

## Repository Structure

- `Codes_cen_eco.do` — Complete Stata do-file for data cleaning and analysis
- `Cleaned_Merged_Dataset.dta` — Final panel dataset used for regressions
- `Jahan,ARTahseen_WS.Thesis.pdf` — Full undergraduate thesis (methods, theory, results)

---

## How to Run the Analysis

### Requirements
- **Stata (any recent version)**

### Steps
1. Clone or download this repository
2. Open Stata
3. Set the working directory to the project folder
4. Run:
   ```stata
   do Codes_cen_eco.do

---
