# FME-PhotoAnnotation

## Overview of the tool
This FME tool will annotate photo with information of the survey information such as feature class and GPS location.And put in the metadata into the photo file as well.

## Problem
We encounter issue at work where GIS users try to find photo that go along with survey data. There's no good way to know where the location of the photo took place. If we got lucky the photo meta data has geotag location, majority of the time it was not there. Sometimes the crew using third party photo up and embedded location into the picture, but you will still need to type in this location into the map for each photo which can take time to go through all the photo in each dataset.

## Solution
We update the survey codelist to include photo fields. Instead of the crew using the third party app. They can collect each data point like normal, and if they feel like this feature needing a picture, they just take the picture going along with that point. Use FME to read the data point like normal but now it will manipulate the picture and put in information that we need and rename the source file and meta to however we want it.

## Tools Dependencies
1) FME
2) add photo field to the FXL (Survey Codelist)
3) Survey file collected using the above FXL.

## Example Product
Below is picture of what the workspace looks like in FME.
![FME workspace](https://github.com/pandaacoding/FME-PhotoAnnotation/assets/80724379/8b6842e7-6bfd-4f84-b9d1-00221a314279)

This is the picture of the product.
