---
layout: datasets
title: Datasets
sidebar: toplevel
---
## Hosting
[SpaceNet](https://aws.amazon.com/public-datasets/spacenet/) is a corpus of commercial satellite imagery and labeled
 training data to use for machine learning research. The dataset is currently hosted as an [Amazon Web Services (AWS) Public Dataset](https://aws.amazon.com/public-datasets/).

## The SpaceNet Src Imagery Catalog
1. [Area of Interest 1 (AOI 1) - Location: Rio de Janeiro.](/AOI_Lists/AOI_1_Rio.html) 50cm imagery collected from DigitalGlobe’s [WorldView-2 satellite](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf). The dataset includes building footprints and 8-band multispectral data.
2. [Area of Interest 2 (AOI 2) - Location: Vegas.](/AOI_Lists/AOI_2_Vegas.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
3. [Area of Interest 3 (AOI 3) - Location: Paris.](/AOI_Lists/AOI_3_Paris.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
4. [Area of Interest 4 (AOI 4) - Location: Shanghai.](/AOI_Lists/AOI_4_Shanghai.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
5. [Area of Interest 5 (AOI 5) - Location: Khartoum.](/AOI_Lists/AOI_5_Khartoum.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.

## The SpaceNet Competition Datasets
1. [SpaceNet Buildings Dataset v1](/datasets/spacenetBuildings-V1summary.html)
2. [SpaceNet Buildings Dataset v2](/datasets/spacenetBuildings-V2summary.html)
3. [SpaceNet Roads Dataset](/datasets/spacenetRoads-summary.html)

## Remote Sensing Competition Datasets
4. [IARPA Multi-View Stereo 3D Mapping Challenge](/datasets/mvs_summary.html)
5. [The IARPA Functional Map of the World (fMoW) Challenge](/datasets/fmow_summary.html)


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

| AOI            | Area of Raster (Sq. Km) | Building Labels (Polygons) | Road Labels (LineString)   |
|----------------|-------------------------|----------------------------|----------------------------|
| [AOI_1_Rio](/AOI_Lists/AOI_1_Rio.html)      | 2,544                   | 382,534                  | N/A                |
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     | 151,367                    |3685 km                  |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   | 23,816                     |425 km                  |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   | 92,015                     |3537 km                  |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     | 35,503                    |1030 km                 |

## Other Competition datasets stored on the SpaceNet Repository
1. [IARPA Multi-View Stereo 3D Mapping Challenge Dataset](/datasets/mvs_summary.html)
2. [IARPA Funtional Map of the World (fMoW) Dataset](/datasets/fmow_summary.html)

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

```commandline
aws s3 ls s3://spacenet-dataset/ 
```

# License:
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">The SpaceNet Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io/" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Partners</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.


