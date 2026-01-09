
# Restaurant Tipping Analysis (Python / pandas)

## Objective
The goal of this project was to explore restaurant tipping data to understand how tips relate to group size and day of the week, and to distinguish between total tipping behavior and per-person tipping behavior.

## Dataset
Public restaurant tipping dataset (244 observations, 7 original variables) containing:
- total bill  
- tip  
- day  
- time  
- smoker  
- sex  
- group size  

(Source: seaborn “tips” dataset)

## Workflow

### 1. Data loading and orientation
- Loaded CSV data into pandas  
- Checked shape, columns, and first rows  

### 2. Data quality checks
- Verified no missing values  
- Checked for fully blank rows  
- Confirmed numeric data types  
- Ensured no zero group sizes before division  

### 3. Exploratory analysis
- Summarized total_bill and tip  
- Compared averages by day, time, and group size  

### 4. Feature engineering
Created a new variable:

tip_per_person = tip / size

to separate group effects from individual tipping behavior.

### 5. Structured results
Built a grouped summary table by day including:
- average group size  
- average total bill  
- average total tip  
- average tip per person  

### 6. Visualization
Plotted average tip per person by day.

## Key findings

- Sundays have the highest average group size, total bill, and total tip.  
- Fridays have the highest average tip per person.

This shows that higher total tips on Sundays are mainly driven by larger groups, whereas on Fridays individuals tend to tip more generously per person.

## Tools and skills demonstrated

- Python  
- pandas  
- data validation  
- exploratory data analysis  
- groupby aggregations  
- feature engineering  
- result structuring  
- basic visualization  
- analytical interpretation  

## One-sentence summary

Analyzed restaurant tipping data in Python using pandas, built grouped summaries and a derived “tip per person” metric, and showed that while Sundays generate higher total tips due to larger groups, Fridays have the highest average tip per person.
