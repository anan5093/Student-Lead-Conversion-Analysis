# Student Lead Management & Conversion Analysis Report

A full data analytics project involving data cleaning, robust de-duplication methodology, and creation of a multi-dimensional dashboard for performance monitoring of educational consulting admission pipeline.

 **[Click Here to View the Live Google Sheets Dashboard](https://docs.google.com/spreadsheets/d/14gp_H1U4MpJUli8tOo1gFI10CMImS7MxMYOKMUErdhc/edit?usp=sharing)**

##  Project Objective
In order to make the project happen, we needed to convert 66 unstandardized records of students' inquiries into an operational intelligence system. This would entail such activities as standardization of inconsistent program data entries, cross tabulation of communications, workload assessment of counselors, as well as the creation of an active queue.

##  Data Governance & Methodology
* **Taxonomy Standardization:** Mapped disparate raw course entries into structured core categories (e.g., normalising variant programs into clean tracks like General Education Counselling and Bachelor of Hospital Administration).
* **Geographic Resolution:** Verified and completed missing regional data fields, standardizing all locations to explicit 'State, India' formatting.
* **Non-Destructive Deduplication:** Implemented a system-level duplicate checking array based exclusively on `Student Name`. Using a conditional count sequence, the first instance of a name is designated as `Unique`, while subsequent occurrences are flagged as `Duplicate` or marked for operational `Review` without purging historical activity logs.
* **Tech Stack:** Google Sheets / Microsoft Excel utilizing logical indexing (IFS, COUNTIFS, XLOOKUP), dynamic matrix tables, and interactive data filters.

##  Core Analytics & Insights

###  Data Quality & Integrity Metrics
* **Total Pipeline Intake:** 66 records
* **Gross Duplicate Profile Rate:** 22.7% (15 records identified as duplicates or flagged for review based on student names).
* **Overall Baseline Data Health:** 81.8% valid baseline data capture.

###  Counsellor Performance & Capacity Matrix
The entire team processed 66 gross leads, resulting in 6 absolute conversions and an overall baseline team conversion rate of 9.1%.
* **Anjali (Top Performer):** Handled the highest operational load with 16 total leads, securing 2 conversions for a team-leading individual conversion rate of 12.5%.
* **Arun & Sneha:** Each managed 11 leads, yielding 1 conversion apiece for an individual conversion rate of 9.1%.
* **Priya:** Handled 13 leads, achieving 1 conversion for a conversion rate of 7.7%.
* **Rahul:** Managed 15 leads, achieving 1 conversion for a conversion rate of 6.7%.

###  Funnel Bottlenecks & Operational Priority Queue
* **Follow-up Volume:** Identified a critical operational segment of 17 active leads currently residing in the `Follow-up` stage.
* **High-Priority Queue:** Out of the 17 stagnant follow-up rows, 5 leads are explicitly tagged as `Interested in admission`. These represent immediate, high-probability closing targets for the admissions team.

###  Niche Program & Regional Yields
* **Volume Distribution:** General Education Counselling drives the highest top-of-funnel volume, accounting for 43.9% of the pipeline (29 leads), but yields a low conversion rate of 6.9%.
* **High-Yield Conversions:** Specialized niche programs (including BHA, Animation Film Design, and Game Design) account for only a fraction of initial lead volume but generate 66.7% of all terminal conversions.
* **Geographic Efficiency:** West Bengal and Telangana represent the most high-yielding geographic territories, with each region generating 2 conversions from 7 total leads (28.6% conversion rate).

##  Repository Structure
* `/data`: Contains raw and processed dataset configurations.
* `/dashboard`: Houses the final metrics delivery framework, formula logs, and dynamic visualizations.
