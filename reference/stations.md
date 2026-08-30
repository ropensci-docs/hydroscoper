# stations

Stations' data from the Greek National Data Bank for Hydrological and
Meteorological Information. This dataset is a comprehensive look-up
table with geographical and ownership information of the available
stations in all Hydroscope's databases.

## Usage

``` r
stations
```

## Format

A tibble with 2,322 rows and 9 variables:

- station_id:

  The station's ID from the domain's database

- name:

  The station's name

- water_basin:

  The station's Water Basin

- water_division:

  The station's Water Division

- owner:

  The station's owner

- longitude:

  The station's longitude in decimal degrees, ETRS89

- latitude:

  The station's latitude in decimal degrees, ETRS89

- altitude:

  The station's altitude, meters above sea level

- subdomain:

  The corresponding Hydroscope's database
