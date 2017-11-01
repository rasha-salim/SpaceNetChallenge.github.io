---
layout: competitions
title: "Road Extraction and Routing: Round 1"
sidebar: RoadsExtractor
---
## SpaceNet Challenge: Road Extraction and Routing: Round 1


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. DigitalGlobe, CosmiQ Works, and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as recently observed by the need to map buildings in Haiti during the response to Hurricane Matthew. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.
For more information see the [SpaceNet Challenge Round 3 Competition Page](http://crowdsourcing.topcoder.com/spacenet)




## Prize List

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

| Prize              |             USD         |
|--------------------|-------------------------|
|  1st               |           $25,000       |
|  2nd               |           $15,000       |
|  3rd               |           $10,500       |
|  Total Prizes      |           $50,000       |



# The Metric
In the SpaceNet Roads Challenge, the metric for ranking entries is the APLS metric.  This metric is based on graph theory and empahsizes the creation of a valid road network
Sample code for implementation of the metric is available at the [CosmiQ Works Repository](www.github.com/cosmiq)

For more information read the full article written by Adam Van Etten [The DownlinQ](https://medium.com/the-downlinq/2nd-spacenet-competition-winners-code-release-c7473eea7c11).


# The Data
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

| AOI            | Area of Raster (Sq. Km) | Building Labels (Polygons) |
|----------------|-------------------------|----------------------------|
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     | 151,367                    |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   | 23,816                     |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   | 92,015                     |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     | 710,960                    |


# Sample Code:

# Competition Updates:



For previous SpaceNet Competitions see the [Round 1 Site](/Competitions/Competition2.html)