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

### 2. The Existing Pricing Strategy Was Stable but Had Reached a Ceiling

Weekly sales without discounts remained consistently around £9.5 million with only minor fluctuations throughout the analysis period. While this demonstrated a stable customer base and predictable demand, the lack of meaningful growth suggested the business had reached a pricing equilibrium where current prices maintained sales but were no longer driving additional revenue.

A notable sales spike during the week of April 8th indicated that demand could increase under certain conditions, highlighting opportunities to optimise pricing and promotional strategies further.

Business Insight: The pricing strategy successfully protected revenue stability but appeared to limit future growth potential.
<img width="767" height="390" alt="image" src="https://github.com/user-attachments/assets/b4b88b73-ca7b-4729-a2c6-7130b18442de" />

 *Line Plot showing the company’s sales without discounts*

### 3. Demand Was Relatively Price Inelastic

Price elasticity analysis produced an elasticity score of -0.288, indicating relatively inelastic demand. Customers continued purchasing despite price changes, suggesting that moderate price increases would have limited impact on sales volume.

This finding challenged the company's heavy reliance on discounting. The data suggested that many products could potentially support higher prices without significantly reducing demand.

Business Insight: The business was potentially leaving revenue on the table by discounting products that customers were willing to purchase at higher prices.

<img width="785" height="511" alt="image" src="https://github.com/user-attachments/assets/f70f10c6-59ad-4e32-a692-29cafd133b2c" />

*Demand Curve Showing Price Elasticity of Demand*

### 4. Competitors Consistently Operated at Higher Price Points

Competitor pricing analysis revealed a highly structured market rather than one driven by reactive price changes. Box plot analysis across fiscal weeks showed that competitor median prices remained largely stable over time, indicating disciplined pricing strategies and a predictable competitive landscape. Despite operating in the same market conditions, competitors consistently maintained higher price points without significant week-to-week volatility.

<img width="772" height="425" alt="image" src="https://github.com/user-attachments/assets/5730238f-031d-487c-89a8-3e7602eaf226" />

*Box Plots Showing Price Distribution of Competitors by Fiscal Week*

Further analysis of the top 10 merchants revealed distinct pricing approaches. Some merchants concentrated on narrow price ranges targeting specific customer segments, while others operated across broader pricing bands to serve multiple segments. This created a multimodal pricing distribution, with clear clusters in both mid-range (£100-150) and premium (£200-250) categories.

<img width="777" height="507" alt="image" src="https://github.com/user-attachments/assets/8ff26f53-30b8-41f8-af1c-beadbb55d140" />

*Box Plots Showing Price Distribution by Top 10 Merchants*

When competitor pricing was integrated with company sales data, several competitors were found to price products significantly above our costs, with differences reaching as high as $70 per item. Across nearly every price bracket, competitors generated higher sales values while maintaining higher prices, suggesting that customers were willing to pay more than the company's current pricing strategy assumed.

Business Insight: Competitors were not winning through aggressive discounting. They were using stable, segmented pricing strategies that successfully captured both value-conscious and premium customer groups, indicating substantial pricing headroom within the market.
<img width="770" height="502" alt="image" src="https://github.com/user-attachments/assets/8257de6c-15be-4e4e-a754-bd3e3a267124" />

*Distribution of Prices of Competitor’s Pricing Data*

### 5. Not All Customer Segments Responded to Pricing in the Same Way

Segmentation analysis uncovered significant differences in customer price sensitivity.

Medium-price segment: Elasticity of -0.191, indicating relatively inelastic demand.
High-price segment: Elasticity of 0.509, indicating significantly greater sensitivity to price changes.

These findings showed that a single pricing strategy was suboptimal. Some products could tolerate price increases, while others required more competitive pricing to maintain demand.

Business Insight: Pricing decisions should be tailored by product segment rather than applying a uniform pricing approach across the portfolio.

### 6. Dynamic Pricing Outperformed Static Pricing Models

By combining elasticity analysis, competitor intelligence and sales performance data, the project demonstrated that dynamic pricing could create a stronger balance between revenue growth and competitiveness.

The analysis suggested:

Increasing prices within inelastic segments to improve margins.
Maintaining or reducing prices within elastic segments to protect volume.
Using competitor benchmarks to identify products with pricing headroom.

Business Insight: A data-driven dynamic pricing model offered greater revenue optimisation potential than the company's existing static pricing strategy.

<img width="711" height="236" alt="image" src="https://github.com/user-attachments/assets/33b2e94b-b5ba-4db0-887b-4323a3996279" />

*Sales Summary Showing Dynamic Prices of Items*

### The Overall Story
When viewed together, the analysis revealed a business caught in a pricing contradiction:

- Demand was stable.
- Customers were relatively insensitive to price changes.
- Competitors were charging higher prices.
- Discounts increased sales but reduced profitability.

The evidence suggested that shifting from broad discounting to elasticity-driven dynamic pricing would improve both profitability and competitive positioning while maintaining customer demand.
## *The company did not have a demand problem, it had a pricing optimisation problem.*

## 7. Recommendations

### Introduce Elasticity-Based Pricing
Increase prices in low-sensitivity segments while maintaining competitive pricing in high-sensitivity categories.

### Reduce Reliance on Blanket Discounting
Move away from broad discounts that erode profitability.

### Implement Segment-Based Pricing
Create differentiated pricing strategies for:

- High-value products
- Medium-demand products
- Price-sensitive products

### Monitor Competitor Pricing Continuously
Incorporate competitor intelligence into pricing decisions to maintain market positioning.

## 8. Business Impact

The analysis demonstrated that:

- Revenue optimisation opportunities existed without significant demand loss.
- Competitor benchmarking revealed pricing headroom.
- Dynamic pricing strategies offered a more sustainable alternative to discount-driven growth.
- Price elasticity provided a practical framework for future pricing decisions.

## 9. Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook 

## Repository Structure:

## Dataset Files:
- **Competitors pricing.csv**: This file contains the pricing data of competitors, including their pricing strategies for various products over time.
- **sales summary.csv**: This file includes the sales data from our company, including sales amounts, quantities sold, and other relevant metrics.

## Analysis Notebooks:
- **EDA of Company Sales Data.ipynb**: A Jupyter Notebook dedicated to the exploratory data analysis of the company's sales data. This analysis includes identifying trends, patterns, and key insights that will inform the dynamic pricing strategy.
- **EDA of competitors pricing.ipynb**: A Jupyter Notebook that performs exploratory data analysis on the competitor pricing data, allowing us to understand their pricing strategies and identify potential competitive advantages.
- **Price Distribution - Merged Data.ipynb**: This notebook merges the company's sales data with competitor pricing data to perform a comparative analysis. The goal is to analyze price distributions and determine the impact of competitor pricing on our sales performance.

## Documentation:
- **README.md**: This document provides an overview of the project, the structure of the repository, and instructions for running the analysis.

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
