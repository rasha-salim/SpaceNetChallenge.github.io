---
layout: aoi
title: AOI 1 Rio
sidebar: aoi
---

## SpaceNet AOI 1 Area covered
<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/utilities/spacenetV3/spacenetutilities/datasets/AOI_1_Rio/AOI_1_Rio_SrcTindexex.geojson"></script>

## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 1)
```
s3://spacenet-dataset/
-- AOI_1_Rio
    |-- processedData
    |   -- processedBuildingLabels.tar.gz  # Compressed 3band and 8band 200m x 200m tiles with associated building foot print labels                                 # This dataset is the Training Dataset for the first Top Coder Competition
    `-- srcData
        |-- rasterData
        |   |-- 3-Band.tar.gz # 3band (RGB) Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by WorldView-2
        |    -- 8-Band.tar.gz # 8band Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by WorldView-2
         -- vectorData
            |-- Rio_BuildingLabels.tar.gz # Source Dataset that contains Building the building foot prints traced from the Mosaic
            |-- Rio_HGIS_Metro.gdb.tar.gz  # Source Point of Interest Dataset in GeoDatabase Format.  Best if Used with ESRI
             -- Rio_HGIS_Metro_extract.tar # Source Point of Interest Dataset in GeoJSON with associated .jpg.  Easy to Use without ESRI toolset
```
## Download instructions

### AOI 1 - Rio de Janeiro
To view the contents of the dataset
```commandline
aws s3 ls spacenet-dataset/AOI_1_Rio/ --request-payer requester
```

To download processed 200mx200m tiles of AOI 1 (3.4 GB) with associated building footprints do the following:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/processedData/processedBuildingLabels.tar.gz --request-payer requester processedBuildingLabels.tar.gz
```
To download the Source Imagery Mosaic (3-band = 2.3 GB and 8-band = 6.5 GB):
```
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/rasterData/3-Band.tar.gz --request-payer requester 3-Band.tar.gz
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/rasterData/8-Band.tar.gz --request-payer requester 8-Band.tar.gz
```
To download the Source Vector Data (0.18 GB):
```
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_BuildingLabels.tar.gz --request-payer requester Rio_BuildingLabels.tar.gz
```

### Point of Interest Dataset in ESRI GeoDatabase Form (31 GB)
```
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro.gdb.tar.gz --request-payer requester Rio_HGIS_Metro.gdb.tar.gz
```

### Point of Interest Dataset Extracted into GeoJSONs with associated .jpg (29 GB)
```
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro_extract.tar --request-payer requester Rio_HGIS_Metro_extract.tar
```
