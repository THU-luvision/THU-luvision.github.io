---
sort: 1
---

# INS-Conv: Incremental Sparse Convolution for Online 3D segmentation


Han Lei, Tian Zheng, Lan Xu, Lu Fang.<br/>**InProceedings of the IEEE/CVF conference on computer vision and pattern recognition.** 2020.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/INS-Conv)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://openaccess.thecvf.com/content/CVPR2022/papers/Liu_INS-Conv_Incremental_Sparse_Convolution_for_Online_3D_Segmentation_CVPR_2022_paper.pdf) &nbsp;&nbsp;&nbsp;
<!-- [![video](/pic/video.png){: width="50px" }](https://www.youtube.com/watch?v=co7y6LQ7Kqc) -->

## Introduction

This is the incremental sparse convolution (Ins-Conv) library implemented based on SparseConvNet and Live Semantic 3D Perception for Immersive Augmented Reality. The later describes a more efficient GPU implementation of the original submanifold sparse convolution. Our method supports incremental computing of sparse convolution, including SSC, convolution/deconvolution, BN, IO, and residual structure, etc.

{:refdef: style="text-align: center;"}
![Framework](/pic/insconv.png){: width="800" }
{: refdef}


## Citing

If you find our code useful, please kindly cite our paper:

```bibtex
@inproceedings{liu2022ins,
  title={INS-Conv: Incremental Sparse Convolution for Online 3D Segmentation},
  author={Liu, Leyao and Zheng, Tian and Lin, Yun-Jou and Ni, Kai and Fang, Lu},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={18975--18984},
  year={2022}
}
```

