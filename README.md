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
1. **Data Source**: [HR_Employee_Dataset](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/20a51a91a18969990e283af127c025a1bc142abe/HR_Analysis/HR_Employee_Dataset.csv)

2. **Data Dictionary**: [HR_Dataset_Data_Dictionary](https://github.com/Adabusonma/HR-Analytics-Dashboard/blob/20a51a91a18969990e283af127c025a1bc142abe/HR_Analysis/HR_Dataset_Data%20Dictionary.docx)

3.**Data description**
 | Category | Columns |
 |---|---|
 | **Identity & Demographics** | Employee_ID, Full_Name, Gender, Age, Marital_Status, Number_of_Dependents, State_of_Origin |
 | **Role & Structure** | Education_Level, Department, Job_Title, Job_Level, Employment_Type, Work_Location |
 | **Tenure** | Hire_Date, Years_of_Service, Years_Since_Last_Promotion |
 | **Compensation** | Monthly_Salary_NGN |
 | **Performance & Engagement** | Performance_Rating, Job_Satisfaction_Score, Employee_Engagement_Score, Training_Hours_Per_Year |
 | **Risk Indicators** | Overtime_Flag, Absences_Per_Year, **Attrition** |




