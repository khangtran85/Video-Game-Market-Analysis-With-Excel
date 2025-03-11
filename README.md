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
# Recommendation
