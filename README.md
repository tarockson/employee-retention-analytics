# Employee Retention Analytics
## Predictive Modeling & Risk Identification

### Overview
Built a machine learning model to predict which employees are at risk of leaving 
before they depart. Combines HRIS data, engagement survey sentiment scores, and 
exit interview analysis to identify actionable retention opportunities.

### Business Problem
Organizations lose $15,000-$40,000 per employee departure through recruiting, 
training, lost productivity, and institutional knowledge loss. Identifying at-risk 
employees enables proactive retention interventions.

### Key Results
- **Model Accuracy**: 74% (ROC AUC)
- **At-Risk Employees Identified**: ~165 out of ~900
- **Estimated Savings**: $1.25M-$2.5M (if recommendations implemented)
- **Primary Risk Factor**: Tenure in first 2 years (59% importance)

### Key Finding
Employees in their first 2 years leave at **5 times the rate** of those with 2+ 
years tenure. The dominant retention lever is **first-year experience**, not 
compensation.

### What's Included
- `employee_retention_and_culture_analysis.ipynb` - Complete analysis covering both projects
- `index.html` - Interactive visualization of results
- `sample_hris_anonymized.csv` - Example retention dataset
- `CASE_STUDY.md` - Detailed methodology and findings

### How to Run This Project

**Option 1: View the Notebook Online**
Simply click on `employee_retention_and_culture_analysis.ipynb` to view the entire analysis.

**Option 2: Run Locally**
1. Clone this repository:
```bash
   git clone https://github.com/YOUR-USERNAME/employee-retention-analytics.git
   cd employee-retention-analytics
```

2. Install dependencies:
```bash
   pip install -r requirements.txt
```

3. Start Jupyter:
```bash
   jupyter notebook
```

4. Open `notebooks/employee_retention_and_culture_analysis.ipynb`

5. View dashboard: [Retention Analytics project](https://tarockson.github.io/employee-retention-analytics/)

### Data
- **HRIS Dataset**: ~900 employees, 3+ years of history (anonymized)
- **Engagement Surveys**: Department-level sentiment scores (3,120+ comments)
- **Exit Interviews**: 50+ departures coded for themes
- Sample data provided in `data/` folder

### Methodology
**Feature Engineering**: Tenure years, engagement score, department, job title
**Models Tested**: Logistic Regression, Random Forest, XGBoost
**Model Selected**: Random Forest (74% ROC AUC)
**Validation**: 20% hold-out test set, stratified split

### Key Recommendations
1. **Immediate** (30 days): Audit 90-day onboarding program
2. **Short-term** (60-90 days): Launch supervisor training and onboarding redesign
3. **Long-term** (6-12 months): Implement career pathways and accountability metrics

### ROI
- Investment: $100K
- At-Risk Population: ~165 employees
- Risk Exposure: $4.15M
- Conservative Scenario: Keep 50 = $1.25M saved (1,250% ROI)
- Realistic Scenario: Keep 75-100 = $1.875M-$2.5M saved (1,875%-2,500% ROI)

### Technologies Used
- Python 3.9+
- pandas, scikit-learn, XGBoost
- Jupyter notebooks
- HTML/JavaScript dashboard

### Notes
- Data has been anonymized to protect the organization
- Analysis demonstrates end-to-end data science workflow
- For detailed methodology and findings, see [`CASE_STUDY.md`](https://github.com/tarockson/employee-retention-analytics/blob/main/case_study/CASE_STUDY.md)

## 📊 Interactive Dashboard

View the combined interactive dashboard in the 
[Retention Analytics project](https://tarockson.github.io/employee-retention-analytics/)

### Questions?
Feel free to open an issue or contact me.

### License
MIT License - See LICENSE file for details
