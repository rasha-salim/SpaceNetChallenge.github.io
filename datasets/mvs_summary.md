---
layout: datasets
title: MVS Dataset
sidebar: datasets
---

<div id="imagesMain">
  <img src="/assets/images/MVS_Logo.png" style="height: 100%; width:1--%; margin-top 0px;">
</div>
# [IARPA Multi-View Stereo 3D Mapping Challenge](https://www.iarpa.gov/challenges/3dchallenge.html)


The availability of public multiple view stereo (MVS) benchmark datasets has been instrumental in enabling research to advance the state of the art in the field and to apply and customize methods to real-world problems. In this work, we provide a public benchmark data set for multiple view stereo applied to 3D outdoor scene mapping using commercial satellite imagery.

This data set includes DigitalGlobe WorldView-3 panchromatic and multispectral images of a 100 square kilometer area near San Fernando, Argentina. We also provide 20cm airborne lidar ground truth data for a 20 square kilometer subset of this area and performance analysis software to assess accuracy and completeness metrics. Commercial satellite imagery is provided courtesy of DigitalGlobe, and ground truth lidar is provided courtesy of IARPA.

This data supported the IARPA Multi-View Stereo 3D Mapping Challenge and is now made publicly available with no restrictions to support continued research. JHU/APL does not plan to maintain an online benchmark leaderboard, but we welcome your feedback and would love to hear about what you’re doing with the data and include your published results on this page.

SpaceNet is hosting the Multi-View Stereo 3D Mapping dataset in the spacenet repository to ensure easy access to the data.

## Competition Websites
For more information about the IARPA Competition, Please visit the [Multi-View Stereo 3D Mapping Challenge Website](https://www.iarpa.gov/challenges/3dchallenge.html)

For more information about the MVS benchmark please visit the [JHUAPL competition webpage](http://www.jhuapl.edu/satellite-benchmark.html)

## Please reference the following when reporting results using any of this data:

* M. Bosch, A. Leichtman, D. Chilcott, H. Goldberg, M. Brown. [“Metric Evaluation Pipeline for 3D Modeling of Urban Scenes”](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLII-1-W1/239/2017/isprs-archives-XLII-1-W1-239-2017.pdf), ISPRS Archives, 2017.
* M. Bosch, Z. Kurtz, S. Hagstrom, and M. Brown. “A multiple view stereo benchmark for satellite imagery”. In Proceedings of the Applied Imagery Pattern Recognition Workshop (AIPR), Washington, DC, USA, 2016
* Commercial satellite imagery in the MVS benchmark data set was provided courtesy of DigitalGlobe.
* Dataset was created for the IAPRA Multi-View Stereo 3D Mapping Challenge
* Data hosted through the [The SpaceNet Data Repository](https://spacenetchallenge.github.io/)

## Catalog
```commandline
aws s3 ls s3://spacenet-dataset/mvs_dataset --request-payer requester

```
The catalog contains the following packages:

* Updated metric analysis software with examples from contest winners
* Challenge data package with instructions, cropped TIFF images, ground truth, image cropping software, and metric scoring software (1.2 GB)
* JHU/APL example MVS solution (451 MB)
* NITF panchromatic, multispectral, and short-wave infrared DigitalGlobe WorldView-3 satellite images (72.1 GB)
* LAZ lidar point clouds with SBET (2.2 GB)
* Spectral image calibration software (84 MB)

# Software Code with regard to this dataset:

### Available solutions from contest winners:

* 1st place: [https://github.com/MISS3D/s2p](https://github.com/MISS3D/s2p)
* 2nd place: [https://github.com/FakePsyho/mvs](https://github.com/FakePsyho/mvs)
* 3rd place: [https://github.com/sdrdis/iarpa](https://github.com/sdrdis/iarpa)
* 4th place: [http://u.osu.edu/qin.324/rsp/](http://u.osu.edu/qin.324/rsp/)

### Published Papers
Published results:

1.  G. Facciolo, C. de Franchis, E. Meinhardt-Llopis, “Automatic 3D Reconstruction from Multi-Date Satellite Images,” IEEE International Conference on Computer Vision and Pattern Recognition, EARTHVISION Workshop, 2017.

2.  R. Qin, “Automated 3D recovery from very high resolution multi-view images,” ASPRS 2017 Annual Conference, 2017.

## Dependencies
The [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/) must be installed with an active AWS account. Configure the AWS CLI using 'aws configure'


