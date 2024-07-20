Project Objective

The client is a global nonprofit organization that supports unemployed individuals by training them for careers in various industries. The organization partners with employers to develop job-training programs that match the skills needed in the market. Since its inception, the organisation has focused on providing not only the technical skills required for specific roles but also the life skills and mindset necessary for long-term employment success.

The objective of this project is to clean, analyze, and derive actionable insights from the provided dataset. The analysis will include creating age groupings and generating key metrics related to employment rates and speed to employment for the organization. Insights will be presented in the form of graphs and statistics, with detailed explanations of the data cleaning steps and calculation methods used.

Data Prepation Steps

Each column was validated according to its data type as Number, Date and Text consistency and correct formatting.

Color-coded column headers for easier navigation and distinction among data types.

All date columns were reformatted from DDMMYYYY to MMDDYYYY format to align with regional data handling standards.

Created  'Age Group' column using the IF function and referencin data in the 'Age_at_Cohort_Start' column to enable segmented analysis based on age groups.

In the 'Cohort_City' column, the entry 'Kumasi' was recoded to 'Ashanti' to ensure consistency across the dataset. Same was done in the 'LocalRecruitmentChannel' (In-Person-Refferal).

Using the IF(ISBLANK()) function, the 'Days_to_Employment' column was created and populated by referencing the 'Attainment_Date' and 'Cohort_Graduation' columns.    

 Using the formula IF(AND(ISNUMBER())), the 'Employment_Status' column was generated based on the values in the 'Days_to_Employment' column, distinguishing employed from unemployed graduates.

The IF(OR()) function was employed to reference the 'Combined_Status' column for creating the 'Graduate_Status' column, categorizing each entry based on predefined criteria.

Utilized pivot tables to generate comprehensive graphs and charts for Total learners admitted across the three cohorts, Total number of graduates, Employment rates among graduates, Employment distribution by gender and age group, The top five learner recruitment channels, Average days to employment post-graduation for each age group across all three cohorts.

INSIGHTS

Data clearly shows the need for enhanced career services, through networking events, and  partnerships with local businesses to improve employment outcomes since only 55% of the graduates are employed from the 3 cohorts.

A comparative analysis of the WD_3_MEST_2 and WD_GEN_1 indicates that younger cohort members (18-24) take longer days in finding employment, therefore, career coaching and internship programs can be designed to to prepare learners for the job market. 

The variation in employment rate by gender suggests more strategies to ensure equitable opportunities for gender-focused career workshops.

Resources can be increased focusing on 'In-Person-Referral' and 'Other' channels of recruitment because of their effectiveness as compared to other methods of recruitment.
