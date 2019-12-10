FROM rocker/r-rev:3.6.1
LABEL maintainer="Antoine Sachet <antoine.sac@gmail.com>" \
org.label-schema.vcs-url="https://github.com/antoine-sachet/docker-plumber"

# Required libs + curl
RUN apt-get update -qq && apt-get install -y \
libssl-dev \
libcurl4-openssl-dev \
libsodium-dev \
curl

# Some standard packages to speed up the next layers
RUN install2.r -s --error \
config \
dplyr \
forcats \
future \
glue \
jsonlite \
logging \
promises \
purrr \
readr \
remotes \
rlang \
stringi \
tidyr \
&& rm -rf /tmp/downloaded_packages/

# Installing latest version of plumber + 
# my version of remotes fixing issues with bitbucket (pending PR approval)
RUN install2.r -s --error remotes \
&& installGithub.r trestletech/plumber antoine-sachet/remotes \
&& rm -rf /tmp/downloaded_packages/

