## CrossNet++: Cross-Scale Large-Parallax Warping for Reference-Based Super-Resolution

Yang Tan, Haitian Zheng, Yinheng Zhu, Xiaoyun Yuan, Xing Lin, David Brady, Lu Fang.<br/>**IEEE Transactions on Pattern Analysis and Machine Intelligence.** 2020 May 25.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/CrossNetPP)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://ieeexplore.ieee.org/document/9099445) &nbsp;&nbsp;&nbsp;



## Introduction
The ability of camera arrays to efficiently capture higher space-bandwidth product than single cameras has led to various multiscale and hybrid systems. These systems play vital roles in computational photography, including light field imaging, 360 VR camera, gigapixel videography, etc. One of the critical tasks in multiscale hybrid imaging is matching and fusing cross-resolution images from different cameras under perspective parallax. CrossNet++ is an end-to-end network containing novel two-stage cross-scale warping modules, image encoder and fusion decoder. The stage I learns to narrow down the parallax distinctively with the strong guidance of landmarks and intensity distribution consensus. Then the stage II operates more fine-grained alignment and aggregation in feature domain to synthesize the final super-resolved image. To further address the large parallax, new hybrid loss functions comprising warping loss, landmark loss and super-resolution loss are proposed to regularize training and enable better convergence. CrossNet++ significantly outperforms the state-of-art on light field datasets as well as real dual-camera data.

This repo contains the implementation of the 'CrossNet++: Cross-Scale Large-Parallax Warping for Reference-Based Super-Resolution'. The improvements include multistage warping, keypoint guidence as well as extend real-world training set using hikvision dual camera.

{:refdef: style="text-align: center;"}
![Framework](/pic/crossnetpp.png){: width="800" }
{: refdef}



## Citation

If you find this project useful for your research, please cite:

```
@ARTICLE{9099445,
  author={Tan, Yang and Zheng, Haitian and Zhu, Yinheng and Yuan, Xiaoyun and Lin, Xing and Brady, David and Fang, Lu},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
  title={CrossNet++: Cross-Scale Large-Parallax Warping for Reference-Based Super-Resolution}, 
  year={2021},
  volume={43},
  number={12},
  pages={4291-4305},
  doi={10.1109/TPAMI.2020.2997007}}
```



