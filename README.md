# NYC Taxi Trend Analysis

A data-science course project exploring NYC yellow taxi trip records with Python notebooks.

## Questions

The project explored how demand, destinations, and recorded tips vary by time, location, and passenger count. The initial dataset covered February 2022 and contained approximately three million trips.

## Data and Workflow

The records include pickup and drop-off times and zones, passenger counts, distances, fares, payment types, and recorded tips.

- [NYC TLC trip records](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- [Analysis notebook 1](termProject_1.ipynb)
- [Analysis notebook 2](termProject_2.ipynb)

I used this project to practice examining a large real-world dataset and looking for patterns through grouped analysis in Python.

## Scope

This repository contains exploratory analysis notebooks. The patterns in one period should not be treated as a validated demand-forecasting model.

The `tip_amount` field includes automatically recorded credit-card tips and excludes cash tips, which matters when interpreting tipping patterns. The source records are supplied to the TLC by technology providers and may contain data-quality issues.

<details>
<summary>Dataset fields</summary>

|column_name|description|
|-----------|:-----------|
|VendorID|A code indicating the TPEP provider that provided the record. <br>1 : Creative Mobile Technologies <br>2 : VeriFone Inc.|
|tpep_pickup_datetime|The date and time when the meter was engaged.|
|tpep_dropoff_datetime|The date and time when the meter was disengaged.|
|passenger_count|The number of passengers in the vehicle. This is a driver-entered value.|
|trip_distance|The elapsed trip distance in miles reported by the taximeter.|
|RatecodeID|The final rate code in effect at the end of the trip. <br>1 : Standard rate <br>2 : JFK <br>3 : Newark <br>4 : Nassau or Westchester <br>5 : Negotiated fare <br>6 : Group ride|
|store_and_fwd_flag|This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka “store and forward,” because the vehicle did not have a connection to the server.  <br>Y : store and forward trip <br>N : not a store and forward trip|
|PULocationID|TLC Taxi Zone in which the taximeter was engaged.|
|DOLocationID|TLC Taxi Zone in which the taximeter was disengaged.|
|payment_type|A numeric code signifying how the passenger paid for the trip. <br>1 : Credit card <br>2 : Cash <br>3 : No charge <br>4 : Dispute <br>5 : Unknown <br>6 : Voided trip|
|fare_amount|The time-and-distance fare calculated by the meter.|
|extra|Miscellaneous extras and surcharges. Currently, this only includes. the 0.50 dollar and 1 dollar rush hour and overnight charges.|
|mta_tax|0.50 MTA tax that is automatically triggered based on the metered rate in use.|
|tip_amount|Tip amount – This field is automatically populated for credit card tips.Cash tips are not included.|
|tolls_amount|Total amount of all tolls paid in trip.|
|improvement_surcharge|0.30 improvement surcharge assessed trips at the flag drop. the improvement surcharge began being levied in 2015.|
|total_amount|The total amount charged to passengers. Does not include cash tips.|
|congestion_surcharge|It represents the additional cost of New York traffic congestion.|

</details>
