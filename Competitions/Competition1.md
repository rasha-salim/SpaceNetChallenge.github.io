---
layout: competitions
title: "Building Foot Print Extraction: Round 1"
sidebar: BuildingExtractor
---
## SpaceNet Challenge Implementations

## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. DigitalGlobe, CosmiQ Works, and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as recently observed by the need to map buildings in Haiti during the response to Hurricane Matthew. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.
For more information see the [SpaceNet Challenge Round 1 Competition Page](http://crowdsourcing.topcoder.com/spacenet)

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

| Prize             |             USD         |
|-------------------|-------------------------|
|  1st              |           $10,000       |
|  2nd              |            $8,000       |
|  3rd              |            $6,500       |
|  4th              |            $5,500       |
|  5th              |            $4,500       |
|  Docker Incentive |              $500       |
|  Total Prizes     |           $35,000       |



# The Metric
In SpaceNet Challenge, the metric for ranking entries is based on the Jaccard Index, also called the Intersection-over-Union (IoU).
For more information read the full article on [The DownlinQ](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).

# Getting Started  
For a great article on how to get started with SpaceNet data read CosmiQ Works' Adam Van Etten's article [Getting Started With SpaceNet Data](https://medium.com/the-downlinq/getting-started-with-spacenet-data-827fd2ec9f53)
or NVIDIA's Jon Barker and Allison Gray's article [Exploring the SpaceNet Dataset Using DIGITS]
(https://devblogs.nvidia.com/parallelforall/exploring-spacenet-dataset-using-digits/)

# Winning solutions:
The top five solutions have been open sourced at the [SpaceNet Challenge Github Repository](https://github.com/SpaceNetChallenge/BuildingDetectors/) 

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

| Competitor             |             Final Score         |
|-------------------|-------------------------|
|1. [wleite](https://github.com/SpaceNetChallenge/BuildingDetectors/tree/master/wleite) | 0.255292|
|2. [marek.cygan](https://github.com/SpaceNetChallenge/BuildingDetectors/tree/master/marek.cygan) | 0.249985 |
|3. [qinhaifang](https://github.com/SpaceNetChallenge/BuildingDetectors/tree/master/qinhaifang) | 0.225655|
|4. [fugusuki](https://github.com/SpaceNetChallenge/BuildingDetectors/tree/master/fugusuki) | 0.217141|
|5. [bic-user](https://github.com/SpaceNetChallenge/BuildingDetectors/tree/master/bic-user) | 0.167367|

[Click Here For the full leaderboard and submission history](https://community.topcoder.com/longcontest/stats/?module=ViewOverview&rd=16835)

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
| [AOI_1_Rio](/AOI_Lists/AOI_1_Rio.html)      | 2,544                   | 4,082,529                  |


For Round 2 results please see the [Round 2 Site](/Competitions/Competition2.html)