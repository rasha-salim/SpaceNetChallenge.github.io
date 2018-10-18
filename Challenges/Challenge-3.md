---
layout: competitions
title: "Road Extraction and Routing"
sidebar: competitions
---
## SpaceNet Challenge: Road Extraction and Routing


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. DigitalGlobe, CosmiQ Works, and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists to work with this data.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.



# The Metric
In the SpaceNet Roads Challenge, the metric for ranking entries is the APLS metric.  This metric is based on graph theory and empahsizes the creation of a valid road network

The current version of the metric is open sourced on github:  [Average Path Length Similarity (APLS) metric](https://github.com/CosmiQ/apls)
For more information read the [SpaceNet Road Detection and Routing Challenge Series, Part 1](https://medium.com/the-downlinq/spacenet-road-detection-and-routing-challenge-part-i-d4f59d55bfce), and [Part 2](https://medium.com/the-downlinq/spacenet-road-detection-and-routing-challenge-part-ii-apls-implementation-92acd86f4094),  written by [Adam Van Etten](https://medium.com/@avanetten) at [The DownlinQ](https://medium.com/the-downlinq).

# Winning solutions:
The top five solutions have been open sourced at the [SpaceNet Challenge Github Repository](https://github.com/SpaceNetChallenge/RoadDetector) 

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

**Place**|**Entrant**|**Country**|**Average Score**|**Las Vegas**|**Paris**|**Shanghai**|**Khartoum**
:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:
1|albu|Russia|0.6663|0.7977|0.604|0.6543|0.6093
2|cannab|Russia|0.6661|0.7804|0.6446|0.6398|0.5996
2|pfr|France|0.666|0.8009|0.6008|0.6646|0.5975
4|selim\_sef|Germany|0.6567|0.7884|0.5991|0.6472|0.5922
5|fbastani|America|0.6284|0.771|0.5474|0.6326|0.5628
6|ipraznik|Germany|0.6215|0.7578|0.5668|0.6078|0.5537
7|tcghanareddy|India|0.6182|0.7591|0.571|0.6014|0.5415
8|hasan.asyari|Norway|0.6097|0.7407|0.5557|0.5952|0.5472
9|aveysov|Russia|0.5943|0.7426|0.5805|0.5751|0.4789


Top 5 Solutions:
1. [Albu](https://github.com/SpaceNetChallenge/RoadDetector/blob/tree/albu-solution/)

2. (tie)[cannab](https://github.com/SpaceNetChallenge/RoadDetector/blob/tree/cannab-solution/)

3. (Tie)[pfr](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/pfr-solution)

4.  [selim_sef](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/selim_sef-solution)

5.  [fbastani](https://github.com/SpaceNetChallenge/BuildingDetectors_Round2/tree/master/fabastani-solution)


[Click Here For the full leaderboard and submission history](https://community.topcoder.com/longcontest/stats/?module=ViewOverview&rd=16892)


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



| AOI            | Area of Raster (Sq. Km) | Road Centerlines (LineString)   |
|----------------|-------------------------|----------------------------|
| [AOI_2_Vegas](/AOI_Lists/AOI_2_Vegas.html)     | 216                     |3685 km                  |
| [AOI_3_Paris](/AOI_Lists/AOI_3_Paris.html)    | 1,030                   |425 km                  |
| [AOI_4_Shanghai](/AOI_Lists/AOI_4_Shanghai.html) | 1,000                   |3537 km                  |
| [AOI_5_Khartoum](/AOI_Lists/AOI_5_Khartoum.html) | 765                     |1030 km                 |


### For more details on the dataset visit the [SpaceNet Roads Dataset](/datasets/spacenetRoads-summary.html) website

# Competition Updates:
The Roads competition is now over and the top 5 Algorithms have been open sourced.  To see the code visit the [SpaceNet Road Network Extraction and Routing Challenge Github repository](https://github.com/SpaceNetChallenge/RoadDetectors)
 
For competition email updates, [Sign up here](http://explore.digitalglobe.com/spacenet)

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)
or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)

For general details about SpaceNet Competitions see the [SpaceNet Competition Summary](/Challenges/competitionsSummary.html)
