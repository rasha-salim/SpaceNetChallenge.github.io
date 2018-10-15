---
layout: datasets
title: IARPA CORE3D Public Data
sidebar: datasets
---

# [IARPA CORE3D Public Data](https://www.iarpa.gov/index.php/research-programs/core3d)

IARPA has publicly released DigitalGlobe satellite imagery for the Creation of Operationally Realistic 3D Environment (CORE3D) program to enable performer teams to crowdsource manual labeling efforts and to promote public research that aligns well with the CORE3D program’s objectives.

SpaceNet is hosting the CORE3D public dataset in the SpaceNet repository to ensure easy access to the data.

## Reference Requirement

Please reference the following when reporting results using any of this data:

* M. Brown, H. Goldberg, K. Foster, A. Leichtman, S. Wang, S. Hagstrom, M. Bosch, and S. Almes, “Large-Scale Public Lidar and Satellite Image Data Set for Urban Semantic Labeling,” in Proc. SPIE Laser Radar Technology and Applications XXII, 2018.

* Commercial satellite imagery in the CORE3D public dataset was provided courtesy of DigitalGlobe.

* Dataset was created for the IARPA CORE3D program: https://www.iarpa.gov/index.php/research-programs/core3d.

* SpaceNet on Amazon Web Services (AWS). “Datasets.” The SpaceNet Catalog. Last modified October 15, 2018. Accessed on [Insert Date]. https://spacenetchallenge.github.io/datasets/datasetHomePage.html.



## Catalog
```commandline
aws s3 ls s3://spacenet-dataset/Hosted-Datasets/CORE3D-Public-Data/

```

Catalog

aws s3 ls s3://spacenet-dataset/core3d_datasetß

* One WorldView-2 PAN and MSI image for Jacksonville, FL; Tampa, FL; Richmond, VA; and Omaha, NE

* Tiled WorldView-2 data sets including ground truth building labels for comparison with the USSOCOM Urban 3D Challenge

* 26 WorldView-3 PAN and MSI images over Jacksonville, FL

* 43 WorldView-3 PAN and MSI images over Omaha, NE

* 35 WorldView-3 PAN and MSI images over UCSD, CA

* 44 WorldView-2 PAN and MSI images over UCSD, CAß

* See the referenced SPIE paper for information about where to find corresponding lidar and other complementary data sets for each location

* For images over San Fernando, Argentina for the IARPA Multi-View Stereo 3D Mapping Challenge, see https://spacenetchallenge.github.io/datasets/mvs_summary.html

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'

## Questions and Comments
For questions and comments about the dataset or the open source software, please contact pubgeo(at)jhuapl(dot)edu. 



