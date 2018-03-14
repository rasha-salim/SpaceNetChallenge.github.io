---
layout: datasets
title: "SpaceNet Buildings Dataset V1"
sidebar: datasets
---

## The SpaceNet Buildings Dataset


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. CosmiQ Works, Radiant Solutions and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists to work with this data.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.




## The Data - Over 685,000 footprints across the Five SpaceNet Areas of Interest.



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



|  AOI            | Area of Raster (Sq. Km) | Building Labels (Polygons) | 
|----------------|-------------------------|----------------------------|
| [AOI_1_Rio](/AOI_Lists/AOI_1_Rio.html)      | 2,544                   | 382,534                  | 
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     | 151,367                    |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   | 23,816                     |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   | 92,015                     |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     | 35,503                    |


## Catalog
The data is hosted on AWS in a requester pays bucket.
```commandline
aws s3 ls s3://spacenet-dataset/SpaceNet_Buildings_Dataset_Round1/ 

```

# The Metric
In the SpaceNet Roads Challenge, the metric for ranking entries is the [SpaceNet Metric](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).  
This metric is an F1-Score based on  the intersection over union of two building footprints with a threshold of 0.5


For more information read the full article written by Patrick Hagerty at the [DownlinQ](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).  


## Training Data
### AOI 1 - Rio -  Building Extraction Training
To download processed 200mx200m tiles of AOI 1 (23 GB) with associated building footprints for training do the following:
```
aws cp s3://spacenet-dataset/spacenet_TrainData/3band.tar.gz .
aws cp s3://spacenet-dataset/spacenet_TrainData/8band.tar.gz .
```



## Test Data
### AOI 1 - Rio - Building Extraction Testing
To download processed 200mx200m tiles of AOI 1 (7.9 GB) for testing do:
```
aws cp s3://spacenet-dataset/spacenet_TestData/3band.tar.gz .
aws cp s3://spacenet-dataset/spacenet_TestData/8band.tar.gz .
```


# Competition Updates:

For more details about the [SpaceNet Building Extraction Challenge: Round 1](/Competitions/Competition1.html)  visit it's [website](/Competitions/Competition1.html)  

Also check out the Round 2 Competition
For more details about the [SpaceNet Building Extraction Challenge: Round 2](/Competitions/Competition2.html)  visit it's [website](/Competitions/Competition2.html)  

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)
or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)



## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">The SpaceNet Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io/" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Partners</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
