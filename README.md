# HR Analytics Dashboard

## **Introduction**
This project is an interactive HR Analytics Dashboard built in Power BI to help organisations monitor workforce performance, understand employee demographics, and identify the key factors driving employee attrition and retention. It demonstrates the complete analytics workflow, including data cleaning, data modeling, DAX calculations, and dashboard design to support data-driven HR decisions.
<br>
## **Business Problem**
Employee attrition is a significant workforce challenge that impacts productivity, increases recruitment costs, and disrupts business operations. Without understanding why employees leave, organisations struggle to implement effective retention strategies.
The HR department needs a data-driven solution to identify the key drivers of attrition and workforce engagement. This project aims to analyse the HR data to answer critical business questions, including:
- Which departments experience the highest attrition rates?.
- Which employee groups (job level, age, gender, salary band) are most at risk of leaving?.
- How do job satisfaction and employee engagement differ between employees who stayed and those who left?.
- Is there a relationship between overtime, absenteeism, and employee attrition?.
- Does training contribute to improved employee performance?.
- Which departments have the highest employee retention rates?.
- How do performance ratings vary across different employee groups?.
## **Project Objectives**
To design an interactive HR Analytics dashboard that enables HR leaders to:
- Monitor workforce and attrition KPIs in real time.
- Identify high-risk departments and employee segments.
- Analyse workforce demographics, performance, engagement, and retention.
- Support evidence-based decisions that improve employee retention and organisational performance.
## **Power BI Dashboard Snapshots**
The dashboard provides comprehensive insights across the following pages:
1. **Workforce Overview & Dempgraphic Page**: Displays headcount, employee distribution, salary, and workforce composition.
    ![Workforce Overview & Demographic](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/c96780dddec426bf8518c01f673b71ff6c4aead3/HR_Analysis/Workforce%20Overview%20%26%20Demographic_Page.png)
    
2. **Compensation & Performance Page**: Displays employees compensation, performance ratings, training, and engagement analysis.
    ![Workforce Overview & Demographic](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/83511423daa87713048f88a508d74de60ab106ea/HR_Analysis/Compensation%20%26%20Performance.png)

3. **Attrition & Retention Page**: Displays Attrition trends, retention metrics, and analysis of the factors influencing employee turnover.
    ![Workforce Overview & Demographic](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/a585a089c30ad72ef430af35625cb484d9164fda/HR_Analysis/Attrition%20%26%20Retention%20Analysis.png)
    
## **Dataset Overview**
1. **Dataset Source**: [HR_Employee_Dataset](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/20a51a91a18969990e283af127c025a1bc142abe/HR_Analysis/HR_Employee_Dataset.csv)

2. **Dataset Dictionary**: [HR_Dataset_Data_Dictionary](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/20a51a91a18969990e283af127c025a1bc142abe/HR_Analysis/HR_Dataset_Data%20Dictionary.docx)

 3.**Dataset description** :
 | Category | Columns |
 |---|---|
 | **Identity & Demographics** | Employee_ID, Full_Name, Gender, Age, Marital_Status, Number_of_Dependents, State_of_Origin |
 | **Role & Structure** | Education_Level, Department, Job_Title, Job_Level, Employment_Type, Work_Location |
 | **Tenure** | Hire_Date, Years_of_Service, Years_Since_Last_Promotion |
 | **Compensation** | Monthly_Salary_NGN |
 | **Performance & Engagement** | Performance_Rating, Job_Satisfaction_Score, Employee_Engagement_Score, Training_Hours_Per_Year |
 | **Risk Indicators** | Overtime_Flag, Absences_Per_Year, **Attrition** |
 
 ## **Dataset Cleaning** 
 The dataset cleaning was performed in **Power Query**
 1. **Remove Duplicates** : Removed 50 exact duplicate rows using `Employee_ID` as the unique identifier.
 2. **Fixed Typos in Categorical Columns** : Standardised inconsistent casing and corrected geographic misspellings.
 3. **Impute Missing Values** : The columns that had nissing values had a threshold of **5%**.


| Column | Missing % | Method | Justification |
|---|---|---|---|
| `Job_Satisfaction_Score` | 2.5% | **Column median** | Ordinal 1–5 scale. Median preserves integer-like nature and is robust to skew. |
| `Training_Hours_Per_Year` | 2.0% | **Column median** | Right-skewed distribution. Median more representative than mean. |
| `Education_Level` | 3.0% | **Mode (B.Sc/B.A)** |  Majority of employees hold a first degree. Mode imputation minimises distribution distortion. |
| `Marital_Status` | 2.0% | **"Unknown"** | Imputing the mode (Married) would misrepresent individual profiles and artificially inflate one group's count. |

## Data Model
The data model follows a **star schema pattern** .One central fact table connected to four dimension tables. This structure separates measurable metrics from descriptive attributes, enabling efficient DAX computation and clean dimensional filtering.

![Data Model](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/373a8ccb34f8c036b52740dadaaf6c03fd68fcfe/HR_Analysis/Data%20Model.png)

## **Key Insights**
The dashboard provides insights to:
- **Workforce Stability** : The organization retains 82% of its workforce, with an 18% attrition rate, indicating opportunities to strengthen employee retention.
- **High-Risk Department** : Customer Service recorded the highest attrition (22%), making it the primary focus for retention initiatives.
- **Experienced Talent Loss** : Employees with 11–15 years of tenure have the highest attrition (19%), highlighting the need to retain experienced talent.
- **Performance & Training** : Employees get about the same amount of training (23.5 hours) no matter how well they perform. This means more training hours alone doesn't lead to better performance.
- **Career Development** :Junior employees have the highest attrition (26%), indicating challenges in retaining early-career talent.
- **Overtime & Absenteeism** : Employees with high absenteeism and overtime show a slightly higher risk of leaving, indicating potential burnout.
-  **Employee Satisfaction** : Employee satisfaction averaging 3.4/5 remains consistent across departments, suggesting that other factors drive employee retention and performance.

By leveraging on these insights,the HR department can identify workforce trends, improve employee retention and support smarter, data-driven HR decisions.

## **Resource Guide**
Executive report : [HR_Executive_report_analysis](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/94c6779e7ebf45cc7316d6f126589413f8b2b212/HR_Analysis/HR_Executive_report_analysis.pdf)

## **Author**
**Adaeze Princess Ekwuruke**    
- **LinkedIn**: [Connect with Me](www.linkedin.com/in/adaeze-ekwuruke)  





