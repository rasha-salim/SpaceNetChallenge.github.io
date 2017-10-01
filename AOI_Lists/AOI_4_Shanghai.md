---
layout: aoi
title: AOI 4 Shanghai
sidebar: aoi
---
## SpaceNet AOI 4 Area covered
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
      
```
## Download instructions


### AOI 4 - Shanghai - Training
To download processed 200mx200m tiles of AOI 2 (23.4 GB) with associated building footprints do the following:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_4_Shanghai/AOI_4_Shanghai_Train.tar.gz --request-payer requester AOI_4_Shanghai_Train.tar.gz
```

### AOI 4 - Shanghai - Testing
To download processed 200mx200m tiles of AOI 2 (7.7 GB) for testing do:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_4_Shanghai/AOI_4_Shanghai_Test_public.tar.gz --request-payer requester AOI_4_Shanghai_Train.tar.gz
```