# Supply Chain Procurement & Logistics Analytics

## 📊 Project Overview
This project features an end-to-end Power BI report and data model built for a logistics-sector client. It unifies scattered operational datasets—such as purchase orders, supplier assessments, carrier metrics, warehouse logs, and monthly financial targets—into a single, decision-ready analytics dashboard[cite: 3].

---

## 🛠️ Data Architecture & Schema
- **Schema Type:** Galaxy Schema (Multi-Fact Star Schema)
- **Primary Fact Tables:**
  - `Fact_procurement`: Captures transactional PO line data, actual spend, unit prices, and freight costs[cite: 1, 3].
  - `Fact_Procurement_Target`: Captures planned monthly budgets by product category[cite: 1, 3].
- **Conformed Dimensions:** `Dim_supplier`, `Dim_product`, `Dim_Buyer_Master`, `Dim_Warehouse_Master`, `Diim_Carrier_Master`, `Dim_category`, and `Dim_date`[cite: 1, 3].

---

## 📈 Key Dashboard Pages & Objectives

1. **Page 1: Overview (Executive Summary)**
   - Tracks actual vs. target spend, order volumes, delivery health, supplier risk distribution, and delay root causes[cite: 3].
2. **Page 2: Supplier & Procurement**
   - Focuses on pricing control, Purchase Price Variance (PPV %), supplier quality/delivery scores, and risk profiling[cite: 3].
3. **Page 3: Logistics & Delivery**
   - Analyzes freight cost distribution, transport modes (Road, Rail, Air), carrier SLA adherence, and transit times[cite: 3].

---

## 🔑 Core KPIs Defined
- **Actual Spend:** `Actual Unit Price × Ordered Qty`[cite: 3]
- **Spend Variance:** `Target Spend − Actual Spend`[cite: 3]
- **PPV %:** `(Actual Spend − Contract Spend) ÷ Contract Spend`[cite: 3]
- **OTD %:** On-time delivered shipments ÷ Total delivered shipments[cite: 3]
- **Rejection Rate %:** Rejected quantity ÷ Received quantity[cite: 3]

---

## 🚀 Repository Structure
```text
├── Data/                   # Raw or sample datasets (.xlsx / CSV)
├── Model/                  # Power BI report file (.pbix)
├── Docs/                   # Architecture diagrams and presentations
└── README.md               # Project documentation
