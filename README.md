<h1 align="center">Uber Data Analytics</h1>
This project analyzes Uber trip data and creates a dimensional data model to enable detailed analysis.

## Data
The data used is Uber trip data for New York City covering a period of 1 month. It contains over 100,000 records with the following columns:
- VendorID
- tpep_pickup_datetime
- tpep_dropoff_datetime
- passenger_count
- trip_distance
- pickup_longitude
- pickup_latitude
- RatecodeID
- store_and_fwd_flag
- dropoff_longitude
- dropoff_latitude
- payment_type
- fare_amount
- extra
- mta_tax
- tip_amount
- tolls_amount
- improvement_surcharge
- total_amount

## Analysis
1. The raw data is cleaned by dropping duplicate rows, formatting date columns and adding a trip_id column.
2. The data is transformed into fact and dimension tables as follows:
3. fact_table: Contains trip details with foreign keys to dimension tables
4. datetime_dim: Contains date and time information for pickups and drop offs
5. passenger_count_dim: Contains passenger count for each trip
6. trip_distance_dim: Contains trip distance for each trip
7. rate_code_dim: Contains rate code details for each trip
8. pickup_location_dim: Contains pickup location longitude and latitude
9. dropoff_location_dim: Contains dropoff location longitude and latitude
10. payment_type_dim: Contains payment type details for each trip
11. Visualizations are created to determine optimal advertising times based on order time histograms and rate code usage patterns.
12. Insights are generated regarding total fare amounts by rate code, most common passenger counts, average trip distance etc.
In short, a comprehensive dimensional data model is created to enable detailed analysis of the Uber trip data.

## Requirements
- Python 3
- Pandas
- Matplotlib (for visualizations)

Feel free to use and modify the code as needed. Let me know if you have any other questions!
