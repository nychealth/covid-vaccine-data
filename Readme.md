# COVID-19 Vaccination Reporting
This repository contains data on COVID-19 vaccinations administered by New York City (NYC) vaccinating facilities and reported to the Citywide Immunization Registry (CIR).

You can view a visualization of these data on the NYC Health Department's [COVID-19 Vaccines Data webpage](https://www1.nyc.gov/site/doh/covid/covid-19-data-vaccines.page). 

The CIR keeps immunization records for all city residents — children and adults — throughout their lives. COVID-19 vaccination data are reported by vaccinating facilities to the CIR and may be delayed. Data are updated daily with a 7-day lag, meaning that the most recent data in today's update are from the 7 days before. Data are preliminary and subject to change.
 
Data on second booster doses are included as of 6/10/2022.

***

## This Readme includes:

- Key Technical Notes
- Definitions
- Contents

***

## Key Technical Notes

### Citywide Immunization Registry and Reporting:

Since 1996, the CIR has been used as a database of patient immunization records submitted by NYC health care providers. It is accessible to authorized health care providers, schools, individuals and agencies concerned with public health to help ensure that NYC residents receive all recommended immunizations. NYC health care providers report immunizations to the CIR as mandated by New York State (NYS) Public Health Law and the NYC Health Code. Pediatric providers are required to report all immunizations administered to children 0-18 years. Reporting adult immunizations requires consent. However, from December 14, 2020 to June 26, 2021, the consent requirement was suspended by the [Governor’s executive order](https://www.governor.ny.gov/news/no-20282-continuing-temporary-suspension-and-modification-laws-relating-disaster-emergency) and the [Health Commissioner's order (PDF)](https://www1.nyc.gov/assets/doh/downloads/pdf/covid/covid-19-vaccine-reporting-order.pdf). These orders required providers to report COVID-19, flu and all other vaccinations administered to adults to the CIR. 

Currently, reporting adult immunizations requires patient consent. Immunization data are submitted to the CIR through electronic health record systems or through the [CIR’s Online Registry](https://www1.nyc.gov/site/doh/providers/reporting-and-services/citywide-immunization-registry-cir.page). 

### Reporting Timing: 

Data published each morning include entries recorded in the CIR by 3 PM the previous day. Providers are required to report COVID-19 vaccine doses to the CIR within 24 hours of administration. Pharmacies getting vaccine from the Federal Retail Pharmacy Programs are required to report within 72 hours of administration. Despite the requirements, reporting delays still exist due to technical difficulties in reporting for some providers. Therefore, our counts may underestimate the actual number of COVID-19 vaccine doses administered in NYC to date.

#### Report Date Versus Date of Event: 

Immunization data are published by date of vaccination. Vaccination data may be entered into CIR several days after the vaccine was administered. Therefore, new records reported to CIR each day contain a mix of vaccines that were administered the day prior, as well as vaccines that were administered on previous days. 

This approach may differ from data published by other state and local health departments. Publishing data by date of event better reflects when things happened, as opposed to when the Health Department learned about them. We strongly discourage data users from using daily changes to cumulative files as trend data, as this represents information by report date and is prone to misuse and misinterpretation.

### Differences Between City and State Values: 

Generally, numbers reported by the NYC Health Department and NYS Department of Health will be close but may not match exactly. Reasons for the discrepancies include:

- Inclusion of different vaccination programs, such as the CDC's Long-term Care Facility Program and Retail Pharmacy Program, or NYS-run vaccination hubs
- Different data sources for different metrics
- Different analytical and informatics processes
- Different uses of [event date or report date](#report-date-versus-date-of-event)


### Vaccine Eligibility:

As of November 3 2021, all U.S. residents 6 months of age and older are eligible to be vaccinated in NYC. Read more [here](https://www1.nyc.gov/site/doh/covid/covid-19-vaccines.page) about COVID-19 vaccine eligibility. 

Vaccine eligibility has expanded in phases as outlined by CDC and NYS, starting in Phase 1a with health care personnel and long-term care facility residents. In Phase 1b, COVID-19 vaccine was offered to persons aged ≥75 years and non-health care frontline essential workers, and in Phase 1c, to persons aged 65–74 years, persons aged 16–64 years with high-risk medical conditions, and essential workers not included in Phase 1b. Both the characteristics of people vaccinated (e.g., age, occupation) and the number of vaccinations administered shift over time, reflecting the populations that were eligible to be vaccinated and the supply of vaccine available.

Timeline of eligibility:

|Date |Eligibility |
|-----|------------|
|12/14/2020| - Patient-facing health care personnel <br /> - Long-term care residents and staff |
|1/4/2021 | - Ambulatory health care personnel <br /> - Home care and hospice workers |
|1/11/2021 | - First responders <br /> - Public safety officers <br /> - School staff <br /> - People 75 years or older|  
|1/19/2021 | - People 65 years or older <br /> - Congregate shelter residents and staff| 
|3/10/2021 | - People 60 years or older | 
|3/23/2021 | - People 50 years or older | 
|3/30/2021 | - People 30 years or older | 
|4/6/2021 | - People 16 years or older | 
|5/12/2021 | - People 12 years or older | 
|8/13/2021 | - Additional primary series dose authorized for immunocompromised people 12 years or older | 
|11/3/2021 | - People 5 years or older authorized for COVID-19 vaccine | 
|11/29/2021 | - Monovalent boosters authorized for people 18 years or older  | 
|12/9/2021 | - Monovalent boosters authorized for people 16 years or older  | 
|1/4/2022 | - Additional primary series dose authorized for immunocompromised children 5-11  | 
|1/5/2022 | - Monovalent boosters authorized for people 12 years or older  | 
|3/29/2022 | - Second monovalent booster authorized for older and immunocompromised individuals  | 
|5/25/2022 | - Monovalent boosters authorized for people 5 years or older  | 
|6/20/2022 | - People 6 months or older authorized for COVID-19 vaccine |
|8/31/2022 | - People 18 years or older authorized for Moderna bivalent dose; People 12 years or older authorized for Pfizer-BioNTech bivalent dose | 
|10/14/2022 | - People 6 years or older authorized for Moderna bivalent dose; People 5 years or odler authorized for Pfizer-BioNTech bivalent dose |
|12/8/2022 | - People 6 months or older authorized for bivalent dose |






### Vaccines Available:

Three COVID-19 vaccines have received emergency use authorizations for use in the U.S. by the [Food and Drug Administration (FDA)](https://www.fda.gov/emergency-preparedness-and-response/coronavirus-disease-2019-covid-19/covid-19-vaccines): Pfizer-BioNTech, Moderna, and Johnson & Johnson. These vaccines have been shown to be very safe and effective in protecting people from severe COVID-19 illness, hospitalization and death. Read more [here](https://www1.nyc.gov/site/doh/covid/covid-19-vaccines.page) about COVID-19 vaccines. 


## Definitions

* **Doses Delivered**: The number of COVID-19 vaccine doses that have been delivered to immunizing providers since December 14, 2020, including hospitals, community health centers, clinics, mass vaccination hubs and pharmacies.

* **Doses Administered**: The number of COVID-19 vaccine doses that have been administered in NYC and reported to the CIR. This includes doses administered to NYC residents and non-NYC residents.

* **Doses Number**: Dose information is reported by date of vaccination. Data is broken-out by the two-dose Pfizer, Moderna, or Novavax primary vaccine series, the one dose Johnson & Johnson primary vaccine series and additional doses of Pfizer, Moderna or Johnson & Johnson.
	* **Dose 1 of 2**: First dose administered of a two-dose primary vaccine series (Pfizer-BioNTech, Moderna, and Novavax)
	* **Dose 2 of 2**: Second dose administered of a two-dose primary vaccine series (Pfizer-BioNTech, Moderna, and Novavax)
	* **Single dose**: The dose administered of a single-dose primary vaccine series (Johnson & Johnson)
	* **Additional/booster doses**: Doses administered after the primary COVID-19 vaccine series, including monovalent booster and monovalent additional doses for people with a weakened immune system. 
    * **Bivalent dose**: Doses of Bivalent vaccines administered after the primary COVID-19 vaccine series, including both Moderna and Pfizer bivalent vaccines.
* **People Vaccinated**: The number of NYC residents vaccinated at an NYC facility, as well as city residents who were vaccinated outside of NYC and reported to us by: a provider in the city; the New York State Immunization Information System; the New Jersey Immunization Information System; or the Connecticut Immunization Registry and Tracking System. Information on the number of non-residents vaccinated in NYC can also be found in select datasets of this repository. Patient records are deduplicated since information on the same patient may be submitted by multiple providers. Vaccination status is classified into the following categories: 

    * **Partially Vaccinated**: The number of people who have received the first dose of a two-dose primary vaccine series (i.e. Pfizer-BioNtech or Moderna).
    * **Completed the primary series**: People who have received both doses of the Pfizer, Moderna, Novavax or AstraZeneca primary vaccine series or the one dose of the Johnson & Johnson vaccine primary vaccine series.
    * **At least one dose**: People who have received either the first dose of the two-dose Pfizer or Moderna primary vaccine series or the one dose of the Johnson & Johnson primary vaccine series. New Yorkers who received the AstraZeneca vaccine are only counted if they received both doses of the two-dose vaccine. 
    *  **Additional/booster doses**: People who have received additional doses of an FDA-approved monovalent vaccine after completing their primary series. This includes first and second booster shots, as well as additional doses for people who are immunocompromised.
    * **Bivalent dose**: People who have received a bivalent dose of vaccine. This may include people who completed the primary series outside of NYC and received a bivalent dose in NYC.

**Percent of NYC Residents Vaccinated, by Demographic Group and Geography**: 
The percent of NYC residents vaccinated is calculated against the total population estimate for a specific geographic area or demographic category. Population counts were calculated using intercensal estimates updated on October 9, 2020 to reflect annual population estimates for all New Yorkers as of July 1, 2019. The Health Department produced these population estimates using data from the U.S. Census Bureau and incorporating additional data from the NYC Department of City Planning and the Department of Buildings on new housing construction

Please note that the number of people vaccinated may exceed the estimated population and lead to more than 100% vaccination coverage, especially for smaller demographic categories and geographies. These estimates do not represent the 2020 Census or recent changes to NYC’s population as a result of in-migration or out-migration. Additional factors contributing to these inconsistencies may be that people who identify as Multi-race are misreported under a single race, and self-reported ZIP code at the time of vaccination may not correspond to the vaccine recipient’s primary home address. For example, people may use their work address for the purposes of vaccination.


***


### Demographic Characteristics

A large proportion of the COVID-19 data reported to the Citywide Immunization Registry (CIR) come from proprietary health care provider EHR systems that are not managed by the NYC Health Department. Data in the CIR are limited to what is available in EHR systems and to the fields required for submission. For example, information on race, ethnicity, sexual orientation, and gender identity (SOGI) can be incomplete. Current standards for reporting do not capture the diversity of NYC, particularly with respect to multi-racial people, gender expansive people, and those who identify across the spectrum of sexual orientation. 

New York City is striving to improve the way EHR systems collect and communicate information on race, ethnicity and SOGI. The Interoperability Standards Advisory provide a single, public list of health IT standards and implementation specifications. National guidance was last updated in 2000 [Interoperability Standards Advisory, 2000](https://www.healthit.gov/isa/representing-patient-race-and-ethnicity), and as of March 2021 had only 3 values for sex and none for SOGI information. Currently, the Advisory is expanding its guidance for collection of sex and SOGI fields. On 5/19/2021 the CIR modified its systems to capture an expanded list of values for sex, and SOGI fields. Updating the minimum national standards is vital to advancing health equity and addressing the intersectional needs of NYC’s diverse communities. 


### ZIP Codes and ZIP Code Tabulation Areas (ZCTAs):

We report information by geography using modified ZIP Code Tabulation Areas (MODZCTA) based on the ZIP code of residence reported by the vaccination recipient at the time of vaccination. A ZIP code does not refer to a specific area, but rather a collection of addresses that make up a mail delivery route. ZIP codes may be applied to individual buildings and non-residential areas in addition to residential areas.

To deal with the challenges of ZIP Codes, the Health Department uses ZCTAs which solidify ZIP codes into units of area. Often, data reported by ZIP code are mapped by ZCTA. The ZCTA geography was developed by the U.S. Census Bureau. MODZCTA is a geography used to analyze health data. The MODZCTA geography combines census blocks with smaller populations to allow more stable estimates of population size for rate calculation. See [here](https://nychealth.github.io/covid-maps/modzcta-geo/about.html) to identify which MODZCTA a ZIP code is in. 

Please note that the number of people vaccinated in some neighborhoods may exceed the estimated population. The [percentage of people vaccinated](#percent-of-nyc-residents-vaccinated-by-demographic-group-and-geography) are calculated using intercensal population estimates from 2019, which do not reflect the most recent 2020 Census numbers. Additional factors contributing to these inconsistencies may be that self-reported ZIP code at the time of vaccination may not correspond to the vaccine recipient’s primary home address. For example, people may use their work address for the purposes of vaccination.

Individuals whose addresses are not valid and who could not be mapped to a MODZCTA are not included in the map or the data download.


### Age Groups:

Data are reported for the following age groups per U.S. Census age categories: 0-4, 5-12, 13-17, 18-24, 25-34, 35-44, 45-54, 55-64, 65-74, 75-84, and 85+ years. Among people under 18, only those aged 6 months to 17 years are currently eligible for COVID-19 vaccination. See [here](https://www1.nyc.gov/site/doh/covid/covid-19-vaccines.page?utm_source=Google_Search&utm_medium=English&utm_campaign=COVID19Vaccine) for more information on vaccine eligibility. 


### Race/Ethnicity: 

Although CDC requires providers to report demographic information, including race/ethnicity, these data have not been consistently captured in COVID-19 vaccination records, particularly at the beginning of the vaccination campaign. The Health Department has been working with health care providers to improve capture of race/ethnicity information in the CIR, and the completeness of race/ethnicity data has improved over time. 

The Health Department classifies the proportion of people vaccinated by race/ethnicity into the following mutually exclusive categories: Asian/Native Hawaiian or other Pacific Islander (NHPI), Black/African-American, Hispanic/Latino, Native American/Alaska Native, and White. The Hispanic/Latino category includes people of any race, and all other categories exclude those who identify as Hispanic/Latino. Disaggregated information on vaccinations among people identified as Native Hawaiian or other Pacific Islander, other races/ethnicities, and multi-racial are provided only as counts due to small numbers and population estimates for these groups. Please see people/coverage_by_demo.csv and people/by_demo_residency.csv for those counts. 

The Health Department is committed to ensuring that access to the vaccine is fair and equitable and reaches communities hardest hit by COVID-19. COVID-19 has disproportionately impacted communities of color due to long-term institutional and personal biases against people of color. Lasting racism and an inequitable distribution of resources needed for wellness cause these health inequities. Key drivers include quality jobs, housing, health care and food, among others. The Health Department is closely monitoring disparities in neighborhood vaccination rates and by race/ethnicity to inform community outreach efforts and address gaps in vaccine access.

### Sex, Gender Identity, Sexual Orientation: 

The CIR currently only captures "sex" categorized as Male, Female, Other, Prefer not to answer and Unknown. The data do not currently capture gender identity or sexual orientation of adults vaccinated. Most of the data in the CIR come from health care providers’ EHR systems, which capture a limited number of fields. The Health Department uses NYS guidance for capturing sexual orientation and gender identity related data (SOGI). For CIR reporting, we do not regulate health care providers or determine what information a provider includes in their EHR systems. Read more [here](#demographic-characteristics) about SOGI data collection.

***


## Repository Contents

### doses/

This folder contains data on COVID-19 vaccines that were administered by vaccinating facilities in NYC and reported to the CIR. This includes doses that were administered to NYC residents and eligible non-NYC residents, including individuals who work or study in NYC. 

### people/ 

This folder contains information on the number of people who received at least 1 dose, the primary vaccine series, and additional/booster doses. These data include the number of NYC residents vaccinated at an NYC facility, as well as city residents who were vaccinated outside of NYC and reported to us by: a provider in the city; the New York State Immunization Information System; the New Jersey Immunization Information System; or the Connecticut Immunization Registry and Tracking System. Files that begin with ‘by-residency’ also include data on the number of non-NYC residents vaccinated at a NYC facility.
