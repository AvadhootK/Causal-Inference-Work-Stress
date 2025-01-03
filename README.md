# Causal Inference of Hours Worked on Stress Levels

## Overview
This project investigates the causal relationship between hours worked per week and stress levels, with a focus on the confounding effect of work location (remote, hybrid, onsite). Using an Ordered Logistic Regression model and Bayesian inference, the study analyzes data to provide insights into workplace stress dynamics, contributing to informed policy-making in employee well-being.

## Key Objectives
1. Evaluate the impact of hours worked per week on stress levels.
2. Analyze the role of work location as a confounding factor.
3. Provide actionable insights for workplace policies and stress management.

## Dataset
**Source:** [Kaggle - Remote Work and Mental Health Dataset](https://www.kaggle.com/datasets/waqi786/remote-work-and-mental-health/data)

The dataset includes:
- **Treatment Variable**: Hours worked per week (continuous: 20–60 hours).
- **Outcome Variable**: Stress levels (ordered categorical: Low, Medium, High).
- **Confounder**: Work location (categorical: Remote, Hybrid, Onsite).

## Methodology
- **Causal Framework**: Directed Acyclic Graphs (DAGs) represent causal relationships.
- **Statistical Modeling**:
  - Total causal effect: Hours worked on stress levels.
  - Adjusted causal effect: Accounting for work location as a confounder.
- **Prior Predictive Simulations**: Priors informed by domain knowledge to validate assumptions.
- **Bayesian Inference**: Utilized PyMC for robust statistical modeling.

## Tools & Technologies
- **Programming**: Python
- **Libraries**: PyMC, ArviZ, Matplotlib, Seaborn, Pandas
- **Modeling Techniques**: Ordered Logistic Regression, Bayesian inference
- **Data Visualization**: Stress levels vs. hours worked, work location influence

## Key Findings
1. No significant correlation was found between hours worked per week and stress levels, even when accounting for work location.
2. Remote workers showed slightly higher sensitivity to hours worked compared to hybrid and onsite workers.
3. The findings emphasize the complexity of workplace stress and suggest other factors (e.g., job demands, interpersonal relationships) play a more significant role.

## Limitations
- Reliance on self-reported data may introduce bias.
- Missing variables such as workload intensity and job satisfaction limit the scope.
- Assumption of linear relationships between variables may oversimplify complex dynamics.

## Future Directions
- Incorporate additional variables (e.g., job satisfaction, support systems).
- Explore non-linear modeling techniques.
- Use richer, longitudinal datasets for more comprehensive analysis.

## Visualizations
- **Bar Plots**: Stress levels normalized by hours worked.
- **Posterior Predictive Distributions**: Highlighting model accuracy and variability.
- **Causal Diagrams (DAGs)**: Representing treatment, outcome, and confound relationships.
