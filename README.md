### <img src="https://raw.github.com/YingqianWang/Awesome-LF-Image-SR/master/Fig/Thumbnail.jpg" width="1000">
#### With recent advances in camera manufacturing, light field (LF) imaging technology becomes increasingly popular and is commonly used in various applications such as mobile phones, biological microscope, VR/AR etc. Since both intensity and directions of light rays are recorded by LF cameras, the resolution of LF images can be enhanced by using these additional angular information. LF image super-resolution (SR), also known as LF spatial SR, aims at reconstructing high-resolution (HR) LF images from their low-resolution (LR) counterparts. In this repository, we present a collection of papers and datasets on LF image SR, together with their codes and repos. 
#### Note: This repository will be updated on a regular basis, so stay tuned~~🎉🎉🎉

## Datasets
#### A more comprehensive overview of LF datasets can be viewed through [**this link**](https://github.com/lightfield-analysis/resources). Here, we only list several popular datasets which are commonly used for LF image SR: 
* **New light field image dataset (EPFL)**. [**website**](https://www.epfl.ch/labs/mmspg/downloads/epfl-light-field-image-dataset/); [**paper**](https://infoscience.epfl.ch/record/218363/files/Qomex2016_shortpaper.pdf?version=1); [**download through Baidu Drive**](https://pan.baidu.com/s/1175dV3Sj8y9K2FPYxjsuEg) (Keys:NUDT)
* **Datasets and Benchmarks for Densely Sampled 4D Light Fields (HCIold)**. [**paper**](https://pdfs.semanticscholar.org/1a86/e03c229adb5b94e1f43f8508f033f74e94ae.pdf)
* **4D Light Field Dataset (HCInew)**. [**website**](https://lightfield-analysis.uni-konstanz.de/); [**paper**](https://infoscience.epfl.ch/record/218363/files/Qomex2016_shortpaper.pdf?version=1)
* **INRIA Light field dataset (INRIA)**. [**website**](https://www.irisa.fr/temics/demos/lightField/LowRank2/datasets/datasets.html); [**paper**](https://hal.archives-ouvertes.fr/hal-01720622/file/LFInpaintTIP.pdf)
* **The (New) Stanford Light Field Archive (STFgantry)**. [**website**](http://lightfield.stanford.edu/)
* **Stanford Lytro Light Field Archive (STFLytro)**. [**website**](http://lightfields.stanford.edu/LF2016.html)



## Methods
|     Model     |   Published |  Codes | Keywords | Better Performance than|
| :----------: |  :-----: | :-------: | :-------: | :-------: |
| **Bishop et al.** | [**TPAMI2012**](https://ieeexplore.ieee.org/abstract/document/5989827/) | -- | **pioneering work, variational Bayesian, Lambertian prior** | -- |
| **GMM** | [**CVPRW2012**](https://www.ece.rice.edu/~av21/Documents/2012/Light%20field%20denoising,%20light%20field%20superresolution%20and%20stereo%20camera%20based%20refocussing%20using%20a%20GMM%20light%20field%20patch%20prior.pdf) | -- | **pioneering work, Gaussian mixture model, subspace projection** | -- |
| **Wanner et al.** | [**ECCV2012**](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2012/papers/7576/75760608.pdf) & [**TPAMI2013**](https://ieeexplore.ieee.org/abstract/document/6574844/) | -- | **pioneering work, structure tensor, variational framework** | -- |
| **LFCNN** | [**ICCVW2015**](http://openaccess.thecvf.com/content_iccv_2015_workshops/w3/papers/Yoon_Learning_a_Deep_ICCV_2015_paper.pdf) & [**SPL2017**](https://ieeexplore.ieee.org/abstract/document/7856946) | [**TensorFlow**](https://github.com/youngjinYoon/SPL_LF_SR) | **first CNN-based method** | **GMM, Wanner et al.** |
| **PCA_rr** | [**JSTSP2017**](https://hal.archives-ouvertes.fr/hal-01591488/file/lightfield_SR_v02.pdf) | [**Matlab**](https://github.com/rrfarr/LF-Editing) | **PCA, ridge regression, patch matching** | **LFCNN**, *SRCNN, ANR, NCSR* |
| **LFSR_Gul** | [**TIP2018**](https://arxiv.org/pdf/1707.00815) | -- | **CNN** | **LFCNN**, *DRRN* |
| **GB** | [**MMSP2017**](https://infoscience.epfl.ch/record/230084/files/superMMSP_1.pdf) & [**TIP2018**](https://arxiv.org/pdf/1701.02141) | [**Matlab**](https://github.com/rossimattia/light-field-super-resolution) | **graph-based regularization** | **Wanner et al., GMM**, *SRCNN* |
| **LFNet** | [**TIP2018**](https://ieeexplore.ieee.org/abstract/document/8356655/) | [**Theano**](https://github.com/wylcasia/LFNet) | **bidirectional recurrent CNN** | **LFCNN**, *FSRCNN, VDSR, BRCN, DRRN* |
| **LRP** | [**TPAMI2018**](https://arxiv.org/pdf/1801.04314) | -- | **low-rank prior, SVD, QR decomposition, CNN** | **LFCNN, PCA_rr**, *VDSR* |
| **LFBM5D** | [**ICIP2018**](https://v-sense.scss.tcd.ie/wp-content/uploads/2018/05/LFBM5D_SR.pdf) | [**Matlab/C++**](https://github.com/V-Sense/LFBM5D/tree/SR) | **entend SR-BM3D to LFs** | **PCA_rr**, *SR-BM3D* |
| **LF-DCNN** | [**SPL2018**](https://ieeexplore.ieee.org/abstract/document/8411485) | -- | **EDSR + EPI enhancement** | **LFCNN, GB**, *EDSR* |
| **LFSSR** | [**TIP2018**](https://ieeexplore.ieee.org/abstract/document/8561240) | [**MatConvNet**](https://github.com/spatialsr/DeepLightFieldSSR) | **spatial-angular separable convolution** | **LFCNN, PCA_rr, GB**, *VDSR, LapSRN* |
| **MCSTF** | [**IJCV2019**](https://link.springer.com/article/10.1007/s11263-019-01200-5) | -- | **motion-compensated spatio-temporal filtering** | **LFBM5D, GB**, *SRCNN, VSR, DeepSR, SPMC* |
| **EPGB** | [**TMM2019**](https://ieeexplore.ieee.org/abstract/document/8861391) | -- | **edge-preserved graph-based regularization** | **GMM, LFNet, GB**, *SRCNN* |
| **LF-FusNet** | [**ICIP2017**](https://ieeexplore.ieee.org/abstract/document/8296554) & [**TCSVT2019**](https://ieeexplore.ieee.org/abstract/document/8733069/) | [**Caffe**](https://github.com/Joechann0831/LFSR-FusNet) | **internal and external similarity** | **PCA_rr, LFNet, GB,** *VDSR* |
| **resLF** | [**CVPR2019**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Residual_Networks_for_Light_Field_Image_Super-Resolution_CVPR_2019_paper.pdf) | [**PyTorch**](https://github.com/shuozh/resLF) | **multi-branch inputs, residual blocks** | **GMM, Wanner et al., LFCNN, LFNet, GB**, *EDSR* |
| **Zhu et al.** | [**CVPRW2019**](http://openaccess.thecvf.com/content_CVPRW_2019/papers/NTIRE/Zhu_An_Epipolar_Volume_Autoencoder_With_Adversarial_Loss_for_Deep_Light_CVPRW_2019_paper.pdf) | [**TensorFlow**](https://github.com/MinchenZKN/LFSR) | **epipolar volume autoencoder, adversarial loss** | **GB**, *SRGAN* |
| **HDDRNet** | [**TPAMI2019**](https://arxiv.org/pdf/1910.01426.pdf) & [**AAAI2020**](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-MengN.6416.pdf) | [**TensorFlow**](https://github.com/monaen/LightFieldReconstruction) | **4D convolution, dense residual connection** | **LFCNN, PCA_rr, LFNet, resLF**, *VDSR, MSLapSRN, RDN, ESPCN, DUF* |
| **LF-ATO** | [**CVPR2020**](https://arxiv.org/pdf/2004.02215.pdf) | [**PyTorch**](https://github.com/jingjin25/LFSSR-ATO) | **combinatorial geometry embedding, structural consistency regularization** | **PCA_rr, LFNet, GB, resLF**, *EDSR* |
| **LF-InterNet** | [**ECCV2020**](https://arxiv.org/pdf/1912.07849.pdf) | [**PyTorch**](https://github.com/YingqianWang/LF-InterNet) | **spatial-angular interaction** | **LFBM5D, GB, LFSSR, resLF, LF-ATO**, *VDSR, EDSR, RCAN, SAN, SRGAN, ESRGAN* |
| **LFDCSR**|[**Arxiv**](https://arxiv.org/abs/2009.12537)|    | Deep Selective Combinatorial Embedding and Consistency Regularization for Light Field Super-resolution | **Deep Selective Combinatorial Embedding** and **Consistency Regularization** |
| **LF-DFnet** | [**TIP2020**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9286855) | [**PyTorch**](https://github.com/YingqianWang/LF-DFnet) | **angular deformable alignment module** | **LFBM5D, GB, LFSSR, resLF, LF-InterNet**, *VDSR, EDSR, RCAN, ESRGAN* |
| **LFSR-AFR** | [**TIP2021**](https://ieeexplore.ieee.org/document/9394760) | [**PyTorch**](https://github.com/keunsoo-ko/LFSR-AFR) | **Feature Remixing** | **LFCNN, GB, LFNet, LFSSR, resLF**, *RCAN* |

## Acknowledgement
**We would like to thank [Zhen Cheng](https://github.com/Joechann0831) for the helpful discussion and insightful advice regarding this work.**

## Other Recources
* [**YapengTian/Single-Image-Super-Resolution**](https://github.com/YapengTian/Single-Image-Super-Resolution)
* [**LoSealL/VideoSuperResolution**](https://github.com/LoSealL/VideoSuperResolution)
* [**ChaofWang/Awesome-Super-Resolution**](https://github.com/ChaofWang/Awesome-Super-Resolution)
* [**ptkin/Awesome-Super-Resolution**](https://github.com/ptkin/Awesome-Super-Resolution)
* [**lightfield-analysis/resources**](https://github.com/lightfield-analysis/resources)
* [**Joechann0831/LFSRBenchmark**](https://github.com/Joechann0831/LFSRBenchmark)
