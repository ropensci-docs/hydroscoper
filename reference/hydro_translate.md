# Translate Greek names and terms to English

`hydro_translate` translates various Hydroscope's names and terms to
English.

## Usage

``` r
hydro_translate(x, value = c("owner", "variable", "timestep", "division"))
```

## Arguments

- x:

  a string vector

- value:

  One of the predefined values in
  `c("owner", "variable", "timestep", "division")`

## Value

If `value` is one of:

- `owner`, organizations' names.

- `variable`, hydrometeorological term.

- `timestep`, timestep term.

- `division`, Water Division.

returns a character vector with translations of various
hydrometeorological terms or organizations' names from Greek (with latin
characters) to English.

The organizations' names in `owner` are:

|                      |                                           |
|----------------------|-------------------------------------------|
| **Code**             | **Name**                                  |
| min_envir_energy     | Ministry of Environment and Energy        |
| min_agricult         | Ministry of Rural Development and Food    |
| natio_meteo_service  | National Meteorological Service           |
| natio_observ_athens  | National Observatory of Athens            |
| public_power_corp    | Public Power Corporation                  |
| natio_argic_resear   | National Agricultural Research Foundation |
| greek_perfectures    | Greek Prefectures                         |
| crete_eng_faculty    | Technical University of Crete             |
| crete_natural_museum | Natural History Museum of Crete           |

The Greek Water Divisions codes in `division` are:

|          |                         |
|----------|-------------------------|
| **Code** | **Name**                |
| GR01     | Dytike Peloponnesos     |
| GR02     | Boreia Peloponnesos     |
| GR03     | Anatolike Peloponnesos  |
| GR04     | Dytike Sterea Ellada    |
| GR05     | Epeiros                 |
| GR06     | Attike                  |
| GR07     | Anatolike Sterea Ellada |
| GR08     | Thessalia               |
| GR09     | Dytike Makedonia        |
| GR10     | Kentrike Makedonia      |
| GR11     | Anatolike Makedonia     |
| GR12     | Thrake                  |
| GR13     | Krete                   |
| GR14     | Nesoi Aigaiou           |

## Note

The dictionary used for the Greek to English translation is:

|                         |                    |
|-------------------------|--------------------|
| **Transliterated term** | **English term**   |
| agnosto                 | unknown            |
| anemos                  | wind               |
| dieuthynse              | direction          |
| parelthon               | past               |
| tachyteta               | speed              |
| mese                    | average            |
| brochoptose             | precipitation      |
| diarkeia                | duration           |
| exatmise                | evaporation        |
| exatmisodiapnoe         | evapotranspiration |
| thermokrasia            | temperature        |
| edaphous                | ground             |
| bathos                  | depth              |
| elachiste               | min                |
| megiste                 | max                |
| piese                   | pressure           |
| semeiake                | point              |
| chioni                  | snow               |
| ypsometro               | elevation          |
| stathme                 | level              |
| plemmyra                | flood              |
| paroche                 | flow               |
| broche                  | precipitation      |
| katastase               | condition          |
| ektimemene              | estimation         |
| athroistiko             | cumulative         |
| stereo                  | sediment           |
| ygrasia                 | humidity           |
| ygro                    | wet                |
| apolyte                 | absolute           |
| schetike                | relative           |
| asbestio                | calcium            |
| wetu                    | precipitation      |
| chionobrochometro       | snow_rain_gauge    |
| xero                    | dry                |
| ydrometrese             | flow_gauge         |
| thalasses               | sea                |
| semeio_drosou           | dew_point          |
| oratoteta               | visibility         |
| steria                  | land               |
| thalassa                | sea                |
| barometro               | barometer          |
| tase_ydratmon           | vapour_pressure    |
| psychrometro            | psychrometer       |
| isodynamo_ypsos         | water_equivalent   |
| agogimoteta             | conductance        |
| aktinobolia             | radiation          |
| anthraka                | carbon             |
| dioxeidio               | dioxide            |
| ypoloipo                | residual           |
| argilio                 | aluminum           |
| argilos                 | clay               |
| arseniko                | arsenic            |
| pyritiou                | silicon            |
| aera                    | air                |
| nephokalypse            | cloud_cover        |
| nephose                 | clouds             |
| axiosemeiota            | remarkably         |
| nephe                   | clouds             |
| kairos                  | weather            |
| diafora                 | difference         |
| atmosfairiki            | atmospheric        |
| stathera                | constant           |
| parousa                 | present            |
| parelthousa             | past               |
| kalymeno                | cover              |
| el.                     | min                |
| meg.                    | max                |
| skleroteta              | hardness           |
| eliophaneia             | sunshine           |
| eisroe_se_tamieuteres   | inflow_reservoir   |

## Examples

``` r
if (FALSE) { # \dontrun{

# get data from the Ministry of Environment and Energy
kyy_owners <- get_owners("kyy")
kyy_vars <- get_variables("kyy")
owners_names <- hydro_translate(kyy_owners$name, "owner")
vars <- hydro_translate(kyy_vars$descr, "variable")
} # }
```
