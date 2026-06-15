# Optimization of Pricing Strategies Using Price Elasticity and Competitive Analysis

This project focuses on the implementation of dynamic pricing strategies through exploratory data analysis (EDA) of both company sales data and competitor pricing data. The goal is to optimize pricing to maximize revenue while remaining competitive in the market.

## 1. Project Background

A retail company was relying on traditional pricing approaches despite operating in a competitive market with changing consumer demand and pricing pressure from competitors.

The objective of this project was to evaluate whether a more data-driven pricing strategy could improve profitability by combining:

- Internal sales performance analysis
- Price elasticity modelling
- Competitor pricing intelligence

The project used commercial datasets provided through ElectrifAi's AWS Marketplace package and focused on identifying pricing opportunities that could increase revenue while maintaining competitiveness.

## 2. Business Objectives

The project aimed to answer three key business questions:
- Is the current pricing strategy maximising revenue and profitability?
- How do competitor pricing strategies compare to the company's pricing approach?
- How can price elasticity and competitor intelligence be combined to create a more effective pricing framework?

## 3. Data Structure & Initial Checks

- **Competitors pricing.csv**: This file contains the pricing data of competitors, including their pricing strategies for various products over time.
- **sales summary.csv**: This file includes the sales data from our company, including sales amounts, quantities sold, and other relevant metrics.

### Data Quality Checks
- Assessed missing values
- Converted temporal fields for time-series analysis
- Validated pricing fields
- Verified dataset completeness before analysis

No significant missing-data issues were identified.

## 4. Executive Summary

### Business Problem
The company relied heavily on discounting to drive sales but lacked a structured understanding of:

- Customer price sensitivity
- Competitive pricing position
- Revenue optimisation opportunities

### Key Findings
- Discounts increased short-term sales but reduced profitability.
- Demand was relatively inelastic (elasticity ≈ -0.288).
- Competitors consistently operated at higher price points.
- Several products showed opportunities for premium pricing.
- Dynamic pricing outperformed static pricing approaches.

### Outcome
The analysis identified opportunities to improve profitability through elasticity-driven pricing adjustments instead of relying on broad discounting strategies.

## 5. Methodology

### Data Preparation
Cleaned and validated sales datasets
Standardised competitor pricing data
Converted fiscal periods into analysable time-series format

### Exploratory Data Analysis
Analysed:

- Weekly sales trends
- Discount performance
- Cost behaviour
- Profitability patterns

### Price Elasticity Analysis
Calculated demand elasticity to understand how sales volume responded to price changes.

### Competitor Analysis
Evaluated:

- Price distributions
- Merchant-level pricing strategies
- Market positioning
- Premium vs budget segments

### Data Integration
Merged internal sales and competitor datasets using product identifiers to compare pricing effectiveness and identify optimisation opportunities.

## 6. Key Findings & Insights

### 1. Discounts Drove Volume but Destroyed Profitability

The sales analysis revealed a clear trade-off between growth and profitability. Average sales with discounts (£11,420) were more than double sales without discounts (£4,766), demonstrating that promotions were highly effective at driving short-term demand. However, profitability analysis showed that discounted sales consistently generated lower profits and failed to create sustained growth. Sales peaked during promotional periods before declining rapidly afterwards, suggesting customers were responding to discounts rather than developing long-term purchasing behaviour.

Business Insight: The company was relying on discounts as a growth mechanism, but the strategy was eroding margins and creating temporary demand spikes rather than sustainable revenue growth.
<img width="770" height="395" alt="image" src="https://github.com/user-attachments/assets/3e43eef6-56de-446f-8f3e-e55cc7b4cd6a" />
 *Line Plot Showing Company’s Sales with Discounts*


- **EDA of Company Sales Data.ipynb**: A Jupyter Notebook dedicated to the exploratory data analysis of the company's sales data. This analysis includes identifying trends, patterns, and key insights that will inform the dynamic pricing strategy.
- **EDA of competitors pricing.ipynb**: A Jupyter Notebook that performs exploratory data analysis on the competitor pricing data, allowing us to understand their pricing strategies and identify potential competitive advantages.
- **Price Distribution - Merged Data.ipynb**: This notebook merges the company's sales data with competitor pricing data to perform a comparative analysis. The goal is to analyze price distributions and determine the impact of competitor pricing on our sales performance.
- **README.md**: This document provides an overview of the project, the structure of the repository, and instructions for running the analysis.

## Project Goals

1. **Understand Competitor Pricing Strategies**: By analyzing competitor pricing data, we aim to uncover their pricing strategies and identify any patterns or trends that might influence our pricing decisions.
2. **Implement Dynamic Pricing**: Using insights from the EDA, we develop and simulate a dynamic pricing model to optimize prices for our products. The goal is to maximize revenue without negatively impacting sales volume.
3. **Comparative Analysis**: We compare the performance of the existing pricing strategy with the dynamic pricing model, assessing the impact on total sales amount and quantity sold.

## Getting Started

To run this project, you will need to have Jupyter Notebook installed along with the necessary Python libraries such as pandas, matplotlib, and seaborn.

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python libraries: pandas, matplotlib, seaborn

### Running the Analysis

1. **Set Up Your Environment**: Ensure that your Python environment has all the required libraries installed. You can install them using pip:

   ```bash
   pip install pandas matplotlib seaborn
2. **Paste it** into a text editor (like Google Colab, Sublime Text, or any IDE you use).
