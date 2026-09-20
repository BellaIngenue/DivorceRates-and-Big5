# Divorce rate - Data package

This data package contains the data that powers the chart ["Divorce rate"](https://ourworldindata.org/grapher/divorces-per-1000-people?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on September 20, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV structure

Each row is an observation for an entity (usually a country or region) at a timepoint.

- "Entity" — the name of the entity, e.g. "United States".
- "Code" — our internal entity code. For most countries this is the [ISO alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code, e.g. "USA"; historical and other non-standard entities get a custom code.
- "Year" or "Day" — the timepoint. Annual data has a "Year" column holding an integer year; otherwise a "Day" column holds a date string in the form "YYYY-MM-DD".
- The final column is the data column — the time series that powers the chart. Downloaded with the "full data" option it corresponds to the time series below; with "only selected data visible in the chart" it is transformed depending on the chart type, so the correspondence may be less direct.


## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc.

## How we process data at Our World in Data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stitch together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

Preparing this data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/).

## Detailed information about the data


### Crude divorce rate
Number of divorces during a given year per 1,000 people.
Last updated: October 7, 2025  
Next expected update: October 2026  
Date range: 1960–2022  
Unit: per 1,000 people  
Source: OECD (2025); OECD (2024); US Census Bureau (1949); Centers for Disease Control and Prevention (2020) – with minor processing by Our World in Data  

#### How to cite this data

OECD (2025) and other sources – with minor processing by Our World in Data

#### How this data is described by its producers
The crude divorce rate is defined as the number of divorces during a given year per 1,000 people.


## Sources

These are the sources behind the data in this package. Each time series above names the ones it draws on in its citation.

### OECD – OECD Family Database – Marriage and Divorce Rates

Marriage and divorce rates data from the OECD Family Database, including mean age at marriage. The OECD Family Database provides cross-national indicators on family outcomes and family policies across the OECD countries, its enhanced engagement partners and EU member states.

Producer: OECD  
Published: 2025-09-03  
Retrieved on: 2025-10-07  
Retrieved from: https://data-explorer.oecd.org/vis?tenant=archive&df[ds]=DisseminateArchiveDMZ&df[id]=DF_FAMILY&df[ag]=OECD  
Direct download: https://webfs.oecd.org/Els-com/Family_Database/SF_3_1_Marriage_divorce_rates.xlsx  
License: OECD Terms of Conditions (https://www.oecd.org/en/about/terms-conditions.html)  

Citation: OECD (2025). OECD Family Database.

### OECD – OECD Family Database

The OECD Family Database provides cross-national indicators on family outcomes and family policies across the OECD countries, its enhanced engagement partners and EU member states. It includes 70 indicators under four main dimensions: (i) structure of families, (ii) labor market position of families, (iii) public policies for families and children and (iv) child outcomes.

Producer: OECD  
Published: 2024-03-27  
Retrieved on: 2024-12-30  
Retrieved from: https://data-explorer.oecd.org/vis?tenant=archive&df[ds]=DisseminateArchiveDMZ&df[id]=DF_FAMILY&df[ag]=OECD&dq=..FAM14%2BFAM13%2BFAM15A%2BFAM15B%2BFAM10C%2BFAM10B%2BFAM10A%2BFAM9C%2BFAM9A%2BFAM9B%2BFAM7%2BFAM17%2BFAM8C%2BFAM8B%2BFAM11D%2BFAM11C%2BFAM11B%2BFAM11A%2BFAM8A%2BFAM5C%2BFAM5B%2BFAM5A%2BFAM4B%2BFAM12A%2BFAM12B%2BFAM4A%2BFAM3&pd=1960%2C2022&to[TIME_PERIOD]=false&vw=tb  
Direct download: https://sdmx.oecd.org/archive/rest/data/OECD,DF_FAMILY,/..FAM14+FAM13+FAM15A+FAM15B+FAM10C+FAM10B+FAM10A+FAM9C+FAM9A+FAM9B+FAM7+FAM17+FAM8C+FAM8B+FAM11D+FAM11C+FAM11B+FAM11A+FAM8A+FAM5C+FAM5B+FAM5A+FAM4B+FAM12A+FAM12B+FAM4A+FAM3?startPeriod=1960&endPeriod=2022&dimensionAtObservation=AllDimensions&format=csvfilewithlabels  
License: OECD Terms of Conditions (https://www.oecd.org/en/about/terms-conditions.html)  

Citation: OECD (2024). OECD Family Database.

### US Census Bureau – Vital Statistics, Health, and Nutrition Series

Vital statistics in the United States, including births, deaths, marriages, and divorces, are compiled nationally by the National Office of Vital Statistics, with data sourced from state and city registration officials.

Producer: US Census Bureau  
Published: 1949  
Retrieved on: 2025-01-22  
Retrieved from: https://www.census.gov/library/publications/1949/compendia/hist_stats_1789-1945.html  
Direct download: https://www2.census.gov/library/publications/1949/compendia/hist_stats_1789-1945/hist_stats_1789-1945-chC.pdf  
License: Open Government at the Census Bureau (https://www.census.gov/about/policies/open-gov.html)  

Citation: National Office of Vital Statistics, "Marriage and Divorce Statistics: United States, 1946," Vital Statistics-Special. Reports, vol. 27, No. 10.

### Centers for Disease Control and Prevention – Marriage Rates in the United States

Marriage license data is collected locally and reported to NVSS via the Vital Statistics Cooperative Program. Coverage varies by year and state: Alaska and Hawaii were included from 1959 and 1960, respectively, while California, Louisiana, and Georgia had exclusions in specific years. Population counts for non-reporting states are excluded from rate calculations for those years. Reports and data are available on the CDC and NCHS websites.

Producer: Centers for Disease Control and Prevention  
Published: 2020  
Retrieved on: 2025-01-22  
Retrieved from: https://www.cdc.gov/nchs/data/hestat/marriage_rate_2018/marriage_rate_2018.pdf  
Direct download: https://www.cdc.gov/nchs/data/hestat/marriage_rate_2018/marriage_rate_2018.pdf  
License: Public domain (https://stacks.cdc.gov/Content%20and%20Copyright)  

Citation: Curtin, S., & Sutton, P. D. (2020). Marriage rates in the United States, 1900–2018. Centers for Disease Control and Prevention.

    