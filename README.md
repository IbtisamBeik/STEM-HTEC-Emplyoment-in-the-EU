# Project: Visualizing Real World Data
## STEM-HTEC-Emplyoment-in-the-EU
Ibtisam Beyk
[Data Analytics, Berlin 10.07.2020)

## Content

* Project Description
* Questions and Hypothesis
* Datasets
* Analysis
* Conclusions
* Limitations
* Presentation

## Project description:

In this project we are investigating the Employment rates in the high tech (HTEC) sector accross the member states of European Union and associated countries (https://ec.europa.eu/research/horizon2020/index.cfm?pg=country-profiles). The data analyzed cover the period from 2010 to 2019 and are published on yearly basis by the European Commission (https://ec.europa.eu/info/index_en). 

## Questions and Hypothesis:

The main aim of this analysis is to recoqnize the hiring trend in the HTEC sector and the level of education required in the field in the different EU states. General assumption is that high tech countries like Germany and UK have the tendecy to hiher individuals with higher education (B.Sc and above). Additionaly, we are testing the hypothesis that creating more positions in the HTEC, in specific, correlates to the EU immigration patterns with countries having higher employment rates receving more immigrants. 

## Datasets: 

The datasets for this project were obtained from the European Commission (https://ec.europa.eu/eurostat/data/database). The dataset was mostly clean and complete. Countries with 2-3 missing values were considered in all the analyses as they provide valuable overview. The original datasets were further divided into seperate tables and data was imported into DataFrames. The two main data sub-sets are: 

1. Employment, and it contains 7 different Excel sheets. The first sheet represents the total employment (in thousands) in HTEC accorss the EU, while the rest of the sheets contain information on the education levels of the employees. For this analysis the sheets (<Secondary (%), <Tertiary (%), and Tertiary(%) were used.

2. Immigration, and it consists of 3 Excel sheet containing data on the total immigration for each member country. For the current analysis, the 1st sheet (Total) was used. 

The datasets used are in the "Datasets" folder.

## Analysis: 

After selecting and cleaning the datasets, the data was imported into DataFrames using pandas. Each of the two types of data (Emyployment and Immigration) were anaylzed as following:

1. Boxplots were used to represent the average and outliers of Employment/Immigration rates for each year accross the member states. 
2. Histograms were used to plot the distribution of the cumulative Emplyoment/Immigration rate up until 2019. 
3. Summary stats were derived for each variable. 
4. Horizontal bar plot was used to represent the countries in descending order according to the cumulative Employment/Immigration. 

Individual countries were chosen for analyzing the Education levels of employees in the top 4 hiring countries. Statsmodels were used to investigate the correlation of the employment in the top 4 countries with the immigration rate. 

## Conclusions: 

#### Employment in HTEC:

1. There is an almost steady trend of the HTEC emplyoment numbers in the EU countries in the past decade.
2. In 2019, there is a slight increase in the employment as indicated by the median and 75th percentile (Stats summary below).
3. The average HTEC cumulative employment in the EU in the period from 2010-2019 reaches ~ 2480000 *Considering the high std value, in this case the median is a more representative statistic *50% of the countries employed up to 1290000 since 2010.
4. The top 4 countries (Cumulative employment > Q3): Germany, UK, Italy, France *Lowest 2 countries (Q1< Cumulative emplyoment <Q2): Slovenia, Croatia *Mid 2 countries (Q2< Cumulative employment <Q3): Slovakia, Bulgaria

#### Immigration: 

1. There is an almost steady trend of the immigration numbers in the EU countries in the past decade.  
2. In 2015, there is a slight increase in the immigration as indicated by the median and the 75th percentile. The highest outlier in this year could be a result of the "Free movement - EU nationals" directive introduced in 2014 allowing citizens of Bulgaria and Romania to live and work freely accross the different EU member states (https://ec.europa.eu/social/main.jsp?catId=457) 

3. The average cumulative immigartion in the EU in the period from 2010-2019 reaches ~ 9.368691e+05 *Considering the high std value, in this case the median is a more representative statistic *50% of the countries employed up to 4.094175e+05 since 2010. *The top 4 countries (Cumulative employment > Q3): Germany, UK, Spain, France

4. There is a strong positive correlation between the Employment opportunities in the HTEC sector in the top 4 countries and the immigration towards the same.

## Limitations:

There were no major factos limiting the analysis, but having data on specific fields of education would have given more valuable insights. Having stats on the education levels of the immigrating individuals would have also been benefical when drawing the final conclusions. 

## Presentation:  
The main findings of this analyses were presented in a powerpoint format (See the Presentation folder). 
