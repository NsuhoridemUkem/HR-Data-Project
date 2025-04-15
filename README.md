# HR-Data-Project
A comprehensive HR analytics dashboard project leveraging synthetic data and Tableau to visualize workforce trends, demographics, and salary insights for strategic decision-making.

Here’s the updated **README.md** with a clean and professional structure—no emojis, and a full table of contents included.

---

# HR Dashboard – Data Analysis & Visualization Project

## Table of Contents
1. [Project Overview](#project-overview)  
2. [User Story](#user-story)  
3. [Project Structure](#project-structure)  
4. [Dashboard Design](#dashboard-design)  
   - [Summary View](#summary-view)  
     - [Overview](#overview)  
     - [Demographics](#demographics)  
     - [Income Analysis](#income-analysis)  
   - [Employee Records View](#employee-records-view)  
5. [Data Generation Process](#data-generation-process)  
   - [Attributes Included](#attributes-included)  
   - [Code Features](#code-features)  
6. [Tools & Technologies](#tools--technologies)  
7. [Outcomes](#outcomes)
8. [Key Insights from the Dashboard](#key-insights-from-the-dashboard)
9. [Contact](#contact)  

---

## Project Overview

This project presents an end-to-end human resources analytics solution using Tableau for visualization and ChatGPT for synthetic data generation. The goal is to provide HR professionals with a comprehensive, interactive dashboard to monitor and explore key HR metrics at a glance, along with detailed employee-level insights.

---

## User Story

> As an HR manager, I want a comprehensive dashboard to analyze human resources data, providing both summary views for high-level insights and detailed employee records for in-depth analysis.

---

## Project Structure

- `hr_dashboard.twbx`: Tableau Workbook File  
- `hr_dataset.csv`: Generated dataset with 8,950 realistic HR records  
- `data_generation_script.py`: Python script used to generate the dataset  
- `README.md`: Project summary and usage guide  

---

## Dashboard Design

### Summary View

Divided into Overview, Demographics, and Income Analysis to cater to strategic and operational HR insights.

#### Overview
- Total count of hired, active, and terminated employees  
- Year-over-year trends of hires vs. terminations  
- Department-wise and job title-wise employee distribution  
- Comparison of total employees in HQ (New York) versus other branches  
- Geographic distribution by city and state  

#### Demographics
- Gender ratio of employees  
- Distribution across age groups and education levels  
- Count of employees per age bracket and education tier  
- Correlation analysis between education level and performance rating  

#### Income Analysis
- Salary comparison across education levels for male vs. female employees  
- Age vs. salary trends across different departments  
- Departmental income distribution for compensation planning

  ![HR Summary View](https://github.com/user-attachments/assets/78c1067f-6e9c-430f-90fa-4fe164a0667a)


### Employee Records View

A fully filterable table containing:
- Name, Gender, Age  
- Department, Job Title  
- Education Level, Performance Rating  
- Salary and Adjusted Salary

  ![HR  Employee Detailes](https://github.com/user-attachments/assets/084e5e19-0c41-4bbb-b1ae-b9232ccee314)


---

## Data Generation Process

Synthetic data was generated using Python with ChatGPT assistance to simulate a realistic HR dataset.

### Attributes Included
- Employee ID, First & Last Name  
- Gender (46% Female, 54% Male)  
- State & City (from predefined U.S. locations)  
- Hire Date (weighted from 2015 to 2024)  
- Department (with department-specific probabilities)  
- Job Title (dependent on department)  
- Education Level (mapped to job titles)  
- Performance Rating (weighted random)  
- Overtime (30% Yes, 70% No)  
- Salary (range based on job and department)  
- Birth Date (aligned with realistic age & hire date)  
- Termination Date (assigned to 11.2% with constraints)  
- Adjusted Salary (derived using age, education, gender-based adjustments)  

### Code Features
- Modular design using Python functions  
- Clean structure with descriptive comments  
- Probabilistic modeling for real-world data realism  
- Output as a CSV file used in Tableau  

---

## Tools & Technologies

- ChatGPT: Prompt-engineered for dataset structure and logic  
- Python: Data generation and preprocessing  
- Tableau: Interactive dashboard development  
- GitHub: Version control and project showcase  

---

## Outcomes

- A reusable framework for generating large, realistic HR datasets  
- A dynamic, user-friendly dashboard suited for HR executives  
- Insights that support employee retention, performance management, and pay equity analysis
  
---

## Key Insights from the Dashboard

- Hiring Trends Over Time: Hiring peaked in 2021 before slowing in 2023, suggesting market or budget-related adjustments.
- Departmental Distribution: Engineering and Customer Support lead in headcount, revealing focus areas.
- Branch vs HQ Staffing: New York HQ employs over 60% of staff; branches add diversity across the U.S.
- Workforce Demographics: Balanced gender ratio; most employees are aged 30–45 with a Bachelor's degree.
- Performance vs Education: Master's degree holders often perform better in managerial roles.
- Salary Insights: Salaries rise with education, though gender-based discrepancies exist in some departments.
- Employee Attrition: 11% attrition rate; Customer Support and Sales have higher churn, often within 2 years.

---

## Full Dashboard

To view the dashboard, click the link: https://public.tableau.com/views/HRTableauDashboard_17358400811890/HRSummary?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

---

## Contact

For questions, improvements, or collaboration, feel free to reach out or connect via LinkedIn: https://www.linkedin.com/in/nsuhoridem-ukem
