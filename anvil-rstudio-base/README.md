| RStudio Version | Date Updated | Questions or Feedback |
| --- | --- | --- |
| 0.0.1 | 10/06/2019 | Adrian Sharma: adrian@broadinstitute.org |

# AnVIL RStudio Image in Terra

This document provides background on the RStudio Docker and using the image in Terra. Unlike the currently existing Terra base images (link), RStudio is not hosted in a Jupyter Notebook; any work performed in Terra RStudio will not be saved. Instructions and suggestions are provided at the end of this document for saving RStudio code. 

## Table of Contents

## RStudio Docker Contents

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

### Copying RStudio work to a workspace google bucket
### Downloading RStudio files to local computer
### Checking code into GitHub

## Versioning
