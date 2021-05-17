# COVID-19 Vaccination Data
This repository contains data on COVID-19 vaccinations administered by New York City (NYC) vaccinating facilities and reported to the Citywide Immunization Registry (CIR).   
You can view a visualization of these data on the [Health Department's COVID-19 Vaccines Data webpage](https://www1.nyc.gov/site/doh/covid/covid-19-data-vaccines.page). 

The CIR keeps immunization records for all city residents throughout their lives. COVID-19 vaccination data are reported by vaccinating facilities to the CIR and may be delayed. Data are updated daily and include all vaccinations administered and reported up to the previous day. Data are preliminary and subject to change.
***

## This README includes:
- Definitions 
- Key Technical Notes

***
	
## Definitions

* **Doses Delivered**: The number of COVID-19 vaccine doses that have been delivered to immunizing providers in NYC since December 13, 2020. Doses delivered to facilities or programs managed by New York State (NYS), Federal Emergency Management Agency (FEMA), and the Center for Disease Control (CDC), including Long-term Care Facility and Retail Pharmacy Programs, are reported separately from doses delivered to New York City health care providers.  

* **Doses Administered**: The number of COVID-19 vaccine doses that have been administered in NYC and reported to the CIR. This includes doses administered to NYC residents, and to non-NYC residents who are eligible for vaccination, such as those who work in NYC. Of the vaccines currently authorized for emergency use in the United States, two vaccines (Pfizer-BioNTech and Moderna) require two doses, and one vaccine (Johnson & Johnson/Janssen) requires a single dose. 

* **Doses on Hand**: The number of COVID-19 vaccine doses available for NYC facilities and providers to use. This excludes doses reserved for the CDC's Long-term Care Facility Program or Retail Pharmacy Program, and vaccination hubs located in NYC, but managed by NYS or FEMA. Dose 1 on-hand includes both single dose vaccines and first doses of a two-dose vaccine series. Dose 2 on-hand refers to second dose vaccine available to complete the two-dose vaccine series.
* **People Vaccinated**: The number of people who have been vaccinated with COVID-19 vaccine in NYC based on CIR reporting. This includes all ages, including those under 18 years old, as people aged 12 to 15 years are currently eligible for COVID-19 vaccination. This definition is further broken down into the subparts below.
    * **Partially Vaccinated**: The number of people who have received only the first dose of a two-dose COVID-19 vaccine series. 
    * **Fully Vaccinated**: The number of people who have received either: a.) both doses of a two-dose COVID-19 vaccine series or b.) a dose of a single-dose COVID-19 vaccine. Currently, Pfizer-BioNtech and Moderna are two-dose vaccine series, and Johnson & Johnson's Janssen COVID-19 vaccine is a single dose vaccine. At this time, only the Pfizer-BioNtech vaccine has received FDA approval for use in people aged 12-15 years old.
    * **At least one dose**: The number of people partially or fully vaccinated who have received either: a.) one or two doses of a two-dose COVID-19 vaccine series or b.) a single-dose COVID-19 vaccine.


**All People Vaccinated**: This section includes both NYC and non-NYC residents. Non-NYC residents include people eligible for vaccination in NYC who reside outside the city, and people with unknown place of residence. Percentages by demographic group are among those vaccinated and do not represent vaccination coverage. Please refer to the sections on NYC Vaccination Coverage and Geography to compare vaccination coverage across demographic groups.

**NYC Vaccination Coverage and Geography**: Data are restricted to NYC residents. The percent of NYC residents vaccinated is calculated against the total population for a specific geographic area or demographic category. Population counts are derived from interpolated intercensal population estimates updated in 2020. The NYC Health Department produced these population estimates based on estimates from the U.S. Census Bureau and NYC Department of City Planning. Data in these sections can be used to compare vaccination coverage between demographic categories and geographies. 

###### *Population estimates were updated on November 9, 2020, to reflect annual population estimates for all New Yorkers as of July 1, 2019. These estimates are prior to the COVID-19 outbreak, and therefore, do not represent any changes to NYC's population in the past year.*

***


## Demographic Characteristics
More than 90% of the data reported to the CIR come from Health Care Provider Electronic Health Record systems that are not managed by the NYC Health Department.

**ZIP Codes and ZCTAs**:

We report information by geography using modified ZIP Code Tabulation Areas (modZCTA). A ZIP code does not refer to a specific area, but rather a collection of addresses that make up a mail delivery route. There are some buildings that have their own ZIP code and some non-residential areas with ZIP codes. 

To account for these ZIP code challenges, the NYC Health Department uses ZCTAs, which solidify ZIP codes into units of area. Often, data reported by ZIP code are mapped by ZCTA. The ZCTA geography was developed by the U.S. Census Bureau.

The modZCTA geography combines census blocks with smaller populations to allow for more stable estimates of population size for rate calculation. Some modZCTAs have more than one ZIP code.


**Age Groups**:

Data are reported for the following age groups: <18, 18-24, 25-34, 35-44, 45-54, 55-64, 65-74 and 75-84, 85+ years. Among people aged <18 years, only those aged 12 to 15 years are currently eligible for COVID-19 vaccination. 

**Race/Ethnicity**: 

Information on race/ethnicity in the CIR is reported from Electronic Health Records and is not complete. Although CDC requires providers to report demographic information, including race/ethnicity, for COVID-19 vaccinations, these data are not consistently captured in the vaccination record. The Health Department is working with health care providers to improve capture of race/ethnicity information in the CIR, and recent improvements in data completeness have been observed.

**Sex, Gender Identity, Sexual Orientation**: 

The CIR currently only captures "sex" categorized as Male, Female, and Unknown. The data do not currently capture gender identity or sexual orientation of people vaccinated. Most of the data input to our CIR come from Health Care Providers' Electronic Health Record systems which the Health Department does not manage. The Health Department uses State guidance for capturing gender and sexual orientation related data. For the CIR, we do not regulate health care providers or determine what information a provider includes in their Electronic Health Record systems. We are working with health care providers to improve how data on gender identity and sexual orientation are collected.

## Key Technical Notes

**Reporting Timing**: 

Data published each morning include entries recorded in CIR through the previous day. Providers are required to report COVID-19 vaccine doses to the CIR within 24 hours of administration. Pharmacies are required to report within 72 hours of administration. Due to potential delays in reporting, our counts may underestimate the actual number of COVID-19 vaccine doses administered in NYC. 

**Report Date Versus Date of Event**: 

Due to reporting delays common with surveillance data, we refresh all data produced each day with data reported for previous days.
Immunization data are published by date of vaccination and not by date of reporting. This approach may differ from the data published by other state and local health departments. Publishing data by date of event better reflects when things happened, as opposed to when the NYC Health Department learned about them. We strongly discourage data users from using daily changes to cumulative files as trend data - this represents information by report date and is prone to misuse and misinterpretation.

**Differences Between City and State Values**: 

Generally, numbers reported by the NYC Health Department and NYS Department of Health will be close but may not match exactly. Reasons for the discrepancies include:

- Inclusion of different vaccination programs, such as the CDC's Long-term Care Facility Program and Retail Pharmacy Program, or NYS- or FEMA-run vaccination hubs
- Different data sources for different metrics
- Different analytical and informatics processes
- Different uses of event date or report date (see above)
