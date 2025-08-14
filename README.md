# Employee Churn Prediction - HR Analytics

## Project Overview
This project leverages machine learning to analyze employee turnover patterns. Through exploratory data analysis and feature engineering, we built predictive models to identify at-risk employees and provide actionable insights for retention strategies.

## Key Features & Engineering

## Tools Used
- **Python Libraries**:
  - Pandas
  - Scikit-learn
  - Matplotlib/Seaborn
- **Models**:
  - Logistic Regression
  - Random Forest

### Engineered Features:
- **`overworked`**: Created binary flag (1/0) for employees working >175 hrs/month
- **Tenure bands**: Analyzed turnover patterns by tenure groups
- **Interaction terms**: Examined relationships between projects/hours/satisfaction

### Data Processing:
- Handled class imbalance (83% stay vs 17% leave)
- Removed duplicates and outliers in tenure data
- Encoded categorical variables (department, salary)

## Key Findings

### Workload Impact
- Employees with excessive workloads (especially those handling 6+ projects or working >175 hours/month) showed significantly higher turnover rates

### Performance Evaluation Patterns
- Employees with high evaluation scores but unsustainable hours were likely to quit
- Those with low scores were at risk of being fired

### Tenure Analysis
- Employees with 3-6 years of tenure exhibited a "retention cliff"
- Common reasons for leaving included burnout and lack of advancement opportunities

### Model Performance
| Metric      | Random Forest Score | Logistic Regression |
|-------------|---------------------|---------------------|
| Accuracy    | 96.2%               | 82%                 |
| Precision   | 87.0%               | 90%                 |
| Recall      | 90.4%               | 82%                 |
| F1-Score    | 88.7%               | 84%                 |
| AUC-ROC     | 93.8%               | 88.2%               |

**Top predictive features:**
1. `last_evaluation` (0.32 importance)
2. `number_project` (0.28) 
3. `tenure` (0.19)
4. `overworked` (0.15)

## Recommendations

### Immediate Actions
1. **Workload Management**
   - Cap projects per employee (3-4 projects optimal)
   - Implement alerts for employees exceeding 175 hours/month

2. **Performance & Recognition**
   - Revise evaluation criteria to reward sustainable performance
   - Address "high performer burnout" with career path discussions

3. **Targeted Retention**
   - Focus retention efforts on employees with 3-6 years tenure
   - Implement mentorship and promotion pathways

## Next Steps
1. **Validation**  
   - Present findings to executive team
   - Conduct focus groups with high-risk employees

2. **Implementation**  
   - Pilot in Sales & Engineering (highest turnover)
   - Develop manager dashboard with risk alerts

3. **Monitoring**  
   - Track key metrics monthly:
     - Turnover rate
     - Average projects/hours
     - Promotion velocity
