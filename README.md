# CIA Factbook Data Analysis with SQL

## Project Overview
The CIA factbook is an annual publication of the US Central Intelligence Agency. It provides basic intelligence by summarizing demographic, geographic and other information about countries and regions worldwide.

This project aims to identify the leading and lagging countries or territories of the world based on demographic indicators like population, mortality, and fertility.

## Data Overview
The project uses data from this [SQLite factbook.db](https://dsserver-prod-resources-1.s3.amazonaws.com/257/factbook.db) database, collected between 2014 and 2015. There are two tables in the database: `sqlite_sequence` and `facts`.

The `facts` table contains 11 columns representing demographic and geographic information across 261 entities. The column names and their definitions are outlined below:

>- **id** - Entry row number.
>- **name** — Name of the country.
>- **code** — Internet code.
>- **area** — Total area (both land and water).
>- **area_land** — Land area in square kilometers.
>- **area_water** — Water area in square kilometers.
>- **population** —  Whole number of people or inhabitants.
>- **population_growth** — Population growth as a percentage.
>- **birth_rate** — Number of births per year per 1,000 inhabitants.
>- **death_rate** — Number of deaths per year per 1,000 inhabitants.
>- **migration_rate** — The difference between the number of persons entering and leaving a country during the year per 1,000 persons. 
 
## Approach
I queried the `facts` table with `SQL` to identify the leading and lagging countries in population statistics, birth rate, death rate, and migration rate. I also obtained additional information from online sources to buttress insights and cited each source with proper references.

## Key Findings
- China, India, the United States, Indonesia, and Brazil are the most populated countries in the world, accounting for 46% of the world's total population. The least populated locations are majorly Islands and dependencies.

- Regions with small land area like Macau, Monaco, Singapore, and Hong Kong are more densely populated than the rest of the world. However, when considering larger land areas, Bangladesh, South Korea, and Japan are the most densely populated countries.

- Birth rates are highest in Africa and lowest in Europe and Asia. 

- The highest death rates are recorded in Africa (Lesotho and Guinea-Bissau) and Eastern Europe (Bulgaria, Ukraine and Latvia). The lowest rates were recorded in the Gulf Cooperation Countries of the Middle-East (Qatar, Kuwait, Oman, UAE, Saudi Arabia and Bahrain).

- Population is rapidly declining in East and South-East Europe. This occurrence is due to reducing birth rates, increasing deaths, and emigration to other countries. Japan is also experiencing a population decline despite the positive forecasts over the years.

