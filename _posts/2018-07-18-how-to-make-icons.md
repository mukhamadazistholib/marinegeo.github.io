---
layout: post
title: How To Make Icons
subtitle: Tips for making icons to use as shortcuts
tags: [help, website]
---

# GIMP

This tutorial uses [GIMP - GNU Image Manipulation Program](https://www.gimp.org/). It is a free and open-source graphics editor.

# Steps

## 1. Find an image to use as the template for the silhouette and open in GIMP

  ![MarineGEO Diver, Bocas del Toro, Panama]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 3.17.49 PM.png" | absolute_url }})

## 2. Crop image to area of interest

  ![Cropped image]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 3.19.14 PM.png" | absolute_url }})

## 3. Convert image to a reduced color palette  

Select Image -> Mode -> Indexed...

The indexed image mode will limit the color palette to a limited number of colors.
Select the maximum number of colors to use for the color map. The lower the number the better, but make sure that there is not too much detail lost.

![Indexed Color Conversion]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 3.23.34 PM.png" | absolute_url }})

Note: you may need to convert the image back to RBG mode in order to complete the next few steps.

## 4. Select the background using the Fuzzy Select Tool

  ![Fuzzy color select tool]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 4.04.18 PM.png" | absolute_url }})

## 5. Delete the selection

Select Edit -> Clear

Then, use the Eraser tool to clean up any remaining background areas

![Delete selection menu]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 3.31.59 PM.png" | absolute_url }})

## 6. Covert image to reduced color palette with fewer colors

Indexed image with few colors (max 2 or 3) and fill selections (Select by Color Tool) to match color schema

![Second Indexed Color Conversion]({{ "img/2018-07-18-how-to-make-icons/Screen Shot 2018-07-20 at 3.37.24 PM.png" | absolute_url }})

## 7. Scale and center image

## 8. Add circle for Background

 - Create new layer
 - Use Ellipse Select Tool (Hold shift to create circle)
 - Fill Selection Outline (Edit menu -> Fill selection outline ... )
 - Fill circle with the desired background color
 - Fit canvas to Selection (Image menu -> Fit Canvas to Selection )

## 9. Export image as a .png

 ![Final Icon of a diver]({{ "img/scuba_diver.png" | absolute_url }})
