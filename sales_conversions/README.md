# Maximising Sales Conversions in A Travel Industry

## Background and Overview

This notebook presents an analysis of lead conversion data collected from a travel booking company. The dataset includes various attributes related to leads, their sources, assigned agents, enquiry destinations, and the outcomes of these leads. 

By examining this data, we aim to uncover key insights and trends that can help in understanding the effectiveness of different lead sources, the performance of agents, and the preferences of clients.

![image](travel.jpeg)

---

## Dataset Description

The dataset contains the following columns:

- **Lead Date:** The date when the lead was generated.
- **Lead Source:** The origin of the lead (e.g., website, referral, advertisement).
- **Name:** The name of the lead.
- **Phone:** The contact phone number of the lead.
- **Assigned To:** The agent assigned to handle the lead.
- **Enquiry Destination:** The travel destination the lead is interested in.
- **ExClient:** A flag indicating whether the lead is an existing client.
- **Status:** The current status of the lead (e.g., converted, not converted (Blank).
- **Conversion Date:** The date when the lead was converted (if applicable).
- **Trip:** Trip Name.
- **Trip Date:** The date of the booked trip (if applicable).
- **Booking ID:** The unique identifier for the booking (if applicable).
- **Pax:** The number of passengers for the booking.
- **Per Person Cost:** The cost per person for the trip.
- **Total Bill:** The total bill amount for the booking.
- **Converted By:** The agent who converted the lead.
- **Date:** The lead date (minus the timestamp). -- An Extracted Column
- **Month:** The month of lead date -- An Extracted Column

---
## Executive Summary

Lead generation peaks in August, driven primarily by Lead Source 1, which accounts for 71.17% of leads but has lower conversion efficiency. Revenue performance shows a decline in August 2024, with high potential in destinations like Ladakh. Sales Person 0 excels in conversions, while 87% of customers prefer trips under ₹400,000.

Focus on optimizing Lead Source 1, replicate successful sales strategies, target high-value destinations like Ladakh, and enhance training for underperforming salespersons to improve conversion rates and revenue based on top performing sales representatives like Sales Person 0.

---

## Insights Deep Dive

Below are detailed version of the insights that we can across analysing this data:

1. **Lead Generation Insights:**
   - **Peak Lead Volume:** Lead count peaks in August (33.55%), with the lowest in July (12.63%), indicating a need to prepare for high lead volumes in the mid-year.
   - **Lead Source 1 Dominates:** Lead Source 1 generates the highest volume of leads (71.17%) but shows inefficiencies in converting those leads to revenue (only 33.72% of revenue).

2. **Trip Performance Insights:**
   - **Seasonal Trip Variations:** August 2023 saw the highest trips (926), with a sharp decline in August 2024 (83.79%). There’s a recovery in October 2024 with a 139.06% increase in trips.
   - **Monthly Fluctuations:** July 2024 had the least trips (64), signaling the need for better performance in the early months of the year.

3. **Revenue Insights:**
   - **Revenue Peaks and Declines:** Revenue peaked in August 2023 (₹5.27M) but saw a decline in October 2024 (₹0.94M). The 2024 recovery shows steady improvement, peaking at ₹1.09M in September.
   - **Low Revenue-Lead Correlation:** A low correlation (0.22) between lead count and revenue highlights inefficiencies in converting leads into revenue.

4. **Destination Insights:**
   - **High Revenue Potential from Ladakh:** Despite fewer leads, Ladakh generates higher revenue (8.52%), indicating high-value customers.
   - **Conversion Rates:** Spiti Valley shows the highest conversion rate (0.277), while destinations like Kashmir and Bhutan show low conversion rates, presenting opportunities for improvement.

5. **Sales Performance Insights:**
   - **Top Performers Stand Out:** Sales Person 0 shows strong conversion rates and should serve as a model for others. Sales Person 33 converts more leads despite being assigned more, suggesting that lead quality matters more than volume.
   - **Low Conversion from Ex-Clients:** While Ex-clients convert at 3.65%, the conversion rate from new clients is only 2%, indicating a need to attract and convert new clients more effectively.

6. **Operational Insights:**
   - **Passenger Count Correlation with Revenue:** A moderate correlation (0.57) exists between the number of passengers and total bill, suggesting more passengers generally lead to higher revenue.

---

## Recommendations

Below are the strategic recommendations that can be made based on the analysis:-


1. **Improve Lead Conversion Efficiency:**
   - **Focus on Lead Source 1:** While Lead Source 1 generates the most leads, improve conversion rates through better lead nurturing, qualification, and follow-up strategies.
   - **Replicate Success from Lead Source 3:** Focus on converting leads from Lead Source 3, as they bring higher revenue despite their lower volume.

2. **Optimize Trip Promotions:**
   - **Increase Early-Year Trip Numbers:** Address the low trip count in July 2024 by launching early-year promotions and packages to boost demand.
   - **Capitalize on Recovery in October:** Analyze the reasons behind the October trip increase and replicate successful strategies for other months.

3. **Boost Revenue by Improving Conversion:**
   - **Enhance Revenue from High-Potential Regions:** Focus on high-revenue generating regions like Ladakh, and explore strategies to increase conversions in underperforming regions like Kashmir and Bhutan.
   - **Optimize for Budget-Conscious Customers:** Since 87% of customers prefer to spend under ₹400,000, create more affordable packages to appeal to a broader customer base.

4. **Sales Strategy Improvements:**
   - **Model Success of Top Performers:** Encourage other salespeople to adopt strategies similar to Sales Person 0, especially promoting high-conversion trips like BYOG.
   - **Target Training to Underperforming Salespeople:** Provide additional training to salespeople with lower conversion rates (e.g., Sales People 52, 49, 50) to improve their efficiency.

5. **Focus on Ex-Client Conversions:**
   - **Nurture Ex-Clients:** Since Ex-clients show a higher conversion rate, invest in targeted outreach to past customers, offering incentives for repeat bookings and upselling.

6. **Operational Adjustments:**
   - **Optimize Passenger Groups:** Since passenger count correlates with total bill, focus on increasing group sizes where possible, adjusting pricing models or optimizing operations to accommodate larger groups.

---

## Caveats and Assumptions

1. **Data Completeness:** The analysis is based on the available dataset, which may not capture all leads or transactions. Missing data could impact the accuracy of insights and trends.

2. **Lead Source Attribution:** The attribution of leads to specific sources may not account for multi-channel interactions, potentially skewing the effectiveness of each lead source.

3. **Temporal Variability:** Seasonal trends and external factors (e.g., economic conditions, travel restrictions) may influence lead generation and conversion rates, which are not fully accounted for in this analysis.

4. **Customer Behavior:** The preferences and behaviors of customers may change over time, and insights drawn from historical data may not fully predict future trends.

5. **Salesperson Performance:** Variability in individual salesperson performance may be influenced by factors beyond their control, such as lead quality and market conditions, which could affect the interpretation of conversion rates.

6. **Revenue Reporting:** Revenue figures may include adjustments or refunds that could distort the actual performance metrics, leading to potential misinterpretations of revenue trends.

7. **Assumption of Consistency:** It is assumed that the patterns observed in the data will remain consistent over time, which may not hold true due to changing market dynamics or business strategies

---

## Installation

To run the project locally, open up the code editor of your choice and move to the terminal. Then follow the instructions below:-

1. Clone the repository:

   ```bash
   git clone https://github.com/dakshbhatnagar/projects/sales_conversions.git
   ```

2. Switch to the directory:
   ```bash
   cd sales_conversions
   ```

You can now start browsing files and exploring data locally on your machine.
   
---
## Usage

Navigate to and open the [Jupyter Notebook](conversions.ipynb) files to view detailed analysis, code, and visualizations.