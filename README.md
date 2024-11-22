[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > C. Climate Data

# C. Climate Data
Climate Data consists of homogenous time series data (1, 2), spatial climate data (3-5), climate normals (6, 7) and scenarios (8):

- C1 - [Climate stations](#1-climate-stations)
- C2 - [Climate precipitation stations](#2-climate-precipitation-stations) :yellow_circle: *documentation upcoming*
- C3 - [Ground-based spatial climate data](#3-ground-based-spatial-climate-data) :yellow_circle: *documentation upcoming*
  - C31 - Gridded precipitation
  - C32 - Gridded relative sunshine duration
  - C33 - Gridded temperature
  - ...
- C4 - [Satellite-based spatial climate data](#4-satellite-based-spatial-climate-data) :yellow_circle: *documentation upcoming*
  - C41 - Gridded cloud fractional cover
  - C42 - Gridded global radiation
  - C43 - Gridded diffuse radiation
  - C44 - Gridded direct radiation
  - ...
- C5 - [Radar-based spatial climate data](#5-radar-based-spatial-climate-data) :yellow_circle: *documentation upcoming*
  - ...
- C6 - [Climate normals](#6-climate-normals) :yellow_circle: *documentation upcoming*
- C7 - [Spatial climate normals](#7-spatial-climate-normals) :yellow_circle: *documentation upcoming*
  - C71 - Precipitation normals
  - C72 - Sunshine duration normals
  - C73 - Temperature normals
- C8 - [Climate scenarios](#8-climate-scenarios) :yellow_circle: *documentation upcoming*

### General information
All MeteoSwiss surface stations have a name and an identfier consisting of three letters (e.g. `BER` for [Bern / Zollikofen](https://www.meteoswiss.admin.ch/services-and-publications/applications/measurement-values-and-measuring-networks.html#param=messnetz-klima&lang=en&station=BER&chart=hour&table=false) or `LUG` for [Lugano](https://www.meteoswiss.admin.ch/services-and-publications/applications/measurement-values-and-measuring-networks.html#param=messnetz-klima&lang=en&station=LUG&chart=hour&table=false)). Data files use this station identifier in the file name throughout all directories. A list of all station identfiers with station names, coordinates, height etc. can be found in the according 'station metadata' sections below.

---

## 1. Climate stations
The [Swiss National Basic Climatological Network "Swiss NBCN"](https://www.meteoswiss.admin.ch/weather/measurement-systems/land-based-stations/swiss-national-basic-climatological-network.html) connects the major ground-based stations within the MeteoSwiss monitoring network. It consists of around 30 climate monitoring stations. 

The [homogenous time series data](https://www.meteoswiss.admin.ch/climate/climate-change/changes-in-temperature-precipitation-and-sunshine/homogeneous-data-series-since-1864.html) for temperature, precipitation and hours of sunshine date back, in some cases, to the mid-nineteenth century.

### 1.1. Data granularity, update frequency, format and volume
If you require daily, monthly or annual values, we strongly recommend that you download the corresponding aggregated [data granularity](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#data-granularity) `D`, `M`, `Y` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) daily (`recent`) or yearly (`historical`) for each station.

Data format of all files is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ≤0.9 MB per file.

See example data files for station `BAS` for all granularities and update frequencies mentioned: [`ogd-nbcn_BAS_(data granularity)_(update frequency)`](https://github.com/MeteoSwiss/publication-opendata/tree/main/data-surface/climate-stations-swiss-nbcn-climate).

### 1.2. Parameter metadata
See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### 1.3. Station metadata
See example [station metadata file](...).

### 1.4. Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 2. Climate precipitation stations
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See example [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 3. Ground-based spatial climate data
Ground-based spatial climate data are statistically derived from *surface data*.

*See the overview of spatial climate products (PDF). For each product see the "detailed product document(s)" below for further information, and the parameter metadata in each example file.*

| Parameter                          | Subparameter         | Data granularities | PERIOD_TX = Update cycle | FILENAME                    | BOUND_BOX_COORD_SYS_TX | OUTPUT_COORDSYS_TX |
| ---------------------------------- | -------------------- | ------------------ | ------------------------ | --------------------------- | ---------------------- | ------------------ |
| Gridded precipitation              | Final analysis       | D                  | previous_month           | RhiresD_ch01h.swiss.lv95    | CH1995                 | EPSG:2056          |
| Gridded precipitation              | Final analysis       | M                  | previous_month           | RhiresM_ch01h.swiss.lv95    | CH1995                 | EPSG:2056          |
| Gridded precipitation              | Final analysis       | Y                  | previous_year            | RhiresY_ch01h.swiss.lv95    | CH1995                 | EPSG:2056          |
| Gridded precipitation              | Preliminary analysis | D                  | previous_day             | RprelimD_ch01h.swiss.lv95   | CH1995                 | EPSG:2056          |
| Gridded precipitation              | ?                    | M                  | previous_month           | RanomM9120_ch01r.swiss.lv95 | CH1995                 | EPSG:2056          |
| Gridded relative sunshine duration |                      | D                  | previous_day             | SrelD_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded relative sunshine duration |                      | M                  | previous_month           | SrelM_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded relative sunshine duration |                      | Y                  | previous_year            | SrelY_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded relative sunshine duration | ?                    | M                  | previous_month           | SanomM9120_ch01r.swiss.lv95 | CH1995                 | EPSG:2056          |
| Gridded temperature                | Absolute             | D                  | previous_day             | TabsD_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Absolute             | M                  | previous_month           | TabsM_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Absolute             | Y                  | previous_year            | TabsY_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Maximum              | D                  | previous_day             | TmaxD_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Maximum              | M                  | previous_month           | TmaxM_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Maximum              | Y                  | previous_year            | TmaxY_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Minimum              | D                  | previous_day             | TminD_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Minimum              | M                  | previous_month           | TminM_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | Minimum              | Y                  | previous_year            | TminY_ch01r.swiss.lv95      | CH1995                 | EPSG:2056          |
| Gridded temperature                | ?                    | M                  | previous_month           | TanomM9120_ch01r.swiss.lv95 | CH1995                 | EPSG:2056          |

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`NetCDF`](...) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
*See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See example [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 4. Satellite-based spatial climate data
Spatial climate data, which contain radiation and cloud cover parameters, are derived from [MeteoSat satellite data](...) together with *surface data*.

*See the overview of spatial climate products (PDF). For each product see the "detailed product document(s)" below for further information, and the parameter metadata in each example file.*

| *Parameter*                        | Data granularities   | FILENAME                              | *PERIOD_TX = Update frequency* | BOUND_BOX_COORD_SYS_TX | OUTPUT_COORDSYS_TX | OUTPUT_FORMAT_TX |
| ---------------------------------- | -------------------- | ------------------------------------- | -------------- | ---------------------- | ------------------ | ---------------- |
| *?*                                | *`H`, `D`, `M`, `Y`* | msg.ALB.H_ch02.lonlat                 | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.ALB.D_ch02.lonlat                 | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.ALB.M_ch02.lonlat                 | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.ALB.Y_ch02.lonlat                 | previous_year  | LL84                   | EPSG:4326          | NETCDF           |
| **Gridded cloud fractional cover** | `D`, `M`, `Y`        | msg.CFC.D_ch02.lonlat                 | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.CFC.M_ch02.lonlat                 | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.CFC.Y_ch02.lonlat                 | previous_year  | LL84                   | EPSG:4326          | NETCDF           |
| **Gridded global radiation**       | *`H`*, `D`, `M`, `Y` | msg.SIS.H_ch02.lonlat                 | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS.D_ch02.lonlat                 | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS.M_ch02.lonlat                 | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS.Y_ch02.lonlat                 | previous_year  | LL84                   | EPSG:4326          | NETCDF           |
| *?*                                | *`H`*                | msg.SISCF-No-Horizon.H_ch02.lonlat    | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
| **Gridded diffuse radiation**      | `H`, *`D`, `M`, `Y`* | msg.SISDIF-No-Horizon.H_ch02.lonlat   | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
| **Gridded direct radiation**       | `H`, `D`, `M`, `Y`   | msg.SISDIR.H_ch02.lonlat              | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR.D_ch02.lonlat              | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR.M_ch02.lonlat              | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR.Y_ch02.lonlat              | previous_year  | LL84                   | EPSG:4326          | NETCDF           |
| *?*                                | *`H`*                | msg.SISDIRCF-No-Horizon.H_ch02.lonlat | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
| *?*                                | *`H`, `D`, `M`, `Y`* | msg.SISDIR-No-Horizon.H_ch02.lonlat   | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR-No-Horizon.D_ch02.lonlat   | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR-No-Horizon.M_ch02.lonlat   | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SISDIR-No-Horizon.Y_ch02.lonlat   | previous_year  | LL84                   | EPSG:4326          | NETCDF           |
| *?*                                | *`H`*                | msg.SISDNI-No-Horizon.H_ch02.lonlat   | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
| *?*                                | *`H`, `D`, `M`, `Y`* | msg.SIS-No-Horizon.H_ch02.lonlat      | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS-No-Horizon.D_ch02.lonlat      | previous_day   | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS-No-Horizon.M_ch02.lonlat      | previous_month | LL84                   | EPSG:4326          | NETCDF           |
|                                    |                      | msg.SIS-No-Horizon.Y_ch02.lonlat      | previous_year  | LL84                   | EPSG:4326          | NETCDF           |

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`NetCDF`](https://www.unidata.ucar.edu/software/netcdf/) with an estimated volume of *0.1* MB per file.

See example data files: [`...`](...).

### Parameter metadata
*See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See example [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 5. Radar-based spatial climate data
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
*See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See example [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 6. Climate normals
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See example [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 7. Spatial climate normals
... 

| PERIOD_TX    | BOUND_BOX_COORD_SYS_TX | OUTPUT_COORDSYS_TX | OUTPUT_FORMAT_TX | filename                                                  |
| ------------ | ---------------------- | ------------------ | ---------------- | --------------------------------------------------------- |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | RnormM9120 Normwert Monatsniederschalg 1991-2020          |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | RnormY9120 Normwert Jahressniederschalg 1991-2020         |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TnormM9120 Normwert Monats-Mitteltemperatur 1991-2020     |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TnormY9120 Normwert Jahres-Mitteltemperatur 1991-2020     |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TminnormM9120 Normwert Monats-Minimumtemperatur 1991-2020 |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TminnormY9120 Normwert Jahres-Minimumtemperatur 1991-2020 |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TmaxnormM9120 Normwert Monats-Maximumtemperatur 1991-2020 |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | TmaxnormM9120 Normwert Jahres-Maximumtemperatur 1991-2020 |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | SnormM9120 Normwert Monats-Sonnenscheindauer 1991-2020    |
| previous_day | CH1995                 | EPSG:2056          | NETCDF           | SnormY9120 Normwert Monats-Sonnenscheindauer 1991-2020    |

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
*See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See example [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 8. Climate scenarios
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### Parameter metadata
See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See example [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>
