# Convert coordinates from Hydroscope's points to a tibble

`hydro_coords` returns a tibble with the stations' longitude and
latitude using as input the variable `point` from `get_stations`
function.

## Usage

``` r
hydro_coords(x)
```

## Arguments

- x:

  a string vector with the points retrieved from Hydroscope

## Value

a tibble with the longitude and latitude values.

## Details

Accepts two-dimensional POINT strings with optional SRID=4326. Points
without an SRID are assumed to use WGS84. No transformation is
performed. Unsupported explicit SRIDs cause an error. Missing, malformed
or out-of-range points return NA coordinates, retaining the input rows.

## Author

Konstantinos Vantas, <kon.vantas@gmail.com>

## Examples

``` r
if (FALSE) { # \dontrun{
# get stations from the Greek Ministry of Environment and Energy
kyy_stations <- get_stations("kyy")

# create a tibble with stations' coords
coords <- hydro_coords(kyy_stations$point)
} # }
```
