# Airbnb ROI Analysis — Open Short-Term Rental Opportunity (Portfolio Project)

**Objective**  
Find Indian cities with the most attractive return-on-investment (ROI) for open short-term rentals (Airbnb-style). The analysis ranks cities by ROI, payback period, and annual net income, and runs a sensitivity analysis to identify resilient opportunities under ADR/occupancy changes.

---

## Dataset
Source: `airbnb_analysis.xlsx` (sheets included)
- `ROI_Data` — city-level metrics (ADR, occupancy, monthly rent, annual revenue, initial investment, net income, ROI, payback)
- `Assumptions` — conversion & assumption notes
- `Potential_Hotspots` — candidate emerging markets

> The dataset was provided by project owner and used as-is; cleaning and validations were performed in the analysis.

---

## Tools
- R (tidyverse, readxl, scales)  
- Output: CSV summaries and PNG charts (saved to `results/`)

---

## Project steps (what I did)
1. Imported and cleaned the Excel dataset; standardized numeric fields and occupancy rates.  
2. Computed derived KPIs: profit margin, capex total, and validated payback calculations.  
3. Ranked cities by ROI (%), annual net income (INR), and shortest payback (years).  
4. Created visualizations: ROI distribution, top-10 ROI bar chart, ADR vs ROI scatter.  
5. Performed a sensitivity analysis (±10% ADR, ±10% occupancy) to identify cities resilient to pricing/occupancy changes.  
6. Exported: cleaned data (`cleaned_ranked_roi_data.csv`), `top_cities_by_roi.csv`, and `sensitivity_summary.csv`.

---

## Quick findings (from the dataset)
Top suggested cities (by ROI % in this dataset): **Mumbai, Udaipur, New Delhi, Kochi, Jaipur**.  
(Full top lists and exported files are in the `results/` folder after running the script.)

---

## What to include in your portfolio / resume
- Project title: *Airbnb ROI Analysis — Short-Term Rental Opportunity (India)*  
- One-line summary: *Analyzed city-level Airbnb economics in R; identified top ROI cities and performed sensitivity analysis for price and occupancy shocks.*  
- Link to GitHub repo: `<ADD_GITHUB_LINK_HERE>`

---

## How to reproduce
1. Clone the repo and place `airbnb_analysis.xlsx` at the repo root.  
2. Open R (or RStudio). Install packages if required:
```r
install.packages(c("tidyverse","readxl","scales"))
