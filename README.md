# employee-churn
HR Analytics: Predicting Employee Turnover
Project Overview
This project leverages machine learning to analyze employee turnover patterns at a company. By examining key factors such as workload, performance evaluations, tenure, and job satisfaction, the goal was to build predictive models that identify employees at risk of leaving. The insights generated aim to help HR and leadership implement targeted retention strategies.

Key Findings
Overwork is a major driver of attrition: Employees with excessive workloads (especially those handling 6+ projects or working >175 hours/month) showed significantly higher turnover rates.

Performance evaluations impact retention: Employees with high evaluation scores but unsustainable hours were likely to quit, while those with low scores were at risk of being fired.

Tenure matters: Employees with 3–6 years of tenure exhibited a "retention cliff," often leaving due to burnout or lack of advancement opportunities.

Model performance:

Random Forest achieved 96.2% accuracy, 87.0% precision, and 90.4% recall in predicting turnover.

Top predictive features: last_evaluation, number_project, tenure, and overworked.

Recommendations
Immediate Actions
Workload Management

Cap projects per employee (3–4 projects optimal).

Implement alerts for employees exceeding 175 hours/month.

Performance & Recognition

Revise evaluation criteria to reward sustainable performance, not just output volume.

Address "high performer burnout" with career path discussions.

Targeted Retention for Critical Tenures

Focus on employees with 3–6 years of tenure (e.g., promotions, mentorship).

Long-Term Strategies
Pilot Workload Balancing: Test in high-risk departments and measure turnover impact.

Manager Training: Equip leaders to identify burnout and redistribute workloads.

Culture Shift: Promote work-life balance through policies and leadership messaging.

Next Steps
Share Insights: Present findings to HR/leadership to align on priority interventions.

Refine Models: Incorporate additional data (e.g., employee surveys) to improve predictions.

Monitor & Iterate: Track turnover rates post-intervention and adjust strategies.

Tools Used: Python (Pandas, Scikit-learn, Matplotlib/Seaborn), Logistic Regression, Random Forest, XGBoost.
