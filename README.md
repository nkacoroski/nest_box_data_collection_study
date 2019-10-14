# Comparison of Manual and eNest Data Collection using Observations of Chickadee Nest Boxes in Washington State
## Project Understanding
Automated data collection of nest boxes for community science projects could decrease observer impact on the nest, improve data quality, and increase participation by decreasing the time commitment for volunteers. The eNest system is a newly available, low cost, automated data collection device for nest bird boxes that could address these issues and expand the scope of data collected. This repository contains work for the [experimental_design](experimental_design.ipynb), [data submission app](data_submission_app.ipynb), and [statistical analysis](statistical_analysis.ipynb) for a study comparing manual and eNest data collection with NestWatch, a volunteer-based nest site monitoring program, using observations of chickadee nest boxes in Washington State. 

This study takes place in the Greater Seattle Area of Washington State during the 2020 nesting season. For experimental control, the scope is limited to chickadee (*Poecile sp.*) nest boxes installed a minimum of 650 feet apart, and 5 to 15 feet off the ground. Volunteers will be recruited from the local community, given a nest box, and split into two groups, manual and eNest assisted monitoring. Volunteers in the manual group will follow the [NestWatch protocol](https://nestwatch.org/learn/how-to-nestwatch/nest-monitoring-protocol/) and collect data on their nest box throughout the nesting season. Volunteers in the eNest assisted group will set up an eNest device in their nest box for the entire nesting season, and then use the eNest app to visualize and interpret the data for important nest observations. For more information, see the [study proposal](eNest_research_proposal.docx).


## Data Understanding
13 important nest observations were identified from the NestWatch protocol to evaluate differences between manual and eNest data collection for monitoring chickadee nest boxes. They are:
* dates of nesting attempts
* number of nesting attempts
* nesting species
* number of eggs
* dates of first egg laid
* hatch dates
* number of nest parasitism events
* dates of nest parisitism events
* number of nest predation events
* dates of nest predation events
* final nest fate (categorical)
* fledge dates
* host species count totals
* number of completed nest reports

In addition, volunteer report success (the number of volunteers who completed nest site reports) was added to provide a measure of the volunteer commitment threshold. To summarize, the study consists of 2 categorical groups and 14 dependent variables, all numerical except final nest fate, which is categorical. 


## Data Preparation
### [Data Submission App](data_submission_app.ipynb)
To allow volunteers to visualize and interpret data for NestWatch, an additional feature will be added to the [eNest app](https://github.com/nkacoroski/animal_data_science_shiny_app), a data visualization tool for eNest currently in development, that allows users to compile data for submission to the NestWatch database.

### [Experimental Design](experimental_design.ipynb)
To determine an appropriate experimental design, I investigated conducting a series of independent t-tests with a Bonferroni correction to address multiple comparisons or using a Multivariate Analysis of Variance (MANOVA) to compare manual and eNest assisted monitoring of nest sites. The series of independent t-tests evaluates differences between manual and eNest assisted monitoring at the level of each dependent variable, the MANOVA allows for comparison in aggregate, treating all 14 dependent variables as a single vector. 

For both types of tests, I used G\*Power, a statistical power analysis program, to calculate the relationship between total sample size and power at small, medium, and large effect sizes with alpha set at the standard 0.05. I graphed the data using a total sample size range of 30 to 100, because that is our target range for volunteer recruitment. 
![power analysis graph](power_analysis.png)
According to the *a priori* power analyses, only the independent t-test achieves a power of 0.8 with a total sample size less than 100. The minimum total sample size is 52 (26 nest boxes per group), and only large effects are detected. I also investigated reducing the number of dependent variables for a MANOVA. The maximum number of variables possible is 7, with a total sample size of 98. Since all of the dependent variables are important, and getting a total sample size of 98 might be challenging, I recommend going with the series of independent t-tests and using the Bonferroni correction to account for multiple comparisons. I plan to investigate using Bayesian and computationally intensive methods as other alternatives.


## [Data Analysis](data_analysis.ipynb)
### Exploratory Data Analysis
Exploratory data analysis will be conducted to characterize and visualize the data.

### Statistical Analysis
A series of independent t-tests with a Bonferroni correction will be used to assess important nest event observations for differences between manual and eNest data collection methods of chickadee nest boxes. Hypotheses tests will be evaluated using p-values and confidence intervals.


## References
[Faul, F., Erdfelder, E., Lang, A.-G., & Buchner, A. (2007). G*Power 3: A flexible statistical power analysis program for the social, behavioral, and biomedical sciences. Behavior Research Methods, 39, 175-191.](http://www.psychologie.hhu.de/arbeitsgruppen/allgemeine-psychologie-und-arbeitspsychologie/gpower.html)