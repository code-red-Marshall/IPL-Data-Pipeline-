![Untitled design (8)](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/d5bf3532-139b-4051-b3af-4cb8dd24e891)

# IPL Data Analysis using Apache Spark and Databricks
This project demonstrates the use of Apache Spark for performing data analysis on the Indian Premier League (IPL) dataset. The data is stored in Amazon S3 and the analysis is performed using Databricks environment.
The project involves several stages, including data extraction, transformation, and loading (ETL), data warehousing, and data analysis.

![Screenshot 2024-05-12 124918](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/512c2fd4-57b6-45d1-a677-10c5d3673e80)


## Prerequisites
- An AWS account with access to S3 services
- Databricks account
- IPL dataset  Link: https://data.world/raghu543/ipl-data-till-2017

## Setup
- Upload the IPL dataset to your AWS S3 bucket.
- Store the AWS access key and secret key in a CSV file and upload it manually to Databricks.

## Dataset
The dataset used in this project is the IPL dataset, which includes details about matches, players, teams, and ball-by-ball data. The dataset is stored in Amazon S3.


## Tools and Technologies
- Apache Spark: Used for data processing and analysis.
- Databricks: Provides an interactive workspace and runtime environment for running Spark.
- Amazon S3: Used as the data storage solution for the dataset.
- Python: The primary programming language used for writing the data processing and analysis code.
- SQL: Used for querying the data and performing analysis.
- Matplotlib and Seaborn: Used for data visualization.

## Mounting S3 Bucket

The S3 bucket is mounted in Databricks using the AWS access key and secret key. The keys are stored in a CSV file that is uploaded manually to Databricks. 

Data Extraction: The IPL data is stored in an Amazon S3 bucket. This is the first step in the ETL pipeline where data is extracted from its source.

Data Transformation: The extracted data is then loaded into Databricks, a platform for big data analytics and artificial intelligence. 
Here, the data is transformed using PySpark, a Python library for Apache Spark. The transformations include cleaning the data, handling missing values, and creating new features.

Data Loading: After the transformations, the data is loaded into a data warehouse or data lake. In this case, the transformed data is loaded back into Databricks. This completes the ETL pipeline.

## Data Analysis 
Once the data is loaded into the data warehouse, it can be analyzed. SQL is used to query the data and generate insights. 
The analysis includes:

- Calculating the total and average runs scored in each match and inning.
- Identifying high impact balls (either a wicket or more than 6 runs including extras).
- Extracting year, month, and day from the match date for more detailed time-based analysis.
- Categorizing win margins into ‘high’, ‘medium’, and ‘low’.
- Analyzing the impact of the toss: who wins the toss and the match.
- Normalizing and cleaning player names.
- Adding a ‘veteran_status’ column based on player age.
- Calculating years since debut.
- Identifying top scoring batsmen per season.
- Identifying the most economical bowlers in powerplay overs.
- Analyzing the impact of winning the toss on match outcomes.
- Calculating average runs scored by batsmen in winning matches.
- Analyzing distribution of scores by venue.
- Identifying the most frequent dismissal types.
- Analyzing team performance after winning the toss.

## Data Visualization 
The results of the data analysis are then visualized using libraries like Matplotlib and Seaborn. These visualizations help in understanding the patterns and trends in the data.

![1](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/72a159d8-e262-4f98-8f6f-c508a4ede80a)

![2](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/27f45b8d-27a5-4277-bcc2-7be0ab74d422)

![3](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/c018a3cc-0d36-4eaf-8fb1-5e04d110a98b)

![4](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/53cb7f1e-7010-4a4e-852a-831ffa936d1e)

![5](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/dc8c8f07-0590-4dde-97de-befb267043e2)

![6](https://github.com/code-red-Marshall/IPL-Data-Pipeline-/assets/82904501/f7f6c8c8-c2c7-4f05-b2ab-377b7ceb81dd)


This workflow allows for efficient processing and analysis of large datasets, and can be scaled up to handle even larger volumes of data.
It also ensures that the data is clean, consistent, and ready for analysis. 
The use of SQL for data analysis allows for complex queries to be executed quickly, while the visualizations provide a clear and concise way to present the results.

## Contributions:
Contributions to this project are welcome. If you find a bug or think of a new feature, please open an issue. If you would like to make changes to the code, please fork the repository and submit a pull request.
