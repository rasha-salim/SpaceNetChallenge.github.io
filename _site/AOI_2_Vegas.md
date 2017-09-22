## SpaceNet AOI 2 Details
<script src="https://embed.github.com/view/geojson/SpaceNetChallenge/utilities/spacenetV3/spacenetutilities/datasets/AOI_2_Vegas/AOI_2_Vegas_SrcTindexex.geojson"></script>

##

## SpaceNet Simple Storage Service (S3) Directory Structure (AOI 2)
```
├── AOI_2_Vegas_Train
│   ├── geojson
│   │   └── buildings  # Contains GeoJson labels of buildings for each tile
│   ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│   ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│   ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│   ├── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3
│   └── summaryData    # Contains CSV with pixel based labels for each building in the Tile Set.
```
## Download instructions

### AOI 1 - Rio de Janeiro
To view the contents of the dataset
```commandline
aws s3 ls spacenet-dataset/AOI_2_Vegas/ --request-payer requester
```

```
### AOI 2 - Vegas
To download processed 200mx200m tiles of AOI 2 (23 GB) with associated building footprints do the following:
```
aws s3api get-object --bucket spacenet-dataset --key AOI_2_Vegas/AOI_2_Vegas_Train.tar.gz --request-payer requester AOI_2_Vegas_Train.tar.gz
```