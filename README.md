# Leveraging Data Analytics for Sales Optimization and Revenue Growth
In the intensely competitive world of online retailing, organizations like Amazon must determine which product aspects drive sales performance. When assessing how well a product sells, factors including pricing, customer rating, product category, and discount are critical. The difficulty, though, is in properly evaluating these variables to produce better choices that increase revenue and satisfy customers.
The objective of this project is to determine which product attributes such as category, price, rating, and discount have the most effects on the performance of sales. Additionally, we want to know how to best optimize discount percentages to maximize customer ratings and sales volume across a range of product categories.
## Dataset Overview
We used an Amazon sales dataset sourced from Kaggle. The dataset includes key attributes like product ID, category, actual price, discounted price, discount percentage, rating, and rating count. Additionally, we derived new attributes such as revenue, sales volume, and normalized metrics to gain a deeper understanding of sales performance. The dataset consists of 1,465 products and is approximately 4.53 MB in size.
## **Tools Used** 
- **Apache NiFi**: Used for ingesting data from the local machine to HDFS.
- **HDFS (Hadoop Distributed File System)**: Served as the storage system for the ingested data. After ingestion via NiFi, the CSV file was stored in HDFS, ensuring scalability, fault tolerance, and efficient data retrieval in a distributed environment. 
- **PySpark**: Employed for pre-processing the data in HDFS. Tasks included cleaning, transforming, deriving additional attributes (e.g., revenue and sales volume), and selecting key columns necessary for analysis.
- **Hive**: Utilized to query the data stored in HDFS and gain insights. SQL-like queries were used to calculate metrics such as average ratings per category or sales volume per category. 
- **Kibana**: Created interactive dashboards and visualizations for presenting insights. 
## **Results**
- **Impact of Discounts**: Analyzed the relationship between discounts and sales performance, uncovering trends in sales volume and revenue.
![image](https://github.com/user-attachments/assets/50ba5535-597c-421b-9f43-4167a530923f)
![image](https://github.com/user-attachments/assets/a18cca4e-cc19-4822-9117-b6908c9a21a5)

- A comprehensive documentation of the project, including visualizations, can be found in the `Reports` directory. 
## **Future Enhancements**
- **Real-Time Insights**: Integrate real-time data pipelines using technologies like Apache Kafka to update Elasticsearch indexes and Kibana dashboards dynamically.
- **Predictive Analytics**: Employ machine learning models to forecast sales patterns, improve inventory control, and identify optimal discount strategies.
- **Consumer Sentiment Analysis**: Use Natural Language Processing (NLP) on customer reviews to gain insights into preferences and areas for improvement.
- **Geospatial Visualizations**: Incorporate geospatial analysis to identify regional trends in sales.
- **Multi-Channel Integration**: Combine data from physical stores and e-commerce platforms for a comprehensive performance overview.
