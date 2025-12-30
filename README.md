# Greenleaf KPI Performance Dashboard

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/07e19ffdf321ef31edaa83fd80c3c3803c564535/Greenleaf_Dashboard_Overview.png)

---

## Project Background

Greenleaf Stores is an early-stage online retailer specializing in eco-friendly home products.
 
The company has significant data on its sales, customer behavior, marketing efforts, and shipping performance that has been previously underutilized. This project thoroughly analyzes and synthesizes this data in other to uncover critical insights that will improve Greenleaf business outcomes.

##### Insights and recommendations are provided in the following key areas:

* Revenue Trends Analysis: Evaluation of historical revenue patterns focusing on Revenue, Order Volume, and Average Order Value(AOV).
* Product Level Performance: An analysis of Greenleaf’s product lines, understanding their impact on revenue and returns.
* Customer Purchase Behavior: An analysis of top customers that contribute significant share of revenue
* State Performance: An assessment of revenue and orders by state.
* Shipping Performance: An analysis of operational efficiency of shipment of orders


An interactive Excel dashboard can be found [here](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/376f065f828be534b521d69bde610f768e20393f/Greenleaf_KPI_Capstone_Remake.xlsx).
The Python notebook contain the code utilized to clean, organize, and prepare data for the dashboard can be found [here](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/565a5973e8461ee9a85b58453d18d562be44acb4/Greenleaf%20Data%20Cleaning%20Project-Copy-checkpoint.ipynb).


---

## Data Structure & Initial Checks

* Sales orders

* Customer data

* Product category master list

* Shipping Breakdown data

* State data

<img width="1423" height="310" alt="image" src="https://github.com/user-attachments/assets/9c542590-31e5-4bad-aa4e-2c5d3d9f069b" />

---

## Insights

### Revenue Trends:
* The monthly revenue trend shows pronounced fluctuations across the year, with revenue peaking in January ($12.5K), April–May (~$11.2K–$11.0K), and October ($11.4K), while experiencing sharp declines in June ($7.1K) and September ($7.1K)—representing drops of about 35–40% from peak months, reflecting seasonality, promotion timing, or operational capacity rather than random variation, Greenleaf’s sales performance is uneven and overly dependent on a few high-performing months to offset weaker periods.
* The uneven revenue growth is driven largely by fluctuations in Lighting, which contributes the largest revenue share but also experiences extreme MoM swings (e.g., +21.4% in April, -46.8% in June, -63.5% in September). At the same time, lower-value categories such as Cleaning and Bags show persistent negative MoM trends (Cleaning declining by 50–70% MoM in multiple months), while Gardening and Kitchenware intermittently offset declines through isolated growth spikes (e.g., Gardening +43.2% in June, Kitchenware +50.0% in October), indicating that overall revenue performance is highly dependent on a small number of volatile product categories rather than balanced portfolio growth.

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/496ce24a058c8aefed870ab19a95a7db7998b521/Monthly%20Revenue%20Trend.png)

### Product Performance:
* The data shows that lighting products—led by the Solar LED Lantern—generate over 40% of total profit while representing only about 23% of total orders, this concentration reflects sustained pricing power rather than temporary demand spikes, Greenleaf’s overall profitability is highly dependent on a narrow set of high-margin products.

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/496ce24a058c8aefed870ab19a95a7db7998b521/Profit%20by%20Product.png)

### State Comparisons:
* The order distribution map shows that Ohio (123 orders), North Carolina (112 orders), Pennsylvania (103 orders), and Illinois (102 orders) account for the highest order volumes, while large markets such as California (87) and Florida (87) underperform relative to their population size, reflecting underlying customer demand and repeat purchase behavior, Greenleaf’s sales traction is strongest in the Midwest and select East Coast states, with uneven national penetration.

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/ce27fd8aff346449b7fdbb0f67652c0ed36bab93/Order%20Distribution%20Across%20State.png)

### Shipping Performance:
* State-level delivery data shows clear variation in outcomes, with Pennsylvania (4.9%) and North Carolina (4.8%) contributing the highest shares of non-delivered orders, and North Carolina (2.2%), Pennsylvania (2.1%), and New York (2.0%) recording the highest Pending + Returned proportions, while Ohio posts the strongest performance with the highest Delivered share (8.0%) and the lowest Pending + Returned share (0.9%), higher levels of unresolved shipments indicate delivery friction rather than weak demand, this pattern signals elevated churn risk concentrated in specific high-impact states.
* Shipment status by product shows that Solar LED Lantern (9.6% non-delivered) and Eco Canvas Tote Bag (8.6% non-delivered) combine strong delivery volumes with the highest non-delivered and pending/returned rates. These unresolved deliveries disproportionately impact high-AOV customers, customer dissatisfaction and churn risk concentrated among GreenLeaf’s most valuable buyers.
*Product-level analysis also shows that Cleaning (8.2%) and Kitchenware (8.1%) have the highest return rates, compared to Bags at 5.0%, while Lighting (57.5%) and Cleaning (57.9%) also record the lowest delivery rates among all product categories, higher return rates and lower delivery success directly degrade customer satisfaction and repeat purchase behavior, these categories present a disproportionate operational risk relative to their order volumes.	

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/6420689ba35e1e9e6e7091433da7358e72294590/Shipping%20Performance%20by%20State.png) ![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/6420689ba35e1e9e6e7091433da7358e72294590/Return%20Rate%20by%20Product%20Category.png)

### Customer Behavior:
* Customer-level analysis indicates that a limited number of customers drives a large revenue share, while the majority contribute smaller, lower-frequency orders; assuming revenue concentration follows a typical Pareto pattern (where ~20% of customers generate ~80% of value), GreenLeaf’s revenue stability is highly dependent on retaining a relatively small group of high-value customers.

![image](https://github.com/debraville7/Greenleaf-KPI-Dashboard-Capstone/blob/d5edea16e26084315f50747be2e6fa77e9bb4168/Top%2010%20Customers.png)

---

## Recommendations:
* Greenleaf should track Monthly Revenue and Month-over-Month (MOM) Growth (%) and proactively deploy targeted promotions, product launches, or demand-stimulation campaigns in historically weak months such as June and September, enabling leadership to smooth revenue volatility, improve forecasting accuracy, and reduce reliance on peak-month performance to hit annual targets.	
* Management should treat lighting as a high-impact but high-risk revenue driver, pairing it with demand forecasting, inventory smoothing, and promotion pacing to reduce extreme MOM swings, while simultaneously investing in Kitchenware and Gardening, which demonstrate the ability to generate positive MOM growth (up to +50% and +43%, respectively) even during broader revenue downturns. This enables leadership to smooth monthly revenue volatility, protect topline performance during seasonal dips, and shift the business away from single-category dependency toward a more resilient, diversified revenue mix—reducing the risk of sharp monthly revenue contractions without increasing acquisition spend.
* Greenleaf should protect Lighting products from margin-eroding discounts and prioritize their availability and premium positioning, enabling leadership to maximize profit growth without increasing order volume and to improve return on inventory and marketing investment.
* Greenleaf should prioritize fulfillment and carrier performance reviews in North Carolina, Pennsylvania, and New York, focusing on reducing Pending and Returned orders while maintaining the strong delivery practices observed in Ohio.	
* Executives should monitor Revenue per Customer, AOV by Customer, and Repeat Purchase Indicators, and implement targeted retention strategies (priority fulfillment, proactive communication, loyalty incentives) for high-value customers, enabling leadership to protect core revenue streams and reduce churn risk without increasing acquisition spend.



