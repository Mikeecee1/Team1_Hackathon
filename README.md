# Project Credit Card Customer Churn Analysis

This project focuses on predicting credit card customer churn to help the bank identify which customers are likely to stop using their services. Using the financial, behavioral and demographic data identify the factors effecting customer churn. Create interactive dashboard using PowerBI to visualize the churn patterns and behaviours, able to identify potential customers who are likely to churn. Thereby providing actionable insights so the bank/institution can come up with strategies to retain customers. 

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* BankChurners.csv downloaded from [Kaggle](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data)
* The dataset contains details of features like customer demographics, credit card usage, credit limit, balance, transaction history, etc.

## Business Requirements
* Identify customers who are at risk of churning (closing their credit card accounts) so that proactive retention strategies can be developed.
* By understanding the factors that contribute to customer churn, the bank can improve its services and customer satisfaction.
* Develop interactive dashboards to visualize churn patterns and behaviors, enabling the bank to make data-driven decisions.

## Hypothesis and how to validate?
* List here your project hypothesis(es) and how you envision validating it (them) 

1.	Customers with higher education levels are less likely to churn. 
2.	Higher-income customers are less likely to churn than lower-income customers.
3.	High card utilisation is positively associated with churn.
4.	Older customers are less likely to churn compared to younger customers.
5.	Customers with more inactive months in the past year are more likely to churn.
6.  Customers with fewer transactions are more likely to churn than those with frequent transaction.
7.  Customers with fewer transactions (Total_Trans_Ct) are more likely to churn than those with frequent            transactions.
8.  Marital status and dependent count might have an impact on customer churn — e.g., single customers or those with fewer dependents may have higher churn rates.


## Project Plan
1. Ideation and Team Collaboration:
    Since its a hackathon project, the team brainstormed ideas and selected the topic of Credit Card Customer Churn Analysis. The team collaborated on defining the project scope, setting up the workspaces, the project board(for various tasks), and deliverables.

2. Data Collection and Understanding:
    The dataset was taken from Kaggle and the team explored the dataset to understand the features and initial observations.

## The rationale to map the business requirements to the Data Visualisations
### Business Requirement 1: Identify at-risk customers
**Rationale**: Create predictive visualizations that highlight customers with high churn probability
- **Churn Probability Heatmap**: Visual representation of customer risk scores across different segments
- **Customer Risk Dashboard**: Interactive filters to identify high-risk customers by demographics and behavior
- **Churn Prediction Model Results**: Confusion matrix and ROC curves to validate model performance

### Business Requirement 2: Understand churn factors
**Rationale**: Develop analytical visualizations to reveal patterns and correlations in customer behavior
- **Feature Importance Charts**: Bar charts showing which factors most influence churn decisions
- **Correlation Matrix**: Heatmap displaying relationships between variables and churn
- **Distribution Analysis**: Histograms and box plots comparing churned vs retained customers across key metrics

### Business Requirement 3: Enable data-driven decisions
**Rationale**: Create executive-level dashboards that translate complex data into actionable business insights
- **Executive Summary Dashboard**: High-level KPIs and trends for leadership decision-making
- **Segment Analysis Views**: Breakdown of churn rates by customer segments (income, age, card type)
- **Retention Strategy Recommendations**: Visual guides for targeted intervention strategies

## Analysis techniques used
### Data Analysis Methods
1. **Exploratory Data Analysis (EDA)**
   - Statistical summaries and distribution analysis
   - Correlation analysis to identify relationships between variables
   - Missing value analysis and data quality assessment
   - Use of y-data to gain deeper insights of datasets including correlations and interactions

2. **Feature Engineering**
   - Created derived features like utilization ratios and transaction frequency metrics
   - Categorical encoding for machine learning models
   - Feature scaling and normalization

3. **Machine Learning Techniques**
   - **Logistic Regression**: Baseline model for interpretability
   - **Random Forest**: Ensemble method for feature importance analysis
   - **Gradient Boosting (XGBoost)**: Advanced ensemble for improved prediction accuracy
   - **Naive Bayes**: Probabilistic classifier (already included in dataset)

### Structure and Justification
The analysis was structured in three phases:
1. **Descriptive Analytics**: Understanding current churn patterns
2. **Predictive Analytics**: Building models to forecast future churn
3. **Prescriptive Analytics**: Developing actionable recommendations

### Data Limitations and Alternative Approaches
- **Limitation**: Imbalanced dataset with fewer churned customers
  - **Solution**: Applied SMOTE (Synthetic Minority Oversampling Technique) and class weighting
- **Limitation**: Limited temporal data for trend analysis
  - **Alternative**: Used cross-sectional analysis with behavioral proxies
- **Limitation**: Missing external economic factors
  - **Mitigation**: Focused on internal behavioral and demographic patterns

### Generative AI Usage
- **Ideation**: Used AI tools to brainstorm feature engineering ideas and hypothesis generation
- **Code Optimization**: Leveraged AI for code review and performance optimization suggestions
- **Design Thinking**: AI-assisted dashboard layout and visualization selection recommendations

## Ethical considerations
### Data Privacy Issues
- **Challenge**: Customer financial data contains sensitive personal information
- **Mitigation**: Implemented data anonymization techniques and removed direct identifiers
- **Compliance**: Ensured adherence to GDPR and banking data protection regulations

### Bias and Fairness
- **Identified Bias**: Potential discrimination based on demographic factors (age, gender, income)
- **Fairness Measures**: Implemented fairness metrics to ensure equal treatment across demographic groups
- **Model Auditing**: Regular bias testing across different customer segments

### Legal and Societal Considerations
- **Transparency**: Developed explainable AI models to ensure decision transparency
- **Customer Rights**: Implemented processes for customers to understand and challenge automated decisions
- **Responsible AI**: Established guidelines for ethical use of churn predictions in customer interactions

## Dashboard Design
### Page 1: Executive Overview
**Content**: High-level KPIs and summary metrics
- **Widgets**: Churn rate gauge, customer count cards, trend line charts
- **Interactive Elements**: Date range selector, segment filters
- **Target Audience**: C-level executives and senior management

### Page 2: Customer Segmentation Analysis
**Content**: Detailed breakdown of churn patterns by customer segments
- **Widgets**: Demographic distribution charts, income category analysis, card type breakdown
- **Interactive Elements**: Multi-select filters, drill-down capabilities
- **Target Audience**: Marketing and customer relationship managers

### Page 3: Behavioral Analytics
**Content**: Transaction patterns and usage behavior analysis
- **Widgets**: Transaction frequency histograms, utilization ratio scatter plots, inactive months analysis
- **Interactive Elements**: Parameter sliders, comparative views
- **Target Audience**: Data analysts and product managers

### Page 4: Predictive Insights
**Content**: Model results and risk scoring
- **Widgets**: Risk score distributions, model performance metrics, feature importance rankings
- **Interactive Elements**: Customer lookup, risk threshold adjustments
- **Target Audience**: Risk management and retention teams

### Communication Strategy
- **Technical Audience**: Detailed statistical metrics, model performance indicators, and technical documentation
- **Non-Technical Audience**: Simplified visualizations with clear narratives, executive summaries, and actionable recommendations
- **Interactive Design**: Self-service analytics capabilities allowing users to explore data independently

## Unfixed Bugs
### Known Issues
1. **Model Overfitting on Small Segments**
   - **Issue**: Some demographic segments have insufficient data leading to overfitted predictions
   - **Reason Not Fixed**: Requires additional data collection or advanced regularization techniques beyond project scope
   - **Workaround**: Added confidence intervals and sample size warnings

2. **Dashboard Performance with Large Datasets**
   - **Issue**: Slow loading times when filtering across all customer records
   - **Reason Not Fixed**: PowerBI limitations with real-time data processing on large datasets
   - **Mitigation**: Implemented data aggregation and caching strategies

### Knowledge Gaps Addressed
- **Initial Gap**: Limited understanding of ensemble methods
  - **Solution**: Completed online courses on advanced machine learning techniques
- **Feedback Integration**: Incorporated peer review suggestions on model validation techniques
- **Continuous Learning**: Regular model retraining based on new data patterns

## Development Roadmap
### Challenges Faced
1. **Data Quality Issues**
   - **Challenge**: Inconsistent data formats and missing values
   - **Strategy**: Developed robust data cleaning pipelines and validation rules

2. **Model Selection Complexity**
   - **Challenge**: Balancing model accuracy with interpretability
   - **Strategy**: Implemented multiple models and created ensemble approaches

3. **Stakeholder Alignment**
   - **Challenge**: Different departments had varying requirements
   - **Strategy**: Conducted regular stakeholder meetings and iterative feedback sessions

### Future Learning Goals
- **Advanced Deep Learning**: Explore neural networks for improved prediction accuracy
- **Real-time Analytics**: Implement streaming data processing for live churn monitoring
- **Causal Inference**: Study causal analysis techniques to better understand churn drivers

### Collaboration methodology
   **Team Strategy**: Held regular meetings via GoogleMeet to discuss strategy and via Discord to coordinate activities
   **Collaboration**: We generally worked in teams of two with each team undertaking to update a single feature and coordinating work and updates. This approach helped avoid merge conflicts, while enabling all team members to make contributions.
   **Ideation/ Exprimentation**: We used a practice repository to explore ideas, test code and work out collaboration methodology.

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.


## Main Data Analysis Libraries
### Core Libraries Used

1. **Pandas** (Data Manipulation)
2. **NumPy** (Numerical Computing)
3. **Matplotlib & Seaborn** (Data Visualization)
4. **y-data_profiling**(Data Extraction/Visualisatiion)


## Credits 

* For git collaboration we drew extensively on [GitCheatsheet](https://github.com/Vasi012/Git-Cheatsheet) produced by our tutor Vasi.
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

### Media

## Acknowledgements (optional)
* Vasi012.