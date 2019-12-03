| RStudio Version | Date Updated | Questions or Feedback |
| --- | --- | --- |
| 0.0.1 | 10/06/2019 | Adrian Sharma: adrian@broadinstitute.org |

# AnVIL RStudio Docker Image

This document provides background on the [RStudio](https://rstudio.com/products/rstudio/) Docker Image and how to use it in the cloud-based platform [Terra](app.terra.bio). Unlike the currently existing [Terra base images](https://github.com/DataBiosphere/terra-docker#terra-base-images), RStudio is not hosted in a Jupyter Notebook; any work performed in Terra RStudio will not be saved. Instructions and suggestions are provided at the end of this document for saving RStudio code. 

## Table of Contents

## RStudio Docker Contents

Teh AnVIL Rstudio Image can be accessed using this URL: us.gcr.io/anvil-gcr-public/anvil-rstudio-base:0.0.1

### Base Image

* [rocker/tidyverse](https://hub.docker.com/r/rocker/tidyverse/)

### Applications

* [RStudio Server](https://www.rstudio.com/products/rstudio-server/)

### Libraries

* tidyverse
* google-cloud-sdk
* googleCloudStorageR
* bigrquery
* DataBiosphere/Ronaldo

### Customizations

* Disabled RStudio login screen
* TODO: RStudio hooks to refresh credentials and pause on inactivity

## Using R Studio in Terra

## Saving RStudio Data

Code and data generated in Terra RStudio will not be saved. Below are three suggestions for saving your work.

### Copying RStudio work to a workspace google bucket



### Downloading RStudio files to local computer
### Checking code into GitHub

## Versioning
