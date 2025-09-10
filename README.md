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

We will utilise predictive visualisations of churn likelihood to identify high-risk customers, enabling early intervention and a deeper understanding of the drivers of churn.

- **Churn Probability Heatmap:** Visual representation of customer risk scores across different segments
- **Customer Risk Dashboard:** Interactive filters to identify high-risk customers by demographics and behavior
- **Churn Prediction Model Results:** Confusion matrix and ROC curves to validate model performance

### Business Requirement 2: Understand churn factors

We will create visualisations of behaviors and patterns linked to churn to clearly communicate the underlying drivers of customer departure.

- **Feature Importance Charts:** Bar charts showing which factors most influence churn decisions
- **Correlation Matrix:** Heatmap displaying relationships between variables and churn
- **Distribution Analysis:** Histograms and box plots comparing at-risk vs retained customers across key metricsoss key metrics

### Business Requirement 3: Enable data-driven decisions

We will present advanced analytics in executive dashboards to support actionable, data-driven decisions.

- **Executive Summary Dashboard:** KPIs and trends for leadership decisions
- **Segment Analysis Views:** Churn rates by customer segments (income, age, card type)
- **Retention Strategy Recommendations:** Visual guides for targeted intervention

## Analysis techniques used

### Data Analysis Methods

1. **Exploratory Data Analysis (EDA)**

   - Statistical summaries and distribution analysis
   - Correlation analysis to identify relationships between variables
   - Missing value analysis and data quality assessment
   - Use of y-data to gain deeper insights into datasets, including correlations and interactions

2. **Feature Engineering**

   - Created derived features like utilisation ratios and transaction frequency metrics
   - Categorical encoding for machine learning models
   - Feature scaling and normalisation

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

- **Ideation**: Used AI tools for feature engineering ideas and hypothesis generation.
- **Code Optimization**: Leveraged AI for code review and performance optimisation suggestions.
- **Design Thinking**: AI-assisted with dashboard layout and visualisation selection.

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

- **Widgets**: Histogram for transaction frequency, scatter plot for utilisation, and analysis of inactive months.
- **Interactive Elements**: Parameter sliders, comparative views
- **Target Audience**: Data analysts and product managers

### Page 4: Predictive Insights

**Content**: Model results and risk scoring

- **Widgets**: Risk score distributions, model performance metrics, feature importance rankings
- **Interactive Elements**: Customer lookup, risk threshold adjustments
- **Target Audience**: Risk management and retention teams

### Communication Strategy

- For technical audiences, use a professional tone when providing detailed statistical metrics, model performance indicators, and technical documentation tailored to their needs.
- For audiences less familiar with technical details, use clear visuals with summaries and recommended actions.
- The use of interactive design will enable users to explore data independently through self-service analytics, allowing them to access and analyse data at their convenience.

## Unfixed Bugs

### Known Issues

1. **Model Overfitting on Small Segments**

   - **Issue**: Some segments have too little data, leading to overfitting.
   - **Reason Not Fixed**: Needs more data or advanced regularisation beyond project scope.
   - **Workaround**: Added confidence intervals and sample size warnings

2. **Dashboard Performance with Large Datasets**
   - **Issue**: Slow loading times when filtering across all customer records.
   - **Reason Not Fixed**: Power BI can't process large datasets in real time.
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

We held regular meetings via Google Meet to discuss strategy. We used Discord to coordinate activities. We typically worked in teams of two. Each team focused on updating a single feature. We coordinated work and updates directly with each other. This approach helped us avoid merge conflicts. It allowed all team members to contribute. We also utilised a practice repository to test ideas, code, and enhance our collaboration.

## Deployment

### Heroku

- The App live link is: https://YOUR_APP_NAME.herokuapp.com/
- Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
- The project was deployed to Heroku using the following steps.

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

- For git collaboration we drew extensively on [GitCheatsheet](https://github.com/Vasi012/Git-Cheatsheet) produced by our tutor Vasi.
- You can break the credits section up into Content and Media, depending on what you have included in your project.

### Content

### Media

## Acknowledgements (optional)

- Vasi012.
