# Project 5: TCR Violations Across 5 States
**Client:** UMass Amherst Water Research Team  
**Analyst:** Aminasahra Warsame 
**Date:** April 2026  

---

## Overview
This project analyzes Total Coliform Rule (TCR) violations across five U.S. states using data from the Safe Drinking Water Information System (SDWIS) database. The five states — Maine, Georgia, Texas, Nebraska, and California — were selected to represent five different EPA regions, providing a geographically representative sample of TCR violations across the United States.

A key focus of the analysis is whether small water systems (serving 10,000 or fewer people) experience disproportionately higher violation rates compared to large systems.

---

## Repository Contents

| File | Description |
|---|---|
| `Project5_TCR_Violations.ipynb` | Main Python notebook with all analysis and figures |
| `Maine.csv` | SDWIS Water System Summary — Maine (EPA Region 1) |
| `Georgia.csv` | SDWIS Water System Summary — Georgia (EPA Region 4) |
| `Texas.csv` | SDWIS Water System Summary — Texas (EPA Region 6) |
| `Nebraska.csv` | SDWIS Water System Summary — Nebraska (EPA Region 7) |
| `California.csv` | SDWIS Water System Summary — California (EPA Region 9) |
| `Project5_SOW.docx` | Scope of Work |
| `Project5_Gantt.xlsx` | Project Gantt Chart |
| `Project5_Timesheet.xlsx` | Project Timesheet |

---

## Data Source
Data was downloaded from the SDWIS Federal Reports Public Dashboard:  
https://sdwis.epa.gov/ords/sfdw_pub/r/sfdw/sdwis_fed_reports_public/1

- Report Type: Water System Summary
- Submission Year: 2026, Quarter 1
- Owner Type: State-owned systems
- Activity Status: Active

---

## How to Run

### Requirements
Install the required Python packages:
```
pip install pandas numpy matplotlib geopandas
```

### Steps
1. Clone or download this repository
2. Place all 5 CSV files in the same folder as the notebook
3. Open `Project5_TCR_Violations.ipynb` in Jupyter
4. Click **Kernel → Restart & Run All**

---

## Analysis Summary

### Figures Produced
- **Figure 1:** Total and average violations per system by state
- **Figure 2:** Small vs. large system violation comparison by state
- **Figure 3:** Choropleth map of violations across the 5 study states

### Key Findings
- California had the highest total number of violations due to its large number of state-owned facilities
- Small water systems (≤10,000 population served) made up the majority of systems in all five states
- Small systems consistently showed higher average violations per system compared to large systems, consistent with national trends reported in peer-reviewed literature
- Differences across states are likely driven by infrastructure age, system size distribution, and regulatory capacity

---

## Python Packages Used
| Package | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and analysis |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `geopandas` | Choropleth map creation *(new package)* |

---

## References
- Allaire, M., Wu, H., & Lall, U. (2018). National trends in drinking water quality violations. *PNAS*, 115(9), 2078–2083.
- U.S. EPA. (2017). *Drinking Water and Wastewater Utility Small Systems*. EPA 816-F-17-003.
- U.S. EPA. (2023). *Total Coliform Rule*. https://www.epa.gov/dwreginfo/total-coliform-rule
- SDWIS Federal Reports. (2026). *Water System Summary*. https://sdwis.epa.gov
