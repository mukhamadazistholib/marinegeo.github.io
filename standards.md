---
layout: page
title: Standards
subtitle: MarineGEO Data Standards and Guidelines
---

Suggestions and guidelines for standardizing MarineGEO data into tidy datasets. These guidelines serve as a reference for best practices across the MarineGEO program.

Because of the wide variety of data types collected by MarineGEO partners, these guidelines might not necessarily fit all specific use cases. Please use these guidelines when possible to contribute to achieving standardization across the network.

**Questions? please contact the MarineGEO Data Manager at <marinegeo-data@si.edu>**

## Data Structure

Flat long files are ideal. Each observation should be an independent row.

## Format

Files should be saved as simple flat files such as comma separated values (.csv) or tab separated values (.tsv).

## Files names

Files should have a common naming convention. Please avoid using spaces, special characters, or symbols in the file name. A good name should be descriptive and should include relevant information about the contents of the file.

A good file name should include the date `YYYY-MM-DD`, [location abbreviation](#site-abbreviations), project type, and version.

`{YYYY-MM-DD}_{LocationCode}_{ProjectType}_{version}.{ext}`

Example : `2018-01-22_CB_SquidPops_v1.2.csv`

Photos and videos that are part of a sequence (ie photos taken along a transect) should be named sequentially.

## Field names

Field names should be simple short and descriptive. Avoid spaces, special characters, or symbols in the field name. Use under_scores or CamelCase instead of having spaces in the field name.


Good:
 - temp_f
 - depthMeters
 - FishLength
 - decimalDegrees

Bad:
 - ~~depth meters below surface~~
 - ~~area_m^2~~
 - ~~DO (mg/L)~~


## Consistent fields

Each column or field of the dataset should only contain a single data type. Common data types include numbers, text and dates. Depending on what numeric value is being recorded fields might need to be restricted to whole numbers (ie there should never be a fish abundance of 2.7 fish).

Units should never be stored with the data. Instead, include the unit in the field name or describe the measurement unit in the metadata. Also, it should go without saying that the units should not change in a single column. Be consistent.

| ~~BadUnits~~ | BetterUnits_meters |
| --- | ------ |
| ~~one meter~~ | 1 |
| ~~2.5 m~~  | 2.5 |
| ~~4 ft~~ | 1.2 |

## Units

Please use SI units. 

## Metadata

 Each dataset should be submitted with the minimum following metadata fields.

| Field         | Description           |
| ------------- | ------------- |
| Title      | Brief unique name to use as a title for the data set. Should include location, data type collected and dates |
| Abstract     | The short abstract should cover what, why, when, where, and how for your dataset       |
| Creator | Full name of dataset creator     |
| CreatorContact | Email address for dataset creator   |
| AdditionalPeople | Names of everyone participating in fieldwork |


## Dates

Dates and timestamps should be stored in a standardized format. The preferred format to store dates is `YYYY-MM-DD HH:MM`. For example, an observation on January 28th, 2017 at 2:15 pm would be stored in the spreadsheet as `2017-01-28 14:00`. Alternative methods for storing dates and times is permissible. A common approach to storing dates is to separate each part of the date as separate columns for year, month, day. If using this approach, make sure to define the metadata for each of the columns.


## Geographic data

There are many ways and formats to store geographic data. Geospatial vector datasets should be stored in shapefiles or geojson files. The ideal format for raster dataset is geotiffs.

For geographic data that is stored in tabular files, latitude and longitude values should be stored in decimal degrees in WGS 1984 projection.


## Controlled Vocabulary

Fields that have a controlled vocabulary should have an additional table with definitions. These definitions should be included in the metadata.


## Suggested file types

| Type | Format | About |
| ---- | ------ | ----- |
| audio | .wav  | audio files |
| video | .mp4  | video |
| vector | .shp | ESRI shapefiles |
| vector | .geojson | GeoJSON spec |
| raster | .tif | geotiffs |
| tabular | .csv | comma separated values |
| tabular | .tsv | tab separated values |
| text | .txt | plain text format-free file |
| text | .md | Markdown used for read me and instructions |


## Site Abbreviations

| Site | Code |
| ---- | ---- |
| Bocas del Toro | BT |
| Carrie Bow | CB |
| Corpus Christi | CC |
| Edgewater (SERC) | EW |
| Friday Harbor | FH |
| Fort Pierce | FP |
| Hakai | HK |
| Kane'ohe Bay | KB |
| Romberg Tiburon | RT |
