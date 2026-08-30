# Changelog

## hydroscoper 1.7.0 (Release date: 2024-07-19)

- `pingr` dependency has been removed. The check if a sub-domain is
  alive is performed by a native R function.

## hydroscoper 1.6.0 (Release date: 2024-01-15)

- Update dependencies

## hydroscoper 1.5.0 (Release date: 2022-09-29)

- remove defunct functions

## hydroscoper 1.4.1 (Release date: 2021-05-14)

CRAN release: 2021-05-14

- remove call to closeAllConnections() command

## hydroscoper 1.4 (Release date: 2021-03-20)

CRAN release: 2021-03-21

- Fail gracefully with an informative message if the hydroscope site is
  not available or has changed
- Update dependencies

## hydroscoper 1.3 (Release date: 2020-07-03)

CRAN release: 2020-03-07

- Update dependencies

## hydroscoper 1.2 (Release date: 2019-06-02)

CRAN release: 2019-06-04

- This version removes plyr dependency.

## hydroscoper 1.1.1 (Release date: 2018-08-25)

CRAN release: 2018-08-25

- This version fixes the errors found in CRAN Package Check Results.

## hydroscoper 1.1.0 (Release date: 2018-07-06)

CRAN release: 2018-07-06

- New functionality:

  - [`find_stations()`](https://docs.ropensci.org/hydroscoper/reference/find_stations.md)
    returns a tibble with the nearest hydroscope’s stations’ distances
    using a given point coordinates.

## hydroscoper 1.0.0 (Release date: 2018-03-16)

CRAN release: 2018-03-16

- `hydroscoper` was transferred to rOpenSci:
  <https://github.com/ropensci/hydroscoper>

- General

  - This is a major update. All the functions are rewritten utilizing
    the Enhydris API.

  - The included data in the package cover all Hydroscope’s databases.

  - Add vignettes “An introduction to `hydroscoper`” and “Using
    `hydroscoper`’s data”.

  - Add package documentation site.

  - All the functions return tibbles.

  - Add `greece_borders` dataset.

- New functionality:

  - [`get_instruments()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the instruments’ data.
  - [`get_water_basins()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Water Basins’ data.
  - [`get_water_divisions()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Water Divisions’ data.
  - [`get_political_divisions()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Political Divisions’ data.
  - [`get_variables()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Variables’ data.
  - [`get_units_of_measurement()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Units’ data.
  - [`get_time_steps()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Time Steps’ data.
  - [`get_owners()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Owners’ data.
  - [`get_instruments_type()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)returns
    a tibble with the Instruments’ type data.
  - [`get_station_type()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Water Basins data.
  - [`get_database()`](https://docs.ropensci.org/hydroscoper/reference/get_tables.md)
    returns a tibble with the Water Basins data.
  - `hydro_coords` returns a tibble with the stations’ longitudes and
    latitudes using as input the variable `point` from `get_stations`
    function.
  - [`hydro_translate()`](https://docs.ropensci.org/hydroscoper/reference/hydro_translate.md)
    translates various Greek terms to English.

- Changes

  - `get_stations` and `get_timeseries` use the Enhydris API and are
    considerably faster.
  - `get_data` uses lower case variable naming: `date, value, comment`

- Defuncs

  - `get_coords` has been removed from the package. Please use
    `hydro_coords` to convert Hydroscope’s points’ raw format to a
    tibble.

------------------------------------------------------------------------

## hydroscoper 0.1.0 (Release date: 2017-12-22)

CRAN release: 2017-12-22

- Initial submission to CRAN.
