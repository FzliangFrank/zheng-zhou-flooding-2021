Precipitation in Zhengzhou
================

<!-- badges: start -->

[![analysis:
exploratory](https://img.shields.io/badge/analysis-exploratory-blue.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

# Data Exploratory Analysis on Zhengzhou Climate Data

A time series analysis on Zhengzhou Precipitation, temperature, and
global warming.

## Data

NOAA data. Details:

> [The Global Historical Climatology Network
> (GHCN)](https://www.ncdc.noaa.gov/data-access/land-based-station-data/land-based-datasets/global-historical-climatology-network-ghcn)
> is an integrated database of climate summaries from land surface
> stations across the globe that have been subjected to a common suite
> of quality assurance reviews. The data are obtained from more than 20
> sources. Some data are more than 175 years old while others are less
> than an hour old. GHCN is the official archived dataset, and it serves
> as a replacement product for older NCEI-maintained datasets that are
> designated for daily temporal resolution (i.e., DSI 3200, DSI 3201,
> DSI 3202, DSI 3205, DSI 3206, DSI 3208, DSI 3210, etc.).

Alternatively some life-saver has wrote an whole package to make API
call easier. See `rnoaa`

Precipitation is measured by tenth of mm (1/100 of cm). Full
abbreviation can be found here:
<https://www1.ncdc.noaa.gov/pub/data/ghcn/daily/readme.txt>

## Methodlogy

### Measuring Rainfall normality

**Parametrizing** distribution density curve of rainfall in an
observation periord. Assumes distribution of rainfall within a time
interval to be exponential distribution. The density curve can be
expressed via a density function.

1.  extract density data point
2.  draw a line
3.  parametrize by drawing a line

Parameter will tell us how left skewed is the rainfall curves. The more
left skewed means more extreme weather forecasting events.

## The Story Goes..

I used to live in Zhengzhou city. The year is 2016, My uni is in far
western end Zhengzhou Two hours ride on subways (or UK they call it
“tube”) from “ErQi Square” which is the vibrant town center of Zhengzhou
City.

I used to ride the tube every now and then. Because the underground rail
way system was new development, comfortable. It is one of few subways
system in China that actually have AC and 4G signals. Zhengzhou is
considering one of four “hottest cities” in mainland China. During hot
boiling summer, the subway is extra-ordinarily chill. For us students
who don’t have AC at dorm, we just wish we could sleep on the railway.

I left the city for UK in 2018. Three years after I left, the city was
flooded. The very tube line I used to ride is compromised. Underground
tubes turns into underground river. People who ride tube on the day and
couldn’t get out in time drowned or suffocated. These are people who
ride the tube every day.

While Zhengzhou is the hottest city, it is also the most populated,
capital of Henan, the province with largest proportion of poverty.
Having the underground tube built was one of the proudest things of
Zhengzhou people. It turns out the tube system did not proofed against
extreme precipitation.

This analysis reveals some obvious participation pattern in Zhengzhou in
the past.
