# PoliScan
POLISCAN – Election Contributions Analytics 🇺🇸
Problem Statement
In the United States, political donations play a major role in shaping election outcomes, yet the data surrounding these contributions is vast, complex, and often difficult to analyze. Publicly available campaign finance data—such as that from the Federal Election Commission (FEC)—contains valuable insights about donor behavior and financial trends. However, raw datasets are large and not easily accessible for meaningful insights.
POLISCAN solves this by creating an end-to-end big data analytics pipeline to clean, transform, and analyze political contribution data at scale. This platform empowers analysts, regulators, journalists, and citizens to understand, explore, and monitor political funding with ease, clarity, and transparency.

 Project Objectives
•	 Clean and prepare OpenFEC datasets for analytics.
•	 Join and enrich contributions, committees, and candidate datasets.
•	 Extract key features such as donation type, demographics, and geography.
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
•	Power BI : Dashboard and reporting layer for insights

Architecture Diagram:

<img width="826" height="723" alt="Screenshot 2025-08-13 135222" src="https://github.com/user-attachments/assets/f401c566-b540-41ca-8a90-9dc95765bc76" />


Key KPIs & Metrics
KPI	Description
Total Contributions	Total donation amount over a time range
Average Donation Size	Mean value of donations
Donor Retention Rate	% of repeat donors
Contribution Frequency	Avg number of donations per donor
Refund Rate	% of refunded donations
Regional Distribution	Donations by state
Donor Demographics	Breakdown by occupation

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
POLISCAN transforms raw and unmanageable political donation data into a powerful analytics tool. By enabling transparency and enhancing accessibility, it supports democratic processes and empowers citizens, analysts, and institutions to better understand how money flows in politics.


DASHBOARD:

<img width="1377" height="751" alt="image" src="https://github.com/user-attachments/assets/068ae842-e0d8-4151-af37-82940b39189f" />

<img width="1339" height="736" alt="image" src="https://github.com/user-attachments/assets/2c3726f0-7c40-4257-b0d7-89d8c3a9d47c" />

<img width="1373" height="749" alt="image" src="https://github.com/user-attachments/assets/90050855-84fa-4501-b0e0-5bb96fdce028" />




