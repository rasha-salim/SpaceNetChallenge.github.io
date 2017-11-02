## Hosting
[SpaceNet](https://aws.amazon.com/public-datasets/spacenet/) is a corpus of commercial satellite imagery and labeled
 training data to use for machine learning research. The dataset is currently hosted as an [Amazon Web Services (AWS) Public Dataset](https://aws.amazon.com/public-datasets/).

SpaceNet offers 

## Catalog
1. [Area of Interest 1 (AOI 1) - Location: Rio de Janeiro.](/SpaceNetChallenge.github.io/AOI_1_Rio.html) 50cm imagery collected from DigitalGlobe’s [WorldView-2 satellite](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf). The dataset includes building footprints and 8-band multispectral data.
2. [Area of Interest 2 (AOI 2) - Location: Vegas.](/SpaceNetChallenge.github.io/AOI_2_Vegas.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
3. [Area of Interest 3 (AOI 3) - Location: Paris.](/SpaceNetChallenge.github.io/AOI_3_Paris.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
4. [Area of Interest 4 (AOI 4) - Location: Shanghai.](/SpaceNetChallenge.github.io/AOI_4_Shanghai.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.
5. [Area of Interest 5 (AOI 5) - Location: Khartoum.](/SpaceNetChallenge.github.io/AOI_5_Khartoum.html) 30cm imagery collected from DigitalGlobe’s [WorldView-3 satellite](https://www.spaceimagingme.com/downloads/sensors/datasheets/DG_WorldView3_DS_2014.pdf). The dataset includes building footprints and 8-band multispectral data.

| AOI            | Area of Raster (Sq. Km) | Building Labels (Polygons) |
|----------------|-------------------------|----------------------------|
| AOI_1_Rio      | 2,544                   | 4,082,529                  |
| AOI_2_Vegas    | 216                     | 151,367                    |
| AOI_3_Paris    | 1,030                   | 23,816                     |
| AOI_4_Shanghai | 1,000                   | 92,015                     |
| AOI_5_Khartoum | 765                     | 710,960                    |

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

```commandline
aws s3 ls s3://spacenet-dataset/ -request-payer requester
```



