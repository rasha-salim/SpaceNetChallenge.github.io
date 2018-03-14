---
layout: datasets
title: "SpaceNet Imagery"
sidebar: datasets
---


## The SpaceNet Imagery Corpus


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. CosmiQ Works, Radiant Solutions and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists to work with this data.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.




## The Data - Over 5700 sq km of satellite imagery across the Five SpaceNet Areas of Interest.



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



|  AOI            | Area of Raster (Sq. Km) |
|----------------|-------------------------|
| [AOI_1_Rio](/AOI_Lists/AOI_1_Rio.html)      | 2,544                   |  
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     |


## Catalog
The data is hosted on AWS in a requester pays bucket.
```commandline
aws s3 ls s3://spacenet-dataset/AOI_1_Rio/srcData/rasterData/ --request-payer requester
aws s3 ls s3://spacenet-dataset/AOI_2_Vegas/srcData/rasterData/ --request-payer requester
aws s3 ls s3://spacenet-dataset/AOI_3_Paris/srcData/rasterData/ --request-payer requester
aws s3 ls s3://spacenet-dataset/AOI_4_Shanghai/srcData/rasterData/ --request-payer requester
aws s3 ls s3://spacenet-dataset/AOI_5_Khartoum/srcData/rasterData/ --request-payer requester
```
For more information visit the [AOI List]('/AOI_Lists/AOI_HomePage.html')

## AOI 1 - Rio
AOI 1 - Rio is composed of a 3-Band and 8 Band mosaic produced from WV-2 0.5m imagery.
```
-- srcData
        |-- rasterData
        |   |-- 3-Band.tar.gz # 3band (RGB) Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by WorldView-2
        |    -- 8-Band.tar.gz # 8band Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by WorldView-2
```

It covers ~2544 sq km of area

## AOI 2-5
AOI 2 - 5 (Las Vegas, Paris, Shanghai and Khartoum) are WV-3 image strips.

```
The imagery is distributed in 4 versions.
srcData/rasterData
│   ├── MUL            # Raw souce geotiffs of 8-Band Multi-Spectral raster data from WorldView-3
│   ├── MUL-PanSharpen # Raw souce geotiffs of 8-Band Multi-Spectral raster data pan-sharpened to 0.3m
│   ├── PAN            # Raw souce geotiffs of Panchromatic raster data from Worldview-3
│   └── RGB-PanSharpen # Raw souce geotiffs of RGB raster data from Worldview-3 pan-sharpened to 0.3m
```
## License
The imagery described aboce in the SpaceNet Dataset is licensed as an Creative Commons Attribution-ShareAlike 4.0 International License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">The SpaceNet Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io/" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Partners</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
