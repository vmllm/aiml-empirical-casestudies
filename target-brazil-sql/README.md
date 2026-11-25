# Target Brazil E-Commerce, Logistics & Payment Analytics (Google BigQuery SQL)

## Problem Statement
Query and analyze a multi-table relational e-commerce dataset (`customers`, `orders`, `order_items`, `payments`) spanning **772 days** (September 2016 – October 2018) across **4,119 cities and 27 Brazilian states** to evaluate revenue growth, regional logistics bottlenecks, delivery speed, and installment payment behavior[cite: 226, 227, 237].

## Technical Stack & SQL Techniques
* **Platform:** Google BigQuery (`SQL`)[cite: 226]
* **Query Patterns:** Multi-table `JOIN`s, Common Table Expressions (`WITH` / CTEs), Window Functions (`RANK() OVER`), Temporal Extraction (`EXTRACT`, `DATE_DIFF`), Conditional Aggregation (`CASE WHEN`), and `UNION ALL`[cite: 226, 227, 228, 229, 230, 233, 234, 235]

## Key Empirical Findings
1. **Revenue & Order Growth:** Revenue (Jan–Aug comparison) surged **136.98%** from 2017 to 2018, with peak order activity occurring in the **Afternoon** (38,135 orders) and **Night** (28,331 orders) and seasonal highs between **May and August**[cite: 228, 230, 231, 238].
2. **Regional Concentration vs. Logistics Friction:** **São Paulo (SP)** leads customer volume (41,746 customers) and achieves the fastest average delivery (**8.30 days**) and lowest average freight (**15.15 BRL**)[cite: 229, 230, 234, 236]. Conversely, remote northern states like **Roraima (RR)** face the longest delivery times (**28.98 days**) and highest average freight (**42.98 BRL**)[cite: 234, 235, 236].
3. **Delivery Buffer Accuracy:** States such as **AC** (19.76 days early) and **RO** (19.13 days early) consistently beat estimated delivery dates, indicating conservative baseline delivery estimates[cite: 236].
4. **Payment Behavior:** Credit cards dominate payment volume, with nearly half of all orders utilizing multi-month installment plans (ranging from 2 to 24 installments)[cite: 238, 239].

## Strategic Recommendations
* **Last-Mile Carrier Partnerships:** Partner with regional logistics carriers in high-freight northern states (RR, PB, RO) to reduce shipping costs and transit times[cite: 234, 239].
* **Shift-Aligned Fulfillment Staffing:** Scale warehouse and support capacity during Afternoon and Night peak ordering windows[cite: 228, 239].
* **Cash-Flow & Seasonal Promotions:** Introduce single-installment payment incentives and targeted Q4/Christmas promotional campaigns to lift September–December order volumes[cite: 239].
