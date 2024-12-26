# TCS-Stock-Analysis-Power-BI-Dashboard
   ![](https://github.com/Anuj-data/TCS-Stock-Analysis-Power-BI-Dashboard/blob/main/Tata_Consultancy_Services_Logo.svgkl.png)

## Project Overview
This project involves creating a professional Power BI dashboard to analyze and visualize the stock performance of Tata. The dataset includes stock market details such as open, high, low, close, adjusted close prices, and volume. Using DAX queries, additional insights like day, month, year, and quarter were extracted to enhance the analysis. The dashboard captures the stock's movement over different time frames, offering valuable insights for financial decision-making.

## Features
- **Dynamic Time Filters**: Analyze stock performance by day, month, year, or quarter.
- **Key Metrics**: Track daily high, low, opening, closing prices, and trading volume.
- **Intuitive Visualizations**: Interactive charts and graphs to visualize stock trends.
- **Custom DAX Queries**: Added columns for granular time-based analysis.

## Dataset Description
| Column Name      | Description                                   |
|------------------|-----------------------------------------------|
| `Date`           | The trading date                             |
| `Tata Open`      | Opening price of Tata stocks                 |
| `Tata High`      | Highest price during the trading session     |
| `Tata Low`       | Lowest price during the trading session      |
| `Tata Close`     | Closing price of Tata stocks                 |
| `Tata Adj Close` | Adjusted closing price                       |
| `Tata Volume`    | Number of stocks traded                      |

## DAX Formulas
Here are the DAX formulas used to derive new columns from the `Date` field:

1. **Day**:
   ```DAX
   Day = DAY('TCS.NS'[Date])
   ```

2. **Month**:
   ```DAX
   Month = MONTH('TCS.NS'[Date])
   ```

3. **Year**:
   ```DAX
   Year = YEAR('TCS.NS'[Date])
   ```

4. **Quarter**:
   ```DAX
   Quarter = "Q" & ROUNDUP(MONTH('TCS.NS'[Date]) / 3, 0)
   ```

## Tools & Technologies Used
- **Power BI**: For data visualization and dashboard creation.
- **DAX (Data Analysis Expressions)**: To create custom time-based columns and measures.
- **GitHub**: For project version control and sharing.

## Key Learnings
1. Leveraged DAX to derive new insights by creating additional columns (`Day`, `Month`, `Year`, `Quarter`) from the `Date` field.
2. Gained proficiency in designing interactive dashboards for financial data analysis.
3. Enhanced skills in communicating data stories effectively using Power BI.

## Dashboard Preview
 ![](https://github.com/Anuj-data/TCS-Stock-Analysis-Power-BI-Dashboard/blob/main/TCS%20Stock%20Analysis.jpg)

## How to Access the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Anuj-data/Tata-Stock-Analysis-Dashboard.git
   ```
2. Open the Power BI file (`TCS.NS.pbix`) using Power BI Desktop.
3. Explore the dataset and interact with the visualizations.

## Repository Structure
```
Tata-Stock-Analysis-Dashboard/
├── Dataset/                # Contains the dataset file used in the project
├── TCS.NS.pbix             # Power BI file for the dashboard
├── README.md               # Project documentation
```

## Future Enhancements
- Integrate live stock market data for real-time analysis.
- Expand the analysis to include other key stocks in the market.
- Add predictive analytics using Python and machine learning.

## Contact
Feel free to connect with me for any queries or collaboration opportunities:
- **Email**: anuj.negi.54@gmail.com
- **LinkedIn**: [Anuj Negi](https://linkedin.com/in/anuj-negi-8a032830b)
- **GitHub**: [Anuj-data](https://github.com/Anuj-data)

---
Let me know if you have more Power BI-related questions! 😊

