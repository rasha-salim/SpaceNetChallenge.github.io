---
layout: datasets
title: "SpaceNet Buildings Dataset Labeling Guide"
sidebar: schema
---
# The SpaceNet Buildings Data set labeling guidelines:

1.  Buildings will primarily be within urban/suburban areas.
2.  Rooflines will first be extracted to best represent the shape of the footprint and for any buildings where the base of the building is partially visible due to off-nadir angle the polygon will be shifted to best fit the base corners.
3.  Buildings will have squared corners (assuming they are true to the shape of the building).
4.  Extraction of building corners will be within 5 pixels of the location on the imagery.
5.  Building footprints will be closed polygons and will not overlap.
6.  No attributes will be populated.
7.  Adjoining buildings with different heights shall be captured at one visible roof for the whole block and shifted to that visible roofs baseline.


## GeoJSON Schema
#### Attributes:
1)	“geometry”: Polygon

