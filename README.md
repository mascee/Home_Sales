## Home Sales Project
## Challenge 22 by Olga Petrova

## What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

|year|average_price_4bedroom_house|
|----|----------------------------|
|2019|                    300263.7|
|2020|                   298353.78|
|2021|                   301819.44|
|2022|                   296363.88|
|----|----------------------------|


## What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

|date_built|average_price_3bedroom_date_built|
|----------|---------------------------------|
|      2010|                        297001.32|
|      2011|                         300603.7|
|      2012|                        298451.99|
|      2013|                        302956.63|
|      2014|                        302426.89|
|      2015|                        299061.15|
|      2016|                        302937.87|
|      2017|                        300313.63|
|----------|---------------------------------|


## What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.


|date_built|average_price_3bed_3bath_2floors_more2000sqrft|
|----------|----------------------------------------------|
|      2010|                                     285010.22|
|      2011|                                     276553.81|
|      2012|                                     307539.97|
|      2013|                                     303676.79|
|      2014|                                     298264.72|
|      2015|                                     297609.97|
|      2016|                                      293965.1|
|      2017|                                     280317.58|
|----------|----------------------------------------------|


## What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
   

|view|average_price_per_view|
|----|----------------------|
| 100|             1026669.5|
|  99|            1061201.42|
|  98|            1053739.33|
|  97|            1129040.15|
|  96|            1017815.92|
|  95|             1054325.6|
|  94|             1033536.2|
|  93|            1026006.06|
|  92|             970402.55|
|  91|            1137372.73|
|  90|            1062654.16|
|  89|            1107839.15|
|  88|            1031719.35|
|  87|             1072285.2|
|  86|            1070444.25|
|  85|            1056336.74|
|  84|            1117233.13|
|  83|            1033965.93|
|  82|             1063498.0|
|  81|            1053472.79|
|----|----------------------|


## Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
## 1.0106594562530518 seconds

## Running the same query on cached data gives this result:
## 0.9537603855133057 seconds

## Parquet data partitioned by "date_built" - same query gives this result:
## 0.7098813056945801 seconds

## It's a relatively small dataset, but the result is fastest if I use parquet method. 

## Table "home_sales" uncached and verified.