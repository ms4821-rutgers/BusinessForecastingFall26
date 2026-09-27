# Dataset Overview & Data Dictionary

## Dataset Summary
- **Dataset Title:** Unemployment in America Per US State
- **Geography:** U.S. States, District of Columbia, and select sub-state areas (e.g., Los Angeles County, New York City)
- **Time Period:** 1976 – 2025
- **Periodicity:** Monthly
- **Total Records:** 31,747 rows across 11 variables

---

## Data Dictionary

| Variable Name | Data Type | Definition | Units / Scale | Notes & Examples |
| :--- | :--- | :--- | :--- | :--- |
| `FIPS Code` | Integer | Federal Information Processing Standard unique numeric identifier for the state or area. | Numeric Code | e.g., `1` for Alabama, `6` for California |
| `State/Area` | Categorical / Text | Name of the U.S. state, territory, or metropolitan area. | String | e.g., `"Alabama"`, `"Los Angeles County"` |
| `Year` | Integer | Four-digit calendar year of the observation. | Year (`YYYY`) | Range: `1976` to `2025` |
| `Month` | Integer | Numerical representation of the observation month. | Month (`1`–`12`) | e.g., `1` for January, `12` for December |
| `Total Civilian Non-Institutional Population in State/Area` | Numeric / Text (Formatted) | Total non-institutionalized civilian population aged 16 and older residing in the state or area. | Persons | Stated with comma formatting (e.g., `"2,605,000"`) |
| `Total Civilian Labor Force in State/Area` | Numeric / Text (Formatted) | Total number of people aged 16+ who are either employed or actively seeking employment. | Persons | Stated with comma formatting (e.g., `"1,486,509"`) |
| `Percent (%) of State/Area's Population` | Numeric / Float | Labor Force Participation Rate: percentage of the civilian non-institutional population in the labor force. | Percent (`%`) | e.g., `57.1` (indicates 57.1%) |
| `Total Employment in State/Area` | Numeric / Text (Formatted) | Total number of employed civilians aged 16 and older in the state or area. | Persons | Stated with comma formatting (e.g., `"1,387,606"`) |
| `Percent (%) of Labor Force Employed in State/Area` | Numeric / Float | Employment-to-Labor-Force ratio: percentage of the active labor force that is currently employed. | Percent (`%`) | e.g., `53.3` (indicates 53.3%) |
| `Total Unemployment in State/Area` | Numeric / Text (Formatted) | Total number of unemployed civilians aged 16 and older actively looking for work. | Persons | Stated with comma formatting (e.g., `"98,903"`) |
| `Percent (%) of Labor Force Unemployed in State/Area` | Numeric / Float | Unemployment Rate: percentage of the active labor force that is unemployed. | Percent (`%`) | Key target variable for forecasting; e.g., `6.7` (indicates 6.7%) |

---

## Data Collection Methodology
- **Data Source:** Bureau of Labor Statistics (BLS) - Local Area Unemployment Statistics (LAUS) program.
- **Collection Frequency:** Updated monthly.
- **Methodology:** Produced via statistical estimation models combining data from the Current Population Survey (CPS), the Current Employment Statistics (CES) program, and state unemployment insurance (UI) claims systems.

## Key Forecasting Target
For time series modeling and forecasting, the main variable of interest is **`Percent (%) of Labor Force Unemployed in State/Area`** (the monthly unemployment rate) or **`Total Unemployment in State/Area`**.

## Data Collection Methodology
- **Data Source:** Bureau of Labor Statistics (BLS) – Local Area Unemployment Statistics (LAUS) program.
- **Collection Method:** Data is produced using statistical estimation models that combine inputs from the Current Population Survey (CPS), the Current Employment Statistics (CES) program, and state unemployment insurance (UI) claims systems.
- **Collector:** U.S. Bureau of Labor Statistics (BLS) in cooperation with State Employment Security Agencies.
- **Update Frequency:** Updated monthly.

---

## Why This Dataset Intrigues Me
I chose this dataset because unemployment rates affect all age groups across the U.S. Tracking state by level monthly data from 1976 through 2025 covers several major economic events, including the 2008 financial crisis and the 2020 COVID-19 pandemic. Analyzing this time series lets me practice building forecasting models that include strong seasonal patterns, economic recessions, and long term state level labor market trends.
