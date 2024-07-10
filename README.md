## [ECCV 2024] Decomposition Betters Tracking Everything Everywhere

[![LICENSE](https://img.shields.io/github/license/qianduoduolr/DecoMotion)](https://github.com/qianduoduolr/DecoMotion/blob/base/LICENSE)

[Rui Li](https://qianduoduolr.github.io/)<sup>1</sup>, [Dong Liu](https://faculty.ustc.edu.cn/dongeliu/en/index/85593/list/index.htm)<sup>1</sup>

<sup>1</sup>University of Science and Technology of China, Hefei, China

#### [[Paper](https://arxiv.org/pdf/2407.06531)] /  [[Demo](https://youtu.be)] / [[Project page](https://github.com/qianduoduolr/DecoMotion)] 

This is the official code for  "**Decomposition Betters Tracking Everything Everywhere**". 



## :star: News
- *2024.07.04:*  Our paper "Decomposition Betters Tracking Everything Everywhere" is accepted to ECCV 2024. Code and models will be released as soon as possible.


## Overview
<!-- ![](figure/framework.png) -->

<div  align="center">    
<img src="figure/framework.png"  height="380px"/> 
</div>
   
Recent studies on motion estimation have advocated an optimized motion representation that is globally consistent across the entire video, preferably for every pixel. This is challenging as a uniform representation may not account for the complex and diverse motion and appearance of natural videos. We address this problem and propose a new test-time optimization method, named DecoMotion, for estimating per-pixel and long-range motion. DecoMotion explicitly decomposes video content into static scenes and dynamic objects, either of which uses a quasi-3D canonical volume to represent. DecoMotion separately coordinates the transformations between local and canonical spaces, facilitating an affine transformation for the static scene that corresponds to camera motion. For the dynamic volume, DecoMotion leverages discriminative and temporally consistent features to rectify the non-rigid transformation. The two volumes are finally fused to fully represent motion and appearance. This divide-and-conquer strategy leads to more robust tracking through occlusions and deformations and meanwhile obtains decomposed appearances. We conduct evaluations on the TAP-Vid benchmark. The results demonstrate our method boosts the point-tracking accuracy by a large margin and performs on par with some state-of-the-art dedicated point-tracking solutions. 