FROM rocker/tidyverse:4.1.0

# Install packages and dependencies for pavo
RUN apt-get update && apt-get install -y \
    libxml2-dev \
    libcurl4-openssl-dev \
    libssl-dev \
    imagemagick \
    libmagick++-dev \
    tcl8.6-dev \
    tk8.6-dev \
      # Install R packages directly from rstudio repo
  && install2.r --error \
    -r "https://packagemanager.rstudio.com/all/__linux__/focal/latest" \
    pavo \
  && apt-get autoclean \
  && apt-get clean \
  && apt-get autoremove