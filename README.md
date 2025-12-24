# Greenleaf KPI Dashboard

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/07e19ffdf321ef31edaa83fd80c3c3803c564535/Greenleaf_Dashboard_Overview.png)

---

## Project Background

Greenleaf Stores is an early-stage online retailer specializing in eco-friendly home products.
 
The company has significant data on its sales, customer behavior, marketing efforts, and shipping performance that has been previously underutilized. This project thoroughly analyzes and synthesizes this data in other to uncover critical insights that will improve Greenleaf business outcomes.

Insights and recommendations are provided in the following key areas:

* Revenue Trends Analysis: Evaluation of historical revenue patterns focusing on Revenue, Order Volume, and Average Order Value(AOV).
* Product Level Performance: An analysis of Greenleaf’s product lines, understanding their impact on revenue and returns.
* Customer Purchase Behavior: An analysis of top customers that contribute significant share of revenue
* State Performance: An assessment of revenue and orders by state.
* Shipping Performance: An analysis of operational efficiency of shipment of orders


An interactive Excel dashboard can be found [here](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/376f065f828be534b521d69bde610f768e20393f/Greenleaf_KPI_Capstone_Remake.xlsx).
The Python notebook contain the code utilized to clean, organize, and prepare data for the dashboard can be found [here](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/565a5973e8461ee9a85b58453d18d562be44acb4/Greenleaf%20Data%20Cleaning%20Project-Copy-checkpoint.ipynb).


---

## Data Structure & Initial Checks

Sales orders

Customer data

Product category master list

Shipping Breakdown data

State data

<img width="1423" height="310" alt="image" src="https://github.com/user-attachments/assets/9c542590-31e5-4bad-aa4e-2c5d3d9f069b" />

---

### Revenue Trends:
* The monthly revenue trend shows pronounced fluctuations across the year, with revenue peaking in January ($12.5K), April–May (~$11.2K–$11.0K), and October ($11.4K), while experiencing sharp declines in June ($7.1K) and September ($7.1K)—representing drops of roughly 35–40% from peak months; assuming these swings reflect seasonality, promotion timing, or operational capacity rather than random variation, Greenleaf’s sales performance is uneven and overly dependent on a few high-performing months to offset weaker periods.
* The uneven revenue growth is driven largely by fluctuations in Lighting, which contributes the largest revenue share but also experiences extreme MoM swings (e.g., +21.4% in April, -46.8% in June, -63.5% in September). At the same time, lower-value categories such as Cleaning and Bags show persistent negative MoM trends (Cleaning declining by 50–70% MoM in multiple months), while Gardening and Kitchenware intermittently offset declines through isolated growth spikes (e.g., Gardening +43.2% in June, Kitchenware +50.0% in October), indicating that overall revenue performance is highly dependent on a small number of volatile product categories rather than balanced portfolio growth.

<br>

### Product Performance:
* The data shows that lighting products—led by the Solar LED Lantern—generate over 40% of total profit while representing only about 23% of total orders; assuming this concentration reflects sustained pricing power rather than temporary demand spikes, Greenleaf’s overall profitability is highly dependent on a narrow set of high-margin products.
