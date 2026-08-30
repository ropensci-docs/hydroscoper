# Greek borders

The borders of Greece are taken from Geoadata.gov.gr. The variables are
created using the function tidy from the broom package. This data frame
was created for use with the geom_polygon from ggplot2 package.

## Usage

``` r
greece_borders
```

## Format

A tibble with 18,474 rows and 8 variables:

- long:

  Longitude in decimal degrees, ETRS89

- lat:

  Latitude in decimal degrees, ETRS89

- order:

  order, integer

- hole:

  hole, boolean

- piece:

  piece, integer

- group:

  group, numeric

## Source

Konstantinos Vantas
