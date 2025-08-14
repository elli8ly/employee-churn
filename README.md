# Employee Churn Prediction - HR Analytics

## Project Overview
This project leverages machine learning to analyze employee turnover patterns at a company. By examining key factors such as workload, performance evaluations, tenure, and job satisfaction, the goal was to build predictive models that identify employees at risk of leaving. The insights generated aim to help HR and leadership implement targeted retention strategies.

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
| Metric      | Random Forest Score |
|-------------|---------------------|
| Accuracy    | 96.2%               |
| Precision   | 87.0%               |
| Recall      | 90.4%               |

**Top predictive features:**
1. `last_evaluation`
2. `number_project` 
3. `tenure`
4. `overworked`

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

### Long-Term Strategies
- Pilot workload balancing in high-risk departments
- Manager training on burnout identification
- Culture shift toward work-life balance

## Next Steps
1. Present findings to HR/leadership
2. Refine models with additional data (employee surveys)
3. Monitor turnover rates post-intervention
4. Adjust strategies based on results

## Tools Used
- **Python Libraries**:
  - Pandas
  - Scikit-learn
  - Matplotlib/Seaborn
- **Models**:
  - Logistic Regression
  - Random Forest
  - XGBoost

[View Dataset on Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction)
