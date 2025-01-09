# Automation of Regulatory Document Reviews in Pharmaceutical Development

This project focuses on creating an automated system to streamline the review of regulatory documents, optimizing the Design History File (DHF) review process for improved quality and compliance. The system leverages Python-based data processing and analytics to identify compliance gaps, conduct root cause analysis, and generate actionable insights.

---

## Project Goals

1. **Automate Document Review**: Build a system that processes and analyzes regulatory document datasets for compliance validation.
2. **Handle Real-World Challenges**: Simulate a complex dataset with missing values and non-linear patterns to reflect real-world scenarios.
3. **Insights and Reporting**: Generate actionable insights, including compliance metrics and root causes of non-compliance.
4. **Scalability**: Develop a modular and scalable framework that can adapt to various document types and volumes.

---

## Features

1. **Data Preprocessing**:
   - Handles missing data intelligently (e.g., filling null values with mean or default values).
   - Engineers additional features, such as composite compliance scores.

2. **Compliance Analysis**:
   - Evaluates documents based on predefined rules.
   - Categorizes documents as "Compliant," "Partially Compliant," or "Non-Compliant."

3. **Root Cause Analysis**:
   - Identifies common reasons for non-compliance.
   - Groups non-compliant documents by critical parameters like risk level and design input.

4. **Visualization**:
   - Generates bar charts and boxplots to visualize compliance status and risk assessment impacts.

5. **Reporting**:
   - Saves detailed reports on compliance analysis and non-compliant documents.

---

## Workflow

### 1. Dataset Generation
A simulated dataset was created with the following structure:
- **Fields**: Document ID, Design Input, Risk Assessment, Compliance Score, Critical Issues, Last Reviewed Date.
- **Challenges Simulated**: Missing values, categorical data, numerical data, and non-linear relationships.

### 2. Data Preprocessing
- Filled missing values in fields like Design Input, Risk Assessment, and Compliance Score.
- Engineered a **Composite Compliance Score** based on risk weight, compliance score, and critical issues.

### 3. Compliance Analysis
- Applied rules to classify documents into three categories:
  - **Compliant**: High composite score and valid design input.
  - **Partially Compliant**: Medium composite score.
  - **Non-Compliant**: Low composite score or high risk.

### 4. Root Cause Analysis
- Analyzed common root causes for non-compliance, such as invalid design input or high risk assessment.

### 5. Visualization
- Generated visualizations to support insights:
  - **Compliance Status Distribution** (Bar Chart).
  - **Impact of Risk Assessment on Composite Score** (Boxplot).

### 6. Reporting
- Generated the following reports:
  - `final_compliance_report.csv`: Full dataset with compliance insights.
  - `non_compliant_docs.csv`: Dataset of non-compliant documents.
  - `compliance_status.png`: Visualization of compliance status distribution.

---

## Results

1. **Compliance Summary**:
   - Majority of documents are "Partially Compliant" (as shown in the bar chart).
   - Non-compliant documents are flagged and analyzed for intervention.

2. **Root Cause Insights**:
   - Invalid design inputs and high-risk assessments were the most common factors leading to non-compliance.

3. **Automation Success**:
   - The system effectively processed a large dataset, generated compliance classifications, and provided actionable insights.

---

## Files and Outputs

1. **Reports**:
   - [Final Compliance Report](./final_compliance_report.csv): Comprehensive report with compliance statuses.
   - [Non-Compliant Documents](./non_compliant_docs.csv): Dataset of flagged non-compliant documents.

2. **Visualizations**:
   - [Compliance Status Chart](./compliance_status.png): Bar chart showing compliance distribution.

---

## Future Enhancements

1. **Integration with Real Datasets**:
   - Extend the system to handle real regulatory documents (e.g., PDFs, text files).
   - Use NLP techniques to parse and analyze textual content.

2. **Advanced Analytics**:
   - Incorporate machine learning to predict non-compliance based on historical data.
   - Automate risk categorization using clustering algorithms.

3. **Scalability**:
   - Optimize the framework for processing larger datasets with distributed computing.

---

## Conclusion

This project demonstrates the successful automation of regulatory document reviews, providing a robust framework for compliance analysis and reporting. The system is adaptable, scalable, and serves as a foundation for future enhancements.

