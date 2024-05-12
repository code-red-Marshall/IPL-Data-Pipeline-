# IPL Data Analysis using Apache Spark

The project involves several stages, including data extraction, transformation, and loading (ETL), data warehousing, and data analysis. Here’s a high-level overview:

![Screenshot 2024-05-12 124918](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/512c2fd4-57b6-45d1-a677-10c5d3673e80)



Data Extraction: The IPL data is stored in an Amazon S3 bucket. This is the first step in the ETL pipeline where data is extracted from its source.

Data Transformation: The extracted data is then loaded into Databricks, a platform for big data analytics and artificial intelligence. 
Here, the data is transformed using PySpark, a Python library for Apache Spark. The transformations include cleaning the data, handling missing values, and creating new features.

Data Loading: After the transformations, the data is loaded into a data warehouse or data lake. In this case, the transformed data is loaded back into Databricks. This completes the ETL pipeline.

Data Analysis: Once the data is loaded into the data warehouse, it can be analyzed. SQL is used to query the data and generate insights. 
The analysis includes calculating average runs, determining the most economical bowlers, and assessing the impact of winning the toss on match outcomes.

Data Visualization: The results of the data analysis are then visualized using libraries like Matplotlib and Seaborn. These visualizations help in understanding the patterns and trends in the data.

![1](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/72a159d8-e262-4f98-8f6f-c508a4ede80a)


This workflow allows for efficient processing and analysis of large datasets, and can be scaled up to handle even larger volumes of data.
It also ensures that the data is clean, consistent, and ready for analysis. 
The use of SQL for data analysis allows for complex queries to be executed quickly, while the visualizations provide a clear and concise way to present the results.
