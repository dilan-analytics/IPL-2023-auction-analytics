# 🏏 IPL 2023 Auction — Data Analytics Project



> A complete end-to-end data analytics project on the IPL 2023 Auction dataset — from raw data cleaning to an interactive Excel KPI dashboard.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Key Insights](#-key-insights)
- [Excel Dashboard](#-excel-dashboard)
- [Author](#-author)

---

## 🔍 Overview

This project performs a full data analytics pipeline on the **IPL 2023 Auction dataset** covering 568 players across 10 franchises. The goal is to uncover spending patterns, player value, team strategies, and squad composition through data cleaning, exploratory data analysis, visualisations, and an interactive Excel dashboard.

---

## 📂 Dataset

| Property | Detail |
|---|---|
| **Source** | IPL 2023 Auction Public Dataset |
| **Rows** | 568 players |
| **Columns** | Player, Base Price, TYPE, Cost (INR & USD), 2022 Squad, Team, Status |
| **Teams** | 10 IPL franchises + Unsold |
| **Player Types** | Batsman, Bowler, All-Rounder, Wicketkeeper |

---

## 📁 Project Structure

```
ipl-2023-auction-analytics/
│
├── data/
│   ├── IPL_Squad_2023_Auction_Dataset.csv    # Raw dataset
│   └── ipl_final_cleaned.csv                 # Cleaned dataset
│
├── notebooks/
│   └── IPL_2023_Data_Analytics.ipynb         # Full Jupyter analysis
│
├── dashboard/
│   └── IPL_2023_Dashboard.xlsx               # Excel KPI dashboard
│
├── visuals/
│   ├── sold_vs_unsold.png
│   ├── team_spend.png
│   ├── price_distribution.png
│   ├── player_type_dist.png
│   ├── top10_expensive.png
│   ├── price_multiplier.png
│   ├── retention_by_team.png
│   └── correlation_heatmap.png
│
└── README.md
```

---

## ✨ Features

### 🧹 Data Cleaning
- Renamed columns for readability
- Handled 325 missing values in auction cost columns
- Created a `Status` flag (Sold / Unsold) from team data
- Converted Base Price from rupees to crores for consistency
- Removed duplicate entries and validated data types

### 📊 Exploratory Data Analysis (EDA)
- **Sold vs Unsold** breakdown overall and by player type
- **Base Price distribution** across all players
- **Auction price distribution** — histogram and boxplot by role
- **Correlation heatmap** between base price, final cost, and price multiplier

### 🏟️ Team-wise Analysis
- Total auction spend per team
- Number of players bought per team
- Average spend per player by team
- Squad composition (player type breakdown per team)

### 🎯 Player Type Analysis
- Distribution of Bowlers, Batsmen, All-Rounders, Wicketkeepers
- Total and average spend by player role
- Sell rate by player type

### 💰 Auction Value Analysis
- **Top 10 most expensive players**
- **Price multiplier** — how many times over base price each player sold for
- **Base price vs final price scatter plot** coloured by role
- Identified most "bid-up" players from low base prices

### 🔄 Retention Analysis
- Players retained by the same team vs those who changed teams
- Retention rate % per franchise
- Teams that lost the most players to rivals

### 📋 Summary Report
- Auto-generated Python print report of all key KPIs

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Python 3.10+** | Core analysis language |
| **Pandas** | Data loading, cleaning, transformation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Static charts and visualisations |
| **Seaborn** | Statistical plots and heatmaps |
| **Jupyter Notebook** | Interactive analysis environment |
| **Microsoft Excel** | Interactive KPI dashboard with slicers |

---

## 📈 Key Insights

- 🏆 **Sunrisers Hyderabad** spent the most — **₹35.7 Crores** in the 2023 auction
- 💸 **Kolkata Knight Riders** had the lowest auction spend at ₹5.4 Crores
- 🎯 Only **42.8%** of players in the auction pool were actually sold
- 🔁 Most sold players **changed teams** — indicating a highly dynamic market
- 💰 Some low base-price players saw **10x–20x price jumps** due to bidding wars
- 🏏 **Bowlers** made up the largest share of players but **All-Rounders** commanded the highest average price

---

## 📊 Excel Dashboard

The project includes a fully interactive **KPI Dashboard** built in Microsoft Excel featuring:

| Element | Description |
|---|---|
| **4 KPI Cards** | Total Players, Total Sold, Total Spend, Avg Price |
| **Bar Chart** | Team-wise auction spend sorted by highest |
| **Donut Chart** | Sold vs Unsold player split |
| **Pie Chart** | Squad composition by player type |
| **Horizontal Bar** | Top 10 most expensive players |
| **Team Slicer** | Click any team to filter all charts instantly |
| **Type Slicer** | Filter by Batsman / Bowler / All-Rounder / Wicketkeeper |

> 💡 All charts are connected to slicers — clicking a team name updates every chart simultaneously.

---

### Excel Dashboard

1. Open `dashboard/IPL_2023_Dashboard.xlsx` in Microsoft Excel
2. Enable editing if prompted
3. Use the **Team** and **TYPE** slicers on the left to filter all charts interactively

---



## 👤 Author

**Your Name**
-Dilan Karunanayake

---

---

⭐ If you found this project helpful, please give it a star on GitHub!
