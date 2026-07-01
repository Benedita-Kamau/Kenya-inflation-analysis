# Kenya Inflation & Commodity Price Analysis (2016–2025)

## Overview
This project analyses Kenya's Consumer Price Index (CPI), inflation trends, and national average retail prices of selected commodities from 2016 to 2025. The analysis uses official data compiled from Kenya National Bureau of Statistics (KNBS) monthly CPI reports, and applies Python data analysis and visualisation techniques to uncover key economic trends and forecast future inflation.

---

## Data Source
- **Kenya National Bureau of Statistics (KNBS)** — official monthly Consumer Price Index (CPI) reports (2016–2025)
- Data was manually compiled from KNBS PDF reports into a structured Excel dataset
- Base period for CPI: **February 2019 = 100**

---

## Dataset Description
| Column | Description |
|---|---|
| Year | Reference year (July of each year) |
| Overall Rate of Inflation | Year-on-year inflation rate (%) |
| Overall CPI | Consumer Price Index value |
| Sugar/2 kg | Average retail price of sugar (KES) |
| Wheat Flour/2 kg | Average retail price of wheat flour (KES) |
| Maize Flour - Sifted/2 kg | Average retail price of sifted maize flour (KES) |
| Fresh Packeted Milk/500 ML | Average retail price of packeted milk (KES) |
| Potatoes (Irish)/1 kg | Average retail price of Irish potatoes (KES) |
| Onions/1 kg | Average retail price of onions (KES) |
| Tomatoes/1 kg | Average retail price of tomatoes (KES) |
| Carrots/1 kg | Average retail price of carrots (KES) |
| Kale-Sukuma Wiki/1 kg | Average retail price of kale (KES) |
| Cabbages/1 kg | Average retail price of cabbages (KES) |
| LPG Gas/13 kg | Average retail price of LPG gas (KES) |
| Kerosene/1 litre | Average retail price of kerosene (KES) |
| Electricity/50 Kw/h | Average cost of 50 kWh electricity (KES) |
| Electricity/200 Kw/h | Average cost of 200 kWh electricity (KES) |
| House rents/1 room | Average single room rent (KES) |
| Petrol/1 litre | Average retail price of petrol (KES) |
| Diesel/1 litre | Average retail price of diesel (KES) |

> **Note:** Some commodity columns contain missing values (NaN) for years where data was not available in the KNBS reports. These were left as NaN to preserve data integrity rather than imputed.

---

## Tools & Libraries
- **Python 3**
- **pandas** — data loading, cleaning, and manipulation
- **matplotlib** — data visualisation
- **seaborn** — chart styling
- **scikit-learn** — linear regression forecasting model
- **numpy** — numerical computations

---

## Project Structure
```
kenya-inflation-analysis/
│
├── README.md
├── kenya_inflation_analysis.py
├── Inflation_2016-2025_.xlsx
└── charts/
    ├── chart1_overall_inflation.png
    ├── chart2_overall_cpi.png
    ├── chart3_fuel_prices.png
    ├── chart4_diesel_prices.png
    ├── chart5_petrol_prices.png
    ├── chart6_staple_foods.png
    └── chart7_inflation_forecast.png
```

---

## How to Run
1. Clone this repository:
```bash
git clone https://github.com/your-username/kenya-inflation-analysis.git
```
2. Install required libraries:
```bash
pip install pandas matplotlib seaborn scikit-learn numpy openpyxl
```
3. Run the analysis:
```bash
python kenya_inflation_analysis.py
```

---

## Key Findings

### Inflation Trends
- Kenya's inflation averaged **6.26%** between 2016 and 2025
- Inflation peaked at **8.30% in 2022**, driven primarily by rising food and fuel prices following global supply chain disruptions and the Russia-Ukraine conflict
- Inflation dropped to its lowest point of **4.30% in 2024**, reflecting stabilising fuel prices and a stronger monetary policy response from the Central Bank of Kenya (CBK)

### Fuel Prices
- Petrol prices rose by approximately **100%** over the decade, from KES 93.81 (2016) to KES 187.37 (2025)
- Diesel followed a similar trend, rising from KES 84.20 (2016) to KES 172.75 (2025)
- The sharpest fuel price increases occurred between 2021 and 2023, coinciding with the peak inflation period

### Staple Food Prices
- Sugar prices were the most volatile staple, rising sharply in 2023 before declining in 2024
- Onion and tomato prices showed significant year-to-year variability, reflecting seasonal supply patterns
- Kale (Sukuma Wiki) remained the most affordable staple throughout the period

### Inflation Forecast (2026–2028)
A Linear Regression model was applied to forecast future inflation:
| Year | Predicted Inflation |
|---|---|
| 2026 | 6.51% |
| 2027 | 6.55% |
| 2028 | 6.60% |

> **Model Limitation:** The R² score of 0.010 indicates a very weak linear relationship, meaning the model has limited predictive power. Kenya's inflation is driven by external shocks — fuel price changes, exchange rate fluctuations, drought, and global commodity trends — that a simple linear model cannot adequately capture. More robust forecasting would require time-series models such as ARIMA that account for seasonality and volatility.

---

## Author
**Benedita Kamau**
BSc Mathematics — Jomo Kenyatta University of Agriculture and Technology (JKUAT)
📧 kamaubeneditawanjira@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/benedita-kamau-81b7961a2)

---

## Data Attribution
All data sourced from official **Kenya National Bureau of Statistics (KNBS)** Consumer Price Index reports.
Website: [www.knbs.or.ke](https://www.knbs.or.ke)
