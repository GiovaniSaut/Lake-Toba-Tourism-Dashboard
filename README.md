# Lake Toba Tourism & Property Performance Dashboard

**Power BI Dashboard | Portfolio Project | 2026**

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=flat&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Data Source](https://img.shields.io/badge/Data-BPS%20Toba%20Regency-blue)](https://tobakab.bps.go.id)

---

## Overview

A five-page interactive Power BI dashboard analysing regional tourism trends across Lake Toba, North Sumatra, Indonesia — benchmarked against the real performance data of an 11-property short-let portfolio operating in Simanindo, Toba Regency.

This project combines three years of government-published tourism statistics (2022–2024) with live operational data from a personally managed Airbnb and Booking.com portfolio, to produce a data-driven view of seasonal demand patterns, occupancy benchmarking, and a forward-looking tourism forecast.

**The analysis answers four business questions:**
1. How has tourism to Lake Toba grown and what are the seasonal patterns?
2. How does our property portfolio perform relative to the regional hotel market?
3. Where do our guests come from and how is that mix shifting?
4. What does the tourism forecast suggest for 2025–2027 demand?

---

## Dashboard Pages

### Page 1 — Tourism Overview
Regional foreign arrivals across North Sumatra from 2022–2024, showing the sharp post-pandemic recovery, year-on-year growth rates, and seasonal demand cycles. Key metrics: total arrivals, average hotel occupancy, and average tourist stay.

![Tourism Overview](screenshots/page1-tourism-overview.png)

---

### Page 2 — Property Performance
Monthly occupancy rate, platform breakdown (Airbnb vs Booking.com vs offline), total bookings, average length of stay, and guest review score across 11 properties from June 2025 to May 2026.

![Property Performance](screenshots/page2-property-performance.png)

---

### Page 3 — Market Context
Benchmarking analysis placing the property portfolio's occupancy performance against the regional hotel occupancy rate (BPS Toba Regency). Regional occupancy peaked at ~57% in September 2024. The property portfolio mirrors the same seasonal pattern in 2025–2026 — with July–August peaks in per-unit occupancy — suggesting strong alignment with regional demand cycles despite operating at smaller scale.

![Market Context](screenshots/page3-market-context.png)

---

### Page 4 — Forecast
Tourism arrival forecast for 2025–2027 using Power BI's built-in exponential smoothing model (95% confidence interval), built on 36 months of monthly BPS data. North Sumatra foreign arrivals are projected to continue growing, supported by Indonesia's national "10 New Balis" tourism development programme of which Lake Toba is a designated priority destination.

![Forecast](screenshots/page4-forecast.png)

---

### Page 5 — Guest Nationalities
Geographic map and monthly bar chart showing international vs domestic guest mix across the portfolio from December 2025 to May 2026. Covers guest origin breakdown by country and the shift in international share across peak and off-peak months.

![Guest Nationalities](screenshots/page5-guest-nationalities.png)

---

## Key Findings

- **Tourism recovery is strong** — North Sumatra foreign arrivals grew 27% year-on-year in 2024, with September 2024 recording the highest hotel occupancy on record at ~57%
- **Seasonal pattern is consistent** — July–September is the peak window every year; January–February is the consistent low. This pattern repeats in our property data
- **Platform diversification is working** — bookings are distributed across Airbnb, Booking.com, and offline channels, reducing single-platform dependency as the portfolio scales
- **Guest mix is predominantly domestic** — international guests represent a smaller but growing share, with Singapore, Malaysia, and Australia the most common origins
- **Forecast supports growth** — the 2025–2027 projection suggests continued upward trend in arrivals, with seasonal peaks intensifying

---

## Data Sources

| Source | Detail | Coverage |
|---|---|---|
| BPS Toba Regency | Monthly foreign tourist arrivals · hotel occupancy rate | Jan 2022 – Dec 2024 |
| Personal host dashboard | Bookings · occupancy · platform · length of stay · review score | Jun 2025 – May 2026 |
| Guest records | Nationality data · international vs domestic split | Dec 2025 – May 2026 |

*All personally identifiable guest information has been aggregated and anonymised. No individual booking or guest data is published.*

---

## Tools & Skills

`Power BI Desktop` `DAX measures` `Data modelling` `Table relationships` `Excel data preparation` `Time series visualisation` `Forecasting` `KPI cards` `Map visuals` `Dashboard design`

**DAX measures written:**
```
Occupancy Rate % = 
DIVIDE(
    SUM(Property_Data[Total_Occupied_Nights]),
    SUM(Property_Data[Total_Available_Nights])
) * 100

Airbnb Share % = 
DIVIDE(
    SUM(Property_Data[Occupied_Airbnb]),
    SUM(Property_Data[Total_Occupied_Nights])
) * 100
```

---

## Files

| File | Description |
|---|---|
| `Lake_Toba.pbix` | Power BI Desktop file — open with Power BI Desktop (free) |
| `LakeToba_Tourism_Clean.xlsx` | Cleaned data file with Tourism_Arrivals and Property_Data sheets |
| `screenshots/` | PNG exports of all five dashboard pages |

---


## Context

Lake Toba is one of Indonesia's designated priority tourism destinations under the national "10 New Balis" development programme. The property portfolio operates in Simanindo, on the eastern shore of Samosir Island, within Toba Regency, North Sumatra. This dashboard was built to support data-driven operational and commercial decisions across the portfolio, and published as a portfolio project demonstrating applied Power BI and data analytics skills.

---

📧 giovani.saut@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/giovani-saut) · 🗂️ [Portfolio](https://github.com/GiovaniSaut)
