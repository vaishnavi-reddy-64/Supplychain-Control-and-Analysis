### 📌 Project Overview
This repository contains the front-end analytical architecture for a global supply chain monitoring system, specifically focusing on the Japan-to-India transit corridor. 

The primary objective of this phase was to engineer realistic logistics data and develop an interactive Business Intelligence dashboard to track operational bottlenecks, measure carrier efficiency, and calculate the financial impact of transit delays. This tool transitions logistics monitoring from a reactive process into a proactive, decision-driving operational control center.

*(Note: Phase 2 of this project will integrate a decentralized blockchain ledger to ensure the immutability and transparency of this transit data.)*
---

### 🖥️ Dashboard Interface

<img width="1167" height="662" alt="supplychain dashboard SC" src="https://github.com/user-attachments/assets/71e5c961-3c6d-4adb-9132-83950bd70795" />

---
### 📈 Phase 1: Descriptive Analytics (Surface-Level Insights)
*These insights were derived directly from the high-level KPI indicators and individual visuals to establish a baseline of current operational health.*

* **Critical Delay Rate:** The network is currently operating with a **49.33%** overall delay rate across all shipments, indicating a severe systemic logistics issue.
* **Geographic Distribution:** Freight volume is heavily concentrated toward two primary Indian destinations: Bengaluru Hub and Chennai Port. 
* **Carrier Reliance:** The logistics network relies predominantly on Sea Freight and Express Road, with minimal utilization of standard rail or air cargo networks.
* **Financial Impact:** The total calculated financial shrinkage due to prolonged transit times and lost inventory exceeds ₹7.65 Billion across the tracked period.

---

### 🔍 Phase 2: Diagnostic Analytics (Cross-Visual Bottleneck Analysis)
*By cross-filtering the geographic maps with specific carrier types and product loss tables, the following root causes for the 49% delay rate were identified:*

#### 1. The "Billion Rupee" Bottlenecks (High-Risk Routes)
Three specific routes are severely underperforming, each crossing the critical threshold of ₹1 Billion in transit-related losses due to chronic delays:
* **Osaka to Bengaluru:** Highest financial loss at **₹1.07bn**, operating with a 19.00% delay rate and averaging over 10 transit days.
* **Nagoya to Chennai:** Highest overall delay rate at **21.14%**, resulting in **₹1.06bn** in losses.
* **Tokyo to Bengaluru:** Yielding a 20.90% delay rate and **₹1.04bn** in losses.
* *The Root Cause:* Cross-referencing these routes reveals they all rely predominantly on **Sea Freight**.

#### 2. Carrier Efficiency: Sea Freight vs. Express Road
The data definitively proves that heavy reliance on Sea Freight directly inflates both transit time and financial loss across this corridor.
* Routes utilizing **Express Road** networks (such as Yokohama to Chennai and Tokyo to Chennai) successfully keep average transit times strictly under 9.8 days.
* **The Yokohama Efficiency:** The Yokohama Port to Bengaluru route is the most efficient corridor in the network. Despite moving heavy volume, it maintains the lowest delay rate (**16.07%**) and the lowest overall financial loss (**₹797.65M**).

#### 3. Q3/Q4 Seasonal Congestion
Trend line analysis across all origins reveals a severe, recurring operational bottleneck between **October and January**. The Tokyo to Bengaluru route experiences its most aggressive delay spike during this specific window, indicating chronic winter port congestion at the Japanese origin locations.

---

### 💡 Strategic Recommendations & Action Plan

To stabilize the transit network and mitigate financial loss, the following operational adjustments are proposed based on the diagnostic data:

1. **Reallocate Freight Volume:** Shift a minimum of 15% of high-priority shipment volume away from the Osaka and Tokyo ports. Reroute this volume through the highly efficient **Yokohama Port**, which demonstrates the most stable transit times to the Bengaluru hub.
2. **Prioritize Express Road for Chennai:** Sea Freight to Chennai is statistically unviable for time-sensitive goods. Operations must prioritize Express Road carriers for the Tokyo-to-Chennai corridor to capitalize on established sub-10-day transit times.
3. **Pre-Emptive Q4 Routing:** Implement a predictive routing model for the October–January risk window. Before the October spikes occur, critical inventory must be shifted to Air Cargo to avoid chronic winter maritime congestion.

---

### 🛠️ Technical Stack
* **Data Engineering:** Python (`Faker`, `Pandas`) to build weighted, synthetic logistics datasets.
* **Data Visualization & BI:** Microsoft Power BI.
* **Metrics & Calculations:** DAX (Data Analysis Expressions) for custom delay duration and financial loss modeling.


