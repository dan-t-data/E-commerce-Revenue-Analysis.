# E-commerce Revenue & Retention Analysis  

## Executive Summary  
After a pandemic-driven sales surge in 2020, this global e-commerce company saw growth level off and repeat purchases decline. Revenue became more volatile, leaning too heavily on new customer acquisition instead of building lasting customer relationships.  

To stabilize growth, the company needs to shift back to **retention-led growth** by:  
- Aligning sales campaigns to seasonal demand patterns  
- Rebalancing the product mix to reduce reliance on a few high-ticket items  
- Expanding loyalty enrollment to increase repeat purchasing  
- Improving visibility into refunds and returns to manage risk  

---

## Business Problem  
The pandemic exposed a key challenge: the company could attract new customers, but it struggled to keep them coming back. As repeat purchases declined, revenue swings grew larger, making the business harder to forecast and sustain.  

To address this, the company must answer two critical questions:  
1. **Where are customers dropping off after their first purchase—by region, month, and product?**  
2. **Which actions will most effectively increase repeat purchases and restore steady, retention-driven revenue?**  

---
## Schema Diagram
Data model combining Order, Customers, Geo_Lookup, and Order_Status for analysis.
<img width="520" height="314" alt="schema diagram" src="https://github.com/user-attachments/assets/c81cb5bf-7870-4ce6-b6ac-89aac6fdc0ca" />

---
## Methodology & Skills  
**SQL** – Created a unified dataset by joining orders, customers, geo data, and order status. Used CTEs, CASE logic, and window/aggregate functions to calculate revenue, AOV, repeat purchase timing, product mix, loyalty behavior, refund rates, and delivery times.  

**Excel** – Validated SQL outputs with PivotTables and PivotCharts. Applied SUMIFS, COUNTIFS, AVERAGEIFS, IF, and INDEX-MATCH to calculate KPIs. Built simple what-if models to test the impact of seasonal alignment, accessory bundling, and loyalty enrollment.  

---

## Key Insights  

1. **Seasonality & Regional Timing**  
   - **Data:** February and October are consistently weak, while December/January peak. In LATAM, April (+20%) and July (+24%) outperform the Nov–Dec holiday period (+10%).  
   - **Insight:** Campaigns are misaligned. Shifting promotions to Feb/Oct globally and Apr/Jul in LATAM could recapture demand.  

2. **Over-Concentration in Product Mix**  
   - **Data:** Laptops and monitors grew to ~95% of sales (up from ≤75%). Headphones—historically 26% of sales with just 2% returns—were nearly absent in 2021.  
   - **Insight:** Heavy reliance on big-ticket items increases volatility. Restoring accessory attach (like headphones) can drive repeat purchases and stability.  

3. **Loyalty Program Underutilized**  
   - **Data:** Loyalty sales surpassed non-loyalty in 2021 and led AOV in 2022. Loyalty buyers also repurchase faster (1.6 vs. 2.3 months).  
   - **Insight:** Loyalty works, but enrollment is too low. Scaling it would pull forward revenue and improve customer lifetime value.  

4. **Refund Blind Spots**  
   - **Data:** Return rates: Headphones ~2%, Laptops ~6%, Monitors 18–22%. Refund tracking dropped in 2021 and vanished in 2022.  
   - **Insight:** Missing refund data hides risk. Full visibility is needed to improve pricing, product content, and quality assurance.  


---
## Data Visuals


---

## Recommendations  

1. **Realign Campaign Timing**  
   - Target promotions in **Feb/Oct** (global).  
   - Shift LATAM focus to **Apr/Jul** where demand peaks.  

2. **Diversify the Product Mix**  
   - Bundle **headphones** with laptops/monitors at checkout.  
   - Improve monitor content and setup guides to reduce returns.  

3. **Expand the Loyalty Program**  
   - Enable easy sign-up at checkout.  
   - Offer perks like early access and simple rewards to drive repeat spend.  

4. **Fix Refund Tracking**  
   - Reinstate >95% refund coverage and capture return reasons.  
   - Use data to address top drivers (spec clarity, packaging, QA).  

---

## Next Steps  

- **Baseline KPIs** – Define metrics for revenue, AOV, repeat rate, attach %, and refund %. Set a 12-month baseline in Excel.  
- **Pilot & Measure** – Test calendar adjustments, accessory bundles, and loyalty sign-ups. Track weekly results in dashboards.  
- **Operationalize Dashboards** – Maintain a live Excel/Power BI view for Sales, Marketing, and CS with filters and version control.  
- **Scale Success** – Roll out proven tactics and track monthly deltas in revenue, repeat, attach, and returns.  
