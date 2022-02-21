## SurfaceNet: An End-to-end 3D Neural Network for Multiview Stereopsis

Mengqi Ji, Juergen Gall, Haitian Zheng, Yebin Liu, Lu Fang.<br/>**IEEE International Conference on Computer Vision.** 2017 Aug 5.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/SurfaceNet)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://arxiv.org/abs/1708.01749) &nbsp;&nbsp;&nbsp;

## Introduction
SurfaceNet is an end-to-end learning framework for multiview stereopsis. It takes a set of images and their corresponding camera parameters as input and directly infers the 3D model. The key
advantage of the framework is that both photo-consistency as well as geometric relations of the surface structure can be directly learned for the purpose of multiview stereopsis in an end-to-end fashion. SurfaceNet is a fully 3D convolutional network which is achieved by encoding the camera parameters together with the images in a 3D voxel representation. 

{:refdef: style="text-align: center;"}
![Framework](/pic/surfacenet_method.png){: width="800" }
![Framework](/pic/surfacenet_experiment.png){: width="800" }
{: refdef}


## Citation

If you find this project useful for your research, please cite:

```
@inproceedings{ji2017surfacenet,
  title={SurfaceNet: An End-To-End 3D Neural Network for Multiview Stereopsis},
  author={Ji, Mengqi and Gall, Juergen and Zheng, Haitian and Liu, Yebin and Fang, Lu},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision (ICCV)},
  pages={2307--2315},
  year={2017}
}
```



