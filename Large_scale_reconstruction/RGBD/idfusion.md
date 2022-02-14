# iDFusion: Globally Consistent Dense 3D Reconstruction from RGB-D and Inertial Measurements.

Dawei Zhong\*, Lei Han\*, Lu Fang.<br/>**InProceedings of the 27th ACM International Conference on Multimedia.** 2019 Oct 15.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/iDFusion)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://dl.acm.org/doi/abs/10.1145/3343031.3351085) &nbsp;&nbsp;&nbsp;
[![video](/pic/video.png){: width="50px" }](https://www.youtube.com/watch?v=tGhJRjxWJ4A)


## Introduction
We present a practical (fast, globally consistent and robust) dense 3D reconstruction system, iDFusion, by exploring the joint benefit of both the visual (RGB-D) solution and inertial measurement unit (IMU). A lobal optimization considering all the previous states is adopted to maintain high localization accuracy and global consistency, yet its complexity of being linear to the number of all previous camera/IMU observations seriously impedes real-time implementation. We show that the global optimization can be solved efficiently at the complexity linear to the number of keyframes, and further realize a real-time dense 3D reconstruction system given the estimated camera states.

![github](/pic/idfusion.png){: width="800px" }


## Citing
If you find our code useful, please kindly cite our paper:
```bibtex
@inproceedings{zhong2019idfusion,
  title={iDFusion: Globally Consistent Dense 3D Reconstruction from RGB-D and Inertial Measurements},
  author={Zhong, Dawei and Han, Lei and Fang, Lu},
  booktitle={Proceedings of the 27th ACM International Conference on Multimedia},
  pages={962--970},
  year={2019}
}

```
