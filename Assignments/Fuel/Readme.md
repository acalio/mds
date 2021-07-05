# Overview
An oil company has 82 gas stations located throughout the national territory. 

It is crucial for who runs the company to understand the right amount of fuel to refill any
of his/her gas stations. 

####  Example
For the sake of simplicity, let assume that the company has a budget of 1 millions euros and only 4 gas stations, located in different cities. 
A liter of fuel costs .669 euros to the company, while it costs 1.6 to the customers.

At the beginning of each week, Mr. Rossi  has to decide how to distribute 
the budget among the 4 stations.

Let us assume that he decides to distribute the budget as follows.


|                            | _Store:1_ (City center) | _Store:2_ (City center) | _Store:3_ (Sea) | _Store:4_ (Sea) |
|:--------------------------:|:-----------------------:|:-----------------------:|:---------------:|:---------------:|
| refill cost                | 250K                    | 250K                    | 250K            | 250K            |
| (new)  liters availability | 374K                    | 374K                    | 374K            | 374K            |


Since we are in the middle of summer, many people
are moving from the city to the sea. 
As a consequence, at the beginning of the following week we have the following situation

|                                   | _Store:1_ (City center) | _Store:2_ (City center) | _Store:3_ (Sea) | _Store:4_ (Sea) |
|:---------------------------------:|:-----------------------:|:-----------------------:|:---------------:|:---------------:|
| original liters availability      | 374K                    | 374K                    | 374K            | 374K            |
| residual                          | 120K                    | 200K                    | 0               | 0               |


In the above scenario, the company has 137K euros worth of unsold fuel.

Clearly, if Mr. Rossi had been able to correctly estimate the  amount of fuel withdrawn in the week, 
the company would have increased its profit.

--- 

In this context, we want to provide Mr. Rossi with an automated system that is able to 
correctly estimate the correct amount of fuel to be purchased for each gas station.

# Data
Each store is associated with two datasets, containing all the transactions recorded 
between 2018  and 2019.


We have two  representing for each store the transactions recorded beetween 2018 and 2019.

The attributes of the datasets are rather self explanatory.
- `consumption2018.xls`, `consumption2019.xls`
* store_id
* date
* liters_dispesed
* city
* year
* day
* month
* paid
* average_temperatures
* maximum_temperature
* minimum_temperature
* average_umidity
* maximum_umidity
* minimum_umidity
* flurry
* medium_visibility
* rainy_day
* dew_point
* phenomena
* average_windspeed
* maximum_windspeed
* average_sealevelpressure
* weather_condition
* number_of_inhabitants
* average_pressure

- `SeaCities.xls`
* city
- `GeoCoordinatesGEO.xls`
* city
* latitude
* longitude


