# Awesome Crowd Counting

If you have any problems, suggestions or improvements, please submit the issue or PR.

## Contents
* [Misc](#misc)
* [Datasets](#datasets)
* [Papers](#papers)
* [Leaderboard](#leaderboard)

## Misc



### Challenge
- [[VisDrone 2020](http://aiskyeye.com/challenge/crowd-counting/)] ~~Crowd counting. ECCV Workshop. Deadline: **2020.07.15**.~~
- [[NWPU-Crowd Counting](https://www.crowdbenchmark.com/nwpucrowd.html)] Crowd counting. Deadline: none.

### Code
- [[C^3 Framework](https://github.com/gjy3035/C-3-Framework)] An open-source PyTorch code for crowd counting, which is released.
- [[CCLabeler](https://github.com/Elin24/cclabeler)] A web tool for labeling pedestrians in an image, which is released.

### Technical blog
- [Chinese Blog] 人群计数论文解读 [[Link](https://zhuanlan.zhihu.com/c_1111215695622352896)]
- [2019.05] [Chinese Blog] C^3 Framework系列之一：一个基于PyTorch的开源人群计数框架 [[Link](https://zhuanlan.zhihu.com/p/65650998)]
- [2019.04] Crowd counting from scratch [[Link](https://github.com/CommissarMa/Crowd_counting_from_scratch)]
- [2017.11] Counting Crowds and Lines with AI [[Link1](https://blog.dimroc.com/2017/11/19/counting-crowds-and-lines/)] [[Link2](https://count.dimroc.com/)] [[Code](https://github.com/dimroc/count)]


## Datasets

Please refer to [this page](src/Datasets.md).

## Papers

Considering the increasing number of papers in this field, we roughly summarize some articles and put them into the following categories (they are still listed in this document):


### arXiv papers
Note that all unpublished arXiv papers are not included in [the leaderboard of performance](#performance).

- Completely Self-Supervised Crowd Counting via Distribution Matching [[paper](https://arxiv.org/abs/2009.06420)][[code](https://github.com/val-iisc/css-ccnn)]
- A Study of Human Gaze Behavior During Visual Crowd Counting [[paper](https://arxiv.org/abs/2009.06502)]

<details>
<summary>Earlier ArXiv Papers</summary>

- Understanding the impact of mistakes on background regions in crowd counting [[paper](https://arxiv.org/abs/2003.13759)]
- CNN-based Density Estimation and Crowd Counting: A Survey [[paper](https://arxiv.org/abs/2003.12783)]
- Encoder-Decoder Based Convolutional Neural Networks with Multi-Scale-Aware Modules for Crowd Counting [[paper](https://arxiv.org/abs/2003.05586)][[code](https://github.com/Pongpisit-Thanasutives/Variations-of-SFANet-for-Crowd-Counting)]

</details>


### 2020

- <a name="AMRNet"></a> **[AMRNet]** Adaptive Mixture Regression Network with Local Counting Map for Crowd Counting (**ECCV**) [[paper](https://arxiv.org/abs/2005.05776)][[code](https://github.com/xiyang1012/Local-Crowd-Counting)]


### 2019

- <a name="D-ConvNet"></a> **[D-ConvNet]** Nonlinear Regression via Deep Negative Correlation Learning (**T-PAMI**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8850209)](extension of [D-ConvNet](#D-ConvNet))[[Project](https://mmcheng.net/dncl/)]
- <a name=""></a>Generalizing semi-supervised generative adversarial networks to regression using feature contrasting (**CVIU**)[[paper](https://arxiv.org/abs/1811.11269)]
- <a name="CG-DRCN"></a> **[CG-DRCN]** Pushing the Frontiers of Unconstrained Crowd Counting: New Dataset and Benchmark Method (**ICCV**)[[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sindagi_Pushing_the_Frontiers_of_Unconstrained_Crowd_Counting_New_Dataset_and_ICCV_2019_paper.pdf)]


### 2018

- <a name="SANet"></a> **[SANet]** Scale Aggregation Network for Accurate and Efficient Crowd Counting (**ECCV**) [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xinkun_Cao_Scale_Aggregation_Network_ECCV_2018_paper.pdf)]
- <a name="ic-CNN"></a> **[ic-CNN]** Iterative Crowd Counting (**ECCV**) [[paper](https://arxiv.org/abs/1807.09959)]



## Leaderboard
The section is being continually updated. Note that some values have superscript, which indicates their source. 


### ShanghaiTech Part A

| Year-Conference/Journal | Methods           | MAE   | MSE   | PSNR  | SSIM | Params | Pre-trained   Model |
| ---- | ------------------------------------ | ----- | ----- | ----- | ---- | ------ | ------------------- |
| 2016--CVPR | [MCNN](#MCNN)     | 110.2 | 173.2 | 21.4<sup>[CSR](#CSR)</sup> | 0.52<sup>[CSR](#CSR)</sup>  | 0.13M<sup>[SANet](#SANet)</sup>  | None  |
| 2017--AVSS | [CMTL](#CMTL)                                | 101.3 | 152.4 | -  | -  | -  | None        |
| 2017--CVPR | [Switching CNN](#SCNN)                       | 90.4  | 135.0 | -  | -  | 15.11M<sup>[SANet](#SANet)</sup>  | VGG-16      |
| 2017--ICIP | [MSCNN](#MSCNN)                              | 83.8  | 127.4 | -  | -  | -  | -           |
| 2017--ICCV | [CP-CNN](#CP-CNN) | 73.6  | 106.4 | 21.72<sup>[CP-CNN](#CP-CNN)</sup> | 0.72<sup>[CP-CNN](#CP-CNN)</sup>  | 68.4M<sup>[SANet](#SANet)</sup>  | - |
| 2018--AAAI | [TDF-CNN](#TDF-CNN)                          | 97.5  | 145.1 | -  | -  | -  | -           |
| 2018--WACV | [SaCNN](#SaCNN)                              | 86.8  | 139.2 | -  | -  | -  | -           |
| 2018--CVPR | [ACSCP](#ACSCP)                              | 75.7  | 102.7 | -  | -  | 5.1M | None      |
| 2018--CVPR | [D-ConvNet-v1](#D-ConvNet)                   | 73.5  | 112.3 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [IG-CNN](#IG-CNN)                            | 72.5  | 118.2 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Query-by-example) | 72.0  | 106.6 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Keyword)          | 73.6  | 112.0 | -  | -  | -  | VGG-16      |
| 2019--CVPRW| [GSP](#GSP) (one stage, efficient)           | 70.7  | 103.6 | -  | -  | -  | VGG-16      |
| 2018--IJCAI| [DRSAN](#DRSAN)                              | 69.3  | 96.4  | -  | -  | -  | -           |
| 2018--ECCV | [ic-CNN](#ic-CNN) (one stage)                | 69.8  | 117.3 | -  | -  | -  | -           |
| 2018--ECCV | [ic-CNN](#ic-CNN) (two stages)               | 68.5  | 116.2 | -  | -  | -  | -           |
| 2018--CVPR | [CSRNet](#CSR)   | 68.2  | 115.0 | 23.79 | 0.76 | 16.26M<sup>[SANet](#SANet)</sup> |VGG-16|
| 2018--ECCV | [SANet](#SANet)                              | 67.0  | 104.5 | -  | -  | 0.91M | None     |
| 2019--AAAI | [GWTA-CCNN](#GWTA-CCNN)                      | 154.7 | 229.4 | -  | -  | -  | -           |
| 2019--ICASSP | [ASD](#ASD)                                | 65.6  | 98.0  | -  | -  | -  | -           |
| 2019--ICCV | [CFF](#CFF)                                  | 65.2  | 109.4 | 25.4  | 0.78 | -     | -   |
| 2019--CVPR | [SFCN](#CCWld)                               | 64.8  | 107.5 | -  | -  | -  | -           |
| 2020--AAAI | [DUBNet](#DUBNet)                            | 64.6  | 106.8 | -  | -  | -  | -           |
| 2019--ICCV | [SPN+L2SM](#L2SM)                            | 64.2  | 98.4  | -  | -  | -  | -           |
| 2019--CVPR | [TEDnet](#TEDnet)                            | 64.2  | 109.1 | 25.88 | 0.83 | 1.63M | -   |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-bAttn-DME)     | 63.2  | 98.9  | 24.48 | 0.88 | -     | -   |
| 2019--CVPR | [PACNN](#PACNN)                              | 66.3  | 106.4 | -  | -  | -  | -           |
| 2019--CVPR | [PACNN+CSRNet](#PACNN)                       | 62.4  | 102.0 | -  | -  | -  | -           |
| 2019--CVPR | [CAN](#CAN)                                  | 62.3  | 100.0 | -  | -  | -  | VGG-16      |
| 2019--TIP  | [HA-CCN](#HA-CCN)                            | 62.9  | 94.9  | -  | -  | -  | -           |
| 2019--ICCV | [BL](#BL)                                    | 62.8  | 101.8 | -  | -  | -  | -           |
| 2019--WACV | [SPN](#SPN)                                  | 61.7  | 99.5  | -  | -  | -  | -           |
| 2019--ICCV | [DSSINet](#DSSINet)                          | 60.63 | 96.04 | -  | -  | -  | -           |
| 2019--ICCV | [MBTTBF-SCFB](#MBTTBF)                       | 60.2  | 94.1  | -  | -  | -  | -           |
| 2019--ICCV | [RANet](#RANet)                              | 59.4  | 102.0 | -  | -  | -  | -           |
| 2019--ICCV | [SPANet+SANet](#SPANet)                      | 59.4  | 92.5  | -  | -  | -  | -           |
| 2019--TIP  | [PaDNet](#PaDNet)                            | 59.2  | 98.1  | -  | -  | -  | -           |
| 2019--ICCV | [S-DCNet](#S-DCNet)                          | 58.3  | 95.0  | -  | -  | -  | -           |
| 2019--ICCV |**[PGCNet](#PGCNet)**                         | 57.0 | **86.0** | -  | -  | -  | -         |
| 2020--CVPR |**[ADSCNet](#ADSCNet)**                       | **55.4** | 97.7 | -  | -  | -  | -         |

