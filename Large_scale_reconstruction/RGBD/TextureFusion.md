# Real-Time Globally Consistent Dense 3D Reconstruction With Online Texturing

Lei Han , Siyuan Gu, Dawei Zhong, Lu Fang.<br/>**IEEE Transactions on Pattern Analysis and Machine Intelligence.** 2020 Sep 2.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/TextureFusion)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9184935) &nbsp;&nbsp;&nbsp;


## Introduction
High-quality reconstruction of 3D geometry and texture plays a vital role in providing immersive perception of the real world. Additionally, online computation enables the practical usage of 3D reconstruction for interaction. We present an RGBD-based globally-consistent dense 3D reconstruction approach, where high-quality (i.e., the spatial resolution of the RGB image) texture patches are mapped on high-resolution geometric models online. The whole pipeline uses merely the CPU computing of a portable device. For real-time geometric reconstruction with online texturing, we propose to solve the texture optimization problem with a simplified incremental MRF solver in the context of geometric reconstruction pipeline using sparse voxel sampling strategy. An efficient reference-based color adjustment scheme is also proposed to achieve consistent texture patch colors under inconsistentluminance situations. Quantitative and qualitative experiments demonstrate that our online scheme achieves a realistic visualization of the environment with more abundant details, while taking fairly compact memory consumption and much lower computational complexity than existing solutions.


{:refdef: style="text-align: center;"}
![Framework](/pic/texturefusion.png){: width="800" }
{: refdef}


## Citing

If you find our code useful, please kindly cite our paper:

```bibtex
@article{Dense3DReconstruction,
  author={Han, Lei and Gu, Siyuan and Zhong, Dawei and Quan, Shuxue and Fang, Lu},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
  title={Real-Time Globally Consistent Dense 3D Reconstruction With Online Texturing}, 
  year={2022},
  volume={44},
  number={3},
  pages={1519-1533},
  doi={10.1109/TPAMI.2020.3021023}}
```

