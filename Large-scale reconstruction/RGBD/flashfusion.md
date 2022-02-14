# FlashFusion: An efficient dense 3D reconstruction that only relies on CPU computing.

Han Lei, Lu Fang.<br/>InRobotics: Science and Systems 2018 Jun.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/Flashfusion)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](http://www.roboticsproceedings.org/rss14/p06.pdf) &nbsp;&nbsp;&nbsp;
[![video](/pic/video.png){: width="50px" }](https://www.youtube.com/watch?v=wWpJJVycOos)

## Introduction

Aiming at the practical usage of dense 3D reconstruction on portable devices, we propose FlashFusion, a Fast
LArge-Scale High-resolution (sub-centimeter level) 3D reconstruction system without the use of GPU computing. It enables
globally-consistent localization through a robust yet fast global
bundle adjustment scheme, and realizes spatial hashing based
volumetric fusion running at 300Hz and rendering at 25Hz
via highly efficient valid chunk selection and mesh extraction
schemes. Extensive experiments on both real world and synthetic
datasets demonstrate that FlashFusion succeeds to enable realtime, globally consistent, high-resolution (5mm), and large-scale
dense 3D reconstruction using highly-constrained computation,
i.e., the CPU computing on portable device.

{:refdef: style="text-align: center;"}
![Framework](/pic/flashfusion_pipeline.png){: width="800" }
{: refdef}

## Citing

If you find our code useful, please kindly cite our paper:

```bibtex
@inproceedings{han2018flashfusion,
  title={FlashFusion: Real-time Globally Consistent Dense 3D Reconstruction using CPU Computing.},
  author={Han, Lei and Fang, Lu},
  booktitle={Robotics: Science and Systems},
  volume={1},
  number={6},
  pages={7},
  year={2018}
}
```

