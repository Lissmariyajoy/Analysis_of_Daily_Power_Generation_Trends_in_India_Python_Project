# ⚡ Analysis of Daily Power Generation Trends in India

## 📌 Project Overview
This project analyzes India's daily power generation data from **2017 to  2020** using Python and data analytics techniques. The study explores electricity generation patterns across different month, years, quarter, regions, states, sectors, station types, and power sources. Through data preprocessing, exploratory data analysis (EDA), and visualizations, the project identifies meaningful trends, relationships, and insights into India's electricity generation landscape.

---

## 🎯 Objectives
- Analyze power generation trends in India from 1 September 2017 to 25 October 2020.
- Study power generation patterns across years, regions, and states.
- Compare planned and actual power generation performance.
- Identify the contribution of different sectors and station types.
- Examine relationships between monitored capacity and electricity generation.
- Generate meaningful insights to support energy planning and decision-making.

---

## 📂 Dataset Information
- **Dataset Source:** Goverment of India Data Portal ((https://indiadataportal.com/p/power/r/mop-power_generation-pl-dl-abc))
- **Dataset Name:** daily-power-generation.csv
- **Study Period:** 1 September 2017 to 25 October 2020
- **Original Dataset Size:** 1,048,575 rows and 12 columns
- **Final Dataset Size:** 992,442 rows and 16 columns (after data cleaning and filtering)

### Dataset Attributes
- Id   
- Date
- Region
- State Name
- State Code
- Sector
- Station Type
- Power Station
- Power Station Unit
- Monitored Capacity
- Todays Gen Prgm (MWh)
- Todays Gen Act (MWh)
- Country
- Power Source
- Generation Status
- Year

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly

### Development Environment
- Visual Studio Code (VS Code)

---

## 🧹 Data Preparation
The following preprocessing steps were performed to ensure data quality and consistency:

- Handled missing values and duplicate records.
- Converted the Date column to datetime format.
- Converted State Code to integer format.
- Standardized categorical values in the Station Type column.
- Created new derived columns:
  - Country
  - Power Source
  - Generation Status
  - Year
- Retained Bhutan records and classified them as Imported Power.
- Filtered records with zero monitored capacity, planned generation, and actual generation values where appropriate.

---

# 🔍 Exploratory Data Analysis (EDA)

## Univariate Analysis
- Analyzed the distribution of numerical variables.
- Examined yearly total power generation trends.
- Studied region-wise and state-wise power generation.
- Evaluated sector-wise and station type contributions.
- Analyzed the distribution of actual generation using histograms and boxplots.

## Bivariate Analysis
- Compared planned and actual power generation.
- Analyzed region-wise and sector-wise power generation.
- Studied the relationship between monitored capacity and actual generation.
- Calculated the number of power stations across states.
- Examined the correlation between planned and actual generation.

## Multivariate Analysis
- Performed year-wise station type analysis.
- Conducted year-wise region-wise power generation analysis.
- Identified top and bottom performing states and power stations.
- Analyzed quarterly generation trends.
- Performed correlation analysis between monitored capacity, planned generation, and actual generation.

---

# 📊 Data Visualization

The project uses Matplotlib, Seaborn, and Plotly to create interactive and statistical visualizations that uncover trends, patterns, distributions, and relationships in India's daily power generation data.

---

## 1. Year-wise Total Power Generation (Line Chart)
**Description:** Displays the total electricity generated in each year from 2017 to 2020.

**Key Insights:**
- Total power generation increased significantly from 2017 and reached its peak during 2018 and 2019.
- Power generation declined in 2020 due to noticeable fluctuations in generation patterns.
- The values for 2017 and 2020 represent partial-year data, as the dataset covers the period from 1 September 2017 to 25 October 2020.

---

## 2. Year-wise Planned vs Actual Generation (Line Plot)
**Description:** Compares planned electricity generation with actual electricity generation across different years.

**Key Insights:**
- Actual generation closely followed planned generation throughout the study period.
- Minor deviations between planned and actual values indicate efficient generation planning and execution.

---

## 3. Month-wise Total Power Generation (Line Chart)
**Description:** Displays monthly power generation trends for each year.

**Key Insights:**
- Monthly generation patterns remained relatively stable during 2018 and 2019.
- Certain months recorded higher generation levels, indicating seasonal variations in electricity demand and production.
- The values for 2017 and 2020 represent partial-year observations.

---

## 4. Region-wise Total Generation (Bar Chart)
**Description:** Compares total electricity generation across different regions of India.

**Key Insights:**
- The Western region generated the highest amount of electricity.
- The Northern region emerged as the second-largest contributor.
- The North Eastern region and imported power from Bhutan contributed comparatively smaller shares.

---

## 5. Top 10 Power Generating States (Bar Chart)
**Description:** Displays the states with the highest total electricity generation.

**Key Insights:**
- Maharashtra emerged as the leading power-generating state.
- Uttar Pradesh, Madhya Pradesh, Chhattisgarh, and Gujarat also contributed significantly.
- Electricity generation is concentrated among a relatively small number of states.

---

## 6. Station Type Contribution (Pie Chart)
**Description:** Shows the contribution of different station types to total electricity generation.

**Key Insights:**
- Conventional Thermal stations contributed nearly 80% of total electricity generation.
- Hydro and Nuclear stations provided comparatively smaller but important contributions.
- Diesel Generator stations contributed only a negligible share.

---

## 7. Sector-wise Planned vs Actual Generation (Grouped Bar Chart)
**Description:** Compares planned and actual generation across different sectors.

**Key Insights:**
- The Central sector recorded the highest electricity generation.
- The State and Private sectors also contributed substantially.
- Actual generation remained close to planned generation across all sectors.

---

## 8. Power Source Contribution (Pie Chart)
**Description:** Shows the contribution of domestic and imported power sources.

**Key Insights:**
- Domestic power contributed approximately 99% of total electricity generation.
- Imported power accounted for only a very small proportion of total generation.

---

## 9. Correlation Heatmap
**Description:** Displays the correlation between monitored capacity, planned generation, and actual generation.

**Key Insights:**
- Planned and actual generation exhibited a strong positive correlation (0.74).
- Monitored capacity showed moderate positive relationships with both planned and actual generation.
- States with larger installed capacities generally generated more electricity.

---

## 10. Distribution of Actual Generation (Histogram)
**Description:** Shows the distribution of actual power generation values.

**Key Insights:**
- The distribution is highly right-skewed.
- Most power stations generated relatively smaller amounts of electricity.
- A few large-capacity stations generated exceptionally high amounts of electricity.

---

## 11. Box Plot (Outlier Detection)
**Description:** Identifies the presence of outliers in actual power generation.

**Key Insights:**
- Numerous high-value outliers are present in the dataset.
- A small number of large-capacity stations contribute disproportionately to total generation.
- The presence of outliers indicates significant variation in generation capacities across stations.

---

## 12. State-wise Capacity vs Generation (Scatter Plot)
**Description:** Examines the relationship between monitored capacity and actual generation across states.

**Key Insights:**
- States with higher monitored capacities generally produced more electricity.
- A positive relationship exists between installed capacity and actual generation.
- Electricity generation capacity and performance vary considerably across states.

---

## 13. Year-wise Station Type Trend (Stacked Bar Chart)
**Description:** Displays yearly power generation across different station types.

**Key Insights:**
- Conventional Thermal stations dominated electricity generation in every year.
- Hydro power remained the second-largest contributor.
- Total generation peaked during 2018 and 2019 and declined in 2020.

---

## 14. Quarterly Trend (Line Chart)
**Description:** Shows quarter-wise power generation trends for each year.

**Key Insights:**
- Power generation remained relatively stable during 2018 and 2019.
- Q2 of 2019 recorded the highest quarterly generation.
- The values for 2017 and 2020 represent partial-year data and do not reflect complete annual generation patterns.

---

## 15. Top 10 Performing Power Stations (Bar Chart)
**Description:** Displays the highest electricity-generating power stations.

**Key Insights:**
- All top-performing stations were Conventional Thermal power stations.
- These stations belonged exclusively to the Central and Private sectors.
- Electricity generation is highly concentrated among a few large-capacity thermal stations.

---

## 16. Bottom 5 States with Lowest Power Generation (Bar Chart)
**Description:** Displays the states with the lowest electricity generation.

**Key Insights:**
- Goa recorded zero actual generation despite having monitored capacity values.
- Ladakh, Andaman and Nicobar Islands, Mizoram, and Nagaland contributed only a negligible share of total generation.
- Significant disparities exist in electricity generation infrastructure across states.

---

# 💡 Key Insights

- Conventional Thermal power stations contributed nearly **80%** of India's total electricity generation.
- Domestic Power accounted for approximately **99%** of total generation.
- Maharashtra, Uttar Pradesh, Madhya Pradesh, Chhattisgarh, and Gujarat were the leading power-generating states.
- Western and Northern regions generated the highest electricity.
- All top-performing power stations were Conventional Thermal stations belonging to the Central and Private sectors.
- Actual generation closely followed planned generation with a correlation coefficient of **0.74**.
- States with higher monitored capacities generally produced more electricity.
- Power generation remained relatively stable during **2018 and 2019**, while **2020** exhibited noticeable fluctuations.
- Power generation infrastructure and output varied significantly across states and regions.
- Goa recorded zero actual generation despite having monitored capacity values, indicating possible missing data or temporarily non-operational stations.

---

# 📋 Recommendations

- Increase investment in renewable and alternative energy sources.
- Strengthen electricity generation infrastructure in low-performing states and regions.
- Improve data monitoring and reporting mechanisms.
- Continuously monitor the performance of major power stations.
- Conduct further studies on demand forecasting and capacity utilization to support future energy planning.

---

# ✅ Conclusion

The analysis reveals that domestic Conventional Thermal power stations predominantly drove India's electricity generation from 2017 to 2020. Electricity generation was concentrated among a few states and large-capacity power stations, while actual generation generally remained close to planned targets. The findings provide valuable insights into generation trends, regional disparities, and infrastructure performance and can support future energy planning and policy decisions.

---

# 👩‍💻 Author

**Lissmariya Joy**

Aspiring Data Analyst | Python | SQL | Power BI | Data Visualization

- Project: Analysis of Daily Power Generation Trends in India
- Tools Used: Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly
- GitHub: *https://github.com/Lissmariyajoy*
- LinkedIn: *www.linkedin.com/in/lissmariya-joy*

---
⭐ If you found this project useful, feel free to star this repository.
