# 🚍 NYC Bus Violation Impact Analysis
## 📖 Project Overview

This project was developed as part of the MHC++ Datathon, a competition focused on data-driven solutions to real-world problems. Our team analyzed MTA Bus Automated Camera Enforcement (ACE) violation data and bus speed data to understand how different types of traffic violations impact travel times and delays.

## 🏙️ Background

The Automated Camera Enforcement (ACE) program is used by the MTA to monitor traffic violations that disrupt bus operations. ACE cameras automatically detect vehicles committing violations and issue fines.

Initial Fine: $50 for a first violation

Uniform Fines: All violations result in the same penalty, regardless of impact.

Main Violation Types:

- Bus lane violations – vehicles blocking or driving in bus-only lanes.

- Bus stop violations – vehicles obstructing designated bus stops.

- Double parking violations – vehicles blocking traffic by parking illegally alongside another vehicle.

## ❓ Research Questions

- Should all fines cost the same amount?

- Do some violations affect travel time more than others?

## 📊 Datasets

We combined violation data with bus route segment speeds to measure the effect of traffic violations on delays.

MTA Bus Automated Camera Enforcement Violations: Beginning 2019

- https://data.ny.gov/Transportation/MTA-Bus-Automated-Camera-Enforcement-Violations-Be/kh8p-hcbm/data_preview

- Contains records of traffic violations (bus lane, double parked, bus stop blockages).

MTA Bus Route Segment Speeds: Beginning 2025

- Records bus speeds by route segment starting in 2025.

MTA Bus Route Segment Speeds (2023–2024)

- Historical dataset of bus segment speeds for 2023–2024.

## 🛠️ Methods

Tools Used:

- Python (Pandas, NumPy, Matplotlib, Seaborn)

- Jupyter Notebook for analysis

- Microsoft PowerPoint for presenting findings

Steps:

1. Cleaned and merged datasets by stop ID, route, date, and hour.

2. Computed average travel times across segments for each violation type.

3. Built bar charts and a pie chart in Python to visualize violation frequency and impact.

4. Designed a PowerPoint presentation to communicate insights and recommendations.

## 🔑 Key Findings

- Bus lane violations added about 5 minutes per segment at certain violation counts, making them the most impactful violation type.

- Even small per-segment delays compound across full bus routes, affecting thousands of riders daily.

- Current fines ($50 first offense) are uniform, but findings suggest some violations (like bus lane blockages) have disproportionately higher impacts — raising the question of whether fines should vary by violation type.

## ⚠️ Limitations

- The analysis could not fully isolate each violation type by holding the other two at zero. For example, bus-lane violations were not measured independently of bus-stop and double-parked violations, so overlap may influence the observed delays.

## 💡 Business Recommendations

Reevaluate Fine Structures: 

- Consider differentiated fines that reflect the severity of travel time impact.

Public Communication Campaigns:

- Share statistics with the public showing how violations slow buses for thousands of riders.

- Example message: “Bus lane violations have the potential to double travel time for NYC buses.”

Deterrence Campaigns:

- Highlight fines and reinforce enforcement efforts.

- Use data-driven messaging to shift driver behavior.

## 📈 Visuals

- Bar chart: violation counts vs. average travel time per segment.

- Pie chart: proportion of violations by type.

- Selected charts integrated into a PowerPoint slide deck for final presentation.

## 🚀 Next Steps

- Develop a pricing model to adequately match fine amounts to the level of delay each violation type causes for NYC buses.

- Create public campaigns to alert citizens how violations can slow down buses for thousands of NYC riders
