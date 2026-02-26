# Telco Customer Churn Analysis

Interactive Power BI dashboard analyzing customer churn behavior and key business insights using the Telco Customer Churn dataset.

---

## Project Overview

This project analyzes customer churn behavior and presents insights through an interactive Power BI dashboard.

The objective is to identify patterns contributing to customer attrition and evaluate the financial impact of churn. The dashboard supports data-driven retention strategies and business decision-making.

---

## Business Objectives

- Measure overall customer churn rate  
- Identify customer segments with high churn probability  
- Analyze churn trends by contract type  
- Evaluate churn behavior across tenure groups  
- Examine churn distribution by internet service type  
- Estimate total revenue loss due to churn  

---

## Dashboard Preview

<img width="891" height="465" alt="image" src="https://github.com/user-attachments/assets/bfacf222-e017-4e33-b52e-566ae58af07b" />


---

## Key Insights

- **Overall churn rate:** 26.54%  
- Month-to-month contract customers show the highest churn rate  
- Customers within their first year are more likely to churn  
- Fiber optic users have relatively higher churn compared to DSL users  
- **Estimated revenue loss due to churn:** 139.13K  

---

## Technical Implementation

- Power BI for interactive data visualization  
- DAX (Data Analysis Expressions) for calculated measures  
- Data cleaning and transformation  
- Data modeling and relationship management  
- Interactive slicers for dynamic filtering  

---

## Sample DAX Measure

```DAX
Churn Rate % =
DIVIDE(
    CALCULATE(COUNT(Telco[customerID]), Telco[Churn] = "Yes"),
    COUNT(Telco[customerID])
)
```

---

## Repository Structure

- `Telco_Churn_Dashboard.pbix` – Power BI dashboard file  
- `dashboard_preview.png` – Dashboard screenshot  
- `README.md` – Project documentation  
- `LICENSE` – MIT License  

---

## Dataset Source

Telco Customer Churn Dataset – Kaggle

---

## Conclusion

The analysis highlights contract structure and early customer lifecycle stages as primary churn drivers.

These insights can help organizations design targeted retention strategies, improve onboarding processes, and reduce revenue loss due to customer attrition.
