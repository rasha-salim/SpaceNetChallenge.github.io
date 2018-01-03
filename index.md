---
layout: toplevel
title: 'SpaceNet'
sidebar: default
---
## Hosting
[SpaceNet](https://aws.amazon.com/public-datasets/spacenet/) is a corpus of commercial satellite imagery and labeled
 training data to use for machine learning research. The dataset is currently hosted as an [Amazon Web Services (AWS) Public Dataset](https://aws.amazon.com/public-datasets/).

## Github Repositories
Check out our SpaceNet Utilities for some helpful tools for using geospatial data for machine learning
1.  [SpaceNetUtilities](https://github.com/SpaceNetChallenge/utilities)
2.  [Average Path Length Similarity (APLS) metric](https://github.com/CosmiQ/apls)
3.  [SpaceNet Challenge Round 1 Solutions](https://github.com/SpaceNetChallenge/BuildingDetectors/)
4.  [SpaceNet Challenge Round 2 Solutions](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2)

## Next Competition
The next competition will be roads extraction.  See the [Roads Competition Page](/Competitions/Competition3.md) for more details


## Catalog
1. [Area of Interest 1 (AOI 1) - Location: Rio de Janeiro.](/AOI_Lists/AOI_1_Rio.html) 50cm imagery collected from DigitalGlobe’s [WorldView-2 satellite](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf). The dataset includes building footprints and 8-band multispectral data.
2. [Area of Interest 2 (AOI 2) - Location: Vegas.](/AOI_Lists/AOI_2_Vegas.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
3. [Area of Interest 3 (AOI 3) - Location: Paris.](/AOI_Lists/AOI_3_Paris.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
4. [Area of Interest 4 (AOI 4) - Location: Shanghai.](/AOI_Lists/AOI_4_Shanghai.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
5. [Area of Interest 5 (AOI 5) - Location: Khartoum.](/AOI_Lists/AOI_5_Khartoum.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.

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


## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

```commandline
aws s3 ls s3://spacenet-dataset/ --request-payer requester
```


# Competition Updates:
For competition email updates, [Sign up here](http://explore.digitalglobe.com/spacenet)

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)

or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)

