[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > C. Climate Data

# C. Climate Data
Climate Data consists of homogenous time series data (1, 2), spatial climate data (3-5), climate normals (6, 7) and scenarios (8):

1. [Climate stations](#1-climate-stations)
2. [Climate precipitation stations](#2-climate-precipitation-stations)
3. [Ground-based spatial climate data](#3-ground-based-spatial-climate-data)
4. [Satellite-based spatial climate data](#4-satellite-based-spatial-climate-data)
5. [Radar-based spatial climate data](#5-radar-based-spatial-climate-data)
6. [Climate normals](#6-climate-normals)
7. [Spatial climate normals](#7-spatial-climate-normals)
8. [Climate scenarios](#8-climate-scenarios)

### General information
All MeteoSwiss surface stations have a name and an identfier consisting of three letters (e.g. `BER` for [Bern / Zollikofen](https://www.meteoswiss.admin.ch/services-and-publications/applications/measurement-values-and-measuring-networks.html#param=messnetz-klima&lang=en&station=BER&chart=hour&table=false) or `LUG` for [Lugano](https://www.meteoswiss.admin.ch/services-and-publications/applications/measurement-values-and-measuring-networks.html#param=messnetz-klima&lang=en&station=LUG&chart=hour&table=false)). Data files use this station identifier in the file name throughout all directories. A list of all station identfiers with station names, coordinates, height etc. can be found in the according 'station metadata' sections below.

---

## 1. Climate stations
The [Swiss National Basic Climatological Network "Swiss NBCN"](https://www.meteoswiss.admin.ch/weather/measurement-systems/land-based-stations/swiss-national-basic-climatological-network.html) connects the major ground-based stations within the MeteoSwiss monitoring network. It consists of around 30 climate monitoring stations. 

The [homogenous time series data](https://www.meteoswiss.admin.ch/climate/climate-change/changes-in-temperature-precipitation-and-sunshine/homogeneous-data-series-since-1864.html) for temperature, precipitation and hours of sunshine date back, in some cases, to the mid-nineteenth century.

### 1.1. Data granularity, update frequency, format and volume
If you require daily, monthly or annual values, we strongly recommend that you download the corresponding aggregated [data granularity](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#data-granularity) `D`, `M`, `Y` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) daily (`recent`) or yearly (`historical`) for each station.

Data format of all files is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ≤0.9 MB per file.

See (example!) data files for station `BAS` for all granularities and update frequencies mentioned: [`ogd-nbcn_BAS_(data granularity)_(update frequency)`](https://github.com/MeteoSwiss/publication-opendata/tree/main/data-surface/climate-stations-swiss-nbcn-climate).

### 1.2. Parameter metadata
See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### 1.3. Station metadata
See (example!) [station metadata file](...).

### 1.4. Data visualisation
See e.g. MeteoSwiss' [...](...).

<br>

## 2. Climate precipitation stations
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See (example!) [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 3. Ground-based spatial climate data
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
*See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See (example!) [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 4. Satellite-based spatial climate data
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
*See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See (example!) [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 5. Radar-based spatial climate data
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
*See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See (example!) [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 6. Climate normals
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See (example!) [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 7. Spatial climate normals
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` *and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.*

Data format is [`...`](...) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
*See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).*

<!-- ### Codes -->
<!-- ... -->

### Station metadata
*See (example!) [station metadata file](...).*

### Data visualisation
See e.g. MeteoSwiss' [...](...).

## 8. Climate scenarios
... 

...

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...`, `...`, `...`, `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) hourly (`now`), daily (`recent`) or yearly (`historical`) for each station.

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of ... MB per file.

See (example!) data files: [`...`](...).

### Parameter metadata
See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See (example!) [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).
