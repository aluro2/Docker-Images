FROM rocker/tidyverse:4.0.4
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
RUN R -e "install.packages('rstan', clean = T, Ncpus = 6)" 
RUN R -e "install.packages('rstanarm', clean = T, Ncpus = 6)" 
RUN R -e "install.packages('brms', clean = T, Ncpus = 6)"
RUN R -e "install.packages('bayestestR', clean = T, Ncpus = 6)" 
RUN R -e "install.packages('tidybayes', clean = T, Ncpus = 6)" 
