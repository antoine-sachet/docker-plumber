FROM asachet/plumber-base:R3.6.1

# MySQL client lib
RUN apt update -qq \
&& apt install -y \
libmariadb-dev \
libmariadbclient-dev
 
# https://github.com/r-dbi/RMariaDB
RUN install2.r -s --error \
DBI \
RMariaDB \
dbplyr \
&& rm -rf /tmp/downloaded_packages/
