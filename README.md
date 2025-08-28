# UK Road Safety Analysis (2021–2022)

## Project Overview
This project analyzes road accident data in the UK over a two-year period (2021–2022). The goal is to identify patterns and trends in road accidents by day of the week, time of day, and severity. The analysis provides insights into when and where accidents are most likely to occur, helping inform road safety measures and resource allocation.

## Motivation
Understanding the distribution of road accidents can help policymakers, urban planners, and emergency services improve road safety. By identifying high-risk times and days, targeted interventions can be implemented to reduce accidents and save lives.

## Dataset
- **Source:** [UK Department for Transport Road Safety Data](https://data.gov.uk/dataset/road-accidents-safety-data)
- **Timeframe:** 1 January 2021 – 31 December 2022
- **Size:** ~300,000 rows of police-reported road traffic accidents
- **Key Columns:**
  - `Time`: Time of the accident
  - `Day_of_Week`: Day of the week the accident occurred
  - `Accident_Severity`: Severity of the accident (Slight, Serious, Fatal)
  - `Location`: Accident location details
  - `Environmental Conditions`: Weather, lighting, and road surface conditions

## Data Cleaning
- Converted `Time` column to a datetime format for easier analysis.
- Corrected typos in the `Accident_Severity` column (e.g., 'Fetal' → 'Fatal').
- Removed unused columns such as `Carriageway_Hazards`, `Police_Force`, and `Vehicle_Type`.
- Handled missing values by filling with median values or flagging them for further review.

## Analysis & Key Findings
### 1. **Accidents by Day of the Week**
- **Monday–Thursday:** Accident totals are stable, averaging ~45,583 accidents per day.
- **Friday:** Accidents increase by 10.85%, likely due to higher evening traffic and weekend travel.
- **Saturday & Sunday:** Accidents decrease, particularly on Sunday, likely due to fewer commuters and closed shops.

### 2. **Accidents by Time of Day**
- Accidents peak during rush hours (8 AM and 5–6 PM) on weekdays.
- Weekend accidents are more evenly distributed throughout the day, with a slight increase in the evening.

### 3. **Severity Analysis**
- **Slight Accidents:** Make up the majority of reported crashes.
- **Serious Accidents:** Less frequent but still significant.
- **Fatal Accidents:** Rare, accounting for only 1.28% of all crashes. Fatal accidents are slightly more common on weekends, possibly due to higher speeds and riskier driving behavior.

### 4. **Visualizations**
- **Bar Charts:** Show total accidents by day of the week and severity.
- **Line Charts:** Highlight hourly accident trends for each day of the week.
- **Subplots:** Provide a detailed breakdown of accidents by time of day for all seven days.

## How to Run
1. Clone the repository  
2. Install required packages:  
   ```bash
   pip install pandas matplotlib

## Future Work
- **Year-by-Year Analysis:** Compare accident trends between 2021 and 2022.
- **Geospatial Analysis:** Map accident hotspots to identify high-risk areas.
- **Predictive Modeling:** Use machine learning to predict accident likelihood based on time, location, and environmental factors.

## Acknowledgments
This project uses data from the [UK Department for Transport](https://data.gov.uk/dataset/road-accidents-safety-data). Special thanks to the contributors of open-source Python libraries such as Pandas, Matplotlib, and Seaborn for enabling this analysis.
