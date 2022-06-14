# doses/
This folder contains data on COVID-19 vaccines that were administered by vaccinating facilities in NYC and reported to the CIR. This includes doses that were administered to NYC residents and non-NYC residents, such as individuals who work or study in NYC.

Data on second booster doses are included as of 6/10/2022.

## Definitions

* **Doses Administered**: The number of COVID-19 vaccine doses that have been administered in NYC and reported to the CIR. This includes doses administered to NYC residents and non-NYC residents.

* **Doses Number**: Dose information is reported by date of vaccination. Data is broken-out by the two-dose Pfizer or Moderna primary vaccine series, the one dose Johnson & Johnson primary vaccine series and additional doses of Pfizer, Moderna, or Johnson & Johnson.
	* **Dose 1 of 2**: First dose administered of a two-dose primary vaccine series (Pfizer-BioNTech and Moderna)
	* **Dose 2 of 2**: Second dose administered of a two-dose primary vaccine series (Pfizer-BioNTech and Moderna)
	* **Single dose**: The dose administered of a single-dose primary vaccine series (Johnson & Johnson)
	*  **Additional/Booster 1**: First booster doses administered after the primary COVID-19 vaccine series. This includes first booster doses or the third dose  for people who are immunocompromised. This measure does not consider whether the vaccine recipient is immunocompromised or has an underlying medical condition.
	*  **Additional/Booster 2**: Second booster doses administered after the primary COVID-19 vaccine series and one booster dose. They could be the second booster doses or the first booster doses for people who are immunocompromised. This measure does not consider whether the vaccine recipient is immunocompromised or has an underlying medical condition.

## Files

### summary-doses.csv

This file contains information on the total number of vaccines delivered, and administered in NYC. 

Indicators include:

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date | |
|DOSE1_CUMULATIVE |Cumulative number of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) |Cumulative |
|DOSE2_CUMULATIVE |Cumulative number of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) |Cumulative |
|SINGLE_CUMULATIVE |Cumulative number of doses administered of a single-dose COVID-19 vaccine (Single dose) |Cumulative |
|ADDITIONAL_CUMULATIVE |Cumulative number of additional doses administered |Cumulative |
|ALLDOSES_CUMULATIVE |Cumulative number of COVID-19 vaccine doses delivered or administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional dose) |Cumulative |

### doses-by-day.csv

This file contains information on the daily and cumulative numbers of COVID-19 vaccine doses administered by vaccinating facilities in NYC. 

These data represent doses and should not be used to calculate the number of individuals who are vaccinated. Data on people vaccinated can be found in the [/people folder](https://github.com/nychealth/draft-data-pages/blob/9a7d696ed5ba5a367376b93f6fc332dc477ae7b7/Vaccine%20data/people/Readme.md).

Indicators include:

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date	|	|
|ADMIN_DOSE1_DAILY |Daily number of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2)|Daily, by date of vaccination |
|ADMIN_DOSE1_CUMULATIVE |Cumulative number of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) |Cumulative |
|ADMIN_DOSE2_DAILY |Daily number of second doses administered of a two dose COVID-19 vaccine series (Dose 2 of 2) |Daily, by date of vaccination |
|ADMIN_DOSE2_CUMULATIVE |Cumulative number of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) |Cumulative |
|ADMIN_SINGLE_DAILY |Daily number of single-dose COVID-19 vaccine administered |Daily by date of vaccination |
|ADMIN_SINGLE_CUMULATIVE |Cumulative number of single-dose COVID-19 vaccine administered |Cumulative |
|ADMIN_ADDITIONAL1_DAILY |Daily number of first booster doses or third doses administered for people who are immunocompromised. |Cumulative |
|ADMIN_ADDITIONAL1_CUMULATIVE |Cumulative number of first booster doses or third doses administered for people who are immunocompromised. |Cumulative |
|ADMIN_ADDITIONAL2_DAILY |Daily number of second booster doses administered after the primary COVID-19 vaccine series and one booster dose. Also includes the first booster dose for people immunocompromised. |Cumulative |
|ADMIN_ADDITIONAL2_CUMULATIVE |Cumulative number of second booster doses administered after the primary COVID-19 vaccine series and one booster dose. Also includes the first booster dose for people immunocompromised. |Cumulative |
|ADMIN_ADDITIONAL_DAILY |Daily number of additional/booster doses of COVID-19 vaccine administered, inclusing first and second boosters |Cumulative |
|ADMIN_ADDITIIONAL_CUMULATIVE |Cumulative number of additional/booster doses of COVID-19 vaccine administered,, inclusing first and second boosters |Cumulative |
|ADMIN_ALLDOSES_DAILY |Daily number of all COVID-19 vaccine doses administered (Sum of Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) |Daily, by date of vaccination |
|ADMIN_ALLDOSES_7DAYAVG |7-day moving average of all COVID-19 vaccine doses administered  (Sum of Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) |Current day and previous 6 days |
|ADMIN_ALLDOSES_CUMULATIVE |Cumulative number of all COVID-19 vaccine doses administered (Sum of Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) |Cumulative |
|INCOMPLETE | Used for display purposes only|


### doses-by-residency.csv

This file contains information on the number and percentage of COVID-19 doses administered to NYC and non-NYC residents at NYC vaccinating facilities. People with unknown place of residence are also included in this file. Residency status (NYC or non-NYC) is based on the address or ZIP code that the vaccine recipient reported.

Indicators include:

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date | |
|RESIDENCY |Residency status (NYC; outside of NYC; unknown) | |
|ADMIN_DOSE1_CUMULATIVE |Cumulative number of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) by place of residence |Cumulative |
|ADMIN_DOSE2_CUMULATIVE |Cumulative number of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) by place of residence |Cumulative |
|ADMIN_SINGLE_CUMULATIVE |Cumulative number of single-dose COVID-19 vaccine administered by place of residence |Cumulative |
|ADMIN_ADDITIONAL_CUMULATIVE |Cumulative number of additional/booster COVID-19 vaccine doses administered by place of residence |Cumulative |
|ADMIN_ALLDOSES_CUMULATIVE |Cumulative number of all COVID-19 vaccine doses administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional dose) by place of residence |Cumulative |
|PERC_ADMIN_DOSE1 |Percent of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) by place of residence |Cumulative|
|PERC_ADMIN_DOSE2 |Percent of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) by place of residence |Cumulative|
|PERC_ADMIN_SINGLE |Percent of single-doses COVID-19 vaccine administered by place of residence|Cumulative|
|PERC_ADMIN_ADDITIONAL |Percent of additional/booster COVID-19 vaccine doses administered by place of residence |Cumulative |
|PERC_ADMIN_ALLDOSES |Percent of all doses administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional dose) by place of residence|Cumulative |


### doses-by-residency-age.csv

This file contains information on the number and percentage of COVID-19 doses administered to NYC and non-NYC residents by age (under 18 and over 18). People with unknown place of residence are also included in this file. Residency status (NYC or non-NYC) is based on the address or ZIP code that the vaccine recipient reported.

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date ||
|RESIDENCY |Residency status (NYC; outside of NYC; unknown) | |
|ADMIN_ALLDOSES_CUMULATIVE_Under18 |Cumulative number of all COVID-19 vaccine doses administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) by place of residence |Cumulative |
|ADMIN_ALLDOSES_CUMULATIVE_18plus |Cumulative number of all COVID-19 vaccine doses administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) by place of residence |Cumulative |
|ADMIN_ALLDOSES_CUMULATIVE_Allages |Cumulative number of all COVID-19 vaccine doses administered (Dose 1 of 2; Dose 2 of 2; Single dose;  Additional/booster doses) by place of residence. This is the same as ADMIN_ALLDOSES_CUMULATIVE in the doses-by-residency.csv file |Cumulative |
|PERC_ADMIN_ALLDOSES_Allages |Percent of all doses administered (Dose 1 of 2; Dose 2 of 2; Single dose; Additional/booster doses) by place of residence. This is the same as PERC_ADMIN_ALLDOSES in the doses-by-residency.csv file |Cumulative |
