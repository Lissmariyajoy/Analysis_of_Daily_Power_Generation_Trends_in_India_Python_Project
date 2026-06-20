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

- Project: Analysis of Daily Power Generation Trends in India
- Tools Used: Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly
- GitHub: *https://github.com/Lissmariyajoy*
- LinkedIn: *www.linkedin.com/in/lissmariya-joy*

---
⭐ If you found this project useful, feel free to star this repository.
