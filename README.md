# Bank-Branches-in-LA-Data-Collection
Using the FDIC BankFind Suite API, location data for all Bank branches in LA region were collected.

The repo includes Jupyter Notebook (Bank_Loc_Data.ipynb), which executes the following steps:

1. API Call: Fetches all bank branch locations (/api/locations) across the state of California (STALP:CA).

2. Field Extraction: Extracts necessary fields including NAME, CITY, DEPSUM (Total Deposits in Millions), ADDRESS, and geographic coordinates.

3. Client-Side Filtering: Filters the entire state dataset to only include branches located in the target CITY: LOS ANGELES.

4. Output: Saves the final, filtered dataset of approximately 300 branch records (299 total, 42 BofA) to la_city_ca_fdic_branches.csv.

la_city_ca_fdic_branches.csv is also made part of this repo.

For details about how to use API
https://api.fdic.gov/banks/docs/

Latitude and Longitude information was added to la_city_ca_fdic_branches.csv using Geoapify (la_city_ca_fdic_branches_lat_long.csv)
https://www.geoapify.com/tools/geocoding-online/
