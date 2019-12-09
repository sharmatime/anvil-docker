| RStudio Version | Date Updated | Questions or Feedback |
| --- | --- | --- |
| 0.0.1 | 10/06/2019 | Adrian Sharma: adrian@broadinstitute.org |

# AnVIL RStudio Docker Image

[Rstudio](https://rstudio.com/products/rstudio/) is an integrated development environment to support the R statistical programming language. The AnVIL RStudio Docker is a version-tagged image of RStudio, providing consistent RStudio software, packages, and dependencies with every use. This document describes the [RStudio](https://rstudio.com/products/rstudio/) Docker Image and how to use it in the cloud-based platform [Terra](app.terra.bio). Unlike the currently existing [Terra base images](https://github.com/DataBiosphere/terra-docker#terra-base-images), RStudio is not hosted in a Jupyter Notebook; any work performed in Terra RStudio will not be saved. At the end of this document, you will find Instructions and suggestions for saving RStudio data and code. 

## Table of Contents

## RStudio Docker Contents

### Accessing the AnVIL RStudio Image

The AnVIL Rstudio Image can be accessed using the following URL: us.gcr.io/anvil-gcr-public/anvil-rstudio-base:0.0.1. 

### Base Image

The base image for the AnVIL RSutio Docker is the [rocker/tidyverse](https://hub.docker.com/r/rocker/tidyverse/) image provided by the [Rocker Project](https://www.rocker-project.org/). This image contains tidyverse and devtools.


### Applications

The AnVIL R Docker contains the [RStudio Server](https://www.rstudio.com/products/rstudio-server/) application which supports a web browser version of RStudio. 

### Libraries

The following packages are pre-loaded in the AnVIL RStudio image:

* [tidyverse](https://www.tidyverse.org/packages/): a suite of packages desigend for data sciences 
* [google-cloud-sdk](https://cloud.google.com/sdk/): tools for the google cloud platform
* [googleCloudStorageR](http://code.markedmondson.me/googleCloudStorageR/): an R library for interacting with google cloud storage
* [bigrquery](https://github.com/r-dbi/bigrquery): a package to allow interaction with Google's BigQuery
* DataBiosphere/Ronaldo: a package of functions commonly used for R Notebooks created from Leonardo

### Customizations

The AnVIL RStudio image is customized to disable the RStudio login screen. Future customizations will include:

* RStudio hooks to refresh credentials 
* An RStudio pause after inactivity

## Using R Studio in Terra

## Saving RStudio Data

Code and data generated in Terra RStudio will not be saved. Below are three suggestions for saving your work.

### Copying RStudio work to a workspace google bucket



### Downloading RStudio files to local computer
### Checking code into GitHub

## Versioning

All updates and changes to the current docker image are listed in the Rstudio image [CHANGELOG.md file](CHANGELOG.md). 
