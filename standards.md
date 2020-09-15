---
layout: page
title: Standards
subtitle: MarineGEO Data Standards and Guidelines
editbutton: true
---
Suggestions and guidelines for standardizing data in preparation for submission to MarineGEO. 

Because of the wide variety of data types collected by MarineGEO partners, these guidelines might not necessarily fit all specific use cases. Please use these guidelines when possible to contribute to achieving standardization across the network.

**Questions? please contact the MarineGEO Data Manager at <marinegeo@si.edu>**

## Data Structure

Please maintain the file structure in the MarineGEO spreadsheet templates. Each spreadsheet file will include protocol metadata and sample metadata pages, a sheet for each type of sample data, and a glossary. Each observation should be an independent row.

## Format

Files should be saved as an Microsoft Excel Open XML spreadsheet file (.xlsx).

## File names

Files should have a common naming convention. Please avoid using spaces, special characters, or symbols in the file name. A good name should be descriptive and should include relevant information about the contents of the file.

A good file name should include the date `YYYY-MM-DD`, [location abbreviation](#site-abbreviations), protocol name, and version.

`{YYYY-MM-DD}_{location_code}_{protocol-name}_{version}.{ext}`

Example : `2018-01-22_CB_seagrass-density_v1.2.csv`

Photos and videos that are part of a sequence (ie photos taken along a transect) should be named sequentially.

## Field names

Field names should not be altered from the template spreadsheet file. Field names are designed to be short and descriptive and use <a href="https://en.wikipedia.org/wiki/Snake_case">snake case</a> (example_field_name). You can click the field name to view a more detailed description. 

## Consistent fields

Each column or field of the dataset should only contain a single data type. Common data types include numbers, text and dates. Depending on what numeric value is being recorded fields might need to be restricted to whole numbers (ie there should never be a fish abundance of 2.7 fish).

Units should never be stored with the data. Instead, units are stored in the field name or are described in the metadata glossary. Units should not change in a single column. Be consistent. In the MarineGEO template spreadsheets, the unit abbreviation is used in the field name (m instead of meters), and you can check the full unit name in the glossary. 

| ~~BadUnits~~ | better_units_m |
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
| protocol_name      | Name of the protocol used |
| abstract     | The short abstract should cover what, why, when, where, and how for your dataset       |
| contact_person | Name of the person to be contacted     |
| contact_email_address | Email address for the contact person   |
| data_entry_person | Name(s) of data entry person(s) |
| data_entry_date | Date of final data entry |
| other_people | Names of everyone participating in fieldwork |
| protocol_version | Version of the MarineGEO protocol referenced to collect these data |


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
| tabular | .xlsx | Microsoft excel spreadsheet file |
| text | .txt | plain text format-free file |
| text | .md | Markdown used for read me and instructions |


## Site Abbreviations

MarineGEO uses a short unique code for each site. This code is assigned by MarineGEO in consultation with the lead of the partner site. The naming pattern is the 3 letter country code (ISO 3166-1 alpha-3) followed by three letters describing the site's geographic region. For sites within the United States, it is recommended to use the state's two letter abbreviation in the code part describing the geographic region.

**If you need help obtaining a site code, contact MarineGEO at <marinegeo@si.edu>**

| Site | Code |
| ---- | ---- |
| Carrie Bow Cay, Belize | BLZ-CBC |
| Calvert Island, British Columbia, Canada  | CAN-BCC |
| Chesapeake Bay, Edgewater, Maryland, USA | USA-MDA |
| Indian River Lagoon, Fort Pierce, Florida, USA | USA-IRL |
| Kane'ohe Bay, Hawai'i, USA  | USA-HIK |
| Hong Kong| HKG-HKG |
| Madeira Island, Portugal | POR-MAD |
| Bocas del Toro, Panama | PAN-BDT |
| San Francisco Bay, California, USA | USA-SFB |
| Tasmania, Australia | AUS-TAS |
| Gulf Coast, Texas, USA | USA-TXS |
| Salish Sea, Washington, USA | USA-WAS |
| Cambridge Bay, Canada | CAN-NCB |
| Central Coast, Peru   | PER-CCP |
