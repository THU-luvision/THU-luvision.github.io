## SurRF: Unsupervised Multi-view Stereopsis by Learning Surface Radiance Field

Jinzhi Zhang\*, Mengqi Ji*, Guangyu Wang, Xue Zhiwei, Shengjin Wang, Lu Fang.<br/>**IEEE Transactions on Pattern Analysis and Machine Intelligence.** 2021 Sep 30.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/SurRF)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://ieeexplore.ieee.org/document/9555381) &nbsp;&nbsp;&nbsp;



## Introduction
In this paper, we propose SurRF, an unsupervised MVS pipeline by learning Surface Radiance Field, i.e., a radiance field defined on a
continuous and explicit 2D surface. Our key insight is that, in a local region, the explicit surface can be gradually deformed from a continuous initialization along view-dependent camera rays by differentiable rendering. That enables us to define the radiance field only on a 2D deformable surface rather than in a dense volume of 3D space, leading to compact representation while maintaining complete shape and realistic texture for large-scale complex scenes. We experimentally demonstrate that the proposed SurRF produces competitive results over the-state-of-the-art on various real-world challenging scenes, without any 3D supervision. Moreover, SurRF shows great potential in owning the joint advantages of mesh (scene manipulation), continuous surface (high geometric resolution), and radiance field (realistic rendering).

{:refdef: style="text-align: center;"}
![Framework](/pic/surf.png){: width="800" }
{: refdef}



## Citation

If you find this project useful for your research, please cite:

```
@ARTICLE{9555381,
  author={Zhang, Jinzhi and Ji, Mengqi and Wang, Guangyu and Zhiwei, Xue and Wang, Shengjin and Fang, Lu},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
  title={SurRF: Unsupervised Multi-view Stereopsis by Learning Surface Radiance Field}, 
  year={2021},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/TPAMI.2021.3116695}}
```



