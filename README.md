# COVID-19 Vaccination Data
This report contains data on COVID-19 vaccinations administered to adults ages 18 in New York City vaccinating facilities. 

You can view a visualization of these data on the [Health Department’s COVID-19 Vaccines Data webpage](https://www1.nyc.gov/site/doh/covid/covid-19-data-vaccines.page). 

Data on this page come from the Citywide Immunization Registry (CIR). COVID-19 vaccination data are reported by vaccinating facilities to the CIR and may be delayed. Data are updated daily and include all vaccinations administered and reported up to and including the day before. Data are preliminary and subject to change.

***

## This README includes:
- Definitions 
- Key Technical Notes

***

## Definitions


* **Doses Delivered**: The number of COVID-19 vaccine doses that have been delivered to immunizing providers in NYC since December 13, 2020. Doses delivered to NYC-run programs are separated into first and second dose shipments, per Federal and State regulations.

* **Doses Administered**: The number of COVID-19 vaccine doses that have been administered to adults in NYC and reported to the CIR. This includes NYC and non-NYC residents who are eligible for vaccination. The two vaccines that are currently authorized for emergency use in the United States, Pfizer-BioNTech and Moderna, require two doses.

* **Doses on Hand**: The number of COVID-19 vaccine available for NYC facilities and providers to use. This excludes doses reserved for the CDC’s Long-term Care Facility or Retail Pharmacy Program and for New York State-run vaccination hubs located in NYC.    

* **Adults Vaccinated**: The number of adults ages 18 and over who have been vaccinated with COVID-19 vaccine in NYC based on CIR reporting. This number includes adults vaccinated in NYC who reside outside NYC, such as adults who work in NYC. Race/ethnicity data are further stratified by place of residence (NYC or non-NYC), and by age group (18-64 years or 65+ years). Vaccination status is further broken down into the following two categories: 

    * **Partially Vaccinated**: The number of adults who have received only the first dose of a two-dose COVID-19 vaccine series. 
    * **Fully Vaccinated**: The number of adults who have received both doses of a two-dose COVID-19 vaccine series.  

* **Vaccination Series**: Currently, Pfizer-BioNtech and Moderna are two-dose series.

* **Race/Ethnicity**: Information on race/ethnicity in the CIR is reported from Electronic Health Records and is not complete . Although CDC requires providers to report demographic information, including race/ethnicity, for COVID-19 vaccinations, these data are not consistently captured in the vaccination record. The Health Department is working with health care providers to improve capture of race/ethnicity information in the CIR, and recent improvements in data completeness have been observed.

* **Proportions**: The percent of NYC residents vaccinated is calculated against the total adult population for a geographic area or demographic category. Population counts are derived from interpolated intercensal population estimates updated in 2020. The NYC Health Department produced these population estimates based on estimates from the U.S. Census Bureau and NYC Department of City Planning.

###### *Population estimates were updated on November 9, 2020, to reflect annual population estimates for all New Yorkers as of July 1, 2019. These estimates are prior to the COVID-19 outbreak, and therefore, do not represent any changes to NYC’s population in the past year.*

## Demographic Characteristics
More than 90% of the data reported to the CIR come from Health Care Provider Electronic Health Record systems that are not managed by the NYC Health Department. Data are restricted to adults ages 18 and over.

**ZIP Codes and ZCTAs**:

We report information by geography using modified ZIP Code Tabulation Areas (modZCTA). A ZIP code does not refer to a specific area, but rather a collection of addresses that make up a mail delivery route. There are some buildings that have their own ZIP code and some non-residential areas with ZIP codes. 

To account for these ZIP code challenges, the NYC Health Department uses ZCTAs, which solidify ZIP codes into units of area. Often, data reported by ZIP code are mapped by ZCTA. The ZCTA geography was developed by the U.S. Census Bureau.

The modZCTA geography combines census blocks with smaller populations to allow for more stable estimates of population size for rate calculation. Some modZCTAs have more than one ZIP code.

**Age Groups**:

The Health Department routinely reports data for the following age groups: 18-24, 25-34, 35-44, 45-54, 55-64, 65-74 and 75+. People under 16 are not currently eligible for COVID-19 vaccination.

**Race/Ethnicity**: 

Information on race/ethnicity in the CIR is reported from Electronic Health Records and is not complete . Although CDC requires providers to report demographic information, including race/ethnicity, for COVID-19 vaccinations, these data are not consistently captured in the vaccination record. The Health Department is working with health care providers to improve capture of race/ethnicity information in the CIR, and recent improvements in data completeness have been observed.

**Sex, Gender Identity, Sexual Orientation**: 

The CIR currently only captures "sex" categorized as Male, Female, and Unknown. The data do not currently capture gender identity or sexual orientation of adults vaccinated. Most of the data input to our CIR come from Health Care Providers’ Electronic Health Record systems which the Health Department does not manage. The Health Department uses State guidance for capturing gender and sexual orientation related data. For the CIR, we do not regulate health care providers or determine what information a provider includes in their Electronic Health Record systems. We are working with health care providers to improve how data on gender identity and sexual orientation are collected.


## Key Technical Notes

**Reporting Timing**: 

Data published each morning include entries recorded in CIR through the previous day. Providers are required to report COVID-19 vaccine doses to the CIR within 24 hours of administration. Pharmacies are required to report within 72 hours of administration. Due to potential delays in reporting, our counts may underestimate the actual number of COVID-19 vaccine doses administered in NYC. 

**Report Date Versus Date of Event**: 

Due to reporting delays common with surveillance data, we refresh all data produced each day with data reported for previous days.
Immunization data are published by date of vaccination and not by date of reporting. This approach may differ from the data published by other state and local health departments. Publishing data by date of event better reflects when things happened, as opposed to when the NYC Health Department learned about them. We strongly discourage data users from using daily changes to cumulative files as trend data – this represents information by report date and is prone to misuse and misinterpretation.

**Differences Between City and State Values**: 

Generally, numbers reported by the NYC Health Department and NYS Department of Health will be close but may not match exactly. Reasons for the discrepancies include:

- Inclusion of different vaccination programs, such as the CDC Long-term Care Facility or Retail Pharmacy Program or NYS-run vaccination hubs
- Different data sources for different metrics
- Different analytical and informatics processes
- Different uses of event date or report date (see above)
