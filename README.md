#  Dockerfiles for R plumber APIs

These images are a stable and convenient base for R APIs.

## plumber-base

[![](https://images.microbadger.com/badges/version/asachet/plumber-base.svg)](https://microbadger.com/images/asachet/plumber-base "Get your own version badge on microbadger.com")  [![](https://images.microbadger.com/badges/image/asachet/plumber-base.svg)](https://microbadger.com/images/asachet/plumber-base "Get your own image badge on microbadger.com")

* Built on the most stable R image, `rocker/r-ver`
* Contains `plumber` and a minimal `tidyverse`
* Contains convenience (and IMO best practice) tools like `logging` and `config`

## plumber-mysql

[![](https://images.microbadger.com/badges/version/asachet/plumber-mysql.svg)](https://microbadger.com/images/asachet/plumber-mysql "Get your own version badge on microbadger.com")  [![](https://images.microbadger.com/badges/image/asachet/plumber-mysql.svg)](https://microbadger.com/images/asachet/plumber-mysql "Get your own image badge on microbadger.com")

* Built on `plumber-base` for robustness
* Adds system libraries and R packages necessary to connect to `MySQL` databases
* NOTE: relies on `RMariaDB` instead of the _legacy_ `RMySQL` package!


