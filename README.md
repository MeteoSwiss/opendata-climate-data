[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > C. Climate Data

# C. Climate Data
Climate Data consists of homogenous time series data (1, 2), spatial climate data (3-5), climate normals (6, 7) and scenarios (8):

- C1 - [Climate stations - Homogeneous measurements](#c1---climate-stations---homogeneous-measurements)
- C2 - [Climate precipitation stations - Homogeneous measurements](#c2---climate-precipitation-stations---homogeneous-measurements)
- C3 - [Ground-based spatial climate data](#c3---ground-based-spatial-climate-data) - Precipitation, Temperature, Relative Sunshine Duration
- C4 - [Satellite-based spatial climate data](#4-satellite-based-spatial-climate-data)
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

## C1 - Climate stations - Homogeneous measurements
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

## C2 - Climate precipitation stations - Homogeneous measurements
... 

...

### 2.1. Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See example data files: [`...`](...).

### 2.2. Parameter metadata
See example parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### 2.3. Station metadata
See example [station metadata file](...).

### 2.4. Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## C3 - Ground-based spatial climate data
The following *grid data products* are statistically derived from *surface data* (see the links for the detailed product documentations):

**Precipitation**
- [Daily Precipitation (Preliminary analysis)](https://www.meteoswiss.admin.ch/dam/jcr:86ca15d3-2b56-4753-84fb-135e40d6a5a1/ProdDoc_RprelimD.pdf)
- [Daily Precipitation (Final analysis)](https://www.meteoswiss.admin.ch/dam/jcr:4f51f0f1-0fe3-48b5-9de0-15666327e63c/ProdDoc_RhiresD.pdf)
- [Monthly and Yearly Precipitation (Final analysis)](https://www.meteoswiss.admin.ch/dam/jcr:d4f53a4a-d7f4-4e1e-a594-8ff4bfd1aca5/ProdDoc_RhiresM.pdf)

**Temperature**
- [Daily Mean, Minimum and Maximum Temperature](https://www.meteoswiss.admin.ch/dam/jcr:818a4d17-cb0c-4e8b-92c6-1a1bdf5348b7/ProdDoc_TabsD.pdf)
- [Monthly and Yearly Mean Temperature](https://www.meteoswiss.admin.ch/dam/jcr:33e26211-9937-4f80-80a3-09cfe54663bc/ProdDoc_TabsM.pdf)

**Relative Sunshine Duration**
- [Daily Relative Sunshine Duration](https://www.meteoswiss.admin.ch/dam/jcr:981891db-30d1-47cc-a2e1-50c270bdaf22/ProdDoc_SrelD.pdf)
- [Monthly and Yearly Relative Sunshine Duration](https://www.meteoswiss.admin.ch/dam/jcr:94421f3c-47f3-46fa-9939-1d494a0ce5fe/ProdDoc_SrelM.pdf)

<br>

Coordinate system is [`Swiss LV95`](https://www.swisstopo.admin.ch/en/the-swiss-coordinates-system) / [`EPSG:2056`](https://epsg.io/2056). 

Data format is [`NetCDF`](https://www.unidata.ucar.edu/software/netcdf/) with an estimated volume of 1.1 MB for *individual files*, and 13 MB for monthly files with daily data.

<br>

The following *example* data files are available for download:

| *Parameter*                        | *Product*            | Time interval      | Update cycle             | *Example* Data files (see STAC Assets) |
| ---------------------------------- | -------------------- | ------------------ | ------------------------ | -------------------------------------- |
| Precipitation                      | Preliminary analysis | Daily              | previous_day             | RprelimD_ch01h.swiss.lv95              |
|                                    | Final analysis       | Daily              | previous_month           | *[RhiresD_ch01h.swiss.lv95_202305010000_202305310000.nc](https://github.com/MeteoSwiss/publication-opendata-spatial-climate-data/blob/main/RhiresD_ch01h.swiss.lv95_202305010000_202305310000.nc)* |
|                                    | Final analysis       | Monthly            | previous_month           | [RhiresM_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Final analysis       | Yearly             | previous_year            | *[RhiresY_ch01r.swiss.lv95_202201010000_202201010000.nc](https://github.com/MeteoSwiss/publication-opendata-spatial-climate-data/blob/main/RhiresY_ch01r.swiss.lv95_202201010000_202201010000.nc)* |
|                                    | ?                    | Monthly            | previous_month           | [RanomM9120_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
| Temperature                        | Absolute or Mean ?   | Daily              | previous_day             | [TabsD_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Absolute or Mean ?   | Monthly            | previous_month           | [TabsM_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Absolute or Mean ?   | Yearly             | previous_year            | TabsY_ch01r.swiss.lv95             |
|                                    | Maximum              | Daily              | previous_day             | [TmaxD_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Maximum              | Monthly            | previous_month           | [TmaxM_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Maximum              | Yearly             | previous_year            | TmaxY_ch01r.swiss.lv95             |
|                                    | Minimum              | Daily              | previous_day             | [TminD_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Minimum              | Monthly            | previous_month           | [TminM_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    | Minimum              | Yearly             | previous_year            | TminY_ch01r.swiss.lv95             |
|                                    | ?                    | Monthly            | previous_month           | [TanomM9120_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
| Relative Sunshine Duration         |                      | Daily              | previous_day             | [SrelD_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    |                      | Monthly            | previous_month           | [SrelM_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |
|                                    |                      | Yearly             | previous_year            | SrelY_ch01r.swiss.lv95      |
|                                    | ?                    | Monthly            | previous_month           | [SanomM9120_ch01r.swiss.lv95](https://sys-data.int.bgdi.ch/browser/index.html#/collections/ch.meteoschweiz.ogd-surface-derived-grid/items/ch?.language=en) |

<br>

## 4. Satellite-based spatial climate data
Spatial climate data, which contain radiation and cloud cover parameters, are derived from [MeteoSat satellite data](...) together with *surface data*.

*See the overview of spatial climate products (PDF). For each product see the "detailed product document(s)" below for further information, and the parameter metadata in each example file.*

| Parameter                      | Subparameter         | Data granularities | PERIOD_TX = Update cycle | FILENAME                              | BOUND_BOX_COORD_SYS_TX | OUTPUT_COORDSYS_TX |
| ------------------------------ | -------------------- | ------------------ | ------------------------ | ------------------------------------- | ---------------------- | ------------------ |
| ?                              |                      | H                  | previous_day             | msg.ALB.H_ch02.lonlat                 | LL84                   | EPSG:4326          |
| ?                              |                      | D                  | previous_day             | msg.ALB.D_ch02.lonlat                 | LL84                   | EPSG:4326          |
| ?                              |                      | M                  | previous_month           | msg.ALB.M_ch02.lonlat                 | LL84                   | EPSG:4326          |
| ?                              |                      | Y                  | previous_year            | msg.ALB.Y_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded cloud fractional cover |                      | H ?                |                          |                                       |                        |                    |
| Gridded cloud fractional cover |                      | D                  | previous_day             | msg.CFC.D_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded cloud fractional cover |                      | M                  | previous_month           | msg.CFC.M_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded cloud fractional cover |                      | Y                  | previous_year            | msg.CFC.Y_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded global radiation       |                      | H                  | previous_day             | msg.SIS.H_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded global radiation       |                      | D                  | previous_day             | msg.SIS.D_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded global radiation       |                      | M                  | previous_month           | msg.SIS.M_ch02.lonlat                 | LL84                   | EPSG:4326          |
| Gridded global radiation       |                      | Y                  | previous_year            | msg.SIS.Y_ch02.lonlat                 | LL84                   | EPSG:4326          |
| ?                              |                      | H                  | previous_day             | msg.SISCF-No-Horizon.H_ch02.lonlat    | LL84                   | EPSG:4326          |
| Gridded diffuse radiation      |                      | H                  | previous_day             | msg.SISDIF-No-Horizon.H_ch02.lonlat   | LL84                   | EPSG:4326          |
| Gridded diffuse radiation      |                      | D ?                |                          |                                       |                        |                    |
| Gridded diffuse radiation      |                      | M ?                |                          |                                       |                        |                    |
| Gridded diffuse radiation      |                      | Y ?                |                          |                                       |                        |                    |
| Gridded direct radiation       |                      | H                  | previous_day             | msg.SISDIR.H_ch02.lonlat              | LL84                   | EPSG:4326          |
| Gridded direct radiation       |                      | D                  | previous_day             | msg.SISDIR.D_ch02.lonlat              | LL84                   | EPSG:4326          |
| Gridded direct radiation       |                      | M                  | previous_month           | msg.SISDIR.M_ch02.lonlat              | LL84                   | EPSG:4326          |
| Gridded direct radiation       |                      | Y                  | previous_year            | msg.SISDIR.Y_ch02.lonlat              | LL84                   | EPSG:4326          |
| ?                              |                      | H                  | previous_day             | msg.SISDIRCF-No-Horizon.H_ch02.lonlat | LL84                   | EPSG:4326          |
| ?                              |                      | H                  | previous_day             | msg.SISDIR-No-Horizon.H_ch02.lonlat   | LL84                   | EPSG:4326          |
| ?                              |                      | D                  | previous_day             | msg.SISDIR-No-Horizon.D_ch02.lonlat   | LL84                   | EPSG:4326          |
| ?                              |                      | M                  | previous_month           | msg.SISDIR-No-Horizon.M_ch02.lonlat   | LL84                   | EPSG:4326          |
| ?                              |                      | Y                  | previous_year            | msg.SISDIR-No-Horizon.Y_ch02.lonlat   | LL84                   | EPSG:4326          |
| ?                              |                      | H                  | previous_day             | msg.SISDNI-No-Horizon.H_ch02.lonlat   | LL84                   | EPSG:4326          |
| ?                              |                      | H                  | previous_day             | msg.SIS-No-Horizon.H_ch02.lonlat      | LL84                   | EPSG:4326          |
| ?                              |                      | D                  | previous_day             | msg.SIS-No-Horizon.D_ch02.lonlat      | LL84                   | EPSG:4326          |
| ?                              |                      | M                  | previous_month           | msg.SIS-No-Horizon.M_ch02.lonlat      | LL84                   | EPSG:4326          |
| ?                              |                      | Y                  | previous_year            | msg.SIS-No-Horizon.Y_ch02.lonlat      | LL84                   | EPSG:4326          |

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

| Parameter                      | Subparameter         | Data granularities | PERIOD_TX = Update cycle | FILENAME                    | BOUND_BOX_COORD_SYS_TX | OUTPUT_COORDSYS_TX |
| ------------------------------ | -------------------- | --- | -------------- | ------------------------------------- | ---- | --------- |
| ? | ? | M | previous_month | hailsizeM_ch01r.swiss.lv95_20020601000000_20020630000000.nc           | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | hailsizeanomM_ch01r.swiss.lv95_20020601000000_20020630000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | hailsizeY_ch01r.swiss.lv95_20020401000000_20020930000000.nc           | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | hailsizeanomY_ch01r.swiss.lv95_20020401000000_20020930000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildaysM_ch01r.swiss.lv95_20020601000000_20020630000000.nc           | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildaysanomM_ch01r.swiss.lv95_20020601000000_20020630000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildaysY_ch01r.swiss.lv95_20020401000000_20020930000000.nc           | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildaysanomY_ch01r.swiss.lv95_20020401000000_20020930000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildaysclimM_ch01r.swiss.lv95_20020401000000_20200430000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildaysclimstdM_ch01r.swiss.lv95_20020401000000_20200430000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildaysclimY_ch01r.swiss.lv95_20020401000000_20200930000000.nc       | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildaysclimstdY_ch01r.swiss.lv95_20020401000000_20200930000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays2cmM_ch01r.swiss.lv95_20020601000000_20020630000000.nc        | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays2cmanomM_ch01r.swiss.lv95_20020601000000_20020630000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays2cmY_ch01r.swiss.lv95_20020401000000_20020930000000.nc        | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays2cmanomY_ch01r.swiss.lv95_20020401000000_20020930000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays2cmclimM_ch01r.swiss.lv95_20020401000000_20200430000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays2cmclimstdM_ch01r.swiss.lv95_20020401000000_20200430000000.nc | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays2cmclimY_ch01r.swiss.lv95_20020301000000_20200930000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays2cmclimstdY_ch01r.swiss.lv95_20020401000000_20200930000000.nc | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays4cmM_ch01r.swiss.lv95_20020601000000_20020630000000.nc        | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays4cmanomM_ch01r.swiss.lv95_20020601000000_20020630000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays4cmY_ch01r.swiss.lv95_20020401000000_20020930000000.nc        | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays4cmanomY_ch01r.swiss.lv95_20020401000000_20020930000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays4cmclimM_ch01r.swiss.lv95_20020401000000_20200430000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | M | previous_month | haildays4cmclimstdM_ch01r.swiss.lv95_20020401000000_20200430000000.nc | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays4cmclimY_ch01r.swiss.lv95_20020301000000_20200930000000.nc    | CH1995 | EPSG:2056 |
| ? | ? | Y | previous_year  | haildays4cmclimstdY_ch01r.swiss.lv95_20020401000000_20200930000000.nc | CH1995 | EPSG:2056 |

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
