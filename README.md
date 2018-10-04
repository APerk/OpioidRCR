# OpioidRCR
##[Master Technical Specifications GoogleDoc](https://docs.google.com/document/d/1ODXc4xo6Lqm6f8BPzVo0nrrG1GtHflRlBCxCQNkzMik/edit)

### [Value Sets](/ValueSets)
* CDC Oral Opioids
* All Opioids
* Risk factors and outcomes- Exclusion criteria
* [Cancer Codes](https://docs.google.com/spreadsheets/d/1YHdHfo-cPb4zBb_vZCQUCgqI_YGeHUaOLzdozmBmNko/edit#gid=0)

### ["Ad Hoc Queries" - Descriptive Statistics for deteriminants and outcomes from logic model](/AdHocQueries)
* Review the table shells
* Crosstabs for value sets over demographic and geographic variables
* High Dose (see [this SAS code](https://www.oig.hhs.gov/oei/reports/oei-02-17-00560.asp) from HHS - June 2018.)
* Possibly useful [toolkit from HHS](https://oig.hhs.gov/oei/reports/oei-02-17-00560.pdf)


### Replicating CDC Results
* [CDC SAS Code](https://www.cdc.gov/drugoverdose/data-files/SAScodetouseMMEconvsnfileSept2017.sas) to modify
* Crosswalks from CDC NDCs to RXNORM with same MMEs [here]
* TODO (if we decide): Crosswalks to average MMEs for less granular matches
* TO DECIDE How to impute MME and days supply when we don't have it (e.g. impute these based on CMS claims data)
* Table shells matching RX to provider zip code
* TODO SAS PROC SQL queries



### Regressions and Predictive Analyses
#### TODO: Specifications for Unit of analysis = zip code (one model)
* Get public data by zip code/county
#### TODO: Unit of analysis = person (one model per DMC)
* Specify Data Set: variables, any temporal conditions, and pivot logic from long to wide
* Specify Analytic Model(s): 
	* Predictors of guideline adherence (unit of analyis = provider)	
	* Predictors of high dose (unit of analysis = patient)
	* Predictors of outcomes (unit of analysis = patient)
