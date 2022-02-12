# SurfaceNet+: An End-to-end 3D Neural Network for Very Sparse Multi-View Stereopsis

By Mengqi Ji, Jinzhi Zhang, Qionghai Dai, Lu Fang* (\*) Corresponding author.
[[Arxiv]](https://arxiv.org/pdf/2005.12690.pdf)

<!-- 
<div align="center">
<img src="assets/images/teaser.png" width="100%" />
</div>
<br> -->


## [Github code](https://github.com/THU-luvision/SurfaceNetPlus)


## Introduction
This is the official code repository for SurfaceNet+, a volumetric method to handle the ‘incompleteness’ and the ‘inaccuracy’ problems induced by a very sparse MVS setup.

This is a project from LuVision SIGMA, Tsinghua University. Visit our website for more interesting works: http://www.luvision.net/

## License
This project is released under the [GPLv3 license](LICENSE). We only allow free use for academic use. For commercial use, please contact us to negotiate a different license by: `fanglu at tsinghua.edu.cn`

## Citing

If you find our code useful, please kindly cite our paper:

```bibtex
@ARTICLE {9099504,
author = {M. Ji and J. Zhang and Q. Dai and L. Fang},
journal = {IEEE Transactions on Pattern Analysis & Machine Intelligence},
title = {SurfaceNet+: An End-to-end 3D Neural Network for Very Sparse Multi-View Stereopsis},
year = {2021},
volume = {43},
number = {11},
issn = {1939-3539},
pages = {4078-4093},
keywords = {three-dimensional displays;cameras;surface reconstruction;two dimensional displays;solid modeling;geometry;image reconstruction},
doi = {10.1109/TPAMI.2020.2996798},
publisher = {IEEE Computer Society},
address = {Los Alamitos, CA, USA},
month = {nov}
}
```

## How to Run

### Installation

* Solving the environment for cuda 9.0, cudnn 7.0 and python 2.7. ``conda create -n myEnv python=2.7`` and ``conda activate myEnv``.
* Install pytorch and other dependencies by ``bash env.sh``

### Download
* The input data contains multiple images, camera position files and bounding box files. In this example, we form the file format as DTU dataset, which you can find the corresponding images, camera matrixes and bounding box in three files: 
images: ``./inputs/DTU_MVS/Rectified/scan9``, 
camera position: ``./inputs/DTU_MVS/SampleSet/MVS Data/Calibration/cal18``,
bounding box: ``./inputs/DTU_MVS/SampleSet/MVS Data/ObsMask``.

* Pretrained models: saved in ``./experiment/network``.



### Testing
* Run ``python -u multi_reconstruct.py`` for multi-scale reconstruction, you can find the reconstruction ply files in ``./experiment/output``
* The main parameters you need to value is the ``reconstruct.params`` in ``multi_reconstruct.py``. It is a dict contains multi-scale parameters

```
.                          
├── level0                 
│   ├── resol: resolution of the coarest level       
│   ├── use_superResol: True,      
│   ├── min_prob:  the minimum probability threshold      
│   ├── tau_list: tau value for post-processing              
│   ├── gamma_list:  gamma value for post-processing 
│   ├── tau_fg: tau value for refinement network   
│   ├── use_fg: bool value to decide whether to use refinement network
│   ├── enable_rayPooling: True 
│   ├── cube_D: cube size
│   └── batch_size: 10  
├── level1                 
│   ├── resol: resolution of the second level       
│   ├── use_superResol: True,      
│   └── ...
├── level2                 
│   ├── resol: resolution of the third level       
│   ├── use_superResol: True,      
│   └── ...  
└── ...            
             
```
* change the ``sparsity`` and ``density`` for sparse reconstruction. Here we set ``sparsity`` = 7 and ``density`` = 1
* Specify your input and output file root in ``./tools/Parameter.py``. This file also contains other file and model indicator parameters. 
* change the view selection rules by setting parameters of ``EmbeddingNet_3d_new_big`` in ``./nets/Surf.py``. Since view selection plays a vital rule in reconstruction, this network combine the automation selection as well as the rule based selection by changing the relative weight. 
* If you want to use your own dataset, first prepare the data followed by ``Download``. Then change the corresponding indicator file name in ``./tools/Parameter.py``. Finally, in ``./tools/Prepair.py`` change the corresponding loading rules.


