---
layout: aoi
title: AOI 5 Khartoum
sidebar: aoi
---
## SpaceNet AOI 5 Khartoum Area covered
<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/utilities/spacenetV3/spacenetutilities/datasets/AOI_5_Khartoum/AOI_5_Khartoum_SrcTindexex.geojson"></script>


## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 5)
```
AOI_5_Khartoum
├── srcData/rasterData
│   ├── MUL            # Raw souce geotiffs of 8-Band Multi-Spectral raster data from WorldView-3
│   ├── MUL-PanSharpen # Raw souce geotiffs of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│   ├── PAN            # Raw souce geotiffs of Panchromatic raster data from Worldview-3
│   └── RGB-PanSharpen # Raw souce geotiffs of RGB raster data from Worldview-3 pansharpened to 0.3m
│      
├── AOI_5_Khartoum_Train.tar.gz
│      ├── geojson
│      │   └── buildings  # Contains GeoJson labels of buildings for each tile
│      ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│      ├── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
│      └── summaryData    # Contains CSV with pixel based labels for each building in the Tile Set.
├── AOI_5_Khartoum_Test_Public.tar.gz
│      ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│      └── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
│
├── AOI_5_Khartoum_Roads_Train.tar.gz
│      ├── geojson
│      │   └── spacenetroads  # Contains GeoJson labels of Roads for each tile
│      ├── MUL                # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen     # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN                # Contains Tiles of Panchromatic raster data from Worldview-3
│      ├── RGB-PanSharpen     # Contains Tiles of RGB raster data from Worldview-3
│      └── summaryData        # Contains CSV with pixel based labels for each road in the Tile Set.
└── AOI_5_Khartoum_Roads_Test_Public.tar.gz
       ├── MUL                # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
       ├── MUL-PanSharpen     # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
       ├── PAN                # Contains Tiles of Panchromatic raster data from Worldview-3
       └── RGB-PanSharpen     # Contains Tiles of RGB raster data from Worldview-3    
```
## Download instructions

### AOI 5 - Khartoum
To view the contents of the dataset
```commandline
aws s3 ls spacenet-dataset/AOI_5_Khartoum/ --request-payer requester
```

# SpaceNet Roads Dataset
### AOI 5 - Khartoum -  Road Network Extraction Training
To download processed 400mx400m tiles of AOI 5 (25 GB) with associated building footprints for training do the following:
```
aws s3api get-object --bucket spacenet-dataset --key SpaceNet_Roads_Competition/AOI_5_Khartoum_Roads_Train.tar.gz --request-payer requester AOI_5_Khartoum_Roads_Train.tar.gz
```
### AOI 5 - Khartoum - Road Network Extraction  Testing
To download processed 400mx400m tiles of AOI 5 (8.1 GB) for testing do:
```
aws s3api get-object --bucket spacenet-dataset --key SpaceNet_Roads_Competition/AOI_5_Khartoum_Roads_Test_Public.tar.gz --request-payer requester AOI_5_Khartoum_Roads_Test_Public.tar.gz
```



### AOI 5 - Khartoum - Training
To download processed 200mx200m tiles of AOI 2 (4.7 GB) with associated building footprints do the following:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_5_Khartoum/AOI_5_Khartoum_Train.tar.gz --request-payer requester AOI_5_Khartoum_Train.tar.gz
```

### AOI 5 - Khartoum - Testing
To download processed 200mx200m tiles of AOI 2 (1.6 GB) for testing do:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_5_Khartoum/AOI_5_Khartoum_Test_public.tar.gz --request-payer requester AOI_5_Khartoum_Train.tar.gz
```