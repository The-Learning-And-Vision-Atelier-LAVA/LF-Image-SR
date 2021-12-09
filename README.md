### <img src="https://raw.github.com/YingqianWang/Awesome-LF-Image-SR/master/Fig/Thumbnail.jpg" width="1000">
#### With recent advances in camera manufacturing, light field (LF) imaging technology becomes increasingly popular and is commonly used in various applications such as mobile phones, biological microscope, VR/AR etc. Since both intensity and directions of light rays are recorded by LF cameras, the resolution of LF images can be enhanced by using these additional angular information. LF image super-resolution (SR), also known as LF spatial SR, aims at reconstructing high-resolution (HR) LF images from their low-resolution (LR) counterparts. In this repository, we present a collection of papers on LF image SR, together with their codes and repos. 
#### Note: This repository will be updated on a regular basis, so stay tuned~~🎉🎉🎉


## News & Updates:
* **2021.12.09: We have reorganized our repo to include more recent works.**

## Survey:

|    **Method Acronym**     |   **Publication** | **Official Repo** |
| :------------: |  :-----: | :-------: |
|                 |  The Light Field Camera: Extended Depth of Field, Aliasing, and Superresolution, [TPAMI, 2012](https://ieeexplore.ieee.org/abstract/document/5989827/).  | -- |
|                 |  Spatial and Angular Variational Super-Resolution of 4D Light Fields, [ECCV 2012](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2012/papers/7576/75760608.pdf).  | -- |
|                 |  Variational Light Field Analysis for Disparity Estimation and Super-Resolution, [TPAMI 2013](https://ieeexplore.ieee.org/document/6574844).   | -- |
| **LFCNN**       |  Learning a Deep Convolutional Network for Light-Field Image Super-Resolution, [ICCVW 2015](https://openaccess.thecvf.com/content_iccv_2015_workshops/w3/papers/Yoon_Learning_a_Deep_ICCV_2015_paper.pdf)<br> Light-Field Image Super-Resolution Using Convolutional Neural Network, [SPL 2017](https://ieeexplore.ieee.org/abstract/document/7856946/) | [youngjinYoon/SPL_LF_SR](https://github.com/youngjinYoon/SPL_LF_SR)  |
| **PCA_rr**      | Super Resolution of Light Field Images using Linear Subspace Projection of Patch-Volumes, [JSTSP 2017](https://hal.archives-ouvertes.fr/hal-01591488/file/lightfield_SR_v02.pdf) | -- | 
| **LFSR_Gul**    | Spatial and Angular Resolution Enhancement of Light Fields Using Convolutional Neural Networks, [TIP 2018](https://arxiv.org/pdf/1707.00815) | -- | 
| **GB** | Light Field Super-Resolution Via Graph-Based Regularization, [TIP 2018](https://arxiv.org/pdf/1701.02141) | [rossimattia/light-field-super-resolution](https://github.com/rossimattia/light-field-super-resolution)  |
| **LFNet** | LFNet: A Novel Bidirectional Recurrent Convolutional Neural Network for Light-Field Image Super-Resolution, [TIP 2018](https://ieeexplore.ieee.org/document/8356655) | [wylcasia/LFNet](https://github.com/wylcasia/LFNet)
| **LRP** | Light Field Super-Resolution using a Low-Rank Prior and Deep Convolutional Neural Networks, [TPAMI 2018](https://arxiv.org/pdf/1801.04314) | -- |
| **LFBM5D** | Light Field Super-Resolution via LFBM5D Sparse Coding, [ICIP 2018](https://v-sense.scss.tcd.ie/wp-content/uploads/2018/05/LFBM5D_SR.pdf) | [V-Sense/LFBM5D](https://github.com/V-Sense/LFBM5D/tree/SR) |
| **LF-DCNN** | Light-Field Image Superresolution Using a Combined Deep CNN Based on EPI， [SPL 2018](https://ieeexplore.ieee.org/document/8411485). | -- |
| **LFSSR-SAS**    | Light Field Spatial Super-Resolution Using Deep Efficient Spatial-Angular Separable Convolution, [TIP 2018](https://ieeexplore.ieee.org/document/8561240) | [jingjin25/LFSSR-SAS-PyTorch](https://github.com/jingjin25/LFSSR-SAS-PyTorch) |
| **EPGB** | Light Field Super-Resolution Using Edge-Preserved Graph-Based Regularization, [TMM 2019](https://ieeexplore.ieee.org/document/8861391).| -- |
| **LF-FusNet** | Light Field Super-Resolution By Jointly Exploiting Internal and External Similarities, [TCSVT 2019](https://ieeexplore.ieee.org/abstract/document/8733069). | [Joechann0831/LFSR-FusNet](https://github.com/Joechann0831/LFSR-FusNet) |
| --- | An Epipolar Volume Autoencoder with Adversarial Loss for Deep Light Field Super-Resolution, [CVPRW 2019](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Zhu_An_Epipolar_Volume_Autoencoder_With_Adversarial_Loss_for_Deep_Light_CVPRW_2019_paper.pdf)** | [MinchenZKN/LFSR](https://github.com/MinchenZKN/LFSR) |
| **resLF**      | Residual Networks for Light Field Image Super-Resolution, [CVPR 2019](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Residual_Networks_for_Light_Field_Image_Super-Resolution_CVPR_2019_paper.pdf) | [shuozh/resLF](https://github.com/shuozh/resLF)|
| **HDDRNet**     | High-Dimensional Dense Residual Convolutional Neural Network for Light Field Reconstruction, [TPAMI 2019](https://arxiv.org/pdf/1910.01426.pdf)| [monaen/LightFieldReconstruction](https://github.com/monaen/LightFieldReconstruction)
| **LF-InterNet** | Spatial-Angular Interaction for Light Field Image Super-Resolution, [ECCV 2020](https://arxiv.org/pdf/1912.07849.pdf) | [YingqianWang/LF-InterNet](https://github.com/YingqianWang/LF-InterNet) |
| **LF-ATO**  | Light field spatial super-resolution via deep combinatorial geometry embedding and structural consistency regularization, [CVPR 2020](https://openaccess.thecvf.com/content_CVPR_2020/papers/Jin_Light_Field_Spatial_Super-Resolution_via_Deep_Combinatorial_Geometry_Embedding_and_CVPR_2020_paper.pdf) | [jingjin25/LFSSR-ATO](https://github.com/jingjin25/LFSSR-ATO) |
| **LFDCSR**| Deep Selective Combinatorial Embedding and Consistency Regularization for Light Field Super-resolution, [arxiv 2020](https://arxiv.org/abs/2009.12537)** | -- |
| **LF-DFnet**    | Light field image super-resolution using deformable convolution, [TIP 2020](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9286855) | [YingqianWang/LF-DFnet](https://github.com/YingqianWang/LF-DFnet) |
| **LF-ZSSR** | Light Field Super-Resolution with Zero-Shot Learning, [CVPR 2021](https://openaccess.thecvf.com/content/CVPR2021/papers/Cheng_Light_Field_Super-Resolution_With_Zero-Shot_Learning_CVPR_2021_paper.pdf) | [Joechann0831/LFZSSR](https://github.com/Joechann0831/LFZSSR) |
| **LFSR-AFR** | Light Field Super-Resolution via Adaptive Feature Remixing, [TIP 2021](https://ieeexplore.ieee.org/document/9394760/). | [keunsoo-ko/LFSR-AFR](https://github.com/keunsoo-ko/LFSR-AFR) |
| **MEG-Net**     | End-to-End Light Field Spatial Super-Resolution Network Using Multiple Epipolar Geometry, [TIP 2021](https://ieeexplore.ieee.org/abstract/document/9465683). | [shuozh/MEG-Net](https://github.com/shuozh/MEG-Net) |



## Acknowledgement
**We would like to thank [Zhengyu Liang](https://github.com/ZhengyuLiang24) and [Zhen Cheng](https://github.com/Joechann0831) for the helpful discussions and insightful suggestions regarding this repository.**

## Contact
**Any question regarding this repo can be addressed to wangyingqian16@nudt.edu.cn.**

