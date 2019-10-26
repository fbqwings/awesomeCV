# Multi-View Stereo Reconstruction
<h1> 

```diff
- Recent papers (from 2017)
```

</h1>

<h3> Keywords </h3>

__`Mon.`__: Monocular &emsp; 

Statistics: :fire: code is available & stars >= 100 &emsp;|&emsp; :star: citation >= 50

---
survey/overview/review

- 本文主要介绍基于image(单目标物体)的三维重建方法，可以看做indoor场景的子集。

  - [2019][Image-based 3D Object Reconstruction: State-of-the-Art and Trends in the Deep Learning Era](https://arxiv.org/pdf/1906.06543.pdf)


- Robust Vision Challenge

  - http://robustvision.net/index.php
---

## Stereo Matching

- [2018][CVPR][Learning for Disparity Estimation Through Feature Constancy(https://arxiv.org/pdf/1712.01039.pdf)

- stereo reconstruction is decomposed into three important steps: feature extraction (for matching cost
computation), matching cost aggregation and disparity prediction.本文主要介绍实现Stereo Matching。

  -[2019][GA-Net: Guided Aggregation Net for End-to-end Stereo Matching](https://arxiv.org/pdf/1904.06587.pdf)
---  
## Multi-View Stereo


- 传统multi-view stereo(MVS)利用空间几何基本原理，旨在利用多张影像(影像及对应的相机几何)恢复出三维场景。香港科技大学和深圳altizure团队提出的基于Deep learning的高精度高效率的三维重建网络，
包括特征提取，Depth map估计，三维点云生成网络。
  - 缺点：过于耗费内存，难以应用到大尺度场景的问题。
  - 在室内数据集和简单室外数据集效果尚可，相比。

  - [2018 ECCV][MVSNet: Depth Inference for Unstructured Multi-view Stereo](https://arxiv.org/pdf/1804.02505.pdf)

- MVSNet改进版。

  - [2019][CVPR][Recurrent MVSNet for High-resolution Multi-view Stereo Depth Inference](https://arxiv.org/pdf/1902.10556.pdf)

- 清华大学与香港科技大学提出，基于Point-MVSNet解决MVS问题。包括Coarse Depth Prediction Network，Coarse Depth Map Prediction,Refned Depth Map Predictions，
Coarse到refined修订。
  - 缺点：主要针对单目标重建，以及scan9这样简单数据集。

  - [2019][ICCV][Point-Based Multi-View Stereo Network](https://arxiv.org/pdf/1908.04422.pdf)[github](https://github.com/callmeray/PointMVSNet)
  

- Andrew教授项目组，基于单目视觉+语义分割的室内语义三维重建方法。

  -[2019][CVPR][SceneCode: Monocular Dense Semantic Reconstruction using Learned Encoded Scene Representations](https://zpascal.net/cvpr2019/Zhi_SceneCode_Monocular_Dense_Semantic_Reconstruction_Using_Learned_Encoded_Scene_Representations_CVPR_2019_paper.pdf)
  

# Dataset

- Stereo benchmark: ETH3D
Aanæs, H., Jensen, R.R., Vogiatzis, G., Tola, E., Dahl, A.B.: Large-scale data for
multiple-view stereopsis. International Journal of Computer Vision (IJCV) (2016)

Knapitsch, A., Park, J., Zhou, Q.Y., Koltun, V.: Tanks and temples: Benchmarking
large-scale scene reconstruction. ACM Transactions on Graphics (TOG) (2017)

  - [2017][CVPR][A Multi-View Stereo Benchmark with High-Resolution Images and Multi-Camera Videos](http://www.cvlibs.net/publications/Schoeps2017CVPR.pdf)
  
  
#待记录

 PoseNet，VINet，Perspective Transformer Net，SfMNet，CNN-SLAM，SurfaceNet，3D-R2N2，MVSNet