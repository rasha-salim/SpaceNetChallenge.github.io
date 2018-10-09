---
layout: datasets
title: "SpaceNet Off-Nadir Dataset"
sidebar: datasets
---
## The SpaceNet Off-Nadir Dataset


## The Problem
The commercialization of the geospatial industry has led to an explosive amount of data being collected to characterize our changing planet. One area for innovation is the application of computer vision and deep learning to extract information from satellite imagery at scale. CosmiQ Works, Radiant Solutions and NVIDIA have partnered to release the SpaceNet data set to the public to enable developers and data scientists to work with this data.

Today, map features such as roads, building footprints, and points of interest are primarily created through manual techniques. We believe that advancing automated feature extraction techniques will serve important downstream uses of map data including humanitarian and disaster response, as observed by the need to map road networks during the response to recent flooding in Bangladesh and Hurricane Maria in Puerto Rico. Furthermore, we think that solving this challenge is an important stepping stone to unleashing the power of advanced computer vision algorithms applied to a variety of remote sensing data applications in both the public and private sector.

In a certain scenarios, the most recent image after an event occurs is Off-Nadir, i.e. it is from an oblique angle.  This dataset allow's researcher's to explore how this type of imagery affect's automated feature extraction techniques




## The Data - Over 120,000 Building footprints over 665 sqkm of Atlanta, GA with 27 associated WV-2 images.

See the [labeling guide and schema](/assets/docs/SpaceNetOff-Nadir_labeling_rules_v2.html) for details about the creation of the dataset



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


## Catalog
The data is hosted on AWS as Public Dataset.  An AWS account is required.   
```commandline
aws s3 ls s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/

```

## Sample Data
### 10 Samples from each Image -  Off-Nadir Imagery Samples
To download processed 450mx450m tiles of AOI 2 (728.8 MB) with associated building footprints:
```
aws s3 cp s3://spacenet-dataset/SpaceNet_Roads_Competition/SpaceNet_Roads_Sample.tar.gz .
```



## Training Data
### AOI 6 Atlanta -  Building Footprint Extraction Training
To download processed 450mx450m tiles of AOI 6 (202 GB):
```
aws s3 cp  s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/SpaceNet_v4_Train.tar.gz .
```

## Test Data
### AOI 2 - Vegas - Road Network Extraction  Testing
To download processed 400mx400m tiles of AOI 2 (8.1 GB) for testing do:
```
aws s3 cp  s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/SpaceNet_v4_Test.tar.gz .
```

# The Metric
In the SpaceNet Roads Challenge, the metric for ranking entries is the [SpaceNet Metric](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).  
This metric is an F1-Score based on  the intersection over union of two building footprints with a threshold of 0.5


For more information read the full article written by Patrick Hagerty at the [DownlinQ](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).  

# Competition Updates:


For more details about previous SpaceNet Building Challenges [SpaceNet Building Extraction Challenge: Round 2](/Competitions/Competition2.html)  visit it's [website](/Competitions/Competition2.html)  

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)
or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)



## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">The SpaceNet Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io/" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Partners</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
