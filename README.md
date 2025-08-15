# Amazon Sales Performance Dashboard - Excel & Power BI

## 📦 Key Insights
- $8.7M annual sales (34% YoY growth in Electronics)  
- Prime members spent 2.3x more than non-Prime customers  
- Q4 holiday surge accounted for 41% of annual revenue  
- Top 5 products generated 28% of total sales  

## 🛠️ How I Built It  

### Excel Backbone  
- Cleaned 12K+ rows of messy marketplace data:  
  - Standardized SKUs (e.g., "AMZ-2023" → "AMZ2023")  
  - Corrected 1,200+ regional tax discrepancies  
- Created dynamic dashboards with:  
  - Slicers for category/membership tier  
  - Conditional formatting for AOV tiers  

### Power BI Upgrade  
- Built real-time sales tracker connecting to Amazon Seller Central  
- Developed geo-map showing regional demand hotspots  
- Automated weekly performance reports with DAX measures:  
  ```DAX
  YoY Growth = 
  DIVIDE(
      [Total Sales] - [Prior Year Sales],
      [Prior Year Sales]
  )
