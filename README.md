Project

Phase 1

Project Title: Data Wrangling for Enhanced Cloud Data Processing at Razbana

Project Description: Data Wrangling for Cloud Computing Analytics at Razbanroject 

Objective: The primary goal of this project is to perform comprehensive data wrangling to prepare a robust dataset for cloud computing analytics at Razbana. By cleaning, transforming, and consolidating data from various sources, the project aims to enhance the accuracy and usability of operational data for subsequent analysis and reporting.

Background: Razbana's cloud computing project involves processing and analyzing large volumes of data from various sources, including operational landscapes, transformation logs, and curated insights. However, inconsistencies, missing values, and fragmented data make it challenging to derive meaningful insights. Effective data wrangling will ensure high-quality data for better decision-making and analytics.

Dataset: The data wrangling process will involve multiple datasets, including:
•	Raw Operational Data: Extracted from Vancouver's operational landscape and stored in the S3 bucket (cov-raw-raz).
•	Transformed Data: Processed and cleaned datasets stored in the transformation bucket (cov-trf-raz).
•	Curated Insights: Summarized and aggregated data stored in the curated bucket (cov-cur-raz).

Methodology:
1.	Data Collection:
o	Upload raw data manually to the S3 bucket for ingestion.
o	Future integration of direct ingestion using PowerShell from operational servers.
3.	Data Assessment:
o	Perform data profiling to examine data quality issues.
o	Identify missing values, inconsistencies, and outliers using AWS Glue Data Brew.
4.	Data Cleaning:
o	Use AWS Glue Data Brew to create cleaning recipes for transformation.
o	Address missing values by filtering out null entries to maintain data integrity.
o	Standardize schema naming conventions (e.g., "ArtistDetails" with no spaces).
5.	Data Transformation:
o	Execute data jobs to apply transformation rules and schema adjustments.
o	Convert date formats and ensure uniform data types for consistency.
o	Aggregate and derive new insights such as total outstanding amounts per artist.

6.	Data Consolidation:
o	Merge cleaned and transformed data into structured tables using AWS Glue Data Catalog.
o	Store structured metadata in databases for easy retrieval and management.

8.	Documentation and Validation:
o	Maintain detailed logs of cleaning processes, transformation steps, and schema changes.
o	Validate final datasets through exploratory data analysis (EDA) to confirm accuracy.

Tools and Technologies:
•	AWS S3: Data storage and management.
•	AWS Glue Data Brew: Data profiling, cleaning, and transformation.
•	AWS Glue Data Catalog: Organizing and structuring metadata.
•	Python & Pandas: Additional data wrangling and validation if needed.
•	SQL (Athena): Querying transformed datasets for analysis.

Deliverables:
•	A cleaned and structured dataset stored in S3 for cloud analytics.
•	A comprehensive report documenting data wrangling steps and challenges.
•	Data visualizations and insights derived from curated datasets.

Timeline:
•	Expected completion: 6 weeks, covering data ingestion, profiling, cleaning, transformation, and validation.
This data wrangling project ensures that Razbana can efficiently process and analyze high-quality cloud computing data, improving business insights and operational efficiency.


