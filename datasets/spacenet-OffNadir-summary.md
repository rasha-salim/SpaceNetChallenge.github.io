---
layout: datasets
title: "SpaceNet Off-Nadir Dataset"
sidebar: datasets
---
## The SpaceNet Off-Nadir Dataset


## The Problem
Can you help us automate mapping from off-nadir imagery? In this challenge, competitors are tasked with finding automated methods for extracting map-ready building footprints from high-resolution satellite imagery from high off-nadir imagery. In many disaster scenarios the first post-event imagery is from a more off-nadir image than is used in standard mapping use cases.  The ability to use higher off-nadir imagery will allow for more flexibility in acquiring and using satellite imagery after a disaster.  Moving towards more accurate fully automated extraction of building footprints  will help bring innovation to computer vision methodologies applied to high-resolution satellite imagery, and ultimately help create better maps where they are needed most.
 
Your task will be to extract building footprints from increasingly off-nadir satellite images. The polygon’s you create will be compared to ground truth, and the quality of the solutions will be measured using the SpaceNet metric.   


## The Data - Over 120,000 Building footprints over 665 sqkm of Atlanta, GA with 27 associated WV-2 images.
This dataset contains 27 8-Band WorldView-2 images taken over Atlanta, GA on December 22nd, 2009.  They range in off-nadir angle from 7 degrees to 54 degrees.  

For the competition, the 27 images are broken into 3 segments based on their off-nadir angle:
* Nadir: 0-25 degrees 
* Off-nadir: 26 degrees - 40 degrees
* Very Off-nadir 40-55 degrees

The entire set of images was then tiled into 450m x 450m tiles. 



See the [labeling guide and schema](/Labeling_Schema/SpaceNetBuildings_labeling_rules_v1.html) for details about the creation of the dataset


<style type="text/css">
	table.tableizer-table {
		font-size: 12px;
		border: 1px solid #CCC; 
		font-family: Arial, Helvetica, sans-serif;
	} 
	.tableizer-table td {
		padding: 4px;
		margin: 3px;
		border: 1px solid #CCC;
	}
	.tableizer-table th {
		background-color: #104E8B; 
		color: #FFF;
		font-weight: bold;
	}
</style>
<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th></th><th>Catalog ID</th><th>Pan Resolution</th><th>Off Nadir Angle</th><th>Target Azimuth</th><th>Catgory</th></tr></thead><tbody>
 <tr><td>1</td><td>1030010003D22F00</td><td>0.48</td><td>7.8</td><td>118.4</td><td>Nadir</td></tr>
 <tr><td>2</td><td>10300100023BC100</td><td>0.49</td><td>8.3</td><td>78.4</td><td>Nadir</td></tr>
 <tr><td>3</td><td>1030010003993</td><td>0.49</td><td>10.5</td><td>148.6</td><td>Nadir</td></tr>
 <tr><td>4</td><td>1030010003CAF100</td><td>0.48</td><td>10.6</td><td>57.6</td><td>Nadir</td></tr>
 <tr><td>5</td><td>1030010002B7D800</td><td>0.49</td><td>13.9</td><td>162</td><td>Nadir</td></tr>
 <tr><td>6</td><td>10300100039AB000</td><td>0.49</td><td>14.8</td><td>43</td><td>Nadir</td></tr>
 <tr><td>7</td><td>1030010002649200</td><td>0.52</td><td>16.9</td><td>168.7</td><td>Nadir</td></tr>
 <tr><td>8</td><td>1030010003C92000</td><td>0.52</td><td>19.3</td><td>35.1</td><td>Nadir</td></tr>
 <tr><td>9</td><td>1030010003127500</td><td>0.54</td><td>21.3</td><td>174.7</td><td>Nadir</td></tr>
 <tr><td>10</td><td>103001000352C200</td><td>0.54</td><td>23.5</td><td>30.7</td><td>Nadir</td></tr>
 <tr><td>11</td><td>103001000307D800</td><td>0.57</td><td>25.4</td><td>178.4</td><td>Nadir</td></tr>
 <tr><td>12</td><td>1030010003472200</td><td>0.58</td><td>27.4</td><td>27.7</td><td>Off-Nadir</td></tr>
 <tr><td>13</td><td>1030010003315300</td><td>0.61</td><td>29.1</td><td>181</td><td>Off-Nadir</td></tr>
 <tr><td>14</td><td>10300100036D5200</td><td>0.62</td><td>31</td><td>25.5</td><td>Off-Nadir</td></tr>
 <tr><td>15</td><td>103001000392F600</td><td>0.65</td><td>32.5</td><td>182.8</td><td>Off-Nadir</td></tr>
 <tr><td>16</td><td>1030010003697400</td><td>0.68</td><td>34</td><td>23.8</td><td>Off-Nadir</td></tr>
 <tr><td>17</td><td>1030010003895500</td><td>0.74</td><td>37</td><td>22.6</td><td>Off-Nadir</td></tr>
 <tr><td>18</td><td>1030010003832800</td><td>0.8</td><td>39.6</td><td>21.5</td><td>Off-Nadir</td></tr>
 <tr><td>19</td><td>10300100035D1B00</td><td>0.87</td><td>42</td><td>20.7</td><td>Very Off-Nadir</td></tr>
 <tr><td>20</td><td>1030010003CCD700</td><td>0.95</td><td>44.2</td><td>20</td><td>Very Off-Nadir</td></tr>
 <tr><td>21</td><td>1030010003713C00</td><td>1.03</td><td>46.1</td><td>19.5</td><td>Very Off-Nadir</td></tr>
 <tr><td>22</td><td>10300100033C5200</td><td>1.13</td><td>47.8</td><td>19</td><td>Very Off-Nadir</td></tr>
 <tr><td>23</td><td>1030010003492700</td><td>1.23</td><td>49.3</td><td>18.5</td><td>Very Off-Nadir</td></tr>
 <tr><td>24</td><td>10300100039E6200</td><td>1.36</td><td>50.9</td><td>18</td><td>Very Off-Nadir</td></tr>
 <tr><td>25</td><td>1030010003BDDC00</td><td>1.48</td><td>52.2</td><td>17.7</td><td>Very Off-Nadir</td></tr>
 <tr><td>26</td><td>1030010003CD4300</td><td>1.63</td><td>53.4</td><td>17.4</td><td>Very Off-Nadir</td></tr>
 <tr><td>27</td><td>1030010003193D00</td><td>1.67</td><td>54</td><td>17.4</td><td>Very Off-Nadir</td></tr>
</tbody></table>


## Catalog
The data is hosted on AWS as Public Dataset.  An AWS account is required.   
```commandline
aws s3 ls s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/

```

## Sample Data
### 2 Samples from each Off-Nadir Image - Off-Nadir Imagery Samples
To download processed 450mx450m tiles of AOI_6_Atlanta (728.8 MB) with associated building footprints:
```
aws s3 cp s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/SpaceNet_Off-Nadir_Competition_Sample.tar.gz .
```


## Training Data

## SpaceNet Off-Nadir Training Base Directory:

```bash
aws s3 ls s3://spacenet-dataset/SpaceNet_Off-Nadir_Dataset/SpaceNet-Off-Nadir_Train/
```
### SpaceNet Off-Nadir Building Footprint Extraction Training Data Labels (15 mb)
```
aws s3 cp s3://spacenet-dataset/SpaceNet_Off-Nadir_Dataset/SpaceNet-Off-Nadir_Train/geojson.tar.gz .
```

### SpaceNet Off-Nadir Building Footprint Extraction Training Data Imagery (186 GB)
To download processed 450mx450m tiles of AOI 6 Atlanta.  

Each of the 27 Collects forms a separate .tar.gz labeled "Atlanta_nadir{nadir-angle}_catid\_{catid}.tar.gz".  Each .tar.gz is ~7 GB

```bash
aws s3 cp s3://spacenet-dataset/SpaceNet_Off-Nadir_Dataset/SpaceNet-Off-Nadir_Train/ . --exclude "*geojson.tar.gz" --recursive
```

## Test Data
### AOI 6 Atlanta -  Building Footprint Extraction Testing Data
To download processed 450mx450m tiles of AOI 6 Atlanta (5.8 GB):
```
aws s3 cp  s3://spacenet-dataset/SpaceNet_Off-Nadir_Competition/SpaceNet-Off-Nadir_Test_Public.tar.gz .
```

# The Metric
In the SpaceNet Off-Nadir Building Extraction Challenge, the metric for ranking entries is the [SpaceNet Metric](https://medium.com/the-downlinq/the-spacenet-metric-612183cc2ddb).  
This metric is an F1-Score based on the intersection over union of two building footprints with a threshold of 0.5

F1-Score is calculated by taking the total True Positives, False Positives, and False Negatives for each nadir segement and then averaging the F1-Score for each segement.  

F1-Score Total = mean(F1-Score-Nadir, F1-Score-Off-Nadir, F1-Score-Very-Off-Nadir)


# Competition Updates:

For information about the currently running challenge visit the [competition site on topcoder.](https://topcoder.com/spacenet)

For more details about previous SpaceNet Building Challenges [SpaceNet Building Extraction Challenge: Round 2](/Challenges/Competition2.html)  visit it's [website](/Challenges/Competition2.html)  

Check out CosmiQ Work's Blog, [The DownLinQ](https://medium.com/the-downlinq)
or follow the [SpaceNetUtilities Github Page](https://github.com/SpaceNetChallenge/utilities)



## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">The SpaceNet Dataset</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://spacenetchallenge.github.io/" property="cc:attributionName" rel="cc:attributionURL">SpaceNet Partners</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
