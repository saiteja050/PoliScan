📊 POLISCAN – Election Contributions Analytics 🇺🇸



📝 1. Problem Statement

In the United States, political donations play a major role in shaping election outcomes.While the Federal Election Commission (FEC) provides public campaign finance data, this data is:

📂 Extremely large in volume

🔍 Complex and hard to process directly

⚙️ Challenging to turn into actionable insights

💡 POLISCAN solves this by creating a scalable, cloud-based analytics platform that cleans, transforms, and analyzes political contribution data at scale — enabling analysts, regulators, journalists, and citizens to explore political funding with clarity and transparency.



🎯 2. Project Objectives

🧹 Clean and prepare OpenFEC datasets for analytics.

🔗 Join and enrich contributions, committees, and candidates datasets.

📌 Extract key features like donation type, demographics, geography.

🛡 Detect anomalies with rule-based checks (non-ML).

📈 Analyze trends in donation behavior.

📊 Visualize contributions and patterns through interactive dashboards.



📂 3. Datasets Used

Source: Federal Election Commission – OpenFEC

Dataset	File Name	Description

Individual Contributions	itcont.txt	All individual contributions to committees
Committee Master	cm.txt	Metadata about political committees
Candidate Master	cn.txt	Candidate details: office, party, election year

Relationships:

👤 Individuals ➡ Committees via CMTE_ID

🏛 Committees ➡ Candidates via CAND_ID

☁ 4. System Architecture


AWS Cloud Workflow:

[Raw Data]
    ↓
📦 Amazon S3 (Raw Zone)
    ↓
⚙️ AWS Glue (PySpark ETL)
    ↓
📦 Amazon S3 (Cleaned Zone - Parquet)
    ↓
🔍 AWS Athena (SQL Queries)
    ↓
📊 Power BI / Tableau (Dashboards)


🖼 Architecture Diagram 

📌 5. Key KPIs & Metrics

📊 KPI	📝 Description

💰 Total Contributions	Total donation amount over a given time period

📏 Average Donation Size	Mean value of donations

🔄 Donor Retention Rate	% of repeat donors

⏳ Contribution Frequency	Avg. number of donations per donor

♻️ Refund Rate	% of refunded donations

🗺 Regional Distribution	Donations segmented by state

👥 Donor Demographics	Breakdown by occupation, employer, gender



🎯 6. Expected Outcomes

✅ Clean, structured, and queryable dataset

📊 Interactive dashboards with KPIs

🌍 Donor insights by region, profession, and behavior

🏛 Transparent system for public & institutional use



💼 7. Use Cases

📈 Political Analysts – Track donation trends.

🗳 Campaign Teams – Optimize fundraising strategies.

👥 Public & Activists – Promote accountability.



🚀 8. Key Features

☁ Cloud-native AWS architecture

🔄 End-to-end pipeline from raw to insights

📰 Stakeholder-focused design for analysts, journalists, and regulators



📊 9. Dashboards

Dashboard 1 – KPIs Overview

💰 Total Contributions

📏 Average Donation

🔄 Retention Rate

Dashboard 2 – Donor Demographics

👩‍💼 Occupation Distribution

🏢 Employer Statistics

🚻 Gender Split

Dashboard 3 – Geographic Insights

🗺 US Map by State Donations

🏛 Party-wise Distribution

🖼 Dashboard Screenshots 



🏁 10. Conclusion
POLYSCAN transforms raw political donation data into clear, insightful, and accessible analytics By improving transparency and accountability, it empowers citizens, institutions, and decision-makers to understand how money flows in politics.
