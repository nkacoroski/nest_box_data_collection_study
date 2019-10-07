# A Comparison of Manual and eNest Assisted Monitoring of Bird Nest Boxes
## Abstract
This repository contains work for a study on manual and eNest assisted monitoring of chickadee (**Poecile sp.**) nest boxes following the NestWatch protocol by the Cornell Lab of Ornithology. Community science projects such as NestWatch expand the capability of researchers to collect data and increase interest in science and the natural world by providing opportunities for volunteers to get involved. Manual monitoring of bird nests through community science, however, faces challenges such as nest disturbance, poor data quality, and volunteer commitment limitations. Technology assisted monitoring of nest sites with devices such as eNest, a bird nest box data collection system, might address these concerns by providing continuous observation throughout the nesting season, and enrich data analysis through additional information from environmental metrics. Designed to be non-invasive, eNest has been field-tested in approximately 50 nest boxes. By comparing eNest to traditional bird nest monitoring methods, this study will also provide initial research on the suitability of eNest in bird nest boxes, and the integration of technology assisted nest box monitoring into community science project projects like NestWatch.In this repository is the work for the [experimental design](experimental_design.ipynb), [data submission app](data_submission_app.ipynb), and [statistical analysis](statistical_analysis.ipynb) of the study.

## Project Understanding
The study will take place in 2020 in the Greater Seattle Area, WA. Volunteers will be recruited from local Audubon Society Chapters between October 2019 and February 2020. All volunteers will complete NestWatch training for monitoring nest sites and using the eNest app. For the purpose of this study, nest sites are limited to chickadee nest boxes that will be provided to volunteers along with all eNest equipment (devices, micro SD cords). Data collection will begin March 1st, 2020. 

### Manual Monitoring
Manual data collection consists of visiting the nest box every 3-7 days to collect data on nest attempts. At the end of each nest attempt, the volunteer records a nest summary. For more information see the [Understanding NestWatch Data](https://nestwatch.org/learn/how-to-nestwatch/understanding-nestwatch-data/) on the NestWatch website.

### eNest Assisted Monitoring
eNest assisted monitoring consists of installing the eNest device at the beginning of the nesting season, and then analyzing the data for important nest events afterwards using the eNest App. 

The eNest device will run on battery or solar power for the entire nesting season, eliminating the need for any visits to the nest. It will collect 1-5 images a day, GPS coordinates, movement in seconds of motion per minute, humidity, temperature, light and air pressure. At the end of the nesting season, the volunteer will collect the eNest device, transfer data to a computer using a micro SD cord, and upload it to the eNest App. Using the eNest App, volunteers will visualize their data and identify relevant information to submit to NestWatch.  


## [Experimental Design](experimental_design.ipynb)

### Power Analysis
### Sample Size
All attempts will be made to randomize manual and eNest assisted monitoring groups, however, since this is a volunteer-based study there may be certain volunteers who can only commit to a specific group. 

## [Data Submission App](data_submission_app.ipynb)
The data submission app will be an enhanced version of the [eNest Dashboard](https://github.com/nkacoroski/animal_data_science_shiny_app), a data visualization app currently in development. Additional features will include a submission form for the NestWatch database.


## [Data Analysis](data_analysis.ipynb)
To be determined once data collection is completed in 2020. 

### Exploratory Data Analysis
Exploratory data analysis will be conducted to provide initial descriptions and visualizations of important nest event statistics.

### Statistical Analysis
Exploratory questions will evaluate if there is any significant difference between important nest event statistics between manual and eNest assisted monitoring. Follow-up questions will be used to further characterize any significant differences.

Exploratory Statistical Questions
1. Is there a significant difference between dates of nesting attempts recorded by manual and eNest assisted monitoring?
2. Is there a significant difference between number of nesting attempts recorded by manual and eNest assisted monitoring?
3. Is there a significant difference between species recorded by manual and eNest assisted monitoring?
4. Is there a significant difference between number of eggs recorded by manual and eNest assisted monitoring?
5. Is there a significant difference between dates of first egg laid recorded by manual and eNest assisted monitoring?
6. Is there a significant difference between hatched young recorded by manual and eNest assisted monitoring?
6. Is there a significant difference between dead young recorded by manual and eNest assisted monitoring?
7. Is there a significant difference between hatch dates recorded by manual and eNest assisted monitoring?
8. Is there a significant difference between nest parasitism recorded by manual and eNest assisted monitoring?
9. Is there a significant difference between dates of nest parasitism recorded by manual and eNest assisted monitoring?
10. Is there a significant difference between nest predation recorded by manual and eNest assisted monitoring?
11. Is there a significant difference between dates of nest predation recorded by manual and eNest assisted monitoring?
12. Is there a significant difference in nest report success recorded by manual and eNest assisted monitoring?
13. Is there a significant difference between final nest fate recorded by manual and eNest assisted monitoring?
14. Is there a significant difference between dates of final nest fate recorded by manual and eNest assisted monitoring?
15. Is there a significant difference in fledge dates recorded by manual and eNest assisted monitoring?
16. Is there a significant difference between host species count totals recorded by manual and eNest assisted monitoring?

## Results
To be determined.

## Recommendations
To be determined.