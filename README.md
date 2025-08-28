# placeholder

# Traffic Crash Analysis (2-Year Dataset)

## Project Overview
This project analyzes traffic accident data over a two-year period to identify patterns in crashes by day of the week, severity, and location. It highlights trends such as increased accidents on Fridays and explores the distribution of slight, serious, and fatal crashes.

## Motivation
Understanding when and where accidents occur can help inform traffic safety measures, targeted campaigns, and resource allocation for emergency services.

## Dataset
- **Source:** [Insert dataset source, e.g., UK Department for Transport or hypothetical dataset]
- **Columns:** `date`, `day_of_week`, `severity`, `location`, etc.
- **Data Cleaning:**
  - Standardized text columns (lowercase, stripped whitespace)
  - Corrected typos (e.g., 'fetal' → 'fatal')
  - Handled missing values by filling or flagging
  - Combined totals across two years, with future analysis planned for year-by-year trends

## Analysis & Key Findings
- **Monday–Thursday:** Stable accident totals (~45,583 per day)
- **Friday:** 10.85% increase in accidents, likely due to higher evening traffic and weekend travel
- **Saturday & Sunday:** Decrease in accidents, particularly Sunday, likely due to fewer commuters and closed shops
- **Severity Analysis:** Fatal crashes are rare; slight and serious crashes dominate
- **Location Analysis:** [Brief note if included, e.g., urban centers have more accidents than rural roads]

## Visualizations
- Bar charts of total accidents per day
- Inset charts highlighting fatal crashes
- Optional: heatmaps or line charts for deeper insights

## How to Run
1. Clone the repository  
2. Install required packages:  
   ```bash
   pip install -r requirements.txt
