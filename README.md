# Comprehensive Analysis and Predictive Modeling of Water Quality Indicators

## Introduction

Water quality is a very critical aspect of public health and environmental sustainability; hence, its ongoing monitoring and analyses must be both intensive and extensive. With this project, it is intended to conduct a comprehensive analysis of all the indicators of water quality in the city of New York, to identify key trends, and to comprehend the distributions of microbial measurements and residual chlorine levels. Through detailed statistical analysis, this project hopes to provide insights regarding factors that affect water quality. It will also use clustering and predictive modeling to classify water samples and inform suggestions to the water treatment plans for both upstream and downstream. The project will help offer improved water quality monitoring and regulatory compliance.

Water quality indicator limits are listed below, based on the City of New York’s water treatment policies, which adhere to federal and state regulatory standards for each parameter.

* Turbidity (NTU) — Acceptable Range (Operational Samples: 5 NTU; Compliance Samples: 0.3 NTU)
* Residual Free Chlorine (mg/L) — Acceptable Range (4mg/L)
* Coliform (MPN /100mL) — Acceptable Range (ND, Max 5% samples positive per month)

## Objectives

These are the main objectives of this project
* Identify key water quality indicators by sample class
* Examine historical data to identify trends and patterns in water quality indicators over the years
* Identify distinct clusters to understand the variability and common characteristics within the data
* Develop predictive models to classify water samples based on their residual free chlorine levels and coliform counts

## Data Wrangling & Analysis

Data was collected from the city of New York Open Data Sources. Rows with a high percentage of missing values are removed. Outliers are assessed and removed before performing K-means which is sensitive to outliers that potentially skew the centroids of clusters. The provided coordinates are converted into degrees using Python’s package.

Methodologies
* K-means Clustering
* Logistic Regression Modelling

The complete analysis of this project is posted via this link
https://medium.com/p/7a8488965aa9

## Conclusion

Given the significant variability and outliers in turbidity, especially within the ‘Compliance’ class, it’s crucial to implement more frequent turbidity checks. For classes with high turbidity, possibly upgrading filtration systems to ensure they can handle higher loads and reduce variability.

The presence of extremely low chlorine levels, particularly in the ‘Compliance’ and ‘Operational’ classes, suggests a need for adjusting chlorine dosing protocols. However, there is no need to adjust chlorine dosing protocols for treatment points where microbial measures downstream are well controlled to avoid unnecessary extra dosage. Instead, resources should be allocated for locations that observed high or abnormal bacteria contain such as site 56000 and site 76550.

Reducing the number of false positives, which are the number of operational cases incorrectly predicted as ‘Compliance, could potentially improve the precision of the model.

## Tech stacks
* Python
* Tableau


## License

This project is licensed under the MIT License.

## References

1. Drinking Water Quality Distribution Monitoring Data | NYC Open Data. (2024, May 16). https://data.cityofnewyork.us/Environment/Drinking-Water-Quality-Distribution-Monitoring-Dat/bkwf-xfky/about_data

2. 2023 Drinking Water Supply Quality Report. (n.d.). Retrieved June 15, 2024, from https://www.nyc.gov/assets/dep/downloads/pdf/water/drinking-water/drinking-water-supply-quality-report/2023-drinking-water-supply-quality-report.pdf

3. Figure 1. Schematic diagram of the process that involves. . . (n.d.). ResearchGate. https://www.researchgate.net/figure/Schematic-diagram-of-the-process-that-involves-post-chlorination-in-the-WTP-under_fig1_327737595