
# 📊 Customer Satisfaction Insights – Global Dashboard

This project provides a high-level analysis of customer satisfaction trends across five countries using aggregated data. While the underlying dataset is not publicly shared due to sensitivity, interactive visualizations are available through Looker Studio.

🔗 [View the Looker Studio Report](https://lookerstudio.google.com/reporting/ae633f3f-8628-4cc3-a12a-eb24f2621c12)

---

## 🧹 Data Preparation

All data cleaning and preprocessing were performed using **Python**, focusing on:
- Handling missing values and outliers
- Standardizing formats across country-level datasets
- Calculating derived metrics like `Existing Customers Average Score`
- Aggregating and reshaping data for visualization in Looker Studio

---

## 📈 Key Metrics & Calculations

### Existing Customers Average Score (Column Q in the sheet):
This metric is derived using the following calculation:

```plaintext
Global_Product = Global Average Score × Global Volume  
New_Customers_Product = New Customers Average Score × New Customers Volume  
Existing Customers Average Score = (Global_Product - New_Customers_Product) / Existing Customers Volume
```

This approach isolates the impact of existing customers on the overall satisfaction scores.

---

## 🧠 Insights & Analysis

### Why didn’t the Global Average Score increase in late 2024?

While average scores rose for individual countries, the **Global Volume** increased disproportionately during the final months of 2024. Since the Global Average Score is volume-weighted, this surge in volume diluted the overall average score, masking improvements at the country level.

> **Global Average Score formula**:  
> *(Sum of Country Scores × Volume) / Global Volume*

---

### Key Contributor to Score Dip – June 2024

Despite improvements in some regions, the **UK** contributed the most to the drop in Global Average Score in June 2024 due to its significantly higher volume.

| Country | Average Score | Volume  | Weighted Contribution |
|---------|---------------|---------|------------------------|
| UK      | 6.1           | 56,595  | 345,229.5              |
| FR      | 7.6           | 7,008   | 53,260.8               |
| DE      | 8.0           | 5,405   | 43,240.0               |
| ES      | 5.2           | 8,041   | 41,813.2               |
| IT      | 2.1           | 130     | 273.0                  |

The UK's large volume had the greatest influence on the overall score drop.

---

## 🔮 2025 Forecast & Trends

### Observations (2023–2024):
- **Global Average Score** fluctuated mid-year with a consistent rebound afterward.
- **Global Volume** has been increasing, especially in Q4 of 2024.
- **New Customers Volume** shows seasonal trends, growing sharply in Q1 and Q4.
- **UK** and **FR** demonstrate stable average scores. **IT** consistently scores the lowest.

### 2025 Predictions:
1. **Global Average Score** is expected to rise slightly in early 2025, dip mid-year, and recover in Q4.
2. **Global Volume** may stabilize in the first half and rise sharply in Q4.
3. **New Customers Volume** is projected to surge in Q1 and Q4, reinforcing seasonal patterns.
4. The **UK** will likely remain the largest contributor to both volume and score impact.

---

## 📌 Conclusion

The upward trend in customer engagement, especially in Q4, is expected to continue through 2025. This suggests higher participation and more robust insights into customer satisfaction. As new customer influx increases, so does the overall score reliability—potentially driving improvements across key markets.

> 📍 *Explore the Looker Studio dashboard for alternative visuals and deeper dive analytics.*
