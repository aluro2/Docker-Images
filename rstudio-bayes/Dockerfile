FROM rocker/rstudio:latest
LABEL maintainer="alec.b.luro@gmail.com"

# Install packages and dependencies 
RUN apt-get update && apt-get install -y \
    pandoc-citeproc \
    pandoc \
    # Extra dependencies for igraph R package
    libxml2-dev \
    libv8-dev \
    libglpk-dev \
    libgmp3-dev 

# Install R packages
RUN RUN R -e "devtools::install_version('rstan', clean = T, Ncpus = 6, quick = T)" 
RUN RUN R -e "devtools::install_version('rstanarm', clean = T, Ncpus = 6, quick = T)" 
RUN RUN R -e "devtools::install_version('brms', clean = T, Ncpus = 6, quick = T)"
RUN RUN R -e "devtools::install_version('bayestestR', clean = T, Ncpus = 6, quick = T)" 
RUN RUN R -e "devtools::install_version('tidybayes', clean = T, Ncpus = 6, quick = T)" 
