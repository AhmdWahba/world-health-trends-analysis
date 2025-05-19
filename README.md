# World Health Trends Analysis

This project presents an in-depth data analysis of global health indicators using a dataset that includes country-level metrics such as life expectancy, mortality rates, disease prevalence, and economic factors. The goal is to identify patterns, highlight anomalies, and understand how various socio-economic variables correlate with health outcomes.

---

## Dataset

The dataset used is `world_health_data.csv`. It includes the following key features:

- `Country`: Name of the country  
- `Year`: Year of the observation  
- `Life expectancy`: Average life expectancy  
- `Adult Mortality`: Number of adult deaths per 1000 individuals  
- `infant deaths`: Infant deaths per 1000 live births  
- `Hepatitis B`: Percentage immunized  
- `Measles`: Reported cases  
- `BMI`: Average BMI in the population  
- `GDP`: Gross Domestic Product per capita  
- `Schooling`: Average number of years of schooling  

---

## Project Objectives

- Clean and preprocess the dataset  
- Explore key health metrics and their distributions  
- Analyze relationships between economic and health factors  
- Visualize life expectancy trends by region and income level  
- Identify patterns and outliers in global health statistics  

---

## Key Findings

### 1. Top and Bottom Life Expectancy Countries (2015)

| Country                     | Life Expectancy |
|----------------------------|-----------------|
| Hong Kong                  | 84.2            |
| Japan                      | 83.6            |
| Switzerland                | 83.4            |
| Sierra Leone               | 50.1            |
| Chad                       | 52.3            |
| Central African Republic   | 52.8            |

Life expectancy varies dramatically across countries, with developed nations surpassing 80 years, while some developing nations fall below 55 years.

---

### 2. Correlation with Life Expectancy

| Feature                           | Correlation |
|----------------------------------|-------------|
| Schooling                        | +0.72       |
| Income composition of resources  | +0.73       |
| BMI                              | +0.57       |
| Adult Mortality                  | **-0.69**   |
| HIV/AIDS                         | **-0.85**   |

Positive values indicate a direct correlation with life expectancy. Economic factors (education, income) strongly contribute to improved life expectancy, while mortality and disease burden negatively impact it.

---

### 3. Regional Trends in Health Metrics

Visualizations showed that:

- **Africa** and **South-East Asia** have higher child mortality and lower immunization rates.  
- **Europe** and **Western Pacific** show consistently high life expectancy and low mortality.  
- A positive trend exists between **GDP per capita** and **life expectancy**.  

---

### 4. Health and Economic Gaps

Scatter plots and boxplots revealed the inequality between countries. Notably:

- Countries with **higher schooling years** show **lower adult mortality**.  
- **HIV/AIDS prevalence** was a major differentiator for African countries.  
- **GDP vs Life Expectancy** was not linear after $40,000+, suggesting a saturation effect.  

---

## Methodology Summary

- **Libraries used**: `pandas`, `matplotlib`, `seaborn`, `numpy`  
- **Missing values handled** using imputation with mean/mode based on feature type  
- **Correlation matrix** was used to filter relevant features  
- **Visualizations** included heatmaps, histograms, scatter plots, boxplots  

---

## License

This project is for educational and demonstration purposes. No official license is attached.
