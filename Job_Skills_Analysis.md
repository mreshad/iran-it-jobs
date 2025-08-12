
# Full Analysis of Job Skills and Data Cleaning

## 1. Association Analysis
- **Skills Parsing**: A custom function was developed to clean and parse skills from job postings, ensuring the data is formatted consistently for analysis.
- **Frequent Itemsets**: Using the **Apriori** algorithm, frequent itemsets (skills) were identified, highlighting the most commonly required skills in the job market.
- **Association Rules**: **Association rules** were generated based on the itemsets, using metrics like **lift** to identify which skills are commonly associated with one another.

### Key Insights:
- Skills like **Python**, **SQL**, and **Machine Learning** often appear together across job postings.
- These relationships can help organizations identify skills that are frequently required in combination for specific job titles.

## 2. Data Cleaning
- **Data Standardization**: The dataset was cleaned using regular expressions to standardize skill lists, city names, and job titles.
- **Unique Values**: We extracted the **unique cities** and **skills** from the dataset, providing insight into where jobs are located and which skills are in demand.
- **Inflation and Exchange Rate Data**: Inflation rates and exchange rates were added to a new dimension table (**dim_inflation**), which will be useful for future salary analysis.

### Key Findings:
- The **dim_skill** table contains all unique skills required for various job titles, mapped to unique skill IDs.
- The **dim_inflation** table shows inflation rates and exchange rates, which can help contextualize salary data.

## 3. Job and Skill Relationships
- **Bridge Table**: A bridge table (**job_bridge_skill**) was created to map job IDs to skill IDs, establishing a connection between job titles and required skills.
- This will allow for detailed analysis of how specific skills correlate with different job roles.

### Key Insights:
- By linking job titles to skills, we can better understand which skillsets are in high demand for specific roles.
- The bridge table will support detailed reporting and analysis, such as finding the most sought-after skills for each job title.

## Conclusion and Recommendations
- **For Job Seekers**: Learning high-demand skills such as Python, SQL, and Machine Learning will make you more competitive in the job market.
- **For Employers**: Identifying the most frequent skill combinations can help in designing targeted job descriptions and improving hiring strategies.
- **For Data Analysts**: Using the **job_bridge_skill** and **dim_skill** tables will allow for advanced analysis of the relationship between job titles and required skills.
