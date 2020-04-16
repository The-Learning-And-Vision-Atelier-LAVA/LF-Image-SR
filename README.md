### <img src="https://raw.github.com/YingqianWang/Awesome-LF-Image-SR/master/Fig/Thumbnail.jpg" width="1000">
#### In this repository, we present a collection of papers and datasets on LF image SR, together with their codes and repos. 
#### This repository will be updated on a regular basis, so stay tuned~~🎉🎉🎉

## Datasets

|     Name     |   links |  Comments |
| :----------: |  :-----: | :-------: |
|     **HCI benchmark**     | [**website**](https://lightfield-analysis.uni-konstanz.de/) & [**paper**](https://lightfield-analysis.uni-konstanz.de/) | **online benchmark, 24 synthetic scenes, groundtruth disparity** |
|     **EPFL**     | [**website**](https://www.epfl.ch/labs/mmspg/downloads/epfl-light-field-image-dataset/) & [**paper**](https://infoscience.epfl.ch/record/218363/files/Qomex2016_shortpaper.pdf?version=1) | **Lytro** |


## Methods
|     Model     |   Published |  Codes | Keywords | Better Performance than|
| :----------: |  :-----: | :-------: | :-------: | :-------: |
| **GMM** | [**CVPRW2012**](https://www.ece.rice.edu/~av21/Documents/2012/Light%20field%20denoising,%20light%20field%20superresolution%20and%20stereo%20camera%20based%20refocussing%20using%20a%20GMM%20light%20field%20patch%20prior.pdf) | -- | **pioneering work, Gaussian mixture model** | -- |
| **Wanner et al.** | [**ECCV2012**](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2012/papers/7576/75760608.pdf) & [**TPAMI2013**](https://ieeexplore.ieee.org/abstract/document/6574844/) | -- | **pioneering work, variational model** | -- |
| **LFCNN** | [**ICCVW2015**](http://openaccess.thecvf.com/content_iccv_2015_workshops/w3/papers/Yoon_Learning_a_Deep_ICCV_2015_paper.pdf) & [**SPL2017**](https://ieeexplore.ieee.org/abstract/document/7856946) | [**TensorFlow**](https://github.com/youngjinYoon/SPL_LF_SR) | **first CNN-based method** | **GMM, Wanner et al.** |
| **PCA_rr** | [**JSTSP2017**](https://hal.archives-ouvertes.fr/hal-01591488/file/lightfield_SR_v02.pdf) | -- | **linear subspace projection** | **LFCNN**, *SRCNN, ANR, NCSR* |

| **LFSR_Gul** | [**TIP2018**](https://arxiv.org/pdf/1707.00815) | -- | **CNN** | **LFCNN**, *DRRN* |
| **GB** | [**MMSP2017**](https://infoscience.epfl.ch/record/230084/files/superMMSP_1.pdf) & [**TIP2018**](https://arxiv.org/pdf/1701.02141) | -- | **graph-based regularization** | **Wanner et al., GMM**, *SRCNN* |
| **LFNet** | [**TIP2018**](https://ieeexplore.ieee.org/abstract/document/8356655/) | -- | **bidirectional recurrent CNN** | **LFCNN**, *FSRCNN, VDSR, BRCN, DRRN* |
| **LFBM5D** | [**ICIP2018**](https://v-sense.scss.tcd.ie/wp-content/uploads/2018/05/LFBM5D_SR.pdf) | [**Matlab/C++**](https://github.com/V-Sense/LFBM5D/tree/SR) | **entend SR-BM3D to LFs** | **PCA_rr**, *SR-BM3D* |
| **LF-DCNN** | [**SPL2018**](https://ieeexplore.ieee.org/abstract/document/8411485) | -- | **EDSR + EPI enhancement** | **LFCNN, GB**, *EDSR* |
| **LFSSR** | [**TIP2018**](https://ieeexplore.ieee.org/abstract/document/8561240) | [**MatConvNet**](https://github.com/spatialsr/DeepLightFieldSSR) | **spatial-angular separable convolution** | **LFCNN, PCA_rr, GB**, *VDSR, LapSRN* |

| **EPGB** | [**TMM2019**](https://ieeexplore.ieee.org/abstract/document/8861391) | -- | **edge-preserved graph-based regularization** | **LFNet, GB**, *SRCNN* |
| **LRP** | [**TPAMI2019**](https://arxiv.org/pdf/1801.04314) | -- | **low-rank prior, deep CNN** | **LFCNN, PCA_rr, VDSR** |
| **LF-FuseNet** | [**ICIP2017**](https://ieeexplore.ieee.org/abstract/document/8296554) & [**TCSVT2019**](https://ieeexplore.ieee.org/abstract/document/8733069/) | -- | **internal and external similarity** | **PCA_rr, LFNet, GB,** *VDSR* |
| **resLF** | [**CVPR2019**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Residual_Networks_for_Light_Field_Image_Super-Resolution_CVPR_2019_paper.pdf) | -- | **multi-branch inputs, residual blocks** | **LFNet, GB**, *EDSR* |

| **HDDRNet** | [**TPAMI2019**](https://arxiv.org/pdf/1910.01426.pdf) & [**AAAI2020**](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-MengN.6416.pdf) | [**TensorFlow**](https://github.com/monaen/LightFieldReconstruction) | **4D convolution, dense residual connection** | **LFCNN, PCA_rr, LFNet, resLF**, *VDSR, MSLapSRN, RDN, ESPCN, DUF* |
| **Jin et al.** | [**CVPR2020**](https://arxiv.org/pdf/2004.02215.pdf) | -- | **combinatorial geometry embedding, structural consistency regularization** | **PCA_rr, LFNet, GB, resLF**, *EDSR* |
| **LF-InterNet** | [**arXiv2020**](https://arxiv.org/pdf/1912.07849v2.pdf) | [**PyTorch**](https://github.com/YingqianWang/LF-InterNet) | **spatial-angular interaction** | **LFBM5D, GB, LFNet, LFSSR, resLF**, *VDSR, EDSR, RCAN, SAN, SRGAN, ESRGAN* |


## Other Recources
* [**YapengTian/Single-Image-Super-Resolution**](https://github.com/YapengTian/Single-Image-Super-Resolution)
* [**LoSealL/VideoSuperResolution**](https://github.com/LoSealL/VideoSuperResolution)
* [**ChaofWang/Awesome-Super-Resolution**](https://github.com/ChaofWang/Awesome-Super-Resolution)
* [**ptkin/Awesome-Super-Resolution**](https://github.com/ptkin/Awesome-Super-Resolution)
