# NTIRE 2023: Light Field Image Super-Resolution Challenge <br> 
<p align="center">  <img src="https://raw.github.com/The-Learning-And-Vision-Atelier-LAVA/LF-Image-SR/NTIRE2023/Fig/logo.jpg" width="400"> </p>

**Light field (LF) image super-resolution (SR) challenge is held as a part of the [NTIRE workshop](https://cvlai.net/ntire/2023/) in conjunction with CVPR 2023. The goal of this challenge is to develop methods to enhance the spatial resolution of LF images.**


## News and Updates:
* **2022-12-16**: The proposal for LF image SR challenge is approved.
<br><br>

## Introduction
With recent advances in camera manufacturing, light field (LF) imaging technology becomes increasingly popular and is commonly used in various applications such as mobile phones, biological microscope, VR/AR etc. Since both intensity and directions of light rays are recorded by LF cameras, the resolution of LF images can be enhanced by using these additional angular information. LF image super-resolution (SR), also known as LF spatial SR, aims at reconstructing high-resolution (HR) LF images from their low-resolution (LR) counterparts. 

Jointly with the NTIRE workshop, we organize a challenge for LF community to focus on enhancing the spatial resolution of LF images, and aspire to highlight the specific challenges and research problems faced by LF image SR. This challenge provides an opportunity for researchers to work together to share their knowledge and insights, advance the algorithm performance, and promote the development of LF image SR.
<br><br>

## Challenge Overview
The objective of this challenge is to reconstruct HR LF images from their LR counterparts.

During the model development phase, the HR training set and the LR validation set will be released. The participants can train their models on the training set and submit their super-resolved validation images to the CodaLab server for validation.

During the test phase, the test set will be released, which includes LR LF images only. Challenge participants can apply their trained models to the LR test images to generate super-resolved test images. These super-resolved images will then be submitted by the participants and evaluated by the organizers with a set of objective quantitative metrics.
<br><br>

## Datasets
### Training Set: *[[Baidu Drive](https://pan.baidu.com/s/1mYQR6OBXoEKrOk0TjV85Yw) (key:7nzy) or [OneDrive](https://stuxidianeducn-my.sharepoint.com/:f:/g/personal/zyliang_stu_xidian_edu_cn/EpkUehGwOlFIuSSdadq9S4MBEeFkNGPD_DlzkBBmZaV_mA?e=FiUeiv)]*

This challenge follows the training set in the paper [DistgSSR](https://yingqianwang.github.io/DistgLF/), and uses the EPFL, HCInew, HCIold, INRIA and STFgantry datasets which totally consist of 144 scenes for training. All the LF images in the training set have an angular resolution of 9x9. The participants can use these HR LF images as groundtruths, and use the [BasicLFSR toolbox](https://github.com/ZhengyuLiang24/BasicLFSR) to train their models. **External training data or pretrained models are NOT allowed in this challenge.**

### Validation Set: *[[Baidu Drive](https://pan.baidu.com/s/1n6TPP7EJlkKPMn-0DkN10g) (key:lfsr) or [OneDrive](https://stuxidianeducn-my.sharepoint.com/:f:/g/personal/zyliang_stu_xidian_edu_cn/Es3gi3N9XuVPpm8a9pysMGcB2-Pxenr5zo0WZXRaz_SaaA?e=1I840e)]*

We collect a new validation set consisting of 16 synthetic scenes rendered by the 3DS MAX software and 16 real-world images captured by a Lytro ILLUM camera. We downsampled original LF images in the validation set by a factor of 4, and provide LR LF images with an angular resolution of 5x5. The participants can download the validation set to evaluate the performance of their developed models by submitting their super-resolved LF images to the CodaLab server.

### Test Set:

We collect a new test set consisting of 16 synthetic scenes rendered by the 3DS MAX software and 16 real-world images captured by a Lytro ILLUM camera. Only 4× bicubically downsampled LR LF images with an angular resolution of 5x5 will be provided. The participants are required to apply their models to the released LR LF images and submit their 4× super-resolved LF images to the CodaLab platform for final ranking. **It should be noted that the images in both the validation and the test sets (even the LR versions) cannot be used for training.**
<br><br>

## Evaluation Metrics
We evaluate the submitted results by comparing them with the ground truth LF images. To measure the fidelity, we use the standard Peak Signal to Noise Ratio (PSNR) and, complementarily, the Structural Similarity (SSIM) index as they are often employed in the literature. PSNR and SSIM implementations can be found in the [BasicLFSR toolbox](https://github.com/ZhengyuLiang24/BasicLFSR). **We report the submissions over the synthetic and real-world images in the test sets, and rank the submissions according to the average PSNR values.** The SSIM metrics will not affect submission rankings but will be used to review the strengths and weaknesses of suggested methods in the final challenge report. 
<br><br>

## Baseline Model
In this challenge, **LF-InterNet** is used as a baseline model and the submitted results should be at least on par with LF-InterNet. The solutions with PSNR values lower than LF-InterNet will not be ranked in the leaderboard. Here, we provide the scores achieved by Bicubic, LF-InterNet, DistgSSR and LFT for reference.

### PSNR and SSIM values achieved by baseline methods on the validation set for 4xSR:
| Method | PSNR (avg)  |  PSNR (syn)  | PSNR (real)  | SSIM (avg)  |  SSIM (syn)  | SSIM (real)  |
|:------:|  :--------: | :--------: | :---------: | :-------: | :-------: | :-------: | 
| Bicubic       | 
| LF-InterNet   | 
| DistgSSR      | 
| LFT           |
<br>

## Submission
We use CodaLab for online submission in the development phase. **Here, we provide an [example]() to help participants to format their submissions.** In the test phase, the final results and the source codes (both training and test) need to be submitted via emails (ntire.lfsr@outlook.com). Please refer to our [online website](https://codalab.lisn.upsaclay.fr/competitions/9201) for details of the submission rules.
<br><br>

## Important Dates
* 2023-01-17: Release of training and validation data;
* 2023-01-27: Validation server online;
* 2023-03-07: Final test data release, validation server closed;
* 2023-03-14: Test result submission deadline;
* 2023-03-15: Fact sheet / code / model submission deadline;
* 2023-03-17: Test preliminary score release to the participants;
* 2023-03-28: Challenge paper submission deadline;
<br><br>

## Group number policy
Each group cannot have more than six group members (i.e., 1 to 6 group members is OK), and each paricipant can only join one group. Each group can only submit one algorithm for final ranking.
<br><br>

## Issues and Questions:
For any question regarding this challenge, raise an issue under this repository. <br>
You can also join our WeChat group by scanning the code below:

<p align="center"> <img src="https://raw.github.com/The-Learning-And-Vision-Atelier-LAVA/LF-Image-SR/NTIRE2023/Fig/WeChat.jpg" width="40%"> </p>

## Organizers:
* [**Yingqian Wang**](https://yingqianwang.github.io/) ([wangyingqian16@nudt.edu.cn](wangyingqian16@nudt.edu.cn))
* [**Longguang Wang**](https://longguangwang.github.io/) ([wanglongguang15@nudt.edu.cn](wanglongguang15@nudt.edu.cn))
* [**Zhengyu Liang**](https://github.com/ZhengyuLiang24) ([zyliang@nudt.edu.cn](zyliang@nudt.edu.cn))
* [**Jungang Yang**]() ([yangjungang@nudt.edu.cn](yangjungang@nudt.edu.cn))
* [**Yulan Guo**](http://yulanguo.me/) ([yulan.guo@nudt.edu.cn](yulan.guo@nudt.edu.cn))
* [**Radu Timofte**](https://people.ee.ethz.ch/~timofter/) ([Radu.Timofte@vision.ee.ethz.ch](Radu.Timofte@vision.ee.ethz.ch))
<br><br>

## NTIRE 2023 Terms and Conditions:
The terms and conditions of this challenge can be viewed [here](https://codalab.lisn.upsaclay.fr/competitions/9201#learn_the_details-terms_and_conditions).


