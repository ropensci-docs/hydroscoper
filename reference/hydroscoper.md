# hydroscoper: Interface to Hydroscope

`hydroscoper` provides an R interface to the Greek National Data Bank
for Hydrological and Meteorological Information
`http://www.hydroscope.gr`.

`hydroscoper` covers Hydroscope's data sources using the `Enhydris API`
and provides functions to:

1.  Transform the available tables and data sets into
    [tibbles](https://tibble.tidyverse.org/).

2.  Transliterate the Greek Unicode names to Latin.

3.  Translate various Greek terms to English.

## Enhydris API

The Enhydris database is implemented in PostgreSQL. Details can be found
[here](https://enhydris.readthedocs.io)

## Data Sources

The data are retrieved from the Hydroscope's databases:

- Ministry of Environment, Energy and Climate Change.

- Ministry of Rural Development and Food.

- National Meteorological Service.

- Greek Public Power Corporation.

## See also

Useful links:

- <https://github.com/ropensci/hydroscoper>

- <https://docs.ropensci.org/hydroscoper/>

- Report bugs at <https://github.com/ropensci/hydroscoper/issues>

## Author

**Maintainer**: Konstantinos Vantas <kon.vantas@gmail.com>
([ORCID](https://orcid.org/0000-0001-6387-8791))

Other contributors:

- Sharla Gelfand (Sharla Gelfand reviewed the package for rOpenSci, see
  https://github.com/ropensci/onboarding/issues/185) \[contributor,
  reviewer\]

- Tim Trice (Tim Trice reviewed the package for rOpenSci, see
  https://github.com/ropensci/onboarding/issues/185) \[reviewer\]
