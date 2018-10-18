---
layout: competitions
title: "Off-Nadir Building Footprint Extraction"
sidebar: buildingextraction
---
## SpaceNet Off-Nadir Building Footprint Extraction

## The Problem

Can you help us automate mapping from off-nadir imagery? In this challenge, competitors are tasked with finding automated methods for extracting map-ready building footprints from high-resolution satellite imagery from high off-nadir imagery. In many disaster scenarios the first post-event imagery is from a more off-nadir image than is used in standard mapping use cases.  The ability to use higher off-nadir imagery will allow for more flexibility in acquiring and using satellite imagery after a disaster.  Moving towards more accurate fully automated extraction of building footprints  will help bring innovation to computer vision methodologies applied to high-resolution satellite imagery, and ultimately help create better maps where they are needed most.
 
Your task will be to extract building footprints from increasingly off-nadir satellite images. The polygon’s you create will be compared to ground truth, and the quality of the solutions will be measured using the SpaceNet metric.   


## Prize List

$50,000 in total prizes


## The Data
This challenge uses the SpaceNet Off-Nadir dataset which contains 27 Worldview-2 images over Atlanta, GA on Dec 22, 2009 with off-nadir angles from 7 to 55 degrees.  ~665 sq km of imagery was then labeled with over 126,000 building footprints.  For more information about the dataset please see the [SpaceNet Off-Nadir Dataset webpage](/datasets/spacenet-OffNadir-summary.html)


## Evaluation Metric

The evaluation metric for this competition is an F1 score with the matching algorithm inspired by Algorithm 2 in the [ILSVRC paper applied to the detection of building footprints](https://arxiv.org/pdf/1409.0575v3.pdf). For each building there is a geospatially defined polygon label to represent the footprint of the building. A SpaceNet entry will generate polygons to represent proposed building footprints.  Each proposed building footprint is either a “true positive” or a “false positive”. For some geospatial examples see the full article on [The DownlinQ](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).

* The proposed footprint is a “true positive” if the proposal is the closest (measured by the IoU) proposal to a labeled polygon AND the IoU between the proposal and the label is about the prescribed threshold of 0.5.
* Otherwise, the proposed footprint is a “false positive”.

There is at most one “true positive” per labeled polygon.
The measure of proximity between labeled polygons and proposed polygons is the Jaccard similarity or the “Intersection over Union (IoU)”, defined as:

![alt text](https://github.com/SpaceNetChallenge/utilities/raw/master/content/IoU.jpg "IoU")

The value of IoU is between 0 and 1, where closer polygons have higher IoU values.

The F1 score is the harmonic mean of precision and recall, combining the accuracy in the precision measure and the completeness in the recall measure. For this competition, the number of true positives and false positives are aggregated over all of the test imagery for three segments, (Nadir, Off-Nadir, Very Off-Nadir) and an F1 score for each off-nadir segment is computed from the aggregated counts.  The Final F1-Score is 

```F1-Score Total = mean(F1-Score-Nadir, F1-Score-Off-Nadir, F1-Score-Very-Off-Nadir)```

For example, suppose there are N polygon labels for building footprints that are considered ground truth and suppose there are M proposed polygons by an entry in the SpaceNet competition.  Let tp denote the number of true positives of the M proposed polygons.  The F1 score is calculated as follows:

![alt text](https://github.com/SpaceNetChallenge/utilities/raw/master/content/F1.jpg "IoU")

The F1 score is between 0 and 1, where larger numbers are better scores.

Hints:
* The images provided could contain anywhere from zero to multiple buildings.
* All proposed polygons should be legitimate (they should have an area, they should have points that at least make a triangle instead of a point or a line, etc).
* Use the [metric implementation code](https://github.com/SpaceNetChallenge/utilities/blob/master/python/evaluateScene.py) to self evaluate.
* All polygons of less than 25 m square (10 pix x 10 pix) are ignored





