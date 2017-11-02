---
layout: competitions
title: "Road Extraction and Routing"
sidebar: RoadsExtractor
---
## SpaceNet Challenge: Road Extraction and Routing


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. DigitalGlobe, CosmiQ Works, and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.



# The Metric
In the SpaceNet Roads Challenge, the metric for ranking entries is the APLS metric.  This metric is based on graph theory and empahsizes the creation of a valid road network

The current version of the metric is open sourced on github:  [Average Path Length Similarity (APLS) metric](https://github.com/CosmiQ/apls)
For more information read the full article written by Adam Van Etten at [The DownlinQ](https://medium.com/the-downlinq/2nd-spacenet-competition-winners-code-release-c7473eea7c11).


# The Data - Over 8000 Km of roads across the four SpaceNet Areas of Interest
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



| AOI            | Area of Raster (Sq. Km) | Road Centerlines (Km of Roads) |
|----------------|-------------------------|----------------------------|
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     | 3686 Km                    |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   | 425 Km                     |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   | 3000 Km                     |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     | 1032 Km                    |




# Competition Updates:
For competition email updates, [Sign up here](http://explore.digitalglobe.com/spacenet)

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)
or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)

For previous SpaceNet Competitions see the [Round 2 Site](/Competitions/Competition2.html)