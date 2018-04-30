---
layout: datasets
title: Urban 3D Challenge Dataset
sidebar: datasets
---

# [The USSOCOM Urban 3D Challenge](https://www.topcoder.com/urban3d)

High-resolution satellite imagery is changing our understanding of the world around us, as well as the way we as humans interact with our planet. However, raw images do little more than pique our interest unless we can superimpose a layer that actually identifies real objects. Reliable labeling of building footprints based on satellite imagery is one of the first and most challenging steps in producing accurate 3D models. While automated algorithms continue to improve, significant manual effort is still required to ensure geospatial accuracy and acceptable quality. Improved automation is required to enable more rapid response to major world events such as humanitarian and disaster response. 3D height data can help improve automated building footprint detection performance, and capabilities for providing this data on a global scale are now emerging. In this challenge, contestants used 2D and 3D imagery generated from commercial satellite imagery along with state of the art machine learning techniques to provide high quality, automated building footprint detection performance over large areas. 

This challenge published a large-scale dataset containing 2D orthrorectified RGB and 3D Digital Surface Models and Digital Terrain Models generated from commercial satellite imagery covering over 360 km of terrain and containing roughly 157,000 annotated building footprints. All imagery products are provided at 50 cm ground sample distance (GSD). This unique 2D/3D large scale dataset provides researchers an opportunity to utilize machine learning techniques to further improve state of the art performance. 

SpaceNet is hosting the Urban 3D Challenge dataset in the spacenet repository to ensure easy access to the data.

## Related Websites

For more information about the Urban 3D Challenge competition, please visit the [Urban 3D Challenge contest website](https://www.topcoder.com/urban3d).

Additional information about obtaining the open source algorithms or visualization tools can be found on the [Urban 3D Challenge GitHub website](https://github.com/topcoderinc/Urban3d).  

More information can also be found at the [JHU Applied Physics Laboratory Public Geospatial Data and Software website](http://www.jhuapl.edu/pubgeo.html). 


## Reference Requirement

Please reference the following when publishing results using this data:

1.  H. Goldberg, M. Brown, and S. Wang, A Benchmark for Building Footprint Classification Using Orthorectified RGB Imagery and Digital Surface Models from Commercial Satellites, 46th Annual IEEE Applied Imagery Pattern Recognition Workshop, Washington, D.C, 2017.

BibTeX:	
```
@inproceedings{Urban3D2017,
  title={A Benchmark for Building Footprint Classification Using Orthorectified RGB Imagery and Digital Surface Models from Commercial Satellites},
  author={Goldberg, Hirsh and Brown, Myron and Wang, Sean},
  booktitle={Proceedings of IEEE Applied Imagery Pattern Recognition Workshop 2017},
  year={2017}
}
```

Alternatively, this dataset may be referenced as, �USSOCOM Urban 3D Challenge Benchmark Dataset.�
 
Please also cite SpaceNet as follows:

```
SpaceNet on Amazon Web Services (AWS). �Datasets.� The SpaceNet Catalog.  Last modified January 4, 2018.
Accessed on [Insert Date]. https://spacenetchallenge.github.io/datasets/datasetHomePage.html.
```

## Catalog
```commandline
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/00-Orig_Source_Data/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/01-Provisional_Train/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/02-Provisional_Test/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/03-Sequestered_Test/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/04-Unused_Data/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/AOI_polygons/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/Pretrained_Models/
aws s3 ls s3://spacenet-dataset/Urban_3D_Challenge/LICENSE.txt
```

# Software Code with regard to this dataset:

### Available open source solutions from contest winners:

* [1st place](https://github.com/topcoderinc/Urban3d/tree/master/01-albu)
* [2nd place](https://github.com/topcoderinc/Urban3d/tree/master/02-selim_sef)
* [3rd place](https://github.com/topcoderinc/Urban3d/tree/master/03-cannab)
* [4th place](https://github.com/topcoderinc/Urban3d/tree/master/04-alina.marcu)
* [5th place](https://github.com/topcoderinc/Urban3d/tree/master/05-kylelee)
* [6th place](https://github.com/topcoderinc/Urban3d/tree/master/06-ZFTurbo)

For more information on how to install and run these solutions, see the [Urban 3D Challenge Github README](https://github.com/topcoderinc/Urban3d/blob/master/README.md).

The pre-trained models associated with each of the winning solution are provided alongside the data as described in the 'Catalog' section of this README. 

Additional open source software for formatting new dataset to be used by these algorithms can be found [here](https://github.com/pubgeo/Urban3DChallenge).

### Published Papers

1.   H. Goldberg, S. Wang, M. Brown, and G. Christie. Urban 3D Challenge: Building Footprint Detection Using Orthorectified Imagery and Digital Surface Models from Commercial Satellites. In Proceedings SPIE Defense and Commercial Sensing: Geospatial Informatics and Motion Imagery Analytics VIII, Orlando, Florida, USA, 2018.
 

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

## Questions and Comments
For questions and comments about the dataset or the open source software, please contact pubgeo(at)jhuapl(dot)edu. 

## License
[Urban 3D Challenge Dataset License](https://github.com/SpaceNetChallenge/SpaceNetChallenge.github.io/tree/master/licenses/Urban3DChallenge_license.md)
