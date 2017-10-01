---
layout: competitions
title: "Building Foot Print Extraction: Round 2"
sidebar: competitions
---
## SpaceNet Round 2 Challenge Implementations
## SpaceNet Challenge Implementations

## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. DigitalGlobe, CosmiQ Works, and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as recently observed by the need to map buildings in Haiti during the response to Hurricane Matthew. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.
For more information see the [SpaceNet Challenge Round 2 Competition Page](http://crowdsourcing.topcoder.com/spacenet)




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
|  1st               |           $6,000       |
|  2nd               |            $3,000       |
|  3rd               |            $1,500       |
|  Best F-score, Las Vegas              |            $1,000    |
|  Best F-score, Paris              |            $1,000    |
|  Best F-score, Shanghai              |            $1,000    |
|  Best F-score, Khartoum              |            $1,000    |
|  Early Incentive  |              $1000      |
|  Total Prizes     |           $15,500       |



# The Metric
In SpaceNet Challenge, the metric for ranking entries is based on the Jaccard Index, also called the Intersection-over-Union (IoU).
For more information read the full article on [The DownlinQ](https://medium.com/the-downlinq/2nd-spacenet-competition-winners-code-release-c7473eea7c11).




# Winning solutions:
The top three solutions have been open sourced at the [SpaceNet Challenge Github Repository](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2) 

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
|1. [XD_XD](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/1-XD_XD) | 0.687740 |
|2. [wleite](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/2-wleite) | 0.642982 |
|3. [nofto](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/3-nofto) | 0.579014 |


[Click Here For the full leaderboard and submission history](https://community.topcoder.com/longcontest/stats/?module=ViewOverview&rd=16892)

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




For Round 2 results please see the [Round 1 Site](/Competitions/Competition1.html)