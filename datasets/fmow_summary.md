---
layout: datasets
title: fMoW Dataset
sidebar: datasets
---

<div id="imagesMain">
  <img src="/assets/images/IARPA-FMoW-Logo-FNL_Large.png" style="height: 100%; width:1--%; margin-top 0px;">
</div>
# [The IARPA Functional Map of the World (fMoW) Challenge](https://www.iarpa.gov/challenges/fmow.html)


Intelligence analysts, policy makers, and first responders around the world rely on geospatial land use data to inform crucial decisions about global defense and humanitarian activities. Historically, analysts have manually identified and classified geospatial information by comparing and analyzing satellite images, but that process is time consuming and insufficient to support disaster response. The fMoW Challenge sought to foster breakthroughs in the automated analysis of overhead imagery by harnessing the collective power of the global data science and machine learning communities; empowering stakeholders to bolster their capabilities through computer vision automation.
The challenge published one of the largest publicly available satellite-image datasets to date, with more than one million points of interest from around the world. The dataset also contains other elements such as temporal views, multispectral imagery, and satellite-specific metadata that researchers can exploit to build novel algorithms capable of classifying facility, building, and land use.

SpaceNet is hosting the fMoW dataset in the spacenet repository to ensure easy access to the data.

## Related Websites
For more information about the IARPA competition, please visit the [fMoW Challenge website](https://www.iarpa.gov/challenges/fmow.html).

Additional information about obtaining the data, baseline algorithm, or visualization tools can be found on the [fMoW GitHub website](https://github.com/fmow).  


## Reference Requirement
Please reference the following when publishing results using this data:

1.  G. Christie, N. Fendley, J. Wilson, and R. Mukherjee. Functional Map of the World. In CVPR, 2018.

BibTeX:	
```
@inproceedings{fmow2018,
  title={Functional Map of the World},
  author={Christie, Gordon and Fendley, Neil and Wilson, James and Mukherjee, Ryan},
  booktitle={CVPR},
  year={2018}
}
```

Alternatively, this dataset may be referenced as, “IARPA’s Functional Map of the World Dataset.”
 
Please also cite SpaceNet as follows:

```
SpaceNet on Amazon Web Services (AWS). “Datasets.” The SpaceNet Catalog.  Last modified January 4, 2018.
Accessed on [Insert Date]. https://spacenetchallenge.github.io/datasets/datasetHomePage.html.
```

## Catalog
```commandline
aws s3 ls s3://spacenet-dataset/fmow/fmow-full 
aws s3 ls s3://spacenet-dataset/fmow/fmow-rgb 
```


# Software Code with regard to this dataset:

### Available solutions from contest winners:

* 1st place: [1st place](https://github.com/fMoW/first_place_solution)
* 2nd place: [2nd place](https://github.com/fMoW/second_place_solution)
* 3rd place: [3rd place](https://github.com/fMoW/third_place_solution)

* Baseline: [Baseline Solution](https://github.com/fMoW/baseline)


### Published Papers
Published results:

1.	R. Minetto, M.P. Segundo, and S. Sarkar. Hydra: an Ensemble of Convolutional Neural Networks for Geospatial Land Classification. In arXiv preprint arXiv:1802.03518, 2018.
2.	G. Christie, N. Fendley, J. Wilson, and R. Mukherjee. Functional Map of the World. In CVPR, 2018. In arXiv preprint arXiv: 1711.07846 2017
3.	M. Pritt, G. Chern. Satellite Image Classification with Deep Learning, 46th Annual IEEE Applied Imagery Pattern Recognition Workshop, Washington, D.C.
 

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

## License
[fMoW License](https://github.com/fMoW/dataset/blob/master/LICENSE)
