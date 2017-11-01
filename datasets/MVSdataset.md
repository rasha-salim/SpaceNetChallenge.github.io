---
layout: dataset
title: MVS Dataset; Argentina
sidebar: dataset
---
## SpaceNet AOI 2 Details
<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/utilities/spacenetV3/spacenetutilities/datasets/AOI_2_Vegas/AOI_2_Vegas_SrcTindexex.geojson"></script>

##

## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 2)
```
Challenge_Data_and_Software	metric_analysis_2017
JHUAPL_Example_Algorithm	readme.txt
WV3

2016-MVS-Benchmark
├── Challenge_Data_and_Software
│      
├── JHUAPL_Example_Algorithm
│
├── srcData/wv3
│      ├── PAN            # Contains Tiles of Panchromatic raster data from WorldView-3
│      └── MSI            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3 in NITF Format
└── srcData/LIDAR
       ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
       └── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
         
```
## Download instructions

### AOI 6 Buenos Aires: MVS Dataset
To view the contents of the dataset
```commandline
aws s3 ls spacenet-dataset/2016-MVS-Benchmark/ --request-payer requester
```

#Distribution statement:
Approved for Public Release; Distribution is Unlimited


#Please reference the following when reporting results using any of this data:
- ìA Multiple View Stereo Benchmark for Satellite Imagery,î Proceedings of the IEEE Applied Imagery Pattern Recognition (AIPR) Workshop, October 2016.
- Commercial satellite imagery in the MVS benchmark data set was provided courtesy of Digital Globe.


For more information, please see:
http://www.jhuapl.edu/satellite-benchmark.html

Dataset was created by IARPA and is hosted as a courtesy
