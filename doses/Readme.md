# doses/
This folder contains data on COVID-19 vaccines that were administered by vaccinating facilities in NYC and reported to the CIR. This includes doses that were administered to NYC residents and eligible non-NYC residents, including individuals who work or study in NYC.

## Files

### summary-doses.csv

This file contains information on the total number of vaccines delivered, and administered in NYC. Data on doses administered is reported separately for each dose of a two-dose vaccine series or single-dose vaccine. As of 5/13/2021, delivery information for Modern/Pfizer vaccine by dose number is no longer tracked separately and only the total number of doses delivered is reported. 

Indicators include:

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date | |
|DOSE1_CUMULATIVE |Cumulative number of first doses delivered or administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) |Cumulative |
|DOSE2_CUMULATIVE |Cumulative number of second doses delivered or administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) |Cumulative |
|SINGLE_CUMULATIVE |Cumulative number of doses delivered or administered of a single-dose COVID-19 vaccine (Single dose) |Cumulative |
|ALLDOSES_CUMULATIVE |Cumulative number of COVID-19 vaccine doses delivered or administered (Dose 1 of 2; Dose 2 of 2; Single dose) |Cumulative |

### doses-by-day.csv

This file contains information on the daily and cumulative numbers of COVID-19 vaccine doses administered by vaccinating facilities in NYC. Data are reported separately for each dose of a two-dose vaccine series or single-dose vaccine. 

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
|ADMIN_ALLDOSES_DAILY |Daily number of all COVID-19 vaccine doses administered (Sum of Dose 1 of 2; Dose 2 of 2; Single dose) |Daily, by date of vaccination |
|ADMIN_ALLDOSES_7DAYAVG |7-day moving average of all COVID-19 vaccine doses administered  (Sum of Dose 1 of 2; Dose 2 of 2; Single dose) |Current day and previous 6 days |
|ADMIN_ALLDOSES_CUMULATIVE |Cumulative number of all COVID-19 vaccine doses administered (Sum of Dose 1 of 2; Dose 2 of 2; Single dose) |Cumulative |
|INCOMPLETE | Used for display purposes only|


### doses-by-residency.csv

This file contains information on the number and percentage of COVID-19 doses administered to NYC and eligible non-NYC residents, including those who work or study in NYC. People with unknown place of residence are also included in this file. Residency status is based on the address or ZIP code that the vaccine recipient reported.

Indicators include:

|Variable Name |Definition |Timeframe|
|--------------|-----------|----------|
|DATE |Date | |
|RESIDENCY |Residency status (NYC; outside of NYC; unknown) | |
|ADMIN_DOSE1_CUMULATIVE |Cumulative number of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) by place of residence |Cumulative |
|ADMIN_DOSE2_CUMULATIVE |Cumulative number of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) by place of residence |Cumulative |
|ADMIN_SINGLE_CUMULATIVE |Cumulative number of single-dose COVID-19 vaccine administered by place of residence |Cumulative |
|ADMIN_ALLDOSES_CUMULATIVE |Cumulative number of all COVID-19 vaccine doses administered (Dose 1 of 2; Dose 2 of 2; Single dose) by place of residence |Cumulative |
|PERC_ADMIN_DOSE1 |Percent of first doses administered of a two-dose COVID-19 vaccine series (Dose 1 of 2) by place of residence |Cumulative|
|PERC_ADMIN_DOSE2 |Percent of second doses administered of a two-dose COVID-19 vaccine series (Dose 2 of 2) by place of residence |Cumulative|
|PERC_ADMIN_SINGLE |Percent of single-dose COVID-19 vaccine administered by place of residence|Cumulative|
|PERC_ADMIN_ALLDOSES |Percent of all doses administered (Dose 1 of 2; Dose 2 of 2; Single dose) by place of residence|Cumulative |

