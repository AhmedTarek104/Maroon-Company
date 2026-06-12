# Maroon Company — Hotel Booking Analytics & Customer Segmentation

End-to-end data analysis project for a real Egyptian property 
management company operating short-term studio rentals.

## Live Dashboards

**[Customer Segmentation Dashboard →](https://public.tableau.com/views/Dashboard2_17813028660750/Dashboard1)**

**[Booking Analytics & Currency Trends →](https://public.tableau.com/views/Dashboard2_17813028660750/Dashboard2)**

---

## Business Context

Maroon Company manages multiple studio units in Egypt, 
accepting bookings through Hotels.com, Airbnb, Booking.com, 
and direct channels. Guests pay in USD, EUR, SAR, and EGP, 
creating a multi-currency revenue tracking challenge.

The company needed answers to two questions:
1. Who are our most valuable customers and how do we treat 
   them differently?
2. Which studios, channels, and months drive the most revenue?

---

## What I Did

**Data Cleaning (R)**
- Processed 1,152 real bookings across 16+ studio units
- Handled 4 currencies (EGP, USD, EUR, SAR) with conversion 
  to a unified EGP baseline
- Cleaned Arabic and English customer names
- Parsed dates and calculated derived metrics

**Customer Segmentation (K-Means Clustering)**
- Aggregated bookings per customer: total spend, avg nights, 
  booking frequency
- Applied K-means clustering (K=3) on scaled features
- Identified 3 distinct customer segments

**Tableau Dashboards**
- Built 2 interactive dashboards covering customer value 
  and operational analytics

---

## Key Findings

### Customer Segments

| Segment | Customers | Total Revenue (EGP) | Avg Nights | Avg Bookings |
|---------|-----------|-------------------|------------|--------------|
| High Value Loyalists | 862 customers | EGP 4,206,864 | High | High |
| Budget Frequent | 14 customers | EGP 607,083 | Medium | Medium |
| Low Engagement | 276 customers | EGP 506,297 | Low | Low |

**High Value Loyalists generate 79% of total revenue** despite 
being the largest segment, these customers should receive 
priority service, loyalty offers, and direct booking incentives.

### Operational Insights
- **Total Revenue**: EGP 5,320,244 across 1,152 bookings
- **705 unique customers** with a 29.93% repeat booking rate
- **Most active month**: July 2024
- **Top studio**: Studio-3-A
- **Top channel**: Hotels.com (500+ bookings)
- **Top payment**: Bank Account (616 bookings), Cash (513)
- **Revenue peak**: August 2024 (EGP 386,151)
- **USD is the dominant foreign currency**

### Business Recommendations
1. **Loyalty program for High Value Loyalists** — 79% of 
   revenue from this segment. A simple loyalty discount for 
   repeat bookings would protect this revenue.
2. **Direct booking incentive** — Hotels.com dominates but 
   charges commission. Converting top customers to direct 
   booking saves 15-20% commission fees.
3. **Revenue dips in Jan-Feb** — consider dynamic pricing 
   or promotional rates in off-peak months.
4. **Saudi market opportunity** — SAR payments growing, 
   Arabic-speaking Gulf guests are a valuable segment.

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| R (tidyverse, factoextra) | Data cleaning & K-means clustering |
| Tableau Public | Interactive dashboards |
| Excel | Source data format |

---

## Files

| File | Description |
|------|-------------|
| `Maroon_project.ipynb` | Full R analysis: cleaning, clustering, export |
| `README.md` | This file |

*Note: Raw booking data not included to protect client privacy.*

---

## About the Client

Maroon Company is an Egyptian property management company 
operating short-term studio rentals, serving both local 
and international guests through major OTA platforms.
