---
layout: toplevel
title: 'SpaceNet'
sidebar: default
---


## The SpaceNet Off-Nadir Building Detection Challenge has launched
The SpaceNet team has launched the SpaceNet Off-Nadir Building Detection Challenge on TopCoder.  The Challenge will run through December 21, 2018 and offer's $50,000 in total prizes.  Read more about the dataset and challenge on the [The DownlinQ](https://medium.com/the-downlinq/introducing-the-spacenet-off-nadir-imagery-and-buildings-dataset-e4a3c1cb4ce3) and visit the [Challenge page to register and compete](http://community.topcoder.com/longcontest/?module=ViewProblemStatement&rd=17313&pm=15148).

This challenge focuses on the use of Off-Nadir imagery for building footprint extraction.  The dataset includes 27 WorldView 2 Satellite images from 7 degrees to 54 degrees off-nadir all captured within 5 minutes of each other. The dataset covers over 665 square kilometers of downtown Atlanta and ~126,747 buildings footprints labeled from a nadir image. It is now available for download — for instructions, see the [SpaceNet Off-Nadir Dataset page](/datasets/spacenet-OffNadir-summary.html)


## Hosting
[SpaceNet](https://registry.opendata.aws/spacenet/) is a corpus of commercial satellite imagery and labeled
 training data to use for machine learning research. The dataset is currently hosted as an [Amazon Web Services (AWS) Public Dataset](https://aws.amazon.com/public-datasets/).

## Github Repositories
Check out our SpaceNet Utilities for some helpful tools for using geospatial data for machine learning
1.  [SpaceNetUtilities](https://github.com/SpaceNetChallenge/utilities)
2.  [Average Path Length Similarity (APLS) metric](https://github.com/CosmiQ/apls)
3.  [SpaceNet Building Footprint Challenge: Round 1 Solutions](https://github.com/SpaceNetChallenge/BuildingDetectors/)
4.  [SpaceNet Building Footprint Challenge: Round 2 Solutions](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2)
5.  [SpaceNet Road Network Extraction and Routing Challenge](https://github.com/SpaceNetChallenge/RoadDetectors)



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

