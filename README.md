# Maroon Company — Hotel Booking Analytics & Customer Segmentation

End-to-end data analysis project for a real Egyptian property 
management company operating short-term studio rentals across 
multiple units in Egypt.

## Live Dashboards

**[Customer Segmentation Dashboard →](https://public.tableau.com/views/Dashboard2_17813028660750/Dashboard1)**

**[Booking Analytics & Currency Trends →](https://public.tableau.com/views/Dashboard2_17813028660750/Dashboard2)**

---

## Business Context

Maroon Company manages multiple studio units in Egypt, accepting 
bookings through Hotels.com, Airbnb, Booking.com, and direct 
channels. Guests pay in USD, EUR, SAR, and EGP — creating a 
multi-currency revenue tracking challenge.

The company needed answers to two questions:
1. Who are our most valuable customers and how should we treat 
   them differently?
2. Which studios, channels, and months drive the most revenue?

---

## What I Did

### Data Cleaning (R)
- Processed 1,152 real bookings across 16+ studio units
- Handled 4 currencies (EGP, USD, EUR, SAR) with conversion 
  to a unified EGP baseline for fair comparison
- Cleaned Arabic and English mixed customer names
- Parsed dates, handled missing values, calculated derived metrics

### Customer Segmentation (K-Means Clustering)
- Aggregated bookings per customer: total spend, average nights, 
  booking frequency
- Applied K-means clustering (K=3) on scaled features
- Identified 3 distinct behavioral customer segments
- Merged segment labels back to booking-level data for Tableau

### Tableau Dashboards
- Built 2 interactive dashboards covering customer value 
  and operational analytics
- Published to Tableau Public for live access

---

## Key Findings

### Customer Segments (K-Means, K=3)

| Segment | Customers | Avg Spend (EGP) | Avg Nights | Avg Bookings | Insight |
|---------|-----------|-----------------|------------|--------------|---------|
| Repeat High Spenders | 37 | 5,207 | 2.9 | 5.65 | Most valuable — book frequently and spend the most |
| Long Stay Guests | 79 | 150 | 9.04 | 1.38 | Stay longest per visit — ideal for weekly/monthly packages |
| One-Time Visitors | 601 | 437 | 2.09 | 1.39 | Largest group — low engagement, single bookings |

**Key insight:** The 37 Repeat High Spenders represent only 5% of 
customers but drive disproportionate revenue through frequent bookings 
(avg 5.65x per customer). Retaining this segment is the company's 
top priority.

### Operational Insights

| Metric | Value |
|--------|-------|
| Total Revenue | EGP 5,320,244 |
| Total Bookings | 1,152 |
| Unique Customers | 705 |
| Repeat Booking Rate | 29.93% |
| Average Revenue per Booking | EGP 4,626 |
| Most Active Month | July 2024 |
| Peak Revenue Month | August 2024 (EGP 386,151) |
| Top Studio | Studio-3-A |
| Top Booking Channel | Hotels.com (500+ bookings) |
| Top Payment Method | Bank Account (616 bookings) |
| Most Used Foreign Currency | USD |

### Business Recommendations

1. **Protect the Repeat High Spenders** — Only 37 customers but 
   booking 5.6x on average. A loyalty discount or direct booking 
   incentive for this group protects the highest-value revenue stream.

2. **Convert Long Stay Guests to packages** — 79 guests averaging 
   9 nights per stay are ideal candidates for weekly/monthly flat 
   rates. This increases predictability and fills low-demand periods.

3. **Reactivation campaign for One-Time Visitors** — 601 customers 
   who booked once and never returned. A targeted offer could convert 
   even 10% of this group into repeat customers.

4. **Address revenue seasonality** — Peak in August 2024 
   (EGP 386,151), trough in August 2023 (EGP 21,805). Dynamic 
   pricing in peak months and promotional rates in slow months 
   could smooth revenue.

5. **Reduce channel dependency** — Hotels.com dominates all bookings. 
   Over-reliance on one OTA means high commission costs. Direct 
   booking incentives for existing customers would reduce this risk.

6. **Capture the Gulf market** — SAR payments and Arabic-speaking 
   Gulf guests represent a growing segment worth targeting directly 
   through Arabic-language marketing.

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| R (tidyverse, factoextra, openxlsx) | Data cleaning, K-means clustering, export |
| Tableau Public | Interactive dashboards |
| Excel | Source data format |
| Google Colab | Development environment |

---

## Files

| File | Description |
|------|-------------|
| `Maroon_project.ipynb` | Full R analysis: cleaning, currency conversion, clustering, export |
| `README.md` | This file |

*Note: Raw booking data is not included to protect client privacy.*

---

## Repository Topics

`tableau` `r` `kmeans` `clustering` `data-analysis` 
`hospitality` `egypt` `customer-segmentation` `business-intelligence`

---

## About the Client

Maroon Company is an Egyptian property management company operating 
short-term studio rentals, serving both local and international 
guests through major OTA platforms including Hotels.com, Airbnb, 
and Booking.com.
