# Freedom of expression index - Data package

This data package contains the data that powers the chart ["Freedom of expression index"](https://ourworldindata.org/grapher/freedom-of-expression-index?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on March 18, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Freedom of Expression and Alternative Sources of Information index – (best estimate)
Best estimate of the extent to which people can discuss political matters at home and in the public sphere, the press, and media are free and can present different political perspectives, and the freedom of academic and cultural expression.
Last updated: March 7, 2024  
Next update: April 2025  
Date range: 1789–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
V-Dem (2024) – processed by Our World in Data

#### Full citation
V-Dem (2024) – processed by Our World in Data. “Freedom of Expression and Alternative Sources of Information index – (best estimate)” [dataset]. V-Dem, “V-Dem Country-Year (Full + Others) v14” [original data].
Source: V-Dem (2024) – processed by Our World In Data

### How is this data described by its producer - V-Dem (2024)?
Question: To what extent does government respect press and media freedom, the freedom of ordinary people to discuss political matters at home and in the public sphere, as well as the freedom of academic and cultural expression?

Clarification: This index includes all variables in the two indices v2x_freexp and v2xme_altinf.

Scale: Interval, from low to high (0-1).

Indicator name: `v2x_freexp_altinf`

### Source

#### V-Dem – V-Dem Country-Year (Full + Others)
Retrieved on: 2024-03-18  
Retrieved from: http://v-dem.net/vdemds.html  

#### Notes on our processing step for this indicator
We expand the years covered by V-Dem further: To expand the time coverage of today's countries and include more of the period when they were still non-sovereign territories, we identified the historical entity they were a part of and used that regime's data whenever available

For example, V-Dem only provides regime data since Bangladesh's independence in 1971. There is, however, regime data for Pakistan and the colony of India, both of which the current territory of Bangladesh was a part. We, therefore, use the regime data of Pakistan for Bangladesh from 1947 to 1970, and the regime data of India from 1789 to 1946. We did so for all countries with a past or current population of more than one million.


    