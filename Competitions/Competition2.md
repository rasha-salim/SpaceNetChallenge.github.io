---
layout: competitions
title: "Building Foot Print Extraction: Round 2"
sidebar: buildingextraction
---
## SpaceNet Round 2 Challenge Implementations

## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale.  CosmiQ Works, DigitalGlobe and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists.

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

and see below

## Evaluation Metric
The evaluation metric for this competition is an F1 score with the matching algorithm inspired by Algorithm 2 in the [ILSVRC paper applied to the detection of building footprints](https://arxiv.org/pdf/1409.0575v3.pdf). For each building there is a geospatially defined polygon label to represent the footprint of the building. A SpaceNet entry will generate polygons to represent proposed building footprints.  Each proposed building footprint is either a “true positive” or a “false positive”.

* The proposed footprint is a “true positive” if the proposal is the closest (measured by the IoU) proposal to a labeled polygon AND the IoU between the proposal and the label is about the prescribed threshold of 0.5.
* Otherwise, the proposed footprint is a “false positive”.

There is at most one “true positive” per labeled polygon.
The measure of proximity between labeled polygons and proposed polygons is the Jaccard similarity or the “Intersection over Union (IoU)”, defined as:

![alt text](https://github.com/SpaceNetChallenge/utilities/raw/master/content/IoU.jpg "IoU")

The value of IoU is between 0 and 1, where closer polygons have higher IoU values.

The F1 score is the harmonic mean of precision and recall, combining the accuracy in the precision measure and the completeness in the recall measure. For this competition, the number of true positives and false positives are aggregated over all of the test imagery and the F1 score is computed from the aggregated counts.

For example, suppose there are N polygon labels for building footprints that are considered ground truth and suppose there are M proposed polygons by an entry in the SpaceNet competition.  Let tp denote the number of true positives of the M proposed polygons.  The F1 score is calculated as follows:

![alt text](https://github.com/SpaceNetChallenge/utilities/raw/master/content/F1.jpg "IoU")

The F1 score is between 0 and 1, where larger numbers are better scores.

Hints:
* The images provided could contain anywhere from zero to multiple buildings.
* All proposed polygons should be legitimate (they should have an area, they should have points that at least make a triangle instead of a point or a line, etc).
* Use the [metric implementation code](https://github.com/SpaceNetChallenge/utilities/blob/master/python/evaluateScene.py) to self evaluate.




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
