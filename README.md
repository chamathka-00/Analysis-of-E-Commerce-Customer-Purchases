# Analysis of E-Commerce Customer Purchases

An R-based data analytics project investigating e-commerce customer transaction data to understand spending behaviour, discount usage, regional differences, and predictive patterns. Using a dataset of 2,000 online purchases, the project applies statistical methods and modelling techniques to explore trends, estimate probabilities, fit distributions, and build regression models.



## Table of Contents

- [Overview](#overview)
- [Project Components](#project-components)
  - [1. Exploratory Data Analysis](#1-exploratory-data-analysis)
  - [2. Probability Analysis](#2-probability-analysis)
  - [3. Distribution Fitting](#3-distribution-fitting)
  - [4. Predictive Modelling](#4-predictive-modelling)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [License](#license)



## Overview

This project analyses a dataset of 2,000 e-commerce customer purchases to uncover patterns in spending behaviour, discount usage, and the relationship between time spent on a website and purchase value. The analysis is fully reproducible using R Markdown and covers the full pipeline from data cleaning through to regression modelling.



## Project Components

### 1. Exploratory Data Analysis

- Summary statistics for all numerical variables
- Data cleaning and missing value checks
- Outlier detection using the interquartile range (IQR) method
- Visualisations:
  - Histogram with density overlay for purchase amounts
  - Boxplot of time spent on site by region
  - Scatterplot of purchase amount vs. time spent

**Key findings:** Purchase amounts are approximately normally distributed. Time spent on site ranges between 1–20 minutes. Outliers are concentrated at higher purchase values.



### 2. Probability Analysis

- Probability that a purchase amount exceeds $75
- Conditional probability of discount usage for high spenders (purchase > $100)
- Contingency tables:
  - Region × Discount Usage
  - Previous Purchases × Discount Usage
- Conditional probabilities broken down by region

**Key findings:** High spenders use discounts more frequently. Regional discount usage patterns show slight variation. Discount behaviour is broadly consistent across different customer experience levels.



### 3. Distribution Fitting

- Poisson distribution fitted to `number_of_previous_purchases`
- Normal distribution fitted to `purchase_amount`
- Histogram with fitted theoretical curve overlay
- Q-Q plot to validate normality assumption

**Key findings:** The Poisson distribution fits repeat-purchase behaviour well. Spending closely follows a normal distribution, with mild deviations in the tails.



### 4. Predictive Modelling

- Scatterplot with fitted linear regression line
- Pearson correlation coefficient and full model summary output
- Derived linear equation
- Prediction of purchase amount at 12 minutes of site time

**Key findings:** A weak positive relationship exists between time spent on site and purchase amount. The model has limited predictive power, suggesting other factors drive spending more strongly.



## Technologies Used

| Tool / Concept | Purpose |
|---|---|
| R & RStudio | Primary analysis environment |
| R Markdown | Reproducible reporting |
| `ggplot2` | Data visualisation |
| Base R stats | Summary statistics, probability, distribution fitting |
| `fitdistrplus` | Distribution fitting (Poisson, Normal) |
| Linear regression (`lm`) | Predictive modelling |



## Getting Started

**Prerequisites:** R (4.0+) and RStudio

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Open the `.Rmd` file in RStudio.

3. Install required packages if not already available:
   ```r
   install.packages(c("ggplot2", "fitdistrplus", "dplyr"))
   ```

4. Knit the R Markdown document to generate the full analysis report (HTML or PDF).



## License

This project is licensed under the [MIT License](LICENSE).
