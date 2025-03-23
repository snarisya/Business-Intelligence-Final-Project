# Business-Intelligence-Final-Project 🎈🎈

This project is part of my assessment for business intelligence class during my master's degree course.
Initially, i want to include the dashboard here as well, but the file is too large hence Github won't allow me to do so.
So here just a screenshot of the dashboard and a little bit explanation for each.
Hope you enjoy & gain extra knowledge from it! 😇


For this project, I used Olist E- commerce dataset available here https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce.
The data is pretty big as it contains around 100K of customers order record.


## Business Problem 🎇

Before creating the dashboard, I would like to identify some specific problems that Olist might encounter to ensure the dashboard is tailored to support their business decisions effectively.

Olist is struggling with several interconnected operational challenges that hinder its ability to make informed decisions and optimize business performance. These challenges include:

1. Lack of a Centralized System for KPI Monitoring: Olist does not have an integrated system to track and analyze key performance indicators (KPIs) across different business areas, which limits the company's ability to gain a comprehensive understanding of its performance and identify areas for improvement.

2. Ineffective Product Portfolio Optimization: Olist needs to identify top-performing product categories to allocate resources effectively and make strategic adjustments to underperforming categories, but currently lacks tools or insights to do so.

3. Customer Satisfaction Insights: The company is unable to effectively monitor customer satisfaction trends, track feedback over time, and identify product categories that may negatively impact customer satisfaction.

4. Delivery Performance Challenges: Olist lacks a streamlined approach to monitor and improve delivery performance, which is crucial for ensuring timely and efficient deliveries that impact customer satisfaction.

5. Lack of Forecasting Capabilities: Olist is unable to anticipate future trends such as revenue, delivery timelines, and customer reviews, making it difficult to engage in strategic planning and long-term growth.

To address these issues, Olist needs a suite of customized dashboards that offer data-driven insights across various operational areas, enabling better decision-making, optimization of resources, and improvements in customer satisfaction and performance.

## Data Preparation 🎆

The core steps in doing analytics is data preparation. I used to do all the cleaning in python but for this project I choose to do all the preparation steps only in power BI. 
The main transformations included:

1. Standardization: The first row of the Excel files was promoted as the header for consistent structuring across all data sources.

2. Data Type Transformation: Columns like 'Customer ID,' 'Order ID,' and 'Review ID' were changed from numerical to textual data types to align with analytical requirements.

3. Data Cleansing: Empty rows were removed from most datasets, except in the 'Review' dataset, where empty 'Review Comment' rows were retained as they weren't critical to analysis.

4. Text Formatting: Columns in the 'Orders Payment,' 'Orders,' and 'Product Category Name Translation' datasets were cleansed by removing unwanted symbols and applying capitalization to ensure uniform formatting.

5. Custom Column Addition: In the 'Orders' dataset, a custom column was created to extract day values from date columns for deeper analysis.

6. Duplicate Removal: Duplicated rows were identified and removed to maintain data integrity.

Furthermore, a manual relationship was established between the 'Product Category Name Translation' and 'Olist Products' datasets, linking them through the 'product category name' column. This relationship enabled seamless retrieval of product category names in English, enhancing the dataset's comprehensibility and analytical capabilities.

These preprocessing steps ensured that the datasets were clean, consistent, and ready for effective analysis and visualization in Power BI.

## Dashboard Storyline 🎇

Now, we've reached the main goal of this project: developing the dashboard! 😄
The dashboard consists of 5 pages, each designed to address the key challenges Olist faces, as outlined in the initial business problems.

### First Page: Olist Overview Report Page ✨
![image](https://github.com/user-attachments/assets/4b06b9e5-8630-4cf2-aba8-7a3936dcaa86)

The journey begins with the Olist Overview report page, aiming to provide a comprehensive view of the company's performance. This report page offers insights into key metrics such as total revenue breakdown by year, allowing us to track financial growth over time. 
It also provides valuable geographical insights by showcasing the regional distribution of customers. Additionally, the report page examines payment types in relation to total orders and reveals the top 5 products ordered by product category, shedding light on product performance. Metrics such as total orders, customers, sellers, and average review scores contribute to a holistic understanding of Olist's strengths and areas for improvement.

### Second Page: Olist Product Analysis Report Page ✨
![image](https://github.com/user-attachments/assets/3ec5ba22-c454-480d-84d0-87f7ddeaf349)

Moving on, the Product Analysis report page refines our understanding of product performance by delving into key aspects that shape Olist's offerings. 
Firstly, it spotlights the top 5 revenue-generating product categories, illuminating which segments are the primary drivers of Olist's financial success. 
This analysis not only identifies the revenue leaders but also presents opportunities for further growth and optimization within these categories. 
Conversely, the report page doesn't shy away from examining the bottom 5 revenue-generating product categories. 
By showcasing these underperforming segments, it provides a platform to identify areas in need of improvement and strategic adjustments, ensuring that Olist maximizes its potential across the board. 
The report page also unveils the top 10 product categories with the highest average prices.
This insight into pricing dynamics sheds light on trends and opportunities, allowing Olist to strategically position its offerings in the market and cater to diverse customer preferences. 
Furthermore, the report page explores the relationship between total order quantities and the average price by product category. 
This illuminates valuable insights into customer behavior, such as whether higher-priced items tend to attract fewer but larger orders or vice versa. 
Understanding this correlation empowers Olist to tailor its product strategies, optimize pricing, and enhance its overall product portfolio to meet customer demands effectively.

### Third Page: Olist Customer Satisfaction Report Page ✨
![image](https://github.com/user-attachments/assets/cf04e987-d85f-401a-975c-b408603f1683)

The journey continues with the Customer Satisfaction report page, enriching our understanding of customer experiences and feedback. 
It provides valuable insights by showing the breakdown of total orders over different time periods, along with their associated review scores. 
This helps us identify trends in customer satisfaction over time and make improvements accordingly. 
Additionally, the report page highlights the top 10 product categories that receive the highest ratings from customers, as well as the bottom 10 categories that may need attention. 
This information guides us in focusing on what's working well and addressing areas that require enhancement. 
Moreover, the report page explores the relationship between average review scores and the average shipping days for different product categories, helping us understand how delivery speed impacts customer satisfaction. 
By using these insights, we can allocate resources effectively and optimize our logistics processes to ensure timely deliveries, ultimately leading to higher customer satisfaction and loyalty.

### Fourth Page: Olist Delivery Performance Report Page ✨
![image](https://github.com/user-attachments/assets/c6d81eda-3f00-4275-9095-5e4d30eccba8)

The Delivery Performance report page at Olist serves as a vital tool to gain a comprehensive understanding of our delivery operations. 
It begins by breaking down total orders based on delivery and order status, providing insights into our delivery performance. 
Additionally, the report page includes key metrics like average shipping days and the sum of freight values, allowing us to evaluate the efficiency and cost-effectiveness of our delivery process. 
We also delve into the average shipping days for each product category, pinpointing areas where improvements in delivery speed may be needed. 
Furthermore, the distribution of payment types based on delivery status is highlighted, offering valuable insights for optimizing payment processing in alignment with delivery timelines. 
As part of our continuous improvement efforts, we also explore the relationship between average shipping days and freight value by product category, aiming to uncover any correlations that can further enhance our delivery operations. 
With this data-driven approach, we can make informed decisions to refine our delivery processes, ensuring a smoother and more efficient customer experience.

### Fifth Page: Olist Forecasting Report Page ✨
![image](https://github.com/user-attachments/assets/02dae632-e7c7-4fbf-aa95-bf70fa207d40)

The final report page in this dashboard is the forecasting report page. The Olist forecasting report page takes center stage in providing valuable insights into our business's future performance. 
With a primary focus on predicting three pivotal factors total revenue, average shipping days, and average review scores. 
This report page harnesses the power of historical data and advanced forecasting techniques. 
By peering into the crystal ball of data, it equips Olist with the ability to anticipate revenue trends over the next 's' years, estimate delivery timelines for our customers, and forecast the average review scores that shape our reputation. 
These invaluable forecasts empower Olist to make strategic decisions, enhance customer satisfaction, and chart a path towards future growth and success.


## DONE with the dashboard!!! 🎉🎉

In conclusion, the Olist Dashboard Suite provides a comprehensive view of our business, enabling informed decisions and continuous improvement. The Overview report page covers financial growth, regional presence, payments, and product performance. 
The Product Analysis report page delves into categories, identifying revenue leaders, underperformers, pricing trends, and customer behavior. 
The Customer Satisfaction report page tracks feedback and optimizes categories. 
The Delivery Performance report page offers insights into delivery efficiency, cost-effectiveness, and payment processing. 
It explores correlations between shipping days and freight values by category. 
The Forecasting report page anticipates revenue trends, delivery timelines, and review scores, empowering Olist for success in the e-commerce landscape.
