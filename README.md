Supply Chain Procurement & Logistics Analytics

📊 Project Overview
This project features an end-to-end Power BI report and data model built for a logistics-sector client. It unifies scattered operational datasets—such as purchase orders, supplier assessments, carrier metrics, warehouse logs, and monthly financial targets—into a single, decision-ready analytics dashboard

---

🛠️ Data Architecture & Schema
- **Schema Type:** Galaxy Schema (Multi-Fact Star Schema)
- **Primary Fact Tables:**
  - `Fact_procurement`: Captures transactional PO line data, actual spend, unit prices, and freight costs.
  - `Fact_Procurement_Target`: Captures planned monthly budgets by product category.
- **Conformed Dimensions:** `Dim_supplier`, `Dim_product`, `Dim_Buyer_Master`, `Dim_Warehouse_Master`, `Diim_Carrier_Master`, `Dim_category`, and `Dim_date`

---

📈 Key Dashboard Pages & Objectives

1. **Page 1: Overview (Executive Summary)**
   - Tracks actual vs. target spend, order volumes, delivery health, supplier risk distribution, and delay root causes
2. **Page 2: Supplier & Procurement**
   - Focuses on pricing control, Purchase Price Variance (PPV %), supplier quality/delivery scores, and risk profiling
3. **Page 3: Logistics & Delivery**
   - Analyzes freight cost distribution, transport modes (Road, Rail, Air), carrier SLA adherence, and transit times

---

🔑 Core KPIs Defined
- **Actual Spend:** `Actual Unit Price × Ordered Qty`
- **Spend Variance:** `Target Spend − Actual Spend`
- **PPV %:** `(Actual Spend − Contract Spend) ÷ Contract Spend`
- **OTD %:** On-time delivered shipments ÷ Total delivered shipments
- **Rejection Rate %:** Rejected quantity ÷ Received quantity

---

🚀 Repository Structure

├── Data/         Raw or sample datasets (.xlsx / CSV)
├── Model/        Power BI report file (.pbix)
├── Docs/         Architecture diagrams and presentations
└── README.md     Project documentation
