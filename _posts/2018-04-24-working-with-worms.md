---
layout: post
title: WoRMS
subtitle: Verify scientific names with WoRMS
tags: [code, help, snippet, taxonomic]
---

Need to make sure that all the scientific names are up to date and valid? Try using the World Register of Marine Species (WoRMS) to validate the species names in your dataset.

In this example, we will use the [`worrms` R package](https://github.com/ropensci/worrms) to verify some scientific names from a diver fish survey.

First, install the required packages

```r
install.packages("worrms")
install.packages("tidyverse")

library(tidyverse)
library(worrms)

```

Next, extract a list of unique species names to test. The list of names should not include any duplicates since there is no need to hit the API multiple times for the same name.

```r
# creates a list of all unique species in the scientificname column
species_list <- df %>% dplyr::select(scientificname) %>%
    dplyr::distinct() %>% dplyr::pull(scientificname)
```

The WoRMS package returns accepted and unaccepted results. To start with, let's send our unique list of species names and return a query filtered by accepted names.

```r
# sends species list to worrms API
worms_rec <-worrms::wm_records_names(name =species_list) # returns list of data frames

# bind dataframes into a single dataframe and filter out unaccepted names
worms_rec_df <- worms_rec %>% dplyr::bind_rows() %>%
  dplyr::filter(status=="accepted")
```
