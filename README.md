# Overview
Dockerfiles to generate Rstudio containers for various analyses. Tags indicate the version of *R* used in the image build. For various configurations to get up and running with an Rstudio container in your browser, see instructions provided by the [Rocker Project](https://github.com/rocker-org/rocker/wiki/Using-the-RStudio-image).

# [Docker](https://docs.docker.com/get-docker/) images
- [rstudio-bayes](https://hub.docker.com/r/aluro2/rstudio-bayes) ~ rstudio-server with select STAN-based Bayesian statistical modeling R packages
  + ``` docker pull aluro2/rstudio-bayes:4.0.3```
  
- [rstudio-visual-modeling](https://hub.docker.com/r/aluro2/rstudio-visual-modeling) ~ rstudio-server with the visual modeling R package [*pavo*](pavo.colrverse.com/)
  + ``` docker pull aluro2/rstudio-visual-modeling:4.0.3```

