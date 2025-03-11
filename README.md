# Video-Game-Market-Analysis-With-Excel
An in-depth analysis of the video game market (1980–2020) using Excel, exploring sales trends and forecasting future performance. This project provides insights into factors driving game sales, helping developers and publishers refine their strategies for game development and marketing across different regions.
# Introduction
The video game industry is a thriving global market with immense potential for developers and publishers. As gaming continues to evolve across diverse platforms and audiences, understanding market trends and sales dynamics is essential for success.

This project leverages a publicly available dataset from Kaggle, featuring sales data from over 16,500 video games. With insights spanning multiple platforms, genres, and regions, the dataset provides a valuable foundation for analyzing historical trends, identifying key success factors, and shaping data-driven strategies for game development and marketing.
# Objectives
- *Market Trends Analysis*: Identify the top-performing gaming platforms and genres based on total sales to understand market preferences and long-term industry trends.  
- *Publisher Influence*: Evaluate the dominance of major publishers across different regions, identifying key players and their impact on the gaming industry.  
- *Regional Sales Insights*: Assess sales distribution and per capita sales across regions to determine where video games have the highest market penetration.  
- *Strategic Recommendations*: Provide data-driven insights for game developers and publishers to optimize market strategies and maximize sales potential.
# Dataset
The dataset consists of 11 columns and 16,598 rows, with the RANK column as the primary key. After removing 271 rows with missing values in the crucial Year and Publisher columns, the dataset is reduced to 16,327 rows.  

No extreme outliers were found. The highest sales recorded is $41.5 million in North America for Wii Sports, which is reasonable. The game was bundled with Wii consoles in many regions, contributing significantly to its sales. It also played a key role in the motion-controlled gaming boom. By 2017, it had sold over 82 million copies, making it the best-selling single-platform game of all time. This revenue figure accurately reflects real-world sales, not data entry errors.  

Conducting the analysis in Excel presents several challenges. Unlike Power BI, SQL, or Python, Excel lacks built-in table relationships, requiring all data to be consolidated in a single worksheet. Interactive dashboards depend on PivotTables, Charts, Slicers, and Filters, all of which must be linked to the same dataset. Since Excel does not support cross-sheet filtering, splitting data across multiple sheets would lead to inefficiencies and inconsistencies.  

To address these limitations, the dataset was restructured by adding a new "Region" column, consolidating regional sales values. This adjustment allows for more flexible analysis, enabling new visualizations and insights. However, it also increases the number of rows fourfold, which may impact Excel’s performance when handling large datasets.
# Processing
After completing the steps in the previous section, we obtain the following table:  

One key point to note is that the original data used to create the dashboard must be in table format. This ensures easier updates and enhances automation.  

The next steps involve creating PivotCharts by first generating PivotTables. Each PivotTable serves as an answer to a specific analytical objective. The creation of PivotCharts is also a way to automate the dashboard.  
## Key PivotTables
### 1. VideoGameReleasesByYear Table
This table is designed to analyze trends in the video game industry by tracking the number of games released and their corresponding **Total Sales** over the years.  

The recommended PivotChart for this table is a **Combo Chart**, which combines:  
- A column chart to visualize the annual growth in the number of video games released.  
- A cumulative line chart to depict the **Total Sales** growth over time.  

The cumulative **Sales** metric highlights the industry's evolution from its inception, particularly starting in 1980, and its rapid expansion in subsequent years.  

---

### 2. Top5PlatformsWithHighestSales Table  
Since there are numerous **Platforms**, displaying all of them in a single PivotChart would be overwhelming and confusing. Therefore, this table focuses on the **top five Platforms with the highest Total Sales**.  

Just as games compete with each other, **Platforms** also compete to attract **Publishers**. The **Platforms** that gain the most **Publisher** trust tend to dominate the market. A **pie chart** is the most suitable choice here, as it clearly illustrates the proportion of **Sales** attributed to each **Platform**.  

---

### 3. Top5GenresWithHighestSales Table  
Similar to the previous table, this one highlights the **top five most successful and popular Genres**, based on **Total Sales**.  

The recommended PivotChart for this table is a **column chart**, which allows for direct comparisons between different **Genres**. Based on data spanning from 1980 to 2020, the **Action** genre has consistently been the most popular.  

---

### 4. TotalSalesByRegion Table  
The data processing step includes the creation of a **Region** column, enabling a more detailed market analysis. Specifically, this table helps track the market share of the video game industry across major regions such as **North America (NA), Europe (EU), and Japan (JP), among others**.  

When discussing market share, a **pie chart** is often the most intuitive choice. Since the data represents percentages, this visualization makes it easier to understand which region dominates the industry. Currently, **North America accounts for nearly 50% of global video game Sales**.  

---

### 5. SalesGrowthByRegion Table  
This table focuses on the **growth trends of the video game industry across different regions**.  

Since growth over time is the primary concern, a **line chart** is the most appropriate choice for visualization.  

---

### 6. Supporting Tables Without PivotCharts  
Certain tables will not have PivotCharts but will occupy dedicated space on the dashboard. These tables provide direct answers to key questions, such as:  
- Which video games have had the highest impact and **Sales**?  
- Which **Publishers** have been the most successful?  
- Which **Genres** have dominated the market?  

---

## The Role of Slicers in the Dashboard  

A collection of PivotTables and PivotCharts alone does not constitute a dashboard—it is the **slicers** that make it interactive.  

Slicers allow users to filter data dynamically, affecting the displayed PivotTables and PivotCharts accordingly. This functionality enables viewers to explore different data perspectives simply by selecting various filter options.  

### Common slicers include:  
- **Genre Slicer**  
- **Platform Slicer**  

### Maintaining Analytical Integrity  
Not all PivotTables should be linked to slicers. Some tables must remain unaffected to preserve their analytical integrity.  

For example, the **Top5GenresWithHighestSales** table is **not** linked to the **Genre** slicer. If users filter by a specific **Genre** (e.g., **Role-Playing**), the table may lose essential information about other **Genres**, resulting in an inaccurate representation of the top five highest-grossing **Genres**. Keeping this table independent ensures it consistently reflects the overall top-performing **Genres**, regardless of user filtering.  

---

### Time Slicer (Timeline)  
One of the most critical slicers is the **Time Slicer (Timeline)**, as time-based analysis is the primary objective of this dashboard.  

---

## Final Outcome  
After implementing these steps, the completed dashboard will provide an automated, interactive, and insightful analysis of the video game industry's development over time.
# Recommendation
