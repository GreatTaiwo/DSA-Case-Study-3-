# DSA-Case-Study-3

This is a project from Digital Skillup Africa (DSA) Data Analysis Class with the Incubator Hub. The training focused on Microsoft Excel, SQL and Power BI. This particular repository is for the Capstone Project titled Case study 3, a Power BI project.  

## Project Topic: Case Study 3: Palmora Group HR Analysis

### Project Overview

The company under review is the Palmoria Group; a manufacturing company that has been accused as a manufacturing patriarchy with gender pay gaps, amongst other possible issues. As a HR analytic expert, the company’s HR data was analysed, to come up with recommendations for management’s attention. This project aims to analyse the company data and generate insights that the Palmoria group management team would need to address, with focus on gender-related issues within the organization and its regions. The following are the analysis tasks:
1. What is the gender distribution in the organization? Distil to regions and departments
2. Show insights on ratings based on gender
3. Analyse the company’s salary structure. Identify if there is a gender pay gap. If there is, identify the department and regions that should be the focus of management
4. A recent regulation was adopted which requires manufacturing companies to pay
employees a minimum of $90,000
- Does Palmoria meet this requirement?
- Show the pay distribution of employees grouped by a band of $10,000. For example:
- How many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000, etc.
- Also visualize this by regions.
5. 	The annual bonus pay to employees based on the performance rating (using bonus rules made available by the company)
a.	Calculate the amount to be paid as a bonus to individual employees.
b.	Calculate the total amount to be paid to individual employees (salary inclusive of bonus) 
c.	Total amount to be paid out per region and company-wide.

## Data Sources

The primary source of the data used were Palmoria Group emp-data, and Palmoria Group Bonus Rules, a Microsoft Excel (.xls) Worksheet. 

## Tools Used
Microsoft Power BI for Data transformation and analysis [Download here](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads) or install directly from Microsoft store, which is strongly adviced.

## Data Cleaning and Preparation

1. There are two genders in the organization. However, some employees refused to disclose their gender.
2. Conditional column was created for gender, where all blanks under the initial gender were made N/A (Not applicable) as a generic gender status to these employees that did not mention and others remained the same (Female/Male).
3. Some employees were taken out from the dataset because they were without a salary, which indicated that they were no longer with the company.
4. Lastly, some departments were taken out because they were indicated as "NULL".
All these reduced the dataset from over a thousand (+1000) rows, to eight hundred and ninety nine (874).

## Data Analysis 

The cleaned data was worked on by creating charts were necessary and creating conditional columns as in the case of salary band, salary band sort (to arrange the salary band from low range to the highest range). To work on the bonus rules made available, the data was worked on in Excel, using VLOOKUP to determine the value of bonus to be assigned to each employee based on the ratings. The Bonus amount was achieved by using = [salary]*[Bonus value], while the total amount was achieved using = [salary]*[Bonus value]+[salary]. The gender distribution by region and department was described with clustered column chart, focus was on those that specified their gender, although the chart showed those that did not.
The gender distribution in regions showed that Kaduna branch had more males (172) than females (151) while Abuja had equal gender and Lagos having three (3) males more than the females, which can be said to be balanced unlike Kaduna with twenty-one (21) differences. This could be due to distance, it is usually convenient for men to work far from home, which might not be convenient for women especially if married. The following departments had more males than females (differences are in bracket): Legal (8), Sales (7), Support (11), Accounting (9). Females were more in Research & Development (4), Human Resource (4), Business Development (5), Services (4). Differences in salary was discovered among genders, males were well paid in certain departments such as legal, product management, support, sales, and accounting. There are some departments where females had more salary but the difference between males was not much. The company have to work on those department where there is gender pay gap and try to balance their pay by probably training the females if they believe the males are more skilled. Although the ratings showed that females were rated better than males which should mean more pay but that is not the case. Finally, the Palmoria group did not meet the requirement of a minimum salary of $90,000, this is evident in the minimum salary chart, showing that some employees received lower than $90,000.

