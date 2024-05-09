# Polish Real Estate Analysis

### Project Overview

This data analysis project aims to provide insights into the price performance of a Polish real estate market over the past half year. By analyzing various aspects of the pricing data, we seek to identify trends, make data-driven recomendations, and gain a deeper understanding of the Polish real estate market performance. 

![Screenshot real estate project](https://github.com/DenysLebid/-Real-Estate-Dashboard/assets/159707774/a190ccf8-1800-4e1d-b7fa-185ff47cab61)


### Data Source
The dataset contains apartment sales and rent offers from the 15 largest cities in Poland (Warsaw, Lodz, Krakow, Wroclaw, Poznan, Gdansk, Szczecin, Bydgoszcz, Lublin, Katowice, Bialystok, Czestochowa). The data comes from local websites with apartments for sale.

### Tools

- Excel - Data Cleaning 
- PowerBI - Data Analysis / Creating reports

### Data Cleaning/Preparation

In the initial data prepararion phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formating

### Exploratory Data Analysis (EDA)

- What is the overall price trend?
- Which apartments are increasing most in price?
- What is approximate ROR over the years for apartments in different cities from rent?

  
### Data Analysis

```Excel
=IF(D2<=40, "Small", IF(AND(D2>=41, D2<=60), "Medium", "Big"))
```
```DAX
Avg Price Diff = (Sheet1[Avg Price m2] - Aparments_23_08[AVG price m2 HYA]) / Sheet1[Avg Price m2]
```
```DAX
Aprx Rent ROR Years = ROUND(Sheet1[Avg price 2] / rent_data_24_4[Avg Rent Price] / 12,0)
```

### Results/Findings

The analysis results are sumarized as follows:
1. The prices of apartments increased by almost 15% over the past half year.
2. The most increased in price the Small apartments that are in a range of 25 to 40 square meters
3. The approximate ROR for Small apartments (25m2 >< 40m2) is 15 years, Medium apartments (40m2 >< 60m2) is 20 years and for big apartments (60m2 >< 80m2) is 26 years

### Recommendations

Based on the analysis, we recommend the following
- Invest in Small apartments that are in a range of 25m2 to 40m2
- Focus more on Smaller cities the prices of apartment are more attractive in other hand the rent difference is not so high.

### Limitations
I had to remove all Apartments from data source that have more than 80m2 and are in a buildings that was build more than 24 years ago. 

