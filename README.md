## Project Title
Supply Chain Performance Analytics

## Brief One Line Summary
Data-driven dashboard to optimize shipments, returns, revenue recognition, and sales rep performance across global supply chains.

## Overview
This project delivers a comprehensive analytics framework for monitoring and optimizing supply chain operations across multiple regions, product categories, and sales representatives. The initiative integrates shipment, revenue, and return data into an interactive dashboard to enable fact-based decision-making.

The intended audience includes **executives**, **logistics managers**, and **sales leadership**, each requiring visibility into distinct KPIs such as return rates, revenue leakage, and rep-level performance. The deliverable is a modular analytics solution that can be embedded into existing BI ecosystems.

By consolidating two years of historical data (Aug 2022 – Jul 2024), the dashboard highlights systemic inefficiencies, regional anomalies, and actionable opportunities to reduce cost and accelerate revenue recognition.

## Problem Statement
The business faced a fragmented view of supply chain performance, with **40% of shipments delayed or returned**, generating revenue leakage and dissatisfied customers. **Australia**, despite high revenue, suffered a return rate 7× higher than Canada. Electronics, the top revenue driver, also led returns, eroding profitability. Success criteria were defined as:  
- Reduce regional return rate by ≥25% (KPI: returns per 1,000 shipments).  
- Improve shipment completion rate from 62% → ≥80%.  
- Shorten revenue recognition lag by ≥2 business days.  
- Improve bottom-decile sales rep completion rates by ≥20 percentage points.

## Dataset
Data sources aggregated from ERP logs, sales systems, and enriched with carrier metadata.

**Schema Example (CSV/Relational):**
```csv
shipment_id, order_id, region, country, product_category, shipment_date, delivery_date, status, revenue, sales_rep_id, carrier, return_reason
10001, 501, APAC, Australia, Electronics, 2023-01-05, 2023-01-11, Returned, 350, SR102, DHL, Damaged in Transit
10002, 502, NA, Canada, Office Equipment, 2023-01-07, 2023-01-09, Completed, 220, SR054, FedEx, 
...
