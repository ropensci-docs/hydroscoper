# Find nearest stations using a point's coordinates

`find_stations` returns a tibble with the nearest stations' distances
using a given point's longitude and latitude values. This function uses
the Haversine formula for distance calculation in km.

## Usage

``` r
find_stations(longitude = 24, latitude = 38)
```

## Arguments

- longitude:

  a numeric value in degrees

- latitude:

  a numeric value in degrees

## Value

If the given longitude is in \[24, 38\] and the latitude is in \[34,
42\] (i.e. are valid values for Greece) returns an ordered tibble with
the station_id, name, subdomain and distance values in km. The station's
data that are used come from the \`stations\` dataset. Otherwise returns
an error message.

## Examples

``` r

# find the five nearest stations to a point near Thessaloniki,
# (lon, lat) = (22.97, 40.60)
head(find_stations(22.97, 40.60), 5)
#> # A tibble: 5 × 4
#>   station_id name                   subdomain distance
#>        <int> <chr>                  <chr>        <dbl>
#> 1      20158 MS Thessalonikes       emy           2.96
#> 2      20201 A.M. SCHOLE THES/NIKES emy           3.97
#> 3      10032 THESSALONIKE           kyy           4.56
#> 4      20032 SEDES                  emy           6.88
#> 5      20033 MIKRA (THES/KES)       emy           8.07
```
