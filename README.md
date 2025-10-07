## Seattle vs Vancouver Rainfall Analysis
## Project Overview

This project analyzes historical precipitation data to determine how rainfall in Seattle compares with Vancouver.
Using NOAA’s Climate Data Online and provided datasets, we perform exploratory data analysis and visualizations.

- Objective: Compare rainfall across Seattle and Vancouver from 2018–2022.

- Domain: Climate / Environmental Data Science

- Key Techniques: Time Series Analysis, Data Cleaning, Data Visualization, Exploratory Data Analysis (EDA)
---

## Project Structure

```
├── data/                     # Raw data files
│   ├── seattle_rain.csv
│   └── vancouver_rain.csv
├── code/                     # Jupyter notebooks and ts
│   └── Seattle_weather_project.ipynb
├── reports/     
|   └── Communicate_the_Results_Weather.pdf # Generated visualizations 
├── requirements.txt          # Project dependencies
└── README.md                 # Project documentation

```

---

## Data

- **Seattle rainfall data**: [seattle_rain.csv](https://github.com/brian-fischer/DATA-5100/blob/main/weather/seattle_rain.csv)
- **Vancouver rainfall data**: Downloaded from [NOAA Climate Data Online](https://www.ncei.noaa.gov/cdo-web/)

---

## Analysis

1.Load and clean data

- Imported Seattle and Vancouver daily rainfall datasets.

- Converted date columns to datetime.

- Removed duplicates and filtered data from 2018–2022.

- Replaced missing precipitation values with the mean for each city.

2.Merge and tidy data

- Combined Seattle and Vancouver datasets by date.

- Converted the dataset into tidy format with columns: date, city, precipitation.

3.Create derived variables

- is_rain: 1 if precipitation > 0, otherwise 0.

- month and year: used for monthly and yearly aggregation.

- monthly_total: total precipitation per month per city.

4.Analysis and visualization

- Line plots and bar plots were created to compare monthly and yearly rainfall.

- Observed that Vancouver generally receives more rain than Seattle, especially in late fall and winter.

## Files

Notebook performing analysis: Seattle_weather_project.ipynb

---

## Results

- Vancouver generally records more rainfall than Seattle across 2018–2022.

- Both cities exhibit strong seasonality, with the most rain in late fall and winter (October–March).

- The rainiest months for Seattle: December 2022.

- The rainiest months for Vancouver: October 2021.

---

## Authors

- Porhay Rouen — [porhay007](https://github.com/porhay007)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- NOAA Climate Data Online for precipitation data
- Python libraries: pandas, matplotlib, seaborn
- Seattle University’s DATA 5100 course for project structure and guidance
