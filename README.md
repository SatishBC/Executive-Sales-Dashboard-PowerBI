# 📊 Executive Sales Performance Dashboard | Power BI & DAX

## 🚀 Project Overview
This project delivers a high-impact **Executive Sales Performance Dashboard** designed to reduce "Time-to-Insight" for senior leadership. It identifies store-level performance gaps in seconds using automated auditing and dynamic visual intelligence.

## 🖼️ Dashboard Preview
![Main Dashboard](Media/Screenshot%202026-02-24%20182849.png)

## 🏗️ Data Architecture (Star Schema)
The model is built on a **Star Schema** to ensure optimal performance and filter propagation:
* **Fact Table:** `fact_sales` (10,000+ records)
* **Dimension Tables:** `dim_products`, `dim_stores`, `dim_customers`, `dim_promotions`, and a custom `DateTable`.

![Data Model](Media/Screenshot%202026-02-26%20105121.png)

## 🧠 Technical Deep-Dive (DAX & Logic)
* **Dynamic Titles:** Used `SELECTEDVALUE` and `CONCATENATEX` to create context-aware headers that update based on slicer selections.
* **Performance Auditing:** Engineered a conditional flagging system to identify stores falling below the **19.5% profit threshold**.
* **Time Intelligence:** Developed MoM (Month-over-Month) growth measures using `CALCULATE` and `DATEADD`.

## 🎨 UI/UX Features
* **Modern Interface:** 10px rounded containers with a high-contrast, professional "Apple-esque" aesthetic.
* **Consistent Scaling:** All financial metrics normalized to **Millions (M)** for executive readability.

## 📁 Repository Structure
* `/Dataset`: Raw CSV business data.
* `/Dashboard`: The `.pbix` Power BI source file.
* `/Media`: High-resolution screenshots of the UI and Data Model.
