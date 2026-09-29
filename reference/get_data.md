# Get time series values in a tibble

`get_data` returns a tibble from a Hydroscope's time-series text file.

## Usage

``` r
get_data(subdomain = c("kyy", "ypaat", "emy", "deh"), time_id)
```

## Arguments

- subdomain:

  One of the subdomains of hydroscope.gr

- time_id:

  A time series ID

## Value

If `subdomain` is one of:

- `kyy`, Ministry of Environment and Energy

- `ypaat`, Ministry of Rural Development and Food

- `deh`, Greek Public Power Corporation

- `emy`, National Meteorological Service

and `time_id` exists in that `subdomain`, returns a tibble with the time
series values. Otherwise returns an error message.

The dataframe columns are:

- date:

  The time series Dates (POSIXct)

- value:

  The time series values (numeric)

- comment:

  Comments about the values (character)

## Note

Data are not available freely in the sub-domains: `"deh"` (Greek Public
Power Corporation) and `"emy"` (National Meteorological Service).

## References

Stations' data are retrieved from the Hydroscope's databases:

- Ministry of Environment, Energy and Climate Change.

- Ministry of Rural Development and Food.

## Author

Konstantinos Vantas, <kon.vantas@gmail.com>

## Examples

``` r
if (FALSE) { # \dontrun{
# get time series 912 from the Greek Ministry of Environment and Energy
time_series <- get_data("kyy", 912)
} # }
```
