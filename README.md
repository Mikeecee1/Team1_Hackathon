# Project Credit Card Customer Churn Analysis

This project aims to predict credit card customer churn, enabling the bank to focus retention efforts on at-risk customers. We will analyse customer data, develop predictive models, and provide actionable insights through an interactive Power BI dashboard to support timely and targeted retention strategies.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

- `BankChurners.csv` downloaded from [Kaggle](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data)
- The dataset contains customer demographics, credit card usage details, credit limit, balance, and transaction history.

## Business Requirements

- Identify customers at risk of churning to enable the development of proactive retention strategies.
- Understanding the factors contributing to churn will help the bank enhance its services and increase customer satisfaction.
- Develop dashboards to visualize churn patterns and support targeted, data-driven decision-making.

## Hypothesis and how to validate?

Key takeaways for churn risk: **(1)** Customers with higher education or income are less likely to churn. **(2)** High card utilisation raises churn risk. **(3)** Older customers are less likely to churn. **(4)** More inactive months and fewer transactions both increase churn risk. **(5)** Marital status and number of dependents may also affect churn.

## Project Plan

1. The team selected the Credit Card Customer Churn Analysis project, defined its scope, set up collaborative workspaces and project management boards, and clarified deliverables.

2. The dataset was obtained from Kaggle and explored to generate initial insights and develop an understanding of its features.

## The rationale to map the business requirements to the Data Visualisations

### Business Requirement 1: Identify at-risk customers

We use cleaned and transformed customer data to identify factors linked to churn, helping to highlight at-risk customers and inform retention strategies.

- **Customer churn Dashboard:** Interactive filters to identify high-risk customers by demographics and behavior

### Business Requirement 2: Understand churn factors

We will create visualisations of behaviors and patterns linked to churn to clearly communicate the underlying drivers of customer departure.

- **Feature Importance Charts:** Bar charts showing which factors most influence churn decisions
- **Correlation Matrix:** Heatmap displaying relationships between variables and churn
- **Distribution Analysis:** Histograms and box plots comparing the distiriubution of key features for churned vs. retained customers.

### Business Requirement 3: Enable data-driven decisions

We will present advanced analytics in executive dashboards to support actionable, data-driven decisions.

- **Executive Summary Dashboard:** KPIs and trends for leadership decisions
- **Segment Analysis Views:** Churn rates by customer segments (income, age, card type)

## Analysis techniques used

### Data Analysis Methods

1. **Exploratory Data Analysis (EDA)**

   - Statistical summaries and distribution analysis
   - Correlation analysis to identify relationships between variables
   - Missing value analysis and data quality assessment
   - Use of y-data to gain deeper insights into datasets, including correlations and interactions
   - Did a chi-square test to check the independence of categorical variables.

2. **Feature Engineering**

   - Since most of the data was cleaned with no missing values, we did very basic feature engineering.
   - Categorical encoding the age into groups for better anaysis in visualisations.
   - Basic outlier detection and treatment using IQR method.

### Structure and Justification

The analysis was structured in 3 phases:

1. **Data Preparation & Cleaning**: Raw customer data was cleaned, transformed, and grouped to ensure consistency and enable meaningful analysis.
2. **Descriptive Analytics**: Conducted basic EDA , Y-datat profiling to find patterns and trends, Chi-square test to check independenc of categorical variables. 
3. **Visualization** : Created basic boxplots, histograms, correlation heatmaps to understand the data better, validate hypothesis and communicate findings effectively.
Created dashboards in Power BI to present insights.


### Data Limitations and Alternative Approaches

- **Limitation**: The dataset was relatively small and clean, with no major quality issues.
Some categorical fields contained "Unknown" values.
-**Mitigation**: Retained "Unknown" entries and treated them as a separate category to preserve data integrity.

### Generative AI Usage

- **Ideation**: Used AI for ideation and analysis and visualisation suggestions.
- **Markdown**: co-pilot assisted in writing and formatting markdown content.

## Ethical considerations

### Data Privacy Issues

- **Challenge**: Customer financial data contains sensitive personal information
- **Mitigation**: Implemented data anonymisation techniques and removed direct identifiers
- **Compliance**: Ensured adherence to GDPR and banking data protection regulations

### Bias and Fairness

- **Identified Bias**: Possible demographic discrimination (age, gender, income).
- **Fairness Measures**: Implemented fairness metrics to ensure equal treatment across demographic groups
- **Model Auditing**: Regular bias testing across different customer segments

### Legal and Societal Considerations

- **Transparency**: Developed explainable AI models to ensure decision transparency.
- **Customer Rights**: Established ways for customers to review and challenge decisions.
- **Responsible AI**: Established guidelines for ethical use of churn predictions in customer interactions.

## Dashboard Design

### Page 1: Executive Overview

**Content**: High-level KPIs and summary metrics

- **Visuals**: 
      * customer count cards and summary cards.
      * Pie chart showing the proportion of churned vs retained customers.
      *  Scatter plot showing churn rate vs age.
      * Bar chart showing the churn count by card category.

- **Interactive Elements**: Slicers for Income Category, Card Category, Gender.


### Page 2: Demographic Insights

**Content**: Detailed breakdown of churn patterns by demographic factors.

- **Visuals**: 
      * Bar charts showing churn rate (%) by gender, education level, and income category.
      * A pie chart showing the churn distribution by marital status.

- **Interactive Elements**: Slicers for Income Category, Card Category, Gender.

### Page 3: Behavioral Insights

**Content**: Analysis of customer behavior and its impact on churn.

**Visuals**: 
- scatter plot showing churn rate vs months inactive.
- Bar chart showing the churn rate by avg utilisation ratio of credit limit.
- Line and clustered column chart showing churn rate and transaction amount by transaction counts (with tooltip showing the statistical summary).


### Communication Strategy

- For audience less familiar with technical details, the clear visuals should help communicate key insights effectively.
- The use of summary cards and KPIs on the executive overview page will highlight the most critical information at a glance.
- Clear labelling and legends on charts will aid interpretation.
- The use of interactive design and slicers will enable users to explore data independently.

## Unfixed Bugs

### Known Issues

**Dashboard Performance with Large Datasets**
   - **Issue**: The dashboard experiences slow loading times when applying filters across all customer records.
   - **Reason Not Fixed**: Power BI has limitations in handling very large datasets in real time, and further optimisation or aggregation strategies are required.

### Knowledge Gaps Addressed

- **Initial Gap**: Limited understanding of how to reorder categories on the x-axis of bar charts in Power BI.
  - **Solution**: Learned and applied techniques for reordering categories on the x-axis to improve clarity and accuracy of visualisations.

## Development Roadmap

### Challenges Faced

1. **Data Quality Issues**

   - **Challenge**: Some categorical fields contained "Unknown" values.
   - **Strategy**: Developed robust data cleaning pipelines and validation rules

2. **Working Collaborative Using Git**

   - **Challenge**: Initially, the team used git clone instead of forking the repository, which required manual merges on GitHub instead of streamlined version control in VS Code.
   - **Strategy**: Established proper Git workflows (forking, branching, and pull requests), improving collaboration efficiency and reducing integration conflicts.

### Future Learning Goals

- **Enhance Power BI Expertise**: Deepen knowledge of DAX and develop skills such as reordering categories on the x-axis of bar charts and applying advanced visualization techniques.
- **Advance Data Analysis Capabilities**: Gain proficiency in predictive analytics and explore advanced machine learning methodologies to deliver deeper insights.

### Collaboration methodology

We held regular meetings via Google Meet to discuss strategy. We used Discord to coordinate activities. We typically worked in teams of two. Each team focused on updating a single feature. We coordinated work and updates directly with each other. This approach helped us avoid merge conflicts. It allowed all team members to contribute. We also utilised a practice repository to test ideas, code, and enhance our collaboration.

## Main Data Analysis Libraries

### Core Libraries Used

1. **Pandas** (Data Manipulation)
2. **NumPy** (Numerical Computing)
3. **Matplotlib & Seaborn** (Data Visualization)
4. **y-data_profiling**(Data Extraction/Visualisatiion)

## Credits

- For git collaboration we drew extensively on [GitCheatsheet](https://github.com/Vasi012/Git-Cheatsheet) produced by our tutor Vasi.

## Content

- Mikeecee1/Team1_Hackathon/jupyter_notebooks
  - Extraction.ipynb
  - Transformation.ipynb
  - Visualisation.ipynb
- Mikeecee1/Team1_Hackathon/Dashboards
  - BankChurners.pbix

## Acknowledgements (optional)

- Vasi012.
