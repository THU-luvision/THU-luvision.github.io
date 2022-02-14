# OccuSeg: Occupancy-aware 3D Instance Segmentation


Han Lei, Tian Zheng, Lan Xu, Lu Fang.<br/>InProceedings of the IEEE/CVF conference on computer vision and pattern recognition 2020.

[![github](/pic/github3.png){: width="50px" }](https://github.com/THU-luvision/OccuSeg)  &nbsp;&nbsp;&nbsp;
[![pdf](/pic/pdf.jpeg){: width="50px" }](https://openaccess.thecvf.com/content_CVPR_2020/papers/Han_OccuSeg_Occupancy-Aware_3D_Instance_Segmentation_CVPR_2020_paper.pdf) &nbsp;&nbsp;&nbsp;
[![video](/pic/video.png){: width="50px" }](https://www.youtube.com/watch?v=co7y6LQ7Kqc)

## Introduction

OccuSeg, an occupancy-aware 3D instance segmentation scheme is proposed. Our multi-task learning produces both occupancy signal and embedding representations, where the training of spatial and feature embedding varies with their difference in scale-aware. Our clustering scheme benefits from the reliable comparison between the predicted occupancy size and the clustered occupancy size, which encourages hard samples being correctly clustered and avoids over segmentation. The proposed approach achieves state-of-the-art performance on 3 real-world datasets, i.e. ScanNetV2, S3DIS and SceneNN, while maintaining high efficiency.

{:refdef: style="text-align: center;"}
![Framework](/pic/occseg.png){: width="800" }
{: refdef}


## Citing

If you find our code useful, please kindly cite our paper:

```bibtex
@INPROCEEDINGS{9157103,
  author={Han, Lei and Zheng, Tian and Xu, Lan and Fang, Lu},
  booktitle={2020 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)}, 
  title={OccuSeg: Occupancy-Aware 3D Instance Segmentation}, 
  year={2020},
  volume={},
  number={},
  pages={2937-2946},
  doi={10.1109/CVPR42600.2020.00301}}
}
```

