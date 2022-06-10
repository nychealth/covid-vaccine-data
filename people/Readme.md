#  people/
This folder contains information on the number of NYC residents vaccinated for COVID-19 in NYC, NYS, NJ or elsewhere and reported to the CIR by NYC providers; the [New York State Immunization Information System (NYSIIS)](https://www.health.ny.gov/prevention/immunization/information_system/); the New Jersey Immunization Information System (NJIIS) or 

Files labeled ‘by-residency’ also have data on the number of eligible non-NYC residents vaccinated at facilities in NYC, such as individuals who work or study in the city.

 Vaccination status is classified into the following categories: 
* **Partially Vaccinated**: People who have received the first dose of a two-dose primary vaccine series (i.e. Pfizer-BioNtech or Moderna).
* **Fully Vaccinated**: People who have received the two-dose series of the Moderna or Pfizer vaccine, or the single-dose series of the Johnson & Johnson vaccine. This was previously referred to as "fully vaccinated."
* **At least one dose**: People who have received either the first dose of the two-dose Pfizer or Moderna primary vaccine series or the one dose of the Johnson & Johnson/Janssen primary vaccine series. New Yorkers who received the AstraZeneca vaccine are only counted if they received both doses of the two-dose vaccine. 
* **Additional/booster doses**: People who have received additional doses of an FDA-approved vaccine after completing their primary series. This includes first and second booster shots, as well as additional doses for people who are immunocompromised.

The number of people who received at least one dose includes people who are both partially and fully vaccinated; percentages and counts should not be summed. 

**Population estimates:** Please note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. Population counts were calculated using intercensal estimates updated on October 9, 2020 to reflect annual population estimates for all New Yorkers as of July 1, 2019. These estimates do not represent the 2020 Census or recent changes to NYC’s population as a result of in-migration or out-migration. Additional factors contributing to these inconsistencies may be that people who identify as Multi-race are misreported under a single race, and self-reported ZIP code at the time of vaccination may not correspond to the vaccine recipient’s primary home address. For example, people may use their work address for the purpose of vaccination.
See [/technical notes](https://github.com/nychealth/covid-vaccine-data/blob/main/Readme.md#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) for more information on population estimates.

**Age groups**: Data are reported for the following age groups per U.S. Census age categories: 5-12, 13-17, 18-24, 25-34, 35-44, 45-54, 55-64, 65-74, 75-84, and 85+ years. Among people under 18, only those aged 5 to 17 years are currently eligible for COVID-19 vaccination.

See [/technical notes](https://github.com/nychealth/covid-vaccine-data#demographic-characteristics) for more information on how CIR demographic information is collected. 

## Files

### coverage-summary-donut1.csv

This file contains information on the estimated percentage of NYC residents who are either partially or completed the primary vaccine series by age group. Percentages are based on estimates of the total NYC population, population aged 18 years and older, and population aged 65 years and older. 

Indicators include: 

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|AGE_GROUP |Age in years (All ages; ages 5 to 17; 18 years and older; 65 years and older) | |
|PERC_PARTIALLY |Estimated percentage of the NYC population partially vaccinated by age group |Cumulative |
|PERC_FULLY |Estimated percentage of the total NYC population who compelted the primary vaccine series by age group |Cumulative |
|PERC_NOVAX |Estimated percentage of the total NYC population who have not been vaccinated for COVID-19 |Cumulative |

### coverage-summary-donut2.csv

This file contains information on the estimated percentage of NYC residents who have received at least one dose of COVID-19 vaccine by age group. Percentages are based on estimates of the total NYC population, population aged 5 to 17, population aged 18 years and older, and population aged 65 and older.

Indicators include: 

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|AGE_GROUP |Age in years (All ages; ages 5 to 17; 18 years and older; 65 years and older) | |
|PERC_1PLUS |Estimated percentage of the NYC population with at least one dose of COVID-19 vaccine |Cumulative |
|PERC_NOVAX |Estimated percentage of the NYC population who have not been vaccinated for COVID-19 |Cumulative |

### coverage-summary-donut3.csv

This file contains information on the estimated percentage of NYC residents who completed the primary vaccine series and received additional/booster doses. Percentages are based on estimates of the total NYC population, population aged 5 to 17, population aged 18 years and older, and population aged 65 and older.

Indicators include: 

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|AGE_GROUP |Age in years (All ages; ages 5 to 17; 18 years and older; 65 years and older) | |
|PERC_ADDITIONAL |Estimated percentage of the NYC population with additional/booster doses |Cumulative |
|PERC_DIFF |  Percent of NYC population without an additional dose|Cumulative |


### coverage-summary-allages.csv

This file contains information on the number and estimated percentage of NYC residents vaccinated (at least 1 dose, completed primary series, additional/booster doses), by borough. 

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|BOROUGH |Name of borough | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by borough |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who received at least one dose of COVID-19 vaccine by borough |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by borough |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series doses by borough |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who received at least 1 dose by borough |Cumulative |
|PERC_ADDITIONAL |Estimated percentage of the population with additional/booster doses by borough |Cumulative |

### coverage-summary-children.csv

This file has the same variable definitions as coverage-summary-allages.csv, but is restricted to vaccine eligible NYC children 5 to 17.

### coverage-summary-adults.csv

This file has the same variable definitions as coverage-summary-allages.csv, but is restricted to NYC adults 18 years and older.

### coverage-summary-65plus.csv

This file has the same variable definitions as coverage-summary-allages.csv, but is restricted to NYC adults 65 years and older.

### coverage-by-modzcta-allages.csv

This file contains information on the number and estimated percentage of NYC residents who completed the primary series and residents who received at least one dose of COVID-19 vaccine by Modified ZCTA (MODZCTA). Percentages of NYC residents vaccinated is calculated against the estimated total population of the specified MODZCTA. 

Note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. See [/technical notes](https://github.com/nychealth/covid-vaccine-data/blob/main/Readme.md#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) for more information on population estimates and MODZCTAs.

Individuals whose addresses are not valid and who could not be mapped to a MODZCTA are not included in the map or the data download.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|NEIGHBORHOOD_NAME |Neighborhood name of the MODZCTA | |
|BOROUGH |Name of borough | |
|MODZCTA |Modified ZCTA (Zip Code Tabulation Area, which solidifies Zip codes into units of area) | |
|Label |List of the ZIP Code Tabulation Areas (ZCTAs) that are bundled into the MODZCTA| |
|AGE_GROUP |Age in years | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_PARTIALLY_CUMULATIVE |Number of people partially vaccinated by MODZCTA |Cumulative |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by MODZCTA |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID_19 vaccine by MODZCTA |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by MODZCTA |Cumulative |
|PERC_PARTIALLY |Estimated percentage of the total population partially vaccinated by MODZCTA |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series by MODZCTA |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who have received at least one dose of COVID-19 vaccine by MODZCTA |Cumulative |
|PERC_ADDIITONAL |Estimated percentage of the population with additinonal/booster doses by MODZCTA |Cumulative |


Neighborhood names represent the [Neighborhood Organizing Census Committee](https://www1.nyc.gov/site/census/index.page) boundaries, which were recently developed by the U.S. Census Bureau with input from community groups.

Note that sum of counts in this file may not match values in citywide tables because of records with missing geographic information.

### coverage-by-modzcta-adults.csv

This file has the same variable definitions as coverage-by-modzcta-allages.csv, but is restricted to NYC residents 18 years and older.

### coverage-by-demo.csv

This file contains information on the number and estimated percentage of NYC residents vaccinated for COVID-19, stratified by age, race/ethnicity and sex. Percentages are calculated against the estimated total population for a specific geographic area or demographic category. Due to small numbers, data on people identified as Native Hawaiian and other Pacific Islander (NHPI) are combined with Asian. Data on people reported with other races/ethnicities and unknown race/ethnicity or sex are available as counts.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|POPULATION |Indicates the age group for the population denominator, either all ages, adults 18 years or older, or children 5 to 17| |
|GROUP |Used for display purposes only | |
|SUBGROUP |Indicates the age group in years, race/ethnicity, sex, or borough of residence | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_PARTIALLY_CUMULATIVE |Number of people partially vaccinated by indicated subgroup |Cumulative |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by indicated subgroup |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by indicated subgroup |Cumulative |
|PERC_PARTIALLY |Estimated percentage of the population partially vaccinated by indicated subgroup |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series by indicated subgroup |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|PERC_ADDITIONAL |Estimated percentage of the population with additional/booster doses by indicated subgroup |Cumulative |


### coverage-by-demo-allages.csv 

This file has the same variable definitions as coverage-by-demo.csv. The population denominator includes NYC residents of all ages. Data on people reported with two or more races, other races/ethnicities and unknown race/ethnicity or sex are not shown. Counts for these groups are available in coverage-by-demo.csv.

### coverage-by-demo-children.csv 

This file has the same variable definitions as coverage-by-demo.csv, but is restricted to NYC children aged 5 to 17. Data on people reported with two or more races, other races/ethnicities and unknown race/ethnicity or sex are not shown. Counts for these groups are available in coverage-by-demo.csv.

### coverage-by-demo-adults.csv 

This file has the same variable definitions as coverage-by-demo.csv, but is restricted to NYC adults 18 years and older. Data on people reported with two or more races, other races/ethnicities and unknown race/ethnicity or sex are not shown. Counts for these groups are available in coverage-by-demo.csv.


### coverage-by-boro-demo.csv

This file contains borough-level information on the number and estimated percentage of NYC residents vaccinated for COVID-19 by age and race/ethnicity. Percentages are calculated against the estimated total population for the specified borough and demographic category. Due to small numbers, data on people who identify as American Indian and Alaska Native, two or more races, and other races/ethnicities are not provided. People with unknown race/ethnicity are also not shown. 

Note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. See [/technical notes](https://github.com/nychealth/covid-vaccine-data/blob/main/Readme.md#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) for more information on population estimates.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|BOROUGH|Borough of residence | |
|RACE_ETHNICITY |Race/ethnicity group | |
|AGE_GROUP |Age group in years | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_PARTIALLY_CUMULATIVE |Number of people partially vaccinated by indicated subgroup |Cumulative |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by indicated subgroup |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by indicated subgroup |Cumulative |

|PERC_PARTIALLY |Estimated percentage of the population partially vaccinated by indicated subgroup |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series by indicated subgroup |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|PERC_ADDITIONAL |Estimated percentage of the population with additional/booster doses by indicated subgroup |Cumulative |


The sum of counts in this file may not match total borough or citywide values because of records with missing demographic or geographic information. Additionally, not all demographic groups at the borough-level are shown. 

### coverage-by-boro-demo-1plus.csv

This file contains borough-level counts and percentages of NYC residents who received at least one dose of COVID-19 vaccine, by age and race/ethnicity. Information is the same as in coverage-by-boro-demo.csv, but has a wide format for display purposes on our COVID-19 vaccine data page. Due to small numbers, data on people who identify as American Indian and Alaska Native, two or more races, and other races/ethnicities are not provided. People with unknown race/ethnicity are also not shown. Percentages are calculated against the estimated total population for a specific geographic area or demographic category. 


Note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. See [/technical notes](https://github.com/nychealth/covid-vaccine-data/blob/main/Readme.md#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) for more information on population estimates.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|RACE_ETHNICITY |Race/ethnicity group | |
|AGE_GROUP |Age group in years | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|CITY_COUNT_1PLUS_CUMULATIVE |Number of residents in NYC who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|BX_COUNT_1PLUS_CUMULATIVE |Number of residents in the Bronx who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|BK_COUNT_1PLUS_CUMULATIVE |Number of residents in Brooklyn who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|MH_COUNT_1PLUS_CUMULATIVE |Number of residents in Manhattan who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|QS_COUNT_1PLUS_CUMULATIVE |Number of residents in Queens who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|SI_COUNT_1PLUS_CUMULATIVE |Number of residents in Staten Island who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|CITY_PERC_1PLUS |Estimated percentage of residents in NYC who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|BX_PERC_1PLUS |Estimated percentage of residents in the Bronx who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|BK_PERC_1PLUS |Estimated percentage of residents in Brooklyn who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|MH_PERC_1PLUS |Estimated percentage of residents in Manhattan who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|QS_PERC_1PLUS |Estimated percentage of residents in Queens who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|SI_PERC_1PLUS |Estimated percentage of residents in Staten Island who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |

The sum of counts in this file may not match total borough or citywide values because of records with missing demographic or geographic information. Additionally, not all demographic groups at the borough-level are shown. 

### coverage-by-boro-demo-fully.csv

This file contains borough-level numbers on the count and percentage of NYC residents who completed the primary series by age and race/ethnicity. Information is the same as in coverage-by-boro-demo.csv, but has a wide format for display purposes on our COVID-19 vaccine data page. Due to small numbers, data on people who identify as American Indian and Alaska Native, two or more races, or other races/ethnicities are not provided. People with unknown race/ethnicity are not shown. Percentages are calculated against the total population for a specific geographic area or demographic category. 
 
Note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. See [/technical notes](https://github.com/nychealth/covid-vaccine-data/blob/main/Readme.md#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) for more information on population estimates.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|RACE_ETHNICITY |Race/ethnicity group | |
|AGE_GROUP |Age group in years | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|CITY_COUNT_FULLY_CUMULATIVE |Number of residents in NYC who completed the primary series by indicated subgroup |Cumulative |
|BX_COUNT_FULLY_CUMULATIVE |Number of residents in the Bronx who completed the primary series by indicated subgroup |Cumulative |
|BK_COUNT_FULLY_CUMULATIVE |Number of residents in Brooklyn who completed the primary series by indicated subgroup |Cumulative |
|MH_COUNT_FULLY_CUMULATIVE |Number of residents in Manhattan who completed the primary series by indicated subgroup |Cumulative |
|QS_COUNT_FULLY_CUMULATIVE |Number of residents in Queens who completed the primary series by indicated subgroup |Cumulative |
|SI_COUNT_FULLY_CUMULATIVE |Number of residents in Staten Island who completed the primary series by indicated subgroup |Cumulative |
|CITY_PERC_FULLY |Estimated percentage of residents in NYC who completed the primary series by indicated subgroup |Cumulative |
|BX_PERC_FULLY |Estimated percentage of residents in the Bronx who completed the primary series by indicated subgroup |Cumulative |
|BK_PERC_FULLY |Estimated percentage of residents in Brooklyn who completed the primary series by indicated subgroup |Cumulative |
|MH_PERC_FULLY |Estimated percentage of residents in Manhattan who completed the primary series by indicated subgroup |Cumulative |
|QS_PERC_FULLY |Estimated percentage of residents in Queens who completed the primary series by indicated subgroup |Cumulative |
|SI_PERC_FULLY |Estimated percentage of residents in Staten Island who completed the primary series by indicated subgroup |Cumulative |

The sum of counts in this file may not match total borough or citywide values because of records with missing demographic or geographic information. Additionally, not all demographic groups at the borough-level are shown. 

### coverage-by-boro-demo-additional.csv

This file contains borough-level numbers on the count and percentage of NYC residents who have received additional/booster doses, by age and race/ethnicity. Information is the same as in coverage-by-boro-demo.csv, but has a wide format for display purposes on our COVID-19 vaccine data page. Due to small numbers, data on people who identify as American Indian and Alaska Native, two or more races, or other races/ethnicities are not provided. People with unknown race/ethnicity are not shown. Percentages are calculated against the total population for a specific geographic area or demographic category. 

The sum of counts in this file may not match total borough or citywide values because of records with missing demographic or geographic information. Additionally, not all demographic groups at the borough-level are shown. 

### coverage-by-boro-age.csv

This file contains borough-level information on the number and estimated percentage of NYC residents vaccinated for COVID-19 by age group. Percentages are calculated against the total population for a specific geographic area and demographic category. Among people under 18 years old, only those aged 5 to 17 years are currently eligible for COVID-19 vaccination. 

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|BOROUGH|Borough of residence | |
|AGE_GROUP |Age group in years | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_PARTIALLY_CUMULATIVE |Number of people partially vaccinated by indicated subgroup |Cumulative |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by indicated subgroup |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by indicated subgroup |Cumulative |
|PERC_PARTIALLY |Estimated percentage of the population partially vaccinated by indicated subgroup |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series by indicated subgroup |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|PERC_ADDITIONAL |Estimated percentage of the population with additional/booster doses by indicated subgroup |Cumulative |

### coverage-by-boro-sex.csv

This file contains borough-level numbers on the count and percentage of NYC residents vaccinated for COVID-19 by sex. Percentages are calculated against the total population for a specific geographic area and demographic category. Counts with less than 10 people are suppressed and displayed as -- in the file.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|BOROUGH |Borough of residence | |
|SEX |Sex | |
|POP_DENOMINATOR |Population denominators derived from intercensal estimates as of 2019. Please see the technical notes for a description. | |
|COUNT_PARTIALLY_CUMULATIVE |Number of people partially vaccinated by indicated subgroup |Cumulative |
|COUNT_FULLY_CUMULATIVE |Number of people who completed the primary series by indicated subgroup |Cumulative |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by indicated subgroup |Cumulative |
|PERC_PARTIALLY |Estimated percentage of the population partially vaccinated by indicated subgroup |Cumulative |
|PERC_FULLY |Estimated percentage of the population who completed the primary series by indicated subgroup |Cumulative |
|PERC_1PLUS |Estimated percentage of the population who have received at least one dose of COVID-19 vaccine by indicated subgroup |Cumulative |
|COUNT_ADDITIONAL_CUMULATIVE |Number of people with additional/booster doses by indicated subgroup |Cumulative |


### by-residency-demo.csv

This file contains information on the number of NYC residents and non-NYC residents who received at least 1 dose of COVID-19 vaccine, stratified by age and race/ethnicity. NYC residents include people who received immunizations in NYC, NYS, NJ or elsewhere and reported to the CIR. Non-residents include people who reside outside the city and received at least one dose from a vaccinating facility located in NYC. Data on people who identify as two or more races, other races/ethnicities, or have unknown race/ethnicity or sex are available as counts. Counts with less than 10 people are suppressed and are displayed as -- in the file.

Data in this section can be used to describe the demographic characteristic of individuals who were vaccinated in NYC. Please refer to coverage-by-demo and coverage-by-boro-demo to compare vaccination coverage/rates in NYC across demographic groups.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|RESIDENCY |Place of residence (NYC; outside of NYC;unknown)| |
|RACE_ETHNICITY |Race/ethnicity group | |
|AGE_GROUP |Age group in years | |
|COUNT_1PLUS_CUMULATIVE |Number of people who have received at least one dose of COVID-19 vaccine by residency |Cumulative |


### by-residency-1plus-allages.csv

This file is used for display purposes on our COVID-19 vaccine data page and contains the same information as by-residency-demo.csv. Data includes people of all ages. People with unknown race/ethnicity or place of residence are not shown, but are available in by-residency-demo.csv.

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|RACE_ETHNICITY |Race/ethnicity group | |
|AGE_GROUP |Age group in years | |
|NON-NYC | Number of people who reside outside the city and received at least one dose from a vaccinating facility located in NYC |Cumulative |
|NYC | Number of NYC residents who received at least 1 dose of COVID-19 vaccine in NYC, NYS, NJ or elsewhere and reported to the CIR |Cumulative |

### by-residency-1plus-under18.csv

This file is used for display purposes on our COVID-19 vaccine data page and has the same variable definitions as by-residency-1plus-allages.csv. Data are restricted to children under 18. Note that only those aged 5 to 17 years are currently eligible for COVID-19 vaccination. 

People with unknown race/ethnicity or place of residence are not shown, but counts are available in by-residency-demo.csv. 

### by-residency-1plus-18to64.csv

This file is used for display purposes no our COVID-19 vaccine data page and has the same variable definitions as by-residency-1plus-allages.csv. Data are restricted to adults between the ages of 18 and 64 years old. People with unknown race/ethnicity or place of residence are not shown, but counts are available in by-residency-demo.csv.

### by-residency-1plus-65plus.csv

This file is used for display purposes on our COVID-19 vaccine data page and has the same variable definitions as by-residency-demo.csv. Data are restricted to adults 65 years and older. People with unknown race/ethnicity or place of residence are not shown, but counts are available in by-residency-demo.csv.

### by-residency-totals

This file is used for display purposes on our COVID-19 vaccine data page and contains the same information as by-residency-demo.csv. The file shows the number of people under 18 and over 18 who have received at least one dose of COVID-19 vaccine by their place of residence (NYC; outside of NYC; unknown). NYC residents include people who received immunizations in NYC, NYS, NJ or elsewhere and reported to the CIR. Non-residents include people who reside outside the city and received at least one dose from a vaccinating facility located in NYC. 

Indicators include:

|Variable |Definition |Timeframe |
|---------|-----------|----------|
|DATE |Date last updated | |
|RESIDENCY |Place of residence (NYC; outside of NYC; unknown)| |
|COUNT_1PLUS_CUMULATIVE_Under18 | Number of people under 18 who have received at least one dose of COVID-19 vaccine by place of residence |Cumulative |
|COUNT_1PLUS_CUMULATIVE_18plus | Number of people over 18 who have received at least one dose of COVID-19 vaccine by place of residence |Cumulative |
|COUNT_1PLUS_CUMULATIVE_Allages | Number of people who have received at least one dose of COVID-19 vaccine by place of residence |Cumulative |
|PERC_1PLUS_CUMULATIVE_Allages | Percentage of the total number of people vaccinated with at least 1 dose by place of residence |Cumulative ||


### trends-byage
This file contains information on the count and percent of NYC residents with at least one dose or fully vaccinated over time by age group. The age and vaccination status is indicated following the underscore (_) in each column heading. Cells less than 10 are suppressed and will show '<10'. 

### trends-byboro

This file contains information on the count and percent of NYC residents vaccinated over time by borough. The borough and vaccination status is indicated following the underscore (_) in each column heading.Cells less than 10 are suppressed and will show '<10'. 

### trends-byrace

This file contains information on the count and percent of NYC residents vaccinated over time by race/ethnicity. The race/ethnicity and vaccination status is indicated following the underscore (_) in each column heading. Cells less than 10 are suppressed and will show '<10'. Race/ethnicity categories shown here include Black, White, Hispanic/Latino, Asian or other Pacific Islander, and American Indian or Alaska Native. "Other" includes people of two or more races or other race/ethnicities. Note that other files in this repository disaggregate two or more races. "Unknown" includes people with incomplete race/ethnicity information. 

### trends-bysex

This file contains information on the count and percent of NYC residents vaccinated over time by sex. The race/ethnicity and vaccination status is indicated following the underscore (_) in each column heading. Cells less than 10 are suppressed and will show '<10'. "Other" includes people whose vaccination record indicates other or neither female or male. "Unknown" includes people with incomplete sex information or reporting prefer not to answer. 
