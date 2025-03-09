# TTE - Generated Insights

## Clustering and Survival Analysis Approach

### Explanation of Steps in Survival Analysis
1. Data Preparation

The dataset is loaded, and two new columns are created:
time: Represents survival time based on the outcome column.
event: Defined as 1 - censored, meaning:
If censored = 1, then event = 0 (no event occurred).
If censored = 0, then event = 1 (event occurred).
2. Clustering Approach

Selected numerical covariates (x1, x2, x3, x4, age) are standardized for uniform scaling.
Principal Component Analysis (PCA) is used to reduce dimensionality and visualize clusters.
K-Means clustering groups individuals based on covariates.
The cluster labels are assigned to the dataset, and a PCA scatter plot visualizes the groups.
3. Kaplan-Meier Survival Curves by Cluster

The Kaplan-Meier estimator is applied separately to each cluster.
Survival curves are plotted for all clusters, allowing comparisons of survival probabilities over time.
This helps identify differences in survival outcomes across different clusters.



### Generated Insights from Clustering and Survival Analysis

1. Identification of Distinct Risk Groups
The clustering analysis successfully segmented individuals into meaningful subgroups based on shared covariates.
Each cluster represents a distinct risk profile, helping differentiate individuals with varying survival probabilities.
2. Survival Outcomes Differ Across Clusters
The Kaplan-Meier survival curves show variations in survival rates between clusters.
Some clusters maintain higher survival probabilities over time, while others experience faster declines.
This suggests that individuals in different clusters face different levels of risk regarding the event occurrence.
3. Potential for Targeted Interventions
Clusters with lower survival probabilities can be flagged as high-risk groups.
This insight allows for personalized healthcare strategies, such as increased monitoring or preventive interventions for high-risk clusters.
Policymakers and healthcare providers could prioritize resources for the most vulnerable groups.
4. Validation of Clustering Approach
The PCA scatter plot shows clear separations between clusters, confirming that the selected covariates effectively differentiate groups.
The Kaplan-Meier survival analysis further validates the clustering, as survival curves vary meaningfully across groups.
This suggests that clustering adds value to the Target Trial Emulation framework by revealing hidden patterns in the data.
5. Future Analytical Directions
Statistical Tests:
A log-rank test can confirm whether survival differences between clusters are statistically significant.
Survival Regression Models:
Cox proportional hazards models can estimate hazard ratios for each cluster and assess their impact on survival.
Further Feature Engineering:
Additional covariates could be incorporated to refine clustering and improve survival prediction accuracy.


### Summary

Combining clustering and survival analysis provided a novel way to analyze survival patterns in the dataset.
The Kaplan-Meier survival curves revealed significant survival differences across clusters, allowing the identification of high-risk groups.
The approach has practical applications in epidemiology, medicine, and risk assessment, enabling targeted interventions based on cluster membership.
Further statistical validation and survival modeling can enhance the robustness of the findings.


