# Vision Zero: quick read on bike + ped crashes

Short, practical analysis for a planning audience. The notebook is analyst‑friendly and fast to skim.

## What’s inside
- Bikes: share, by‑type breakdown, simple bar chart, TL;DR
- Peds: top factors (+ "Other"), simple bar chart, TL;DR
- Multi‑party: distribution and severity mix (stacked bars)
- Bonus: trends, DOW × hour heatmap, KSI cuts (speed/light), and geo hot spots

## Run it
1) Put the CSVs next to the notebook:
   - `testdb_dbo_crash_incident.csv`
   - `testdb_dbo_party.csv`
2) Install deps (in your Jupyter env):
   ```bash
   pip install pandas seaborn matplotlib
   ```
3) Open `vision-zero.ipynb` and run all.

Notes:
- The bonus cells auto‑detect columns (date/time, severity, lat/lon) and skip gracefully if missing.
- Plots use seaborn defaults so they’re readable without extra tuning.