### <img src="https://raw.github.com/YingqianWang/Awesome-LF-Image-SR/master/Fig/Thumbnail.jpg" width="1000">
#### With recent advances in camera manufacturing, light field (LF) imaging technology becomes increasingly popular and is commonly used in various applications such as mobile phones, biological microscope, VR/AR etc. Since both intensity and directions of light rays are recorded by LF cameras, the resolution of LF images can be enhanced by using these additional angular information. LF image super-resolution (SR), also known as LF spatial SR, aims at reconstructing high-resolution (HR) LF images from their low-resolution (LR) counterparts. In this repository, we present a collection of papers on LF image SR, together with their codes and repos. <br>
#### Note: This repository will be updated on a regular basis, so stay tuned~~🎉🎉🎉
<br>

## News: 
**We recommend our newly-released repository [BasicLFSR](https://github.com/ZhengyuLiang24/BasicLFSR), which is an open-source and easy-to-use toolbox for LF image SR. Both this repo and [BasicLFSR](https://github.com/ZhengyuLiang24/BasicLFSR) are developed to make the communities better get access to this area and re-impolement existing methods.

## Updates:
* **2021.12.09: New version is online, more recent methods such as DDAN, LF-IINet and LFT are included.**<br><br><br>

## Methods from 2012 to 2022:
<br>

|    **Acronym**     |   **Publication** | **Official Repo** |
| :-----------------------: |  :-----: | :-------: |
|                 |  The light field camera: extended depth of field, aliasing, and superresolution, [TPAMI, 2012](https://ieeexplore.ieee.org/abstract/document/5989827/).  | -- |
|      --         |  Spatial and angular vriational super-resolution of 4D light fields, [ECCV 2012](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2012/papers/7576/75760608.pdf).  | -- |
|      --         |  Variational light field analysis for disparity estimation and super-resolution, [TPAMI 2013](https://ieeexplore.ieee.org/document/6574844).   | -- |
| **LFCNN**       |  Learning a deep convolutional network for light-field image super-resolution, [ICCVW 2015](https://openaccess.thecvf.com/content_iccv_2015_workshops/w3/papers/Yoon_Learning_a_Deep_ICCV_2015_paper.pdf); Light field image super-resolution using convolutional neural network, [SPL 2017](https://ieeexplore.ieee.org/abstract/document/7856946/) | [youngjinYoon/<br/>SPL_LF_SR](https://github.com/youngjinYoon/<br>SPL_LF_SR)  |
| **PCA_rr**      | Super resolution of light field images using linear subspace projection of patch-volumes, [JSTSP 2017](https://hal.archives-ouvertes.fr/hal-01591488/file/lightfield_SR_v02.pdf) | -- | 
| **LFSR_Gul**  | Spatial and angular resolution enhancement of light fields using convolutional neural networks, [TIP 2018](https://arxiv.org/pdf/1707.00815) | -- | 
| **GB** | Light field super-resolution via graph-based regularization, [TIP 2018](https://arxiv.org/pdf/1701.02141) | [rossimattia/<br/>light-field-super-resolution](https://github.com/rossimattia/light-field-super-resolution)  |
| **LFNet** | LFNet: A Novel Bidirectional Recurrent Convolutional Neural Network for Light-Field Image Super-Resolution, [TIP 2018](https://ieeexplore.ieee.org/document/8356655) | [wylcasia/LFNet](https://github.com/wylcasia/LFNet)
| **LRP** | Light field super-resolution using a low-rank prior and deep convolutional neural networks, [TPAMI 2018](https://arxiv.org/pdf/1801.04314) | -- |
| **LFBM5D** | Light field super-resolution via LFBM5D sparse coding, [ICIP 2018](https://v-sense.scss.tcd.ie/wp-content/uploads/2018/05/LFBM5D_SR.pdf) | [V-Sense/<br/>LFBM5D](https://github.com/V-Sense/LFBM5D/tree/SR) |
| **LF-DCNN** | Light-field image superresolution using a combined deep CNN based on EPI， [SPL 2018](https://ieeexplore.ieee.org/document/8411485). | -- |
| **LFSSR-SAS**    | Light field spatial super-resolution using deep efficient spatial-angular separable convolution, [TIP 2018](https://ieeexplore.ieee.org/document/8561240) | [jingjin25/<br/>LFSSR-SAS-PyTorch](https://github.com/jingjin25/LFSSR-SAS-PyTorch) |
| **EPGB** | Light field super-resolution using edge-preserved graph-based regularization, [TMM 2019](https://ieeexplore.ieee.org/document/8861391).| -- |
| **LF-FusNet** | Light field super-resolution by jointly exploiting internal and external similarities, [TCSVT 2019](https://ieeexplore.ieee.org/abstract/document/8733069). | [Joechann0831/<br/>LFSR-FusNet](https://github.com/Joechann0831/LFSR-FusNet) |
| --- | An epipolar volume autoencoder with adversarial loss for deep light field super-resolution, [CVPRW 2019](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Zhu_An_Epipolar_Volume_Autoencoder_With_Adversarial_Loss_for_Deep_Light_CVPRW_2019_paper.pdf) | [MinchenZKN/<br/>LFSR](https://github.com/MinchenZKN/LFSR) |
| **resLF**      | Residual networks for light field image super-resolution, [CVPR 2019](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Residual_Networks_for_Light_Field_Image_Super-Resolution_CVPR_2019_paper.pdf) | [shuozh/resLF](https://github.com/shuozh/resLF) |
| **HDDRNet**     | High-dimensional dense residual convolutional neural network for light field reconstruction, [TPAMI 2019](https://arxiv.org/pdf/1910.01426.pdf)| [monaen/<br/>LightFieldReconstruction](https://github.com/monaen/LightFieldReconstruction)
| **LF-InterNet** | Spatial-angular interaction for light field image super-resolution, [ECCV 2020](https://arxiv.org/pdf/1912.07849.pdf) | [YingqianWang/<br/>LF-InterNet](https://github.com/YingqianWang/LF-InterNet) |
| **LF-ATO**  | Light field spatial super-resolution via deep combinatorial geometry embedding and structural consistency regularization, [CVPR 2020](https://openaccess.thecvf.com/content_CVPR_2020/papers/Jin_Light_Field_Spatial_Super-Resolution_via_Deep_Combinatorial_Geometry_Embedding_and_CVPR_2020_paper.pdf) | [jingjin25/<br/>LFSSR-ATO](https://github.com/jingjin25/LFSSR-ATO) |
| **LFDCSR**| Deep selective combinatorial embedding and consistency regularization for light field super-resolution, [arxiv 2020](https://arxiv.org/abs/2009.12537) | -- |
| **LF-DFnet**    | Light field image super-resolution using deformable convolution, [TIP 2020](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9286855) | [YingqianWang/<br/>LF-DFnet](https://github.com/YingqianWang/LF-DFnet) |
| **LF-ZSSR** | Light field super-resolution with zero-shot learning, [CVPR 2021](https://openaccess.thecvf.com/content/CVPR2021/papers/Cheng_Light_Field_Super-Resolution_With_Zero-Shot_Learning_CVPR_2021_paper.pdf) | [Joechann0831/<br/>LFZSSR](https://github.com/Joechann0831/LFZSSR) |
| **LFSR-AFR** | Light field super-resolution via adaptive feature remixing, [TIP 2021](https://ieeexplore.ieee.org/document/9394760/). | [keunsoo-ko/<br/>LFSR-AFR](https://github.com/keunsoo-ko/LFSR-AFR) |
| **MEG-Net**     | End-to-end light field spatial super-resolution network using multiple epipolar geometry, [TIP 2021](https://ieeexplore.ieee.org/abstract/document/9465683). | [shuozh/MEG-Net](https://github.com/shuozh/MEG-Net) |
| **DDAN**     | Dense dual-attention network for light field image super-resolution, [TCSVT 2021](https://arxiv.org/pdf/2110.12114.pdf). | -- |
| **LF-IINet**     | Intra-inter view interaction network for light field image super-resolution, [TMM 2021](https://ieeexplore.ieee.org/document/9599365). | [GaoshengLiu/<br/>LF-IINet](https://github.com/GaoshengLiu/LF-IINet) |
| **LFT**     | Light field image super-resolution with Transformers, [arxiv 2021](https://arxiv.org/pdf/2108.07597.pdf). | [ZhengyuLiang24/LFT](https://github.com/ZhengyuLiang24/LFT) |

## Acknowledgement
**We would like to thank [Zhengyu Liang](https://github.com/ZhengyuLiang24) and [Zhen Cheng](https://github.com/Joechann0831) for the helpful discussions and insightful suggestions regarding this repository.**

## Contact
**Any question regarding this repo can be addressed to wangyingqian16@nudt.edu.cn.**

