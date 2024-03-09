# FME-PhotoAnnotation

## Overview of the tool
This FME tool will annotate photo with the survey information such as feature class, GPS location, and Coordinate System. The information will be put in the metadata of the photo file as well.

## Problem
We encounter issue at work where GIS users try to find photos that go along with survey data. There's no good way to know where the location of the photo took place. If we got lucky the photo meta data has geotag location, majority of the time it was not there. Sometimes the crew using third party photo up and embedded location into the picture, but you will still need to type in this location into the map for each photo which can take time to go through all the photo in each dataset.

## Solution
We update the survey codelist to include photo fields. Instead of the crew using the third party app. They can collect each data point like normal, and if they feel like this feature needing a picture, they just take the picture going along with that point. Use FME to read the data point like normal but now it will manipulate the picture and put in information that we need and rename the source file and meta to however we want it. GIS user will now be able to search photo by point number associate with the data, or they can just open the photo and knows what kind of features they are looking at and they have point number reference back to the dataset.

## Tools Dependencies
1) FME
2) add photo field to the FXL (Survey Codelist)
3) Survey file collected using the above FXL.

## Example Product
Below is picture of what the workspace looks like in FME.
![FME workspace](https://github.com/pandaacoding/FME-PhotoAnnotation/assets/80724379/8b6842e7-6bfd-4f84-b9d1-00221a314279)

This is the picture of the product.

![PhotoAnnotation](https://github.com/pandaacoding/FME-PhotoAnnotation/assets/80724379/518300cf-3b28-4e97-b1f8-1cd9678a3977)
