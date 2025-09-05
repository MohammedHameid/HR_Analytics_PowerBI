# 📊 HR Analytics in Power BI

## 📌 Project Overview  
This project is an **HR Analytics Dashboard** built in **Power BI**.  
It provides HR teams with **data-driven insights** into employee performance, satisfaction, attrition, and training opportunities.  
The data is modeled in a **star schema** with fact and dimension tables (Employee, Education, Rating, Satisfaction).  

---

## 🎯 Business Questions Answered  
- What factors affect **employee satisfaction** and **attrition**?  
- How do **manager ratings vs self-ratings** compare?  
- Which departments have the highest **turnover**?  
- How does **training** impact employee performance and engagement?  

---

## 🛠️ Skills & Tools  
- **Power BI** → Data Modeling & DAX  
- **SQL** → Data extraction & transformations  
- **Data Visualization** → Building interactive dashboards  
- **HR Analytics** → Workforce planning & employee engagement  

---

## 🗂️ Data Model  

### 🔹 Fact Table: Performance  
| Column                         | Type   | Description |
|--------------------------------|--------|-------------|
| PerformanceID                  | text   | Unique performance review ID |
| EmployeeID                     | text   | Links to DimEmployee |
| ReviewDate                     | date   | Date of review |
| EnvironmentSatisfaction        | number | Employee environment satisfaction |
| JobSatisfaction                | number | Job role satisfaction |
| RelationshipSatisfaction       | number | Workplace relationship satisfaction |
| WorkLifeBalance                | number | Work-life balance rating |
| SelfRating                     | number | Self-assessed performance |
| ManagerRating                  | number | Manager-assessed performance |
| TrainingOpportunitiesWithinYear | number | Training opportunities available |
| TrainingOpportunitiesTaken     | number | Training opportunities taken |

---

### 🔹 Dimension Tables  

**Satisfied Level**  
| Column          | Type   | Description |
|-----------------|--------|-------------|
| SatisfactionID  | number | Unique ID |
| SatisfactionLevel | text | Very Satisfied, Satisfied, Neutral, Dissatisfied, Very Dissatisfied |

**Rating Level**  
| Column      | Type   | Description |
|-------------|--------|-------------|
| RatingID    | number | Unique ID |
| RatingLevel | text   | Above & Beyond, Exceeds Expectation, Meets Expectation, Needs Improvement, Unacceptable |

**Education Level**  
| Column           | Type   | Description |
|------------------|--------|-------------|
| EducationLevelID | number | Unique ID |
| EducationLevel   | text   | Doctorate, Masters, Bachelors, High School, No Formal Qualifications |

**Employee**  
| Column                  | Type   | Description |
|--------------------------|--------|-------------|
| EmployeeID               | text   | Unique employee ID |
| FirstName, LastName      | text   | Employee name |
| Gender                   | text   | Gender identity |
| Age                      | number | Current age |
| BusinessTravel           | text   | Frequent, Some Travel, No Travel |
| Department               | text   | Technology, HR, Sales |
| DistanceFromHome         | number | Distance in km |
| State                    | text   | Location |
| Ethnicity                | text   | Self-defined ethnicity |
| Education                | number | Education level (FK) |
| EducationField           | text   | Field of study |
| JobRole                  | text   | Current role |
| MaritalStatus            | text   | Marital status |
| Salary                   | number | Current salary |
| StockOptionLevel         | number | Stock option band |
| Overtime                 | text   | Yes/No |
| HireDate                 | date   | Joining date |
| Attrition                | text   | Yes/No |
| YearsAtCompany           | number | Years since joined |
| YearsInMostRecentRole    | number | Years in latest role |
| YearsSinceLastPromotion  | number | Time since last promotion |
| YearsWithCurrManager     | number | Years with current manager |

---

## 📷 Dashboard Preview  
![HR Analytics Dashboard](https://github.com/MohammedHameid/HR_Analytics_PowerBI/blob/main/HR%20Analytics%20Preview.jpeg)  

---

## 🔗 Links  
- 📂 **GitHub Repo** → [HR Analytics in Power BI](https://github.com/MohammedHameid/HR_Analytics_PowerBI)  
- 🌐 **Portfolio** → [My Portfolio](https://mohammedhameid.github.io/Portfolio/)  

---

## 🚀 Next Steps  
- Add **predictive analytics** for attrition risk using ML models.  
- Connect to **real-time HR data** instead of static datasets.  
- Build **interactive filters** for deeper drill-down analysis (e.g., by department, tenure).  
