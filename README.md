Project

Phase 1

Project Title: Data Wrangling for Enhanced Cloud Data Processing at Razbana

Project Description: Data Wrangling for Cloud Computing Analytics at Razbanroject 

Objective: The primary goal of this project is to perform comprehensive data wrangling to prepare a robust dataset for cloud computing analytics at Razbana. By cleaning, transforming, and consolidating data from various sources, the project aims to enhance the accuracy and usability of operational data for subsequent analysis and reporting.

Background: Razbana's cloud computing project involves processing and analyzing large volumes of data from various sources, including operational landscapes, transformation logs, and curated insights. However, inconsistencies, missing values, and fragmented data make it challenging to derive meaningful insights. Effective data wrangling will ensure high-quality data for better decision-making and analytics.

Dataset: The data wrangling process will involve multiple datasets, including:
•	Raw Operational Data: Extracted from Vancouver's operational landscape and stored in the S3 bucket (cov-raw-raz).

![image](https://github.com/user-attachments/assets/5475356f-c834-42bd-bafc-8a4ecb25bf27)

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

Phase 2

Project Title: Understanding Public Art Data in Vancouver Using AWS

Objective: The primary goal of this project is to conduct a descriptive analysis of public art records in Vancouver. Through this analysis, we aim to summarize key characteristics of artist biographies, identify gaps in documentation, and generate insights that can improve data collection and historical preservation.

Dataset: The dataset includes public art records stored in AWS, containing the following key features:
•	Artist Name: Name of the artist featured in the public art records.
•	Biography: Text data containing the artist’s background information.
•	Artwork Title: Title of the public artwork.
•	Location: Geographical placement of the artwork in Vancouver.
•	Creation Date: The date when the artwork was created or installed.
•	Category: Type of public art (e.g., sculpture, mural, installation).

Methodology:
1.	Data Collection and Preparation:
o	Extract data from the AWS Glue Data Catalog ("con-data-catalog-raz").
o	Perform data cleaning to address missing biographies, correct formatting issues, and remove duplicates.

Descriptive Statistics:
o	Calculate summary statistics for key variables, including:
	Total number of artists with and without biographies.
	Distribution of artwork by category and location.
	Average length of artist biographies.

Data Visualization:
o	Create visual representations to illustrate findings:
	Bar charts showing the percentage of artists with and without biographies.
	Heatmaps representing artwork distribution by location.
	Pie charts depicting the types of public art installations.

Data Quality Assessment:
o	Identify missing or incomplete data in artist biographies.
o	Assess potential inconsistencies in artwork categorization and location data.

Insights and Findings:
o	Summarize key findings, highlighting:
	The extent of missing biographical data.
	Common trends in public art placement and categorization.
	Potential areas for data enhancement.

Recommendations:
o	Provide actionable recommendations based on the findings to improve data quality and completeness:
	Enhance artist biography documentation efforts.
	Standardize data entry processes for artwork classification.
	Improve data governance for public art records.

Tools and Technologies:
•	AWS Athena: Querying structured datasets.
•	AWS Glue Data Catalog: Organizing and structuring metadata.
•	SQL: Extracting and analyzing data.
•	Python (Pandas, Matplotlib, Seaborn): Data analysis and visualization.

Deliverables:
•	A detailed report summarizing the descriptive analysis, findings, and recommendations.
•	Visualizations and dashboards to present key insights clearly.
•	A presentation for stakeholders to communicate important findings and suggestions for data improvement.
This descriptive analysis project aims to provide a comprehensive understanding of public art records in Vancouver, enabling better historical documentation and improved data management strategies.
