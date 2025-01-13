# 🦈 Dashboard of Shark Attacks

## 📚 About Data
Shark attacks reported over the past 100 years, including location, activity, victim info (name, gender, age), shark species, etc.

This dataset contains a csv table with 6,095 records.

Dataset was extracted from [here](https://www.kaggle.com/datasets/mysarahmadbhat/shark-attacks)

## 💡 Questions to ask
- Have shark attacks been increaseing or decreasing over the past 20 years?
- Which countries report the most shark attacks?
- What body parts are most often injured?
- What time of day are shark attacks most common?
- Which species of shark are attacking most often? Can you compare the last 3 days with top 3 species?

## ✏️ Data Wrangling
- Removed unnecessary columns
- Removed duplicate rows
- If Country, Area, and Location columns are all missing, then deleted the rows
- If unable to determine what Country it is by either Area or Location, deleted the rows
- Modified Year column using Case Number and Date columns. If 2 years were given (due to unsure of date), then averaged the year
- Missing values under Area, Location, Activity, and Sex columns were filled in as Unknown
- If anything other than number under Age column, they're Unknown. If 2 numbers were given, then averaged the age
- Missing values under Injury were filled in as Unknown. Cleaned the column as which body part was injured
- If anything other than time under Time column, they're Unknown. Cleaned the time into 2 digits (01, 02...)
- Missing values under Species, no species were given, "large" or "small" shark, only size given, they were filled in as Unknown

📍 Clean Data: [shark_data_cleaned.csv](https://github.com/andyalwaysok/Shark-Attack-Tableau/blob/main/Shark%20Attacks%20Clean.csv)

## 📊 Visualization
Tableau: [Dashboard](https://public.tableau.com/app/profile/sung.yoon7327/viz/DashboardofSharkAttacks/SharkAttacksDashboard)


<img width="1000" alt="image" src=https://github.com/andyalwaysok/Shark-Attack-Tableau/blob/98dce55ae5d63fe486d7c5c8c8689f1e5acdd99e/Shark%20Attacks%20Dashboard.png>
