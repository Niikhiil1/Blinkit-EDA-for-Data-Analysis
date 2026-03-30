# Blinkit-EDA-for-Data-Analysis

# 🛒 Blinkit Sales Data — Exploratory Data Analysis (EDA)

An end-to-end Exploratory Data Analysis on Blinkit's sales data using Python. This project covers data cleaning, KPI calculation, and visual analysis to uncover actionable business insights.

---

## 📌 Project Overview

Blinkit (formerly Grofers) is one of India's leading quick-commerce platforms. This project dives into their sales data to understand product performance, outlet behaviour, and customer preferences.

---

## 📁 Project Structure

```
├── Blinkit_Sales_EDA.ipynb    # Main Jupyter Notebook
└── blinkit_data.csv           # Raw dataset
```

---

## 🔍 What's Inside the Notebook

### 1. 📥 Data Import & Exploration
- Loaded dataset using `pandas`
- Explored shape, columns, data types using `.shape`, `.columns`, `.dtypes`
- Previewed data using `.head()` and `.tail()`

### 2. 🧹 Data Cleaning
- Identified inconsistent labels in the `Item Fat Content` column
- Standardized values:

| Before | After |
|--------|-------|
| `low fat` | `Low Fat` |
| `LF` | `Low Fat` |
| `reg` | `Regular` |

### 3. 📊 KPI Calculation

| KPI | Method |
|-----|--------|
| Total Sales | `df['Sales'].sum()` |
| Average Sales | `df['Sales'].mean()` |
| Number of Items Sold | `df['Sales'].count()` |
| Average Rating | `df['Rating'].mean()` |

### 4. 📈 Visual Analysis

| Chart | Type | Insight |
|-------|------|---------|
| Sales by Fat Content | Pie Chart | Regular vs Low Fat sales share |
| Total Sales by Item Type | Bar Chart | Top revenue-generating product categories |
| Fat Content by Outlet Location Tier | Grouped Bar Chart | Sales breakdown by tier and fat content |
| Sales by Outlet Size | Pie Chart | Revenue contribution by outlet size |

---

## 💡 Key Findings

- **Regular fat content** items outsell low-fat items across all outlet tiers
- **Certain item types** (e.g., fruits & vegetables, snack foods) dominate total revenue
- **Tier 3 outlets** show strong sales performance despite lower visibility
- **Medium-sized outlets** contribute the most to overall sales

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, and aggregation |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `seaborn` | Statistical plotting |

---

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Place `blinkit_data.csv` in the same directory as the notebook
4. Open `Blinkit_Sales_EDA.ipynb` in Jupyter Notebook or VS Code
5. Run all cells top to bottom

---

## 📌 Dataset Columns

| Column | Description |
|--------|-------------|
| `Item Fat Content` | Fat content category (Low Fat / Regular) |
| `Item Type` | Category of product |
| `Sales` | Sales amount for the item |
| `Rating` | Customer rating |
| `Outlet Size` | Size of the outlet (Small / Medium / Large) |
| `Outlet Location Type` | Location tier (Tier 1 / Tier 2 / Tier 3) |

---

## 👨‍💻 Author

**Nikhil Dubey**  
📧 nikhildubey17033@gmail.com

---

## 📌 Status

✅ Complete — EDA finished with KPIs and 4 visualizations.  
🔜 Next step: Dashboard using Power BI or Tableau.

---

*If you found this helpful, consider ⭐ starring the repository!*
