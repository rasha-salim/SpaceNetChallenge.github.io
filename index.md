## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/SpaceNetChallenge/SpaceNetChallenge.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/SpaceNetChallenge/SpaceNetChallenge.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

# SpaceNet Utilities

Instruction for the download of [SpaceNet](https://aws.amazon.com/public-data-sets/spacenet/) satellite imagery data corpus to a format that is consumable by machine learning algorithms.
 
 

## Dependencies
Required that AWS CLI is installed and that an active AWS account with credit card is associated with the aws cli

Configure the AWS CLI using aws configure

SpaceNet AWS Structure
```
s3://spacenet-dataset/
-- AOI_1_Rio
    |-- processedData
    |   -- processedBuildingLabels.tar.gz  # Compressed 3band and 8band 200m x 200m tiles with associated building foot print labels
                                           # This dataset is the Training Dataset for the first [Top Coder Competition](https://community.topcoder.com/longcontest/?module=ViewProblemStatement&rd=16835&pm=14439)
    `-- srcData
        |-- rasterData
        |   |-- 3-Band.tar.gz # 3band (RGB) Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
        |    -- 8-Band.tar.gz # 8band Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
         -- vectorData
            |-- Rio_BuildingLabels.tar.gz # Source Dataset that contains Building the building foot prints traced from the Mosaic
            |-- Rio_HGIS_Metro.gdb.tar.gz # Source Point of Interest Dataset in GeoDatabase Format.  Best if Used with ESRI
             -- Rio_HGIS_Metro_extract.tar # Source Point of Interest Dataset in GeoJSON with associated .jpg.  Easy to Use without ESRI toolset
-- AOI_1_Rio
    |-- processedData
    |   -- processedBuildingLabels.tar.gz  # Compressed 3band and 8band 200m x 200m tiles with associated building foot print labels
                                           # This dataset is the Training Dataset for the first [Top Coder Competition](https://community.topcoder.com/longcontest/?module=ViewProblemStatement&rd=16835&pm=14439)
    `-- srcData
        |-- rasterData
        |   |-- 3-Band.tar.gz # 3band (RGB) Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
        |    -- 8-Band.tar.gz # 8band Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
         -- vectorData
            |-- Rio_BuildingLabels.tar.gz # Source Dataset that contains Building the building foot prints traced from the Mosaic
            |-- Rio_HGIS_Metro.gdb.tar.gz # Source Point of Interest Dataset in GeoDatabase Format.  Best if Used with ESRI
             -- Rio_HGIS_Metro_extract.tar # Source Point of Interest Dataset in GeoJSON with associated .jpg.  Easy to Use without ESRI toolset
-- AOI_1_Rio
    |-- processedData
    |   -- processedBuildingLabels.tar.gz  # Compressed 3band and 8band 200m x 200m tiles with associated building foot print labels
                                           # This dataset is the Training Dataset for the first [Top Coder Competition](https://community.topcoder.com/longcontest/?module=ViewProblemStatement&rd=16835&pm=14439)
    `-- srcData
        |-- rasterData
        |   |-- 3-Band.tar.gz # 3band (RGB) Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
        |    -- 8-Band.tar.gz # 8band Raster Mosaic for Rio De Jenairo area (2784 sq KM) collected by [WorldView-2](http://satimagingcorp.s3.amazonaws.com/site/pdf/WorldView-2_datasheet.pdf)
         -- vectorData
            |-- Rio_BuildingLabels.tar.gz # Source Dataset that contains Building the building foot prints traced from the Mosaic
            |-- Rio_HGIS_Metro.gdb.tar.gz # Source Point of Interest Dataset in GeoDatabase Format.  Best if Used with ESRI
             -- Rio_HGIS_Metro_extract.tar # Source Point of Interest Dataset in GeoJSON with associated .jpg.  Easy to Use without ESRI toolset


```

#Spacenet Processed Imagery Release 1 
##AOI 1 Rio
##To download processed 200mx200m Tiles: AOI 1 Rio with associated building foot prints for building foot print extraction tests do the following
```
## Warning this file is 3.4 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/processedData/processedBuildingLabels.tar.gz --request-payer requester processedBuildingLabels.tar.gz
```

##Spacenet Processed Imagery Release 2
##Tarball details
```
├── AOI_[Num]_[City]_Train
│   ├── geojson
│   │   └── buildings  # Contains GeoJson labels of buildings for each tile 
│   ├── MUL            # Contains Tiles of 8-Band Multi-Spectral raster data from WorldView-3
│   ├── MUL-PanSharpen # Contains Tiles of 8-Band Multi-Spectral raster data pansharpened to 0.3m
│   ├── PAN            # Contains Tiles of Panchromatic raster data from Worldview-3
│   ├── RGB-PanSharpen # Contains Tiles of RGB raster data from Worldview-3 
│   └── summaryData    # Contains CSV with pixel based labels for each building in the Tile Set.  This is equiavalent to the Spacenet Competition 1 summary File.  
```

##AOI 2 Vegas 
##To download processed 200mx200m Tiles: AOI 2 Vegas with associated building foot prints for building foot print extraction tests do the following
```
## Warning this file is 23 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_2_Vegas/AOI_2_Vegas_Train.tar.gz --request-payer requester AOI_2_Vegas_Train.tar.gz
```

##AOI 3 Paris
##To download processed 200mx200m Tiles: AOI 3 Paris with associated building foot prints for building foot print extraction tests do the following
```
## Warning this file is 5 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_3_Paris/AOI_3_Paris_Train.tar.gz --request-payer requester AOI_3_Paris_Train.tar.gz
```

##AOI 4 Shanghai
##To download processed 200mx200m Tiles: AOI 4 Shanghai with associated building foot prints for building foot print extraction tests do the following
```
## Warning this file is 23 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_4_Shanghai/AOI_4_Shanghai_Train.tar.gz --request-payer requester AOI_4_Shanghai_Train.tar.gz
```

##AOI 5 Shanghai
##To download processed 200mx200m Tiles: AOI 5 Khartoum with associated building foot prints for building foot print extraction tests do the following
```
## Warning this file is 4 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_5_Khartoum/AOI_5_Khartoum_Train.tar.gz --request-payer requester AOI_5_Khartoum_Train.tar.gz
```


##To download the Source Imagery Mosaic
```
## Warning this file is 2.3 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/rasterData/3-Band.tar.gz --request-payer requester 3-Band.tar.gz
## Warning this file is 6.5 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/rasterData/8-Band.tar.gz --request-payer requester 8-Band.tar.gz
```

##To download the Source Vector Data for the Building Extraction Challenge
```
## Warning this file is 0.18 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_BuildingLabels.tar.gz --request-payer requester Rio_BuildingLabels.tar.gz

```

##To download the Rio Point of Interest Dataset in ESRI GeoDatabase Form
```
## Warning this file is 31 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro.gdb.tar.gz --request-payer requester Rio_HGIS_Metro.gdb.tar.gz

```

##To download the Rio Point of Interest Dataset Extracted into GeoJSONs with associated .jpg
```
## Warning this file is 29 GB
aws s3api get-object --bucket spacenet-dataset --key AOI_1_Rio/srcData/vectorData/Rio_HGIS_Metro_extract.tar --request-payer requester Rio_HGIS_Metro_extract.tar

```



