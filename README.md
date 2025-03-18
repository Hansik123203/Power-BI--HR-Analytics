# Power-BI--HR-Analytics
## HR Analytics - Employee Retention at Adecco India
### 🚀 Project Overview
This project analyzes employee attrition and identifies key factors influencing job satisfaction and retention at Adecco India. Using Power BI, the goal is to uncover insights that help reduce turnover and improve employee engagement.
### 📌 Business Problem
Adecco India, a technology company, is experiencing high employee turnover, particularly in the sales department among junior employees. This turnover results in reduced productivity, increased hiring costs, and low team morale.
### 🔍 Key Objectives
- Identify major factors contributing to employee attrition.
- Analyze job satisfaction, compensation, work-life balance, and other employee-related metrics.
- Provide data-driven recommendations to improve retention and engagement.
### 📊 Data Sources
The analysis is based on a publicly available HR dataset:
Dataset Link: https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study
### 🔄 Data Transformation Steps
### Data preprocessing was performed within Power Query Editor in Power BI:
1. Created Conditional Columns:
   - Age Group: Categorized employees into different age brackets.
   - Salary Slab: Grouped employees into income ranges.
2. Data Cleaning & Formatting:
   - Ensured all columns had appropriate data types.
   - Removed unnecessary columns to optimize performance.
   - Removed duplicate records to maintain data integrity.
### 📈 Power BI Dashboard Features
The Power BI dashboard provides an interactive view of HR metrics, including:
- Attrition Rate: Percentage of employees leaving over time.
- Department-Wise Turnover: Identifies high-risk departments.
- Job Satisfaction Analysis: Compares satisfaction levels across job roles.
- Income vs. Attrition Trends: Evaluates if compensation impacts retention.
- Work-Life Balance Insights: Examines how balance affects performance.
### 🛠️ Technology Used
- Power BI - Data visualization & interactive reporting.
### 🔢 DAX Measures Used
The following DAX measures were implemented in Power BI: <br> <br>
Attrition Rate = <br>
DIVIDE( <br>
    COUNTROWS(FILTER('HR data', 'HR data'[Attrition] = "Yes")), <br>
    COUNTROWS('HR data'), <br>
    0 <br>
) <br> <br>

Average Age = AVERAGE('HR data'[Age]) <br> <br>

Average Monthly Income = AVERAGE('HR data'[MonthlyIncome]) <br> <br>

Average working year = AVERAGE('HR data'[YearsAtCompany]) <br> <br>

Number of Attritions = <br>
COUNTROWS(FILTER('HR data', 'HR data'[Attrition] = "Yes")) <br>

### Total No. of employees = COUNTROWS('HR data')
🔮 Key Insights & Recommendations
✔️ High Attrition in Sales: Address concerns with better incentives & career growth.
✔️ Low Satisfaction in Certain Job Roles: Implement employee engagement programs.
✔️ Work-Life Balance Impacts Performance: Encourage flexible work arrangements.
✔️ Training & Development: More training opportunities reduce attrition.
### 💡 How to Use This Repository
1. Download the Power BI file (DACS12_HR_analytics.pbix) and open it in Power BI Desktop.
2. Explore interactive dashboards to analyze employee attrition trends.
3. Modify and extend the analysis with additional HR metrics.
### 🤝 Contributors
- Hansika Panchal - Data Analyst | Power BI Developer
- Contributions are welcome! Feel free to submit a pull request.
### 🏆 Acknowledgments
- Adecco India for the case study.
- Kaggle for providing the dataset.
