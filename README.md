# Data_Analysis_Project
# Government Dataset Analysis

## Introduction
This project involves analyzing a government dataset related to the Agriculture Marketing and Cooperation Department. The dataset contains commodity price information, arrivals, and market fee details recorded across various market yards. The analysis aims to discover patterns, trends, and relationships within the data.

## Dataset Description
The dataset contains the following columns:
- `DDate`: Date of data collection (with timezone).
- `AmcCode`, `AmcName`: Codes and names representing Agricultural Market Committees (AMCs).
- `YardCode`, `YardName`: Codes and names representing Market Yards within the AMCs.
- `CommCode`, `CommName`: Codes and names representing commodities (e.g., Onions, Cabbage).
- `VarityCode`, `VarityName`: Codes and names representing commodity varieties.
- `ProgArrivals`: Projected arrivals, mostly recorded as 0.0.
- `Arrivals`: Actual arrivals of commodities (in metric tons).
- `Minimum`, `Maximum`, `Model`: Price details indicating Minimum, Maximum, and Model prices of commodities.
- `Valuation`: Valuation of the commodity, often recorded as 0.0.
- `MarketFee`: Market fee associated with transactions, usually recorded as 0.0.

## Data Preprocessing
- Converted the `DDate` column to datetime format.
- Removed duplicate entries.
- Handled missing values by filling them with 0.
- Applied the Interquartile Range (IQR) method to detect and remove outliers from numerical columns.

## Data Analysis
The analysis involves:
1. **Visualizing Distribution of Arrivals:** Histogram with KDE.
2. **Analyzing Price Range Relationship:** Line plot comparing Minimum and Maximum prices.
3. **Top 10 Commodities Analysis:** Count plot of most frequently recorded commodities.
4. **Time Series Analysis:** Trends of Arrivals over time.
5. **Pair Plot Analysis:** Relationships between numerical columns (Arrivals, Minimum, Maximum, Model).
6. **Commodity Frequency Analysis:** Pie chart showing percentage distribution of commodity arrivals.
7. **Price Analysis:** Box plots comparing Minimum, Maximum, and Model prices.
8. **Monthly Trends:** Line plots for average arrivals over each month.
9. **Price Correlation Analysis:** Heatmap to examine relationships between various price columns.
10. **Scatter Plot Analysis:** Minimum vs. Maximum prices comparison.
11. **Commodity Variety Analysis:** Distribution of varieties for top commodities.
12. **Word Cloud Creation:** Displaying most frequent commodity names.
13. **Summary Statistics:** Descriptive statistics of numerical columns.

## Conclusion
The analysis provides insights into commodity price patterns, arrival trends, and their seasonal variations. The dataset reveals potential areas for predicting commodity prices and further exploration of seasonal trends.

## Requirements
- pandas
- numpy
- seaborn
- matplotlib
- wordcloud

## Usage
- Load the dataset using `pd.read_csv()`.
- Follow the preprocessing steps mentioned above.
- Apply analysis methods as described.
- Visualize results using the visualizations mentioned.
