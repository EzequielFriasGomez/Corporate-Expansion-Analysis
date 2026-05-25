<p align="center">
  <img src="https://github.com/EzequielFriasGomez/Corporate-Expansion-Analysis/blob/main/Presentación_Expansión.gif" width="800"/>
</p>
*Nota: El archivo `.pbix` original se encuentra adjunto en este repositorio para su exploración completa.*

# Corporate Profitability & Expansion Audit (US Market)

**Project Overview** This repository details the data pipeline and commercial analysis for an expanding enterprise. Using a simulated dataset focused exclusively on the United States market, the primary goal was to audit the true financial health of the business. The analysis moves past gross sales volume to uncover net profitability margins and define a data-driven branch expansion strategy.

**The Business Problem** At first glance, the company boasted high gross revenue ($2.30 million), but management lacked visibility into actual operational costs and segmented performance. We needed to identify which regions and product categories were truly keeping the company afloat, and which were masking operational losses.

**Architecture & Process (ETL & BI)** 1. **Python (Pandas):** Built a data cleaning pipeline to drop irrelevant variables, localize the dataset into Spanish (translating business logic), and standardize currency formats. Feature engineering was applied to calculate the operational "Cost" per transaction.
2. **Microsoft Power BI:** Ingested the clean data model to dynamically calculate profitability margins using DAX expressions.

**Commercial Diagnosis (What the Data Shows)** The dashboard analysis exposed critical vulnerabilities:
1. **The Q4 Mirage vs. Q1 Profitability:** The fourth quarter drives massive volume through holiday discounts but severely damages the profit margin. Conversely, Q1 proved to be the most profitable, driven by *necessity-based purchases* rather than price promotions.
2. **A Two-Engine Profit Model:** Profitability relies on two solid pillars. Technology leads with 50.79% of net profit, closely followed by Office Supplies, which drives a massive 42.77%. Combined, they account for 93.56% of the company's total earnings.
3. **The Furniture Burden:** Furniture generates high sales volume but suffocates the overall margin, contributing a mere 6.44% of total profit. This vertical moves almost exclusively during discount seasons, showing that we are a clearance option rather than a furniture reference, likely burdened by high logistics and warehousing costs.
4. **Regional Discrepancies:** The South region is severely underperforming, bringing in nearly half the revenue and profit of the West, highlighting a flaw in market penetration.

**The Strategic Move** 1. **Furniture Vertical:** Execute an immediate audit of the furniture supply chain to drastically cut logistics costs, or begin divesting from the sector to aggressively reallocate capital into Technology and Office Supplies.
2. **Expansion Strategy:** Halt generic branch openings in the South until the commercial bottleneck is identified. Consolidate dominance in major Western and Eastern hubs (New York, Los Angeles, Seattle) by pushing the high-margin Tech and Office Supplies portfolios.

**Tech Stack:** Python (Pandas) | Microsoft Power BI (DAX)
