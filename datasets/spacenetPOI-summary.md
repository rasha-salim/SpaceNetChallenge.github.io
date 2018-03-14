---
layout: datasets
title: "SpaceNet POI Dataset"
sidebar: datasets
---

## The Rio De Janeiro Points of Interest Dataset


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. CosmiQ Works, Radiant Solutions and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists to work with this data.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.

This POI dataset provides an example of a city wide dataset used for GIS applications.

## The Data - Over 120,155 individual points representing 460 features in Rio De Janeiro.

The POI geodatabase contains 12 datasets with 35 unique layers. The total release contains 120,155 individual points representing 460 features. There is a subset of 11,114 points across 139 features that have been confirmed with the provided satellite imagery. 


<style> table{
    border-collapse: collapse;
    border-spacing: 0;
    border:2px solid #000000;
}

th{
    border:2px solid #000000;
}

td{
    border:1px solid #000000;
}
</style>



|  AOI            | Area of Raster (Sq. Km) | Building Labels (Polygons) | 
|----------------|-------------------------|----------------------------|
| [AOI_1_Rio](/AOI_Lists/AOI_1_Rio.html)      | 2,544                   | 382,534                  | 


## Description of Data
<iframe class="airtable-embed" src="https://airtable.com/embed/shrYahk3BpXA6BDyD?backgroundColor=cyan" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>




## Catalog
The data is hosted on AWS and is a public dataset.

```commandline
aws s3 ls s3://spacenet-dataset/AOI_1_Rio/srcData/vectorData/ 
```



## Vector Data
### Point of Interest ESRI GeoDatabase   
To download the ESRI GeoDatabase  (31.2 GiB) with all associated data 
```
aws s3 cp s3://spacenet-dataset/AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro.gdb.tar.gz .
```

### Point of Interest GeoJSONs and associated meta data   
To download the GeoJSONs and assocaited meta data (28.8 GiB) with all associated data 
```
aws s3 cp s3://spacenet-dataset/AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro_extract.tar .
```

For additional information please see [The DownlinQ Blog Post](https://medium.com/the-downlinq/spacenet-update-announcing-rio-de-janeiro-point-of-interest-poi-dataset-release-d8abac6896e1)

See the [NGA Press Release](https://www.nga.mil/MediaRoom/PressReleases/Pages/NGA-capitalizes-on-SpaceNet%E2%80%99s-efforts.aspx)



## Source:
We would like to acknowledge the participation of the National Geospatial-Intelligence Agency (NGA) with the preparation of this research data licensed from Digital Globe to SpaceNet. The SpaceNet POI dataset is released under the Creative Commons license (i.e. CC BY-NC-SA 4.0).

## License
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">SpaceNet Point of Interest Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Point of Interest Dataset</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://spacenetchallenge.github.io/datasets/spacenetPOI-summary.html" rel="dct:source">https://spacenetchallenge.github.io/datasets/spacenetPOI-summary.html</a>