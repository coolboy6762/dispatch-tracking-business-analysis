# dispatch-tracking-business-analysis
End-to-end Business Analyst project for a Dispatch Tracking &amp; Reporting System, covering BRD, business requirements, AS-IS process analysis, KPI definition, Excel data preparation, Power BI dashboard development, DAX, UAT, and business insights.
# Dispatch Tracking & Reporting System

## 📌 Project Overview

The **Dispatch Tracking & Reporting System** is an end-to-end Business Analysis and Power BI project developed for a granite manufacturing and sales business.

The project focuses on replacing manual spreadsheet-based dispatch tracking with a centralized reporting solution that provides better visibility into order status, dispatch performance, delays, locations, products, and priorities.

## 🎯 Business Problem

Dispatch information was maintained across multiple spreadsheets, which resulted in:

- Delayed status updates
- Poor visibility of order status
- Difficulty identifying delayed orders
- Manual reporting effort
- Difficulty analyzing delay reasons
- Limited visibility into location and product-level performance

## 🎯 Business Objectives

- Centralize dispatch information
- Monitor order status
- Identify delayed and pending orders
- Analyze dispatch performance
- Identify major delay reasons
- Track orders by location, product, and priority
- Reduce manual reporting effort
- Provide management with an interactive dashboard

## 👥 Stakeholders

- Sales Team
- Logistics Team
- Dispatch Team
- Operations Team
- Management
- Business Analyst
- Power BI Developer

## 🔄 AS-IS Process

```text
Customer Order
      ↓
Sales Team Records Order
      ↓
Manual Spreadsheet Update
      ↓
Dispatch Team Updates Status
      ↓
Multiple Spreadsheet Files
      ↓
Manual Report Preparation
      ↓
Management Review
```

## 💡 Proposed Solution

A centralized Power BI reporting solution was designed to provide:

```text
Dispatch Data
      ↓
Excel Data Preparation
      ↓
Power Query
      ↓
Data Model
      ↓
DAX Measures
      ↓
Power BI Dashboard
      ↓
Business Insights
```

## 📊 Key KPIs

- Total Orders
- Total Quantity
- Dispatched Orders
- Pending Orders
- Delayed Orders
- Dispatch Rate
- Delay Rate
- Average Delay Days
- Maximum Delay

## 📈 Dashboard Pages

### 1. Dispatch Overview

Includes:

- Total Orders
- Dispatched Orders
- Pending Orders
- Delayed Orders
- Monthly Dispatch Trend
- Dispatch Status
- Orders by Location
- Orders by Product
- Orders by Priority

### 2. Delay Analysis

Includes:

- Delayed Orders
- Delay Rate
- Average Delay Days
- Maximum Delay
- Delay Reasons
- Delayed Orders by Location
- Delayed Orders by Product

### 3. Order Monitoring

Provides order-level details including:

- Order ID
- Customer
- Location
- Product
- Quantity
- Priority
- Order Date
- Expected Dispatch Date
- Actual Dispatch Date
- Dispatch Status
- Delay Days
- Delay Reason

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Excel | Data preparation and validation |
| Power Query | Data cleaning and transformation |
| Power BI | Dashboard and visualization |
| DAX | KPI calculations and business logic |
| Business Analysis | Requirements, process analysis and UAT |
| GitHub | Project documentation and portfolio |

## 📋 Business Requirements

- BR01 – Monitor current order status
- BR02 – Identify delayed dispatches
- BR03 – Analyze delay reasons
- BR04 – Track monthly dispatch trends
- BR05 – Analyze orders by location
- BR06 – Analyze orders by product
- BR07 – Analyze orders by priority
- BR08 – Provide interactive dashboard filters
- BR09 – Provide order-level operational details

## 🧮 Key DAX Measures

```DAX
Total Orders =
DISTINCTCOUNT(DispatchData[Order_ID])
```

```DAX
Dispatched Orders =
CALCULATE(
    [Total Orders],
    DispatchData[Dispatch_Status] = "Dispatched"
)
```

```DAX
Pending Orders =
CALCULATE(
    [Total Orders],
    DispatchData[Dispatch_Status] = "Pending"
)
```

```DAX
Delayed Orders =
CALCULATE(
    [Total Orders],
    DispatchData[Dispatch_Status] = "Delayed"
)
```

```DAX
Dispatch Rate =
DIVIDE(
    [Dispatched Orders],
    [Total Orders],
    0
)
```

```DAX
Delay Rate =
DIVIDE(
    [Delayed Orders],
    [Total Orders],
    0
)
```

## 🧪 UAT Testing

Example UAT scenarios:

| Test Case | Expected Result |
|---|---|
| Dashboard loads | Dashboard displays correctly |
| Total Orders | Matches unique Order IDs |
| Location filter | All visuals update |
| Priority filter | All visuals update |
| Delayed status filter | Only delayed orders displayed |
| Delay Rate | Correct percentage calculated |
| Date filter | Trends update correctly |
| Order details | Correct order-level information displayed |

## 📁 Project Structure

```text
dispatch-tracking-business-analysis/
│
├── README.md
│
├── BRD/
│   └── Dispatch_Tracking_BRD_Complete_Report.docx
│
├── Data/
│   └── Dispatch_Tracking_1000_Rows.xlsx
│
├── PowerBI/
│   └── Dispatch_Tracking_Dashboard.pbix
│
├── Documentation/
│   ├── AS-IS_Process.png
│   ├── Business_Requirements.xlsx
│   └── UAT_Test_Cases.xlsx
│
└── Screenshots/
    ├── dashboard_overview.png
    ├── delay_analysis.png
    └── order_monitoring.png
```

## 📌 Business Analysis Deliverables

- Business Problem Definition
- Project Objectives
- Stakeholder Identification
- AS-IS Process
- Business Requirements
- Business Rules
- KPI Definition
- Data Requirements
- Power BI Dashboard
- DAX Measures
- UAT Test Cases
- Business Insights
- Recommendations

## 🚀 Future Enhancements

- ERP/database integration
- Automated data refresh
- Real-time dispatch tracking
- GPS integration
- Automated delay alerts
- Inventory integration
- Production capacity analysis
- Role-based dashboards

## 👨‍💻 Project Type

**Business Analyst Portfolio Project**

**Domain:** Manufacturing & Logistics  
**Tools:** Excel, Power BI, Power Query, DAX, GitHub  
**Focus:** Business Analysis, Operations Analytics, KPI Reporting & Dashboard Development
<img width="891" height="495" alt="image" src="https://github.com/user-attachments/assets/aebbe2f5-8b2e-49f7-8089-eb0aeb07df4d" />
<img width="891" height="495" alt="image" src="https://github.com/user-attachments/assets/dd9b154c-bd66-4046-82ee-77295c806374" />
<img width="875" height="503" alt="image" src="https://github.com/user-attachments/assets/c444e2b9-d8d0-4720-93b5-051935fa92ae" />


