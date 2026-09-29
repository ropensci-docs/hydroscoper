# timeseries

Time series' data from the Greek National Data Bank for Hydrological and
Meteorological Information. This dataset is a comprehensive look-up
table of all of the available measurements for a given station in a
given Hydroscope's database, with units of measurement and times of
those measurements.

## Usage

``` r
timeseries
```

## Format

A tibble with 10,804 rows and 9 variables:

- time_id:

  The time series ID

- station_id:

  The corresponding station's ID

- variable:

  The time series variable type

- timestep:

  The timestep of time series

- units:

  The units of the time series

- start_date:

  The starting date of time series values

- end_date:

  The ending date of time series values

- subdomain:

  The corresponding Hydroscope's database
