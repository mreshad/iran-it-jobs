
# Full Analysis of IT Job Data Extraction and Web Crawling

## 1. Job Data Extraction
- **Job Title**: Extracted for each job posting to help identify roles in demand.
- **Experience Level**: Collected to understand the type of experience required for various positions.
- **Location**: Cities of job postings were scraped to map out regional demand for specific roles.
- **Company Details**: Information such as company name, remote working options, and company size was captured.
- **Salary Information**: Salaries were extracted and parsed to estimate earnings for different roles.
- **Skills Required**: Key technical skills required for each job were identified and matched against a predefined list (Python, Java, SQL, etc.).
- **Gender Preference**: Gender preferences (if any) were noted for job roles.
  
## 2. Web Scraping Process
- **Selenium** was used to navigate through multiple pages of job listings, simulating human interaction with the website.
- The notebook handles **pagination** and extracts job data from each available page (up to 40 pages).
- The **HTML source code** was saved in case of scraping errors to allow for debugging.

### Key Insights:
- Skills such as **Python**, **Java**, **SQL**, and **React** were frequently mentioned in job postings.
- A variety of roles, from junior to senior positions, were identified, helping job seekers tailor their job search based on experience level.

## 3. Data Cleaning and Saving
- The extracted data was saved in a **CSV file** (`it_jobs_jobinja_quick_test.csv`) for further analysis.
- The dataset includes detailed information for each job posting, ready for analysis of salary trends, skill demand, and regional job distribution.

## Conclusion and Recommendations
- **For Job Seekers**: Identifying high-demand skills like **Python**, **Java**, and **SQL** can increase your chances of finding relevant roles.
- **For Employers**: Understanding the gender preferences and location trends can help design more inclusive and targeted job ads.
- **For Data Analysts**: The CSV file can be used for deeper analysis, such as identifying salary trends, skill gaps, or popular job titles in different regions.
