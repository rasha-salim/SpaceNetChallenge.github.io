---
layout: aoi
title: AOI 4 Shanghai
sidebar: aoi
---
## SpaceNet AOI 4 - Shanghai 
Catalog ID: 104001000C924900

Image Time: 2015-06-06T02:35:27Z

<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/utilities/spacenetV3/spacenetutilities/datasets/AOI_4_Shanghai/AOI_4_Shanghai_SrcTindexex.geojson"></script>


## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 4)
```
AOI_4_Shanghai
├── srcData/rasterData
│   ├── MUL            # Raw souce geotiffs of 8-Band Multi-Spectral raster data from WorldView-3
│   ├── MUL-PanSharpen # Raw souce geotiffs of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│   ├── PAN            # Raw souce geotiffs of Panchromatic raster data from Worldview-3
│   └── RGB-PanSharpen # Raw souce geotiffs of RGB raster data from Worldview-3 pansharpened to 0.3m
│      
├── AOI_4_Shanghai_Train.tar.gz
│      ├── geojson
│      │   └── buildings  # Contains GeoJson labels of buildings for each tile
│      ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│      ├── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
│      └── summaryData    # Contains CSV with pixel based labels for each building in the Tile Set.
├── AOI_4_Shanghai_Test_Public.tar.gz
│      ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│      └── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
│
├── AOI_4_Shanghai_Roads_Train.tar.gz
│      ├── geojson
│      │   └── spacenetroads  # Contains GeoJson labels of Roads for each tile
│      ├── MUL                # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│      ├── MUL-PanSharpen     # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│      ├── PAN                # Contains Tiles of Panchromatic raster data from Worldview-3
│      ├── RGB-PanSharpen     # Contains Tiles of RGB raster data from Worldview-3
│      └── summaryData        # Contains CSV with pixel based labels for each road in the Tile Set.
└── AOI_4_Shanghai_Roads_Test_Public.tar.gz
       ├── MUL                # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
       ├── MUL-PanSharpen     # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
       ├── PAN                # Contains Tiles of Panchromatic raster data from Worldview-3
       └── RGB-PanSharpen     # Contains Tiles of RGB raster data from Worldview-3      
```
## Download instructions
### AOI 3 - Paris
To view the contents of the dataset
```commandline
aws s3 ls s3://spacenet-dataset/AOI_4_Shanghai/
```

# SpaceNet Roads Dataset
### AOI 4 - Shanghai -  Road Network Extraction Training
To download processed 400mx400m tiles of AOI 4 (25 GB) with associated building footprints for training do the following:
```
aws s3 cp s3://spacenet-dataset/SpaceNet_Roads_Competition/AOI_4_Shanghai_Roads_Train.tar.gz .
```
### AOI 4 - Shanghai - Road Network Extraction  Testing
To download processed 400mx400m tiles of AOI 4 (8.1 GB) for testing do:
```
aws s3 cp s3://spacenet-dataset/SpaceNet_Roads_Competition/AOI_4_Shanghai_Roads_Test_Public.tar.gz .
```


# SpaceNet Buildings Dataset
### AOI 4 - Shanghai - Training
To download processed 200mx200m tiles of AOI 4 (23.4 GB) with associated building footprints do the following:
```
aws s3 cp s3://spacenet-dataset/AOI_4_Shanghai/AOI_4_Shanghai_Train.tar.gz .
```

### AOI 4 - Shanghai - Testing
To download processed 200mx200m tiles of AOI 4 (7.7 GB) for testing do:
```
aws s3 cp s3://spacenet-dataset/AOI_4_Shanghai/AOI_4_Shanghai_Test_public.tar.gz .
```