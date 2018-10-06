---
layout: aoi
title: AOI 6 Atlanta
sidebar: aoi
---
<video width="320" height="200" controls preload> 
    <source src="/assets/video/2018-08-24-12_41_41_gif.mp4" type="video/mp4"></source> 
    <source src="/assets/video/2018-08-24-12_42_33.webm"></source> 
</video>


## SpaceNet AOI 6 - Atlanta

Catalog ID: 1030010003D22F00 and others

Image Time: 2009-12-22

<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/SpaceNetChallenge.github.io/master/assets/geojson/Atlanta_Data_summary.geojson"></script>


## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 5)
```
AOI_6_Atlanta

├── srcData/rasterData/AOI_6_Atlanta_nadir{Off-Nadir-Angle}_{CatID}/
│   ├── MUL            # Raw souce geotiffs of 8-Band Multi-Spectral raster data from WorldView-2
│   ├── PAN            # Raw souce geotiffs of Panchromatic raster data from Worldview-2
│   └── Pan-Sharpen # Raw souce geotiffs of RGB+NIR raster data from Worldview-3 pansharpened to 0.3m
│      

```
## Download instructions

### AOI 6 - Khartoum
To view the contents of the dataset
```commandline
aws s3 ls spacenet-dataset/AOI_6_Atlanta/ 
```

