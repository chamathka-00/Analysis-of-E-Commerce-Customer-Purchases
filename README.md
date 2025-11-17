# Analysis of E-Commerce Customer Purchases – Data Analytics Project

CM1606 – Computational Mathematics

BSc (Hons) Artificial Intelligence & Data Science

Robert Gordon University (RGU)

Coursework – Y1S2

## 📌 Project Overview

This project is an R-based data analytics investigation developed for the CM1606 Computational Mathematics module. The coursework focuses on analysing e-commerce customer transaction data to understand spending behaviour, usage of discounts, regional differences, and predictive patterns.

Using a dataset of 2000 online purchases, the project applies statistical methods and modelling techniques to explore trends, estimate probabilities, fit distributions, and build regression models—core skills required in the module.

This work fully aligns with the coursework requirements, including R Markdown analysis, probability estimation, visualisation, interpretation, and mathematical reasoning.

## 🎯 Learning Objectives

This project demonstrates the ability to:

* Perform Exploratory Data Analysis (EDA) using R

* Generate meaningful visualisations (histograms, density plots, boxplots, scatterplots)

* Apply probability theory and interpret conditional probabilities

* Construct and interpret contingency tables

* Fit Poisson and Normal distributions to real-world data

* Build and evaluate simple linear regression models

* Interpret statistical outputs and relate them to real business scenarios

* Produce reproducible analysis using R Markdown

## 🧪 Project Components
🔹 1. Exploratory Data Analysis (EDA)

* Summary statistics for all numerical variables

* Data cleaning and missing value checks

* Outlier detection using IQR

* Visualisations:

* Histogram + density overlay for purchase amounts

* Boxplot of time spent on site by region

* Scatterplot of purchase amount vs time spent

Insights:
Purchase amounts are approx. normally distributed, time spent varies between 1–20 minutes, and outliers mainly occur at higher values.

🔹 2. Probability Analysis

* Probability that purchase amount > $75

* Conditional probability of discount usage for high spenders (> $100)

* Contingency tables:

* Region × Discount Usage

* Previous Purchases × Discount Usage

* Conditional probabilities per region

Insights:
High spenders frequently use discounts; regional discount usage patterns differ slightly; behaviour is consistent across customer experience levels.

🔹 3. Distribution Fitting

* Poisson distribution fitted to number_of_previous_purchases

* Normal distribution fitted to purchase_amount

* Histogram with fitted curve

* Q-Q plot to validate normality

Insights:
Poisson fits repeat-purchase behaviour well; spending aligns closely with a normal distribution except for mild tail deviations.

🔹 4. Predictive Modelling

* Scatterplot with fitted regression line

* Correlation and model summary output

* Fitted linear equation

* Predicted purchase amount at 12 minutes of site time

Insights:
A weak positive relationship exists between time spent and purchase amount; model suggests minimal predictive power.

## ⚙️ Technologies & Concepts Used

* R & RStudio

* R Markdown reporting

* Statistical summaries and probability theory

* Data visualisation

* Poisson & Normal distribution fitting

* Linear regression modelling

* Interpretation and mathematical reasoning

* Reproducible workflow and structured analysis

## 📜 Academic Integrity

This repository contains original code written for submission to RGU. Reusing or submitting this work elsewhere without attribution may violate academic integrity guidelines.

## 📘 License

This project is licensed under the Apache License 2.0. You may view, use, and adapt the code for learning and educational purposes, provided that proper attribution is given as required by the license. 

Submitting this work, or any modified version of it, as part of an academic assessment is strictly prohibited.
