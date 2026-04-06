# 🛒 Blinkit Sales Analytics Dashboard — Power BI

> **India's Last Minute App** — A comprehensive Power BI dashboard analyzing Blinkit's outlet performance, sales trends, item types, and customer ratings across multiple store tiers and locations.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-2012--2022-orange?style=for-the-badge)

---

## 📊 Dashboard Preview

![Blinkit Power BI Dashboard](./assets/dashboard-preview.png)

---

## 📌 Project Overview

This Power BI dashboard provides end-to-end visual analytics for **Blinkit** — India's rapid grocery delivery platform. It enables business stakeholders to monitor sales performance, outlet efficiency, item-level insights, and customer satisfaction metrics at a glance.

### 🎯 Key Metrics

| Metric | Value |
|:---|:---:|
| 💰 Total Sales | **$1.20M** |
| 📦 Avg Sales per Outlet | **$141** |
| ⭐ Avg Customer Rating | **3.9** |
| 🏪 Total No. of Items | **8,523** |

---

## ✨ Features

- **Dynamic Filter Panel** — Filter by Outlet Size, Outlet Location Type, and Item Type
- **Fat Content Analysis** — Donut chart: Low Fat (`$776.32K`) vs Regular (`$425.36K`)
- **Item Type Breakdown** — Bar chart ranking 16+ categories by revenue contribution
- **Fat by Outlet Tier** — Stacked bar segmenting fat content across Tier 1, 2, and 3
- **Outlet Establishment Trend** — Line chart tracking growth from **2012 to 2022**
- **Outlet Size Distribution** — Medium / Small / High outlet proportions
- **Outlet Location Performance** — Tier 3 (`$472.13K`) · Tier 2 (`$393.15K`) · Tier 1 (`$336.40K`)
- **Outlet Type Summary Table** — Sales, Items, Avg Sales, Rating & Visibility per outlet type

---

## 🗂️ Repository Structure

```
blinkit-powerbi-dashboard/
│
├── 📁 assets/
│   └── dashboard-preview.png        # Dashboard screenshot
│
├── 📁 data/
│   └── blinkit_sales_data.xlsx      # Raw/cleaned source dataset
│
├── 📁 report/
│   └── Blinkit_Dashboard.pbix       # Power BI report file
│
├── 📁 docs/
│   └── data_dictionary.md           # Field descriptions and data types
│
└── README.md                        # Project documentation (this file)
```

---

## 📈 Dashboard Sections Explained

### 1️⃣ KPI Summary Cards
Top-level metric cards — Total Sales, Avg Sales, Avg Rating, No. of Items — updated dynamically based on active filter selections.

### 2️⃣ Fat Content Analysis
- **Donut Chart** — Total sales split: Low Fat vs Regular
- **Stacked Bar** — Fat content breakdown across outlet tiers

### 3️⃣ Item Type Performance
Horizontal bar chart ranking 16 categories including Fruits & Vegetables, Snack Foods, Household, Frozen Foods, Dairy, Canned, Baking Goods, Health & Hygiene, Meat, Soft Drinks, Breads, and more.

### 4️⃣ Outlet Establishment Timeline
Area/line chart spanning **2012–2022**, revealing expansion peaks and slowdowns across a decade.

### 5️⃣ Outlet Size & Location
- **Outlet Size Donut** — Medium (`$507.90K`) · Small (`$444.79K`) · High (`$248.99K`)
- **Location Bar Chart** — Tier 3 (`$472.13K`) · Tier 2 (`$393.15K`) · Tier 1 (`$336.40K`)

### 6️⃣ Outlet Type Summary Table

| Outlet Type | Total Sales | No. of Items | Avg Sales | Avg Rating | Item Visibility |
|:---|---:|---:|:---:|:---:|:---:|
| Grocery Store | $151.94K | 1,083 | $140 | 4 | 0.10 |
| Supermarket Type1 | $787.55K | 5,577 | $141 | 4 | 0.06 |
| Supermarket Type2 | $131.48K | 928 | $142 | 4 | 0.06 |
| Supermarket Type3 | $130.71K | 935 | $140 | 4 | 0.06 |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|:---|:---|
| **Microsoft Power BI Desktop** | Report creation & visualization |
| **DAX (Data Analysis Expressions)** | Custom measures & KPIs |
| **Power Query (M Language)** | Data transformation & cleaning |
| **Microsoft Excel / CSV** | Data source |

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) — free download
- Microsoft Excel — for viewing source data

### Steps to Run

**1. Clone this repository**
```bash
git clone https://github.com/your-username/blinkit-powerbi-dashboard.git
cd blinkit-powerbi-dashboard
```

**2. Open the Power BI report**
- Launch **Power BI Desktop**
- Navigate to `File → Open report`
- Select `report/Blinkit_Dashboard.pbix`

**3. Refresh data *(optional)***
- Go to `Home → Refresh`
- Ensure the data source path points to `data/blinkit_sales_data.xlsx`

---

## 📐 DAX Measures Used

```dax
-- Total revenue across all outlets
Total Sales = SUM(Sales[SalesAmount])

-- Per-record average revenue
Avg Sales = AVERAGE(Sales[SalesAmount])

-- Customer satisfaction score
Avg Rating = AVERAGE(Outlets[CustomerRating])

-- Unique product count
No of Items = DISTINCTCOUNT(Items[ItemID])
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. **Fork** the repository
2. **Create** a branch: `git checkout -b feature/your-feature-name`
3. **Commit** your changes: `git commit -m "Add: your feature description"`
4. **Push** to the branch: `git push origin feature/your-feature-name`
5. **Open** a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Your Name**
- 🐙 GitHub: [@your-username](https://github.com/your-username)
- 💼 LinkedIn: [your-linkedin](https://linkedin.com/in/your-profile)

---

<div align="center">

⭐ **If you found this project helpful, please give it a star on GitHub!** ⭐

*Built with ❤️ using Power BI | Data Analytics | Business Intelligence*

</div>
