# 📊 Profit Analysis and Power BI Dashboard

## 🧾 Project Overview
This project analyzes how **Research & Development (R&D)**, **Administration**, and **Marketing** expenditures impact company profit.  
Using **Multiple Linear Regression** and **Power BI**, the project provides both **statistical insights** and **interactive dashboards** to help management make data-driven investment decisions.

---

## 🎯 Objective
- To determine which spending categories most influence profit.
- To develop a **regression model** predicting profit based on spending.
- To create an **interactive Power BI dashboard** for executive decision-making.

---

## 🧮 Methodology

### 1. **Data Preparation**
- Loaded and cleaned the dataset in **Excel**.  
- Verified for missing values and ensured consistent numeric formatting.  

### 2. **Regression Analysis**
- Conducted **Multiple Linear Regression** using Excel Data Analysis Toolpak.  
- Dependent Variable: `Profit`  
- Independent Variables: `R&D Spend`, `Administration`, `Marketing Spend`  

**Regression Equation:**
Profit = 49000 + 0.805(R&D Spend) - 0.0268(Administration) + 0.0272(Marketing Spend)

**Model Summary:**
| Metric | Value | Interpretation |
|:--|:--|:--|
| Multiple R | 0.975 | Strong correlation |
| R² | 0.9507 | 95% of profit variation explained |
| Adjusted R² | 0.9475 | High model accuracy |
| Significance F | 4.53E-30 | Statistically significant model |

---

## 💡 Key Findings
1. **R&D Investment** has the strongest and most significant impact on profit.  
2. **Administration Costs** have minimal or slightly negative impact.  
3. **Marketing Spend** contributes positively, but less strongly than R&D.  
4. The regression model explains **95% of profit variation**, confirming its accuracy.

---

## 🧭 Power BI Dashboard

### 📘 Dashboard Title:
**“Profit Drivers and Spend Efficiency Dashboard”**

### 📊 Dashboard Sections

| **Section** | **Visual Type** | **Description** | **Key Insight** |
|--------------|----------------|-----------------|-----------------|
| **KPI Summary** | Card Visuals | Displays key performance metrics (Total Profit, Total Spend, R&D ROI, Marketing ROI) | Snapshot of financial performance |
| **Sum of Administration** | Gauge / Donut Chart | Visualizes total admin spend vs target | Highlights overhead levels |
| **Profit by Marketing Spend** | Line Chart | Shows correlation between Marketing Spend and Profit | Profit increases with marketing investment |
| **Admin Overhead Ratio by State** | Horizontal Bar | Compares administrative cost ratios | California shows highest overhead |
| **Total Marketing Spend by State** | Donut Chart | Percentage contribution by state | Florida leads in marketing spend |
| **Total Profit by State** | Pie Chart | Profit share by region | New York contributes most profit |
| **R&D Spend vs Profit** | Line Chart | R&D spend plotted against profit | Higher R&D → higher profit |

---

## 🧮 DAX Measures Used

| **Measure** | **Formula** | **Purpose** |
|--------------|-------------|--------------|
| Total Profit | `= SUM('Data'[Profit])` | Total company profit |
| Total R&D Spend | `= SUM('Data'[R&D_Spend])` | Total R&D expenditure |
| Total Marketing Spend | `= SUM('Data'[Marketing_Spend])` | Marketing investment |
| Total Admin Spend | `= SUM('Data'[Administration])` | Administrative expenses |
| Total Spend | `= [Total R&D Spend] + [Total Marketing Spend] + [Total Admin Spend]` | Combined spending |
| Marketing ROI | `= DIVIDE([Total Profit], [Total Marketing Spend])` | Marketing efficiency |
| R&D ROI | `= DIVIDE([Total Profit], [Total R&D Spend])` | R&D efficiency |

---

## 📈 Insights and Recommendations
- 💰 **Increase R&D investment** — strongest profit driver.
- 🏢 **Control administrative costs** — minimal impact on profit.
- 📣 **Optimize marketing ROI** — contributes moderately but efficiently.
- 🔁 **Regularly update the model** as new data becomes available.
- 🧩 **Use Power BI** for continuous, interactive decision-making.

---

## 🧰 Tools and Technologies
- **Microsoft Excel** – Data cleaning and regression analysis  
- **Power BI** – Dashboard creation and visualization  
- **DAX** – Calculated measures for KPIs and ratios  
- **GitHub** – Version control and project documentation  

---

## 📂 Project Files
| File | Description |
|:--|:--|
| `project excel.csv` | Dataset used for regression and dashboard |
| `newproj.pbix` | Power BI dashboard file |
| `PROJECT DOCUMENTATION.docx` | Detailed project documentation |
| `Project PPT[1].pptx` | Presentation summarizing findings |
| `README.md` | Project overview and usage guide |

---

## 🚀 How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/profit-analysis-dashboard.git
2. Open the project excel.csv in Excel for reference.
3. Open the newproj.pbix file in Power BI Desktop.
4. Refresh data or modify visuals as needed.
5. Explore insights interactively through filters and visuals.

🏁 **Conclusion**

This project demonstrates how data analysis and visualization can provide actionable business insights.
By integrating regression modeling and Power BI dashboards, the company can make smarter investment decisions, track profit trends, and continuously optimize its operations.
