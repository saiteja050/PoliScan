# PoliScan
POLYSCAN – Election Contributions Analytics 🇺🇸
Problem Statement
In the United States, political donations play a major role in shaping election outcomes, yet the data surrounding these contributions is vast, complex, and often difficult to analyze. Publicly available campaign finance data—such as that from the Federal Election Commission (FEC)—contains valuable insights about donor behavior and financial trends. However, raw datasets are large and not easily accessible for meaningful insights.
POLYSCAN solves this by creating an end-to-end big data analytics pipeline to clean, transform, and analyze political contribution data at scale. This platform empowers analysts, regulators, journalists, and citizens to understand, explore, and monitor political funding with ease, clarity, and transparency.

 Project Objectives
•	 Clean and prepare OpenFEC datasets for analytics.
•	 Join and enrich contributions, committees, and candidate datasets.
•	 Extract key features such as donation type, demographics, and geography.
•	 Perform rule-based anomaly detection (non-ML).
•	 Generate insights on donation behavior and trends.
•	 Visualize political contributions and suspicious patterns through dashboards.
•	 Support open, fair, and transparent campaign financing.

Datasets Used
All datasets are from the official Federal Election Commission (OpenFEC) source:
1.	Individual Contributions
➤ itcont.txt:
Contains all individual contributions to committees.
2.	Committee Master
➤ cm.txt:
Contains metadata about political committees.
3.	Candidate Master
➤ cn.txt:
Contains candidate details including office, party, and election year.
Relationships:
•	Individuals ➝ Committees via CMTE_ID
•	Committees ➝ Candidates via CAND_ID 

System Architecture
The entire solution is built using a scalable, cloud-based architecture on AWS, consisting of:
•	Amazon S3: Raw and cleaned data storage
•	AWS Glue (PySpark): ETL pipeline for transforming and joining datasets
•	AWS Athena: Querying cleaned Parquet files
•	Power BI / Tableau: Dashboard and reporting layer for insights

Key KPIs & Metrics
KPI	Description
Total Contributions	Total donation amount over a time range
Average Donation Size	Mean value of donations
Donor Retention Rate	% of repeat donors
Contribution Frequency	Avg number of donations per donor
Refund Rate	% of refunded donations
Regional Distribution	Donations by state
Donor Demographics	Breakdown by occupation, employer, gender

Expected Outcomes
•	 Clean, structured, and queryable donation dataset
•	 Interactive dashboard with KPIs
•	 Donor analysis based on region, profession
•	 Transparent and explainable system for public and institutional use

 Use Cases
•	Political Analysts: Track donation trends and behaviors.
•	Campaign Teams: Optimize fundraising and competitor insights.
•	Public & Activists: Drive accountability and transparency.

Key Features
•	Scalable and cloud-native using AWS services.
•	Designed for real-world stakeholders: analysts, journalists, regulators.
•	End-to-end pipeline: from raw data to visual insights.

Conclusion
POLYSCAN transforms raw and unmanageable political donation data into a powerful analytics tool. By enabling transparency and enhancing accessibility, it supports democratic processes and empowers citizens, analysts, and institutions to better understand how money flows in politics.

