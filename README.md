# Seasonal Agriculture Performance Analysis

A data analysis project that studies agricultural performance across Kharif, Rabi, and Zaid seasons using crop, yield, profitability, irrigation, resource usage, environmental conditions, disease/pest risk, and state-level information.


# Project Overview

Agricultural performance can vary significantly depending on the season, crop, irrigation method, resource usage, environmental conditions, and geographical region.

This project performs exploratory and statistical analysis on agricultural data to identify important patterns and differences in:

- Agricultural yield
- Farm profitability
- Crop performance
- Irrigation methods
- Water usage and efficiency
- Environmental conditions
- Resource utilization
- Disease and pest risk
- State-wise agricultural performance
- Seasonal differences in yield and profit

The analysis focuses mainly on the Kharif, Rabi, and Zaid seasons.


#Objectives

The main objectives of this project are:

1. Analyze agricultural yield across different seasons and crops.
2. Compare profitability across Kharif, Rabi, and Zaid seasons.
3. Examine the performance of different irrigation methods.
4. Study relationships between environmental conditions and agricultural yield.
5. Analyze relationships between resource usage and yield.
6. Investigate disease and pest risk across seasons.
7. Compare agricultural yield across different states.
8. Determine whether seasonal differences in yield and profit are statistically significant.
9. Identify meaningful agricultural patterns from the available dataset.
10. Develop recommendations for better seasonal agricultural planning.



#Dataset

The dataset contains agricultural records with information related to:

- Season
- State
- Crop
- Agricultural yield
- Profit
- Irrigation method
- Water usage
- Fertilizer usage
- Nitrogen, phosphorus and potassium usage
- Pesticide usage
- Rainfall
- Temperature
- Humidity
- Sunlight hours
- Soil pH
- Soil moisture
- Water efficiency
- Disease and pest risk


#Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook
- Google Colab


#Analysis Performed

1. Seasonal Agricultural Performance

Agricultural performance was compared across:

- Kharif
- Rabi
- Zaid

The analysis considered yield, profit, percentage of profitable farms, water usage, water efficiency, and disease/pest risk.

2. Crop and Seasonal Yield Analysis

Median yield was compared across different crops and seasons to identify variations in crop performance.

3. Irrigation Analysis

Different irrigation methods were compared using:

- Median agricultural yield
- Median profit
- Water efficiency

4. Environmental Analysis

The relationship between environmental variables and agricultural yield was examined using correlation analysis.

The environmental variables included:

- Rainfall
- Average temperature
- Humidity
- Sunlight hours
- Soil pH
- Soil moisture

5. Resource Usage Analysis

The relationship between resource usage and agricultural yield was analyzed using:

- Water usage
- Fertilizer usage
- Nitrogen
- Phosphorus
- Potassium
- Pesticide usage

6. Water-Use Group Analysis

Water usage was divided into four groups:

- Low
- Medium-Low
- Medium-High
- High

Median agricultural yield was then compared across these groups.

7. Disease and Pest Risk Analysis

Median disease/pest risk was compared across Kharif, Rabi, and Zaid seasons.

8. State-wise Analysis

Median agricultural yield was compared across the eight states represented in the dataset.

9. Statistical Significance Testing

The Kruskal–Wallis test was used to determine whether agricultural yield and profit distributions differed significantly across the three seasons.


#Key Findings

### Seasonal Performance

| Season | Median Yield (Tonnes/Ha) | Median Profit | Profitable Farms |
| Kharif | 1.95 | ₹38,808 | 57.79% |
| Rabi | 1.66 | -₹31,870 | 48.86% |
| Zaid | 1.45 | -₹62,144 | 35.52% |

Kharif showed the strongest overall performance, while **Zaid** showed the weakest economic performance.


#Irrigation Findings

- Drip irrigation showed the highest median yield and median profit in the available dataset.
- Flood irrigation showed the lowest median yield and median profit among the analyzed irrigation methods.

These results suggest that irrigation method can be an important factor when evaluating agricultural performance.


#Resource Usage

Water usage showed the strongest observed linear relationship with agricultural yield among the selected resource variables:

Correlation = 0.389

Other resource variables showed much weaker relationships with yield.

> Correlation indicates association and does not by itself establish causation.


#Environmental Factors

The selected environmental variables showed very weak linear relationships with agricultural yield.

Rainfall had the highest observed correlation among the selected environmental variables:

Correlation = 0.028

This indicates that these environmental variables individually showed little linear association with yield in this dataset.


#Disease and Pest Risk

Median disease/pest risk varied across seasons:

- Kharif: 54.5%
- Rabi: 40.6%
- Zaid: 37.9%

Kharif showed the highest median disease/pest risk.


#State-wise Yield

Among the analyzed states:

- Telangana: 1.84 tonnes/ha
- Karnataka: 1.77 tonnes/ha
- Maharashtra: 1.77 tonnes/ha
- Punjab: 1.74 tonnes/ha
- Tamil Nadu: 1.73 tonnes/ha
- Gujarat: 1.72 tonnes/ha
- Madhya Pradesh: 1.67 tonnes/ha
- Andhra Pradesh: 1.65 tonnes/ha

Telangana had the highest median yield, while Andhra Pradesh had the lowest among the states analyzed.


#Statistical Results

The Kruskal–Wallis test indicated statistically significant differences across the three seasons.

### Agricultural Yield

- H-statistic: 68.604
- p-value: 1.2669 × 10⁻¹⁵

#Agricultural Profit

- H-statistic: 101.926
- p-value: 7.3627 × 10⁻²³

Since the p-values are below 0.05, the analysis provides statistical evidence that the distributions of agricultural yield and profit differ across Kharif, Rabi, and Zaid.

---

#Recommendations

Based on the analysis:

1. Seasonal agricultural planning should consider the differences observed between Kharif, Rabi, and Zaid.
2. The lower profitability observed in Zaid requires further investigation into crop selection, costs, resource usage, and other factors.
3. Irrigation methods should be evaluated using multiple indicators such as yield, profitability, and water efficiency.
4. Drip irrigation deserves further investigation because it showed the highest median yield and profit in the available dataset.
5. Water usage should be monitored carefully because it showed the strongest observed linear relationship with yield among the selected resource variables.
6. Crop-specific and state-specific planning may be useful because agricultural yield varies across crops and geographical regions.
7. Further analysis using more detailed weather, market, and farm-management information could help explain the observed seasonal differences.


#Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── Seasonal_Agriculture_Performance_Analysis.ipynb
├── seasonal_agriculture_performance_dataset.csv
├── requirements.txt
└── README.md
