## 天池医疗AI大赛[第一季]：肺部结节智能诊断
## Pulmonary Nodules AI Diagnosis

### DSB3Tutorial 
> ### mask_segment folder

This code is the companion for the tutorial located at https://www.kaggle.com/c/data-science-bowl-2017#tutorial

### About this repository

This repository is not intended to be an out of the box solution for the DSB challenge. It will not run out-of-the-box
without editing. That was not it's intention. The tutorial was put together rapidly by several people working in tandem
and the code herein is a collection of the code they used to produce the tutorial found on the DSB website. 

The intent behind this tutorial was to presented a series of steps that can be followed as a starting point for competitors. 
Our hope is that this can save competitors time in framing the problem and that they can lift some of this code to speed 
up their own solution generation. We expect that the competitors efforst will supercede this tutorial in short order--which
is, of course, the point of the competition. 

Thanks for participating and helping to advance cancer diagnosis!

### evaluation script 
> ### mask_segment/evaluationScript folder

### Additional data

Optional data could be downloaded from the following links.

> ##### evaluation script: the LUNA16 evaluation script can be found here. The script could be used to locally evaluate the system for development purposes. More info is available here. [updated: 17th June 2016]
> ##### lung segmentation: a drive folder containing the lung segmentation can be found here. [updated: 28th April 2016]
> ##### additional_annotations.csv: the file will be available soon.

### TianChiMedical_AI 天池医疗AI挑战赛 
> ### preprocessing folder
  
这个工程用于托管我分享帖中涉及的代码，有部分病人的文件作为示例。

### 0. 文件说明
##### csv_files
> 存放了那几个csv文件  

##### nodule_cubes
> npy里存放的是提取出来的nodule_cubes  

##### slices_masks
> 存放的是根据annotations.csv文件生成的slices和对应的GroundTruth，可用于训练2D-Unet

### 生成图片来观察分割是否有问题:
##### ![Index Page](https://github.com/JenifferWuUCLA/pulmonary_nodules_AI_diagnosis/blob/master/preprocessing/slices_masks_1/jpg/0004_0908_0380_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.jpg)
##### (1.a) 0004_0908_0380_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.mhd的肺部区域图像

##### ![Index Page](https://github.com/JenifferWuUCLA/pulmonary_nodules_AI_diagnosis/blob/master/preprocessing/slices_masks_1/jpg/0004_0908_0380_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679_o.jpg)
##### (1.b) 0004_0908_0380_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.mhd的结节区域图像

##### ![Index Page](https://github.com/JenifferWuUCLA/pulmonary_nodules_AI_diagnosis/blob/master/preprocessing/slices_masks_1/jpg/0004_0909_0305_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.jpg)
##### (2.a) 0004_0909_0305_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.mhd的肺部区域图像

##### ![Index Page](https://github.com/JenifferWuUCLA/pulmonary_nodules_AI_diagnosis/blob/master/preprocessing/slices_masks_1/jpg/0004_0909_0305_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679_o.jpg)
##### (2.b) 0004_0909_0305_1.3.6.1.4.1.14519.5.2.1.6279.6001.325164338773720548739146851679.mhd的结节区域图像