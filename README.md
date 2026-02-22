# Data Job Analytics by using Excel
The project documented my Excel skills, exploiting PivotTable, Power Query, and PowerPivot to analyse which skills are needed in the data domain. The project also revealed different salary ranges across countries, mostly primarily in the United States and Australia

# Final Dashboard
The final dashboard for my project was illustrated as below:


<img width="1291" height="453" alt="1  Overall Salary Dashboard" src="https://github.com/user-attachments/assets/0c8ba073-0244-40ad-8452-0a0c663bb3c1" />


The dashboard featured three charts: Median Salary by Job Title, Country, and Job Count by Job Title. For the convenience of analysis, I would like to pick job title "Data Analyst" since it is the most commonly searched titles job seekers have been looking for. In the United States, the median salary has been estimated at around US$90,000 with total 6,480 job openings across Full - Time, Part - Time, Contractor, Temporary Work (Temp-Work), and Intership. 

Since I am based in Australia, I also look for the Data Analyst title in Australia: 


<img width="1298" height="447" alt="image" src="https://github.com/user-attachments/assets/74a347a4-7b9d-4bf7-95c4-51f70fcad3b4" />


While building a global salary dashboard, I identified a significant discrepancy between automated data scraping and "ground-truth" recruitment data in Australia. It was clear that the median salary for Data Analyst in Australia has been estimated at US$109,500 (AU$155,000, with current exchange rate: 1 USD = 1.42 AUD). 

According to Hays Australia, the Data Analyst position ranges from AU$80,000 to AU$130,000, depending on the seniority levels (https://www.hays.com.au/it/data-analyst-jobs/salary). The dashboard shows a premium median (AU$155k) which represents the top 10% of the general market. As a professional with a background in engineering and pivoting into data, I apply a "Sensitivity Analysis" to data. I identified three reasons for the AU$155k outlier:
- Platform Bias: High-tier tech platforms capture "Silicon Valley" style salaries in Sydney/Melbourne rather than the broader public sector or SME market.
- Job Title Inflation: Roles labeled "Data Analyst" often encompass "Data Scientist" responsibilities in certain datasets.
- Currency Fluctuations: Real-time conversion (1 USD = 1.42 AUD) impacts perceived value across different reporting periods.
  
To refine these insights and eliminate source bias, I suggest a secondary phase of data validation and integration. Specifically, I will be looking to ingest:
- Jobs and Skills Australia (JSA) official datasets to capture government-verified salary benchmarks.
- Localised vacancy data to better reflect the diverse job markets across Sydney, Melbourne, and Brisbane.
- Seniority-based filtering to distinguish between entry-level Data Analysts and Senior/Lead positions.

# Correlation between Salary and Skills
Besides building up salary dashboards, I also explored the correlation between the skills needed for Data job tiltes and the salary. To capture this, I applied Pivot Table, Power Query, and Power Pivot to develop the data model diagram as below:

<img width="660" height="734" alt="image" src="https://github.com/user-attachments/assets/b9eb4f88-0889-48f9-a53c-f8407492cee0" />


Based on the data model developed from Power Pivot, I developed the correlation diagram as below:

<img width="333" height="239" alt="image" src="https://github.com/user-attachments/assets/25eaad88-1fa3-432f-a3fc-d15995aaa8b0" />


<img width="861" height="546" alt="image" src="https://github.com/user-attachments/assets/c3ae82e3-182e-4030-9ac8-99fe287a3dc7" />


📈 Core Data Insights: The Value of Specialisation
- Identified a Positive Correlation Between Skill Density and Pay: I observed that as the number of skills requested per job posting increased, the median salary followed a consistent upward trend, with roles requiring 7+ skills, such as Senior Data Engineers, commanding over $145,000 USD.
- Discovered the "Efficiency Outlier" in Senior Data Science: I found that Senior Data Scientists represented the most efficient path to high compensation, as they earned the highest median salary (~$155,000 USD) despite requiring fewer total tools than engineering roles, suggesting the market prioritized depth in specialized modeling over a high quantity of tools.
- Quantified the "Engineering Premium": I analyzed the transition from "Analyst" to "Engineer" titles and determined that while it required a ~40% increase in skill count, it yielded a significant salary dividend, moving the median from $90,000 USD for Data Analysts to $125,000 USD for Data Engineers.
- Evaluated the Impact of Seniority for Analysts: I highlighted that moving from a standard Data Analyst to a Senior Data Analyst increased the median salary by approximately $20,000 USD with the addition of only one core skill on average, indicating that project leadership and experience were valued as highly as new technical proficiencies.

# Conclusion
There were three key conclusion I have driven based on my analysi: 
- The Correlation Between Versatility and Compensation: My analysis demonstrates a clear positive correlation between skill density and median salary. While entry-level roles (Business/Data Analyst) focus on a core set of ~3–4 skills, the path to the $150k+ USD bracket requires significant technical expansion into Data Engineering and specialized Machine Learning frameworks. This confirms that in the 2026 market, "upskilling" is not just a career preference but a measurable driver of financial value.
- The "Quality over Quantity" Conclusion: A key discovery in the data is the "Efficiency Peak" of the Senior Data Scientist role. Despite requiring fewer total skills than a Senior Data Engineer, it commands the highest median salary. This suggests that the market places a premium on the depth of high-impact skills (such as advanced statistical modeling) over the breadth of infrastructure tools. For professionals, this highlights a strategic choice: horizontal growth into Engineering or vertical growth into specialized Data Science.
- The "Data Integrity" Conclusion (Specific to Australia): This project revealed a discrepancy in automated salary reporting for the Australian market. While global scrapers suggested a median of AU$155,000 for Data Analysts, cross-referencing with local leaders like Hays and Seek identifies a more realistic range of AU$80,000–$130,000. Consequently, a primary conclusion of this study is that "Data Analysts" must apply a secondary validation layer—such as integrating Jobs and Skills Australia (JSA) data—to ensure insights are localized and free from platform-specific inflation.
