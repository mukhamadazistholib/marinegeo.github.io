---
layout: project
title: Benthic Photos
thumbnail: /img/underwater-camera.png
editbutton: true
---

## Purpose

Benthic photograph quadrants are underwater photos typically taken along a transect at a regular interval.  Photos are taken a few meters above the sea floor and capture the benthic habitat at the site. Divers lay out a transect, and record 20 digital photoquadrats. In each photo a scale should be included, placed flush with the substrate, either in the form of the transect tape itself, or other portable scale (marked PVC, etc.). Photoquadrats are analyzed and scored for benthic community composition, coral disease, rugosity, etc.




## Measured parameters

## Methods

## Data curation     

Photos should be saved in the native format that are exported from the camera. Please do not submit images in a raw image format.

### Data Organization

The original photos and any derived data products should be included in the same project folder. Every transect must be saved as a unique subfolder under the photos directory. Analysis and any derived products should be saved in separate folder called analysis.

The photo subfolder names should contain the date of transect and the location code or name. Please record the date using the YYYYMMDD format (ISO 8601 standard - four-digit year, zero padded month, zero padded day). Use an underscore _ to separate the date and location name. Avoid having any spaces in the folder name, if needed use a dash – to indicate a space in the location name.

All analysis and summary files should be saved under the analysis directory folder. The preferred file format for all files is a flattened csv with an additional metadata file.

<img src="/assets/modules/benthicphotos/Screen Shot 2018-05-31 at 9.51.32 AM.png" alt="Benthic photo file structure" style="width:50%; display: block; margin-left: auto; margin-right: auto"/>

### Photo Names

Each transect folder should contain the original photos and any photos cropped or modified for analysis. The original photos should be named using this pattern: date, MarineGEO site abbreviation, location name/code, “PQ” for photo quadrant, the photo number of in the transect. The photos should be numbered sequentially starting at 1 for the beginning of the transect. If multiple photos are taken at a single transect stop, select the best photo and append “alt” the other photo names to delineate the photos as alternates. If photos need to be modified for analysis, retain the original photo and save a copy in a modified subfolder and note what was changed.

<img src="/assets/modules/benthicphotos/Screen Shot 2018-10-10 at 3.50.12 PM.png" alt="Benthic photos file names" style="width:50%; display: block; margin-left: auto; margin-right: auto"/>


### Photo Metadata

The photos folder should include a metadata file that includes the following information about each of the transect. Since the photos taken along the transect are part of an image sequence, the metadata will be attached to the group of photos.

| Field name         | Description                                                          |
|--------------------|----------------------------------------------------------------------|
| site               | MarineGEO site abbreviation, two letter code                         |
| location           | name of the transect sample spot, alpha numeric identifier preferred |
| locality           | Local or common name of the sampling location                        |
| decimalLatitude    | latitude in decimal degrees (WGS 1984)                               |
| decimalLongitude   | longitude in decimal degrees (WGS 1984)                              |
| habitat            | CMECS habitat classification - https://www.cmecscatalog.org/cmecs/   |
| date               | the date of the transect (use YYYY-MM-DD if possible)                |
| depth_m            | the depth below surface (diver depth) in meters                      |
| notes              | any notes about the location, dive conditions, photos                |
| numberPhotos       | the number of photos in the sequence (don’t count duplicates)        |
| transectDistance_m | the traveled distance for the photo sequence in meters               |
| photographer       | full name of the person taking the photos                            |


## Selected literature
