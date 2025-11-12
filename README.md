# 🚇 TTC Subway Delay Analysis

This project analyzes subway delay patterns in Toronto using real TTC delay data from 2025. It explores which stations, lines, directions, and times of day are most affected — helping identify reliability issues and operational bottlenecks.

##🙌 Acknowledgments
Data for this project was sourced from the City of Toronto Open Data Portal, specifically the TTC Subway Delay Data since 2025 dataset. Special thanks to the City of Toronto and the TTC for making this data publicly available.

## 📊 Key Questions Answered

1. **Which delay codes are most frequent and severe?**
   - Top codes by frequency and average delay duration.
2. **What time of day and day of week see the most delays?**
   - Hourly and daily breakdowns with heatmaps.
3. **Which subway lines and directions (Bound) are most affected?**
   - Total delay, event count, and average delay per event.

---

## 🔍 Methodology

- **Data Cleaning**: Removed entries with missing vehicle IDs and filtered out zero-delay records.
- **Feature Engineering**: Extracted `DateTime`, `Hour`, `Minute`, and `Month` from timestamps.
- **Aggregation**: Grouped by `Code`, `Station`, `Line`, `Bound`, `Day`, and `Hour` to compute:
  - Frequency of delays
  - Total delay minutes
  - Average delay per event
- **Visualization**: Used Seaborn and Matplotlib for bar plots, heatmaps, and trend charts.

---

## 📈 Key Findings

- 🚨 **Most frequent delay code**: `MUSAN`
- 🕔 **Busiest hour for delays**: 5 AM
- 📅 **Worst day for delays**: Tuesday
- 🚉 **Station with most delay events**: Kennedy BD Station
- ⏱️ **Station with highest total delay time**: Eglinton Station
- 🚇 **Line+Bound with most delay events**: YU Southbound
- 🐢 **Worst average delay per event**: SHP Southbound (11 minutes/event)


