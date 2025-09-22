# Single/Multiple Object Tracking and Segmentation

### Codes and comparison of SOTA single/multiple object tracking and segmentation.

## News
:boom: [VLT_SCAR/VLT_TT](https://arxiv.org/abs/2207.01076) is accepted by NeurIPS2022.

:boom: [CNNInMo/TransInMo](https://arxiv.org/abs/2201.02526) is accepted by IJCAI2022.

:boom: [CSTrack](https://pubmed.ncbi.nlm.nih.gov/35412982/) is accepted by IEEE TIP. 

:boom: [OMC](https://arxiv.org/abs/2104.09441) is accepted by AAAI2022.

:boom: [AutoMatch](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhang_Learn_To_Match_Automatic_Matching_Network_Design_for_Visual_Tracking_ICCV_2021_paper.pdf) is accepted by ICCV2021. The training and testing code has been released in this codebase.

:boom: [CSTrack](https://arxiv.org/abs/2010.12138) ranks 5/4000 at `Tianchi Global AI Competition`.

:boom: [Ocean](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123660766.pdf) is accepted by ECCV2020. [OceanPlus] is accepted by IEEE TIP.

:boom: [SiamDW](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Deeper_and_Wider_Siamese_Networks_for_Real-Time_Visual_Tracking_CVPR_2019_paper.pdf) is accepted by CVPR2019 and selected as oral presentation.


## Supported Trackers (SOT and MOT)

### Single-Object Tracking (SOT)
- [x] [**[NeurIPS2022] VLT_SCAR/VLT_TT**](https://arxiv.org/abs/2207.01076)
- [x] [**[IJCAI2022] CNNInMo/TransInMo**](https://arxiv.org/abs/2201.02526)
- [x] [**[ICCV2021] AutoMatch**](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhang_Learn_To_Match_Automatic_Matching_Network_Design_for_Visual_Tracking_ICCV_2021_paper.pdf)
- [x] [**[ECCV2020] Ocean and Ocean+**](https://arxiv.org/abs/2006.10721)
- [x] [**[CVPR2019 Oral] SiamDW**](http://openaccess.thecvf.com/content_CVPR_2019/html/Zhang_Deeper_and_Wider_Siamese_Networks_for_Real-Time_Visual_Tracking_CVPR_2019_paper.html)


### Multi-Object Tracking (MOT)
- [x] [**[IEEE TIP] CSTrack**](https://arxiv.org/pdf/2010.12138) 

## Results Comparison
- [x] [**Comparison**](https://github.com/JudasDie/Comparison)

## Structure
- `experiments:` training and testing settings
- `demo:` figures for readme
- `lib:` core scripts for all trackers
- `tracking:` training and testing interface


## Performance
| <sub>Model</br></sub> | <sub>OTB2015</br> </sub> | <sub>GOT10K</br> </sub> | <sub>LaSOT</br> </sub> | <sub>TNL2K</br></sub> | <sub>TrackingNet</br></sub> | <sub>NFS30</br> </sub> | <sub>TOTB</sub> |<sub>VOT2019</sub> |<sub>TC128</sub> |<sub>UAV123</sub> |<sub>LaSOT_Ext</sub> |<sub>OTB-99-LANG</sub> |
|:-----:|:-:|:----:|:------:|:--------:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| <sub>SiamDW<sub>  | <sub>0.670</sub> | <sub>0.429</sub> | <sub>0.386</sub>|<sub>0.348</sub>|<sub>61.1</sub>| <sub>0.521</sub> |<sub>0.500</sub> |<sub>0.241</sub> |<sub>0.583</sub> |<sub>0.536</sub> |<sub>-</sub> |<sub>-</sub> |
| <sub>Ocean</sub>   |  <sub>0.676</sub> | <sub>0.615</sub> | <sub>0.517</sub>|<sub>0.421</sub>|<sub>69.2</sub>| <sub>0.553</sub> |<sub>0.638</sub> |<sub>0.323</sub> |<sub>0.585</sub> |<sub>0.621</sub> |<sub>-</sub> |<sub>-</sub> |
| <sub>AutoMatch</sub> | <sub>0.714</sub> | <sub>0.652</sub> | <sub>0.583</sub>|<sub>0.472</sub>|<sub>76.0</sub>| <sub>0.606</sub> |<sub>0.668</sub> |<sub>0.322</sub> |<sub>0.634</sub> |<sub>0.644</sub> |<sub>-</sub> |<sub>-</sub> |
| <sub>CNNInMo</sub> | <sub>0.703</sub> | <sub>-</sub> | <sub>0.539</sub>|<sub>0.422</sub>|<sub>72.1</sub>| <sub>0.560</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>0.629</sub> |<sub>-</sub> |<sub>-</sub> |
| <sub>TransInMo</sub> | <sub>0.711</sub> | <sub>-</sub> | <sub>0.657</sub>|<sub>0.520</sub>|<sub>81.7</sub>| <sub>0.668</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>0.690</sub> |<sub>-</sub> |<sub>-</sub> |
| <sub>VLT_SCAR</sub> | <sub>-</sub> | <sub>0.610</sub> | <sub>0.639</sub>|<sub>0.498</sub>|<sub>-</sub>| <sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>0.447</sub> |<sub>0.739</sub> |
| <sub>VLT_TT</sub> | <sub>-</sub> | <sub>0.694</sub> | <sub>0.673</sub>|<sub>0.531</sub>|<sub>-</sub>| <sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>-</sub> |<sub>0.484</sub> |<sub>0.764</sub> |



## Tracker Details
### VLT_SCAR/VLT_TT [NeurIPS2022]
**[[Paper]](https://arxiv.org/abs/2207.01076) [[Raw Results]](https://drive.google.com/drive/folders/1gO_VBm7ucvNwj_Xi8ZKt2rRysrjhyvep?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/SOT/lib/tutorial/sot/sot_vlt.md)** <br/>
VLT explores a different path to achieve SOTA tracking without complex Transformer, i.e., multimodal Vision-Language tracking. The essence is a unified-adaptive Vision-Language representation, learned by the proposed ModaMixer and asymmetrical networks. The experiments show our approach surprisingly boosts a pure CNN-based Siamese tracker to achieve competitive or even better performances compared to recent SOTAs, which also benefits Transformer-based trackers. We hope that this work inspires more possibilities for future tracking beyond Transformer.

<img src="https://github.com/JudasDie/SOTS/blob/SOT/demo/VLT.jpg" width="700" alt="VLT"/><br/>

### CNNInMo/TransInMo [IJCAI2022]
**[[Paper]](https://arxiv.org/abs/2201.02526) [[Raw Results]](https://drive.google.com/drive/folders/10HhdHcrpbnsxnwMlNEDWieDeM9pNiynn?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/sot/sot.md)** <br/>
CNNInMo/TransInMo introduces a novel mechanism that conducts branch-wise interactions inside the visual tracking backbone network (InBN) via the proposed general interaction modeler (GIM). We show that both CNN and Transformer backbones can benefit from InBN, with which more robust feature representation can be learned. Our method achieves compelling tracking performance by applying the backbones to Siamese tracking.

  
<img src="https://github.com/JudasDie/SOTS/blob/SOT/demo/TransInMo.jpg" width="700" alt="TransInMo"/><br/>

### AutoMatch [ICCV2021]
**[[Paper]](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhang_Learn_To_Match_Automatic_Matching_Network_Design_for_Visual_Tracking_ICCV_2021_paper.pdf) [[Raw Results]](https://drive.google.com/drive/folders/1uYDru48cX6oYN8FPt26UD9E_CvsHypvw?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/sot/sot.md) [[Demo]](https://crossminds.ai/video/learn-to-match-automatic-matching-network-design-for-visual-tracking-615cac8654e2c0f6b5817867/)** <br/>
AutoMatch replaces the essence of Siamese tracking, i.e. the cross-correlation and its variants, to a learnable matching network. The underlying motivation is that heuristic matching network design relies heavily on expert experience. Moreover, we experimentally find that one sole matching operator is difficult to guarantee stable tracking in all challenging environments. In this work, we introduce six novel matching operators from the perspective of feature fusion instead of explicit similarity learning, namely Concatenation, Pointwise-Addition, Pairwise-Relation, FiLM, Simple-Transformer and Transductive-Guidance, to explore more feasibility on matching operator selection. The analyses reveal these operators' selective adaptability on different environment degradation types, which inspires us to combine them to explore complementary features. We propose binary channel manipulation (BCM) to search for the optimal combination of these operators. 

<div align="left">
  <img src="https://i.postimg.cc/cHCgTcbN/automatch.jpg" height="200" alt="AutoMatch"/><br/>
</div>

### Ocean [ECCV2020]
**[[Paper]](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123660766.pdf) [[Raw Results]](https://drive.google.com/drive/folders/1fYVTGxMu0Zg5r88dgfTzsd5MOOExQbaF?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/sot/sot.md) [[Demo]](https://www.youtube.com/watch?v=83-XCEsQ1Kg&feature=youtu.be)** <br/>

Ocean proposes a general anchor-free based tracking framework. It includes a pixel-based anchor-free regression network to solve the weak rectification problem of RPN, and an object-aware classification network to learn robust target-related representation. Moreover, we introduce an effective multi-scale feature combination module to replace heavy result fusion mechanism in recent Siamese trackers. This work also serves as the baseline model of OceanPlus. An additional **TensorRT** toy demo is provided in this repo.
<div align="left">
  <img src="https://github.com/JudasDie/SOTS/blob/master/demo/Ocean_overview.jpg" height="300" alt="Ocean"/><br/>
  <!-- <p>Example SiamFC, SiamRPN and SiamMask outputs.</p> -->
</div>

### SiamDW [CVPR2019]
**[[Paper]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Deeper_and_Wider_Siamese_Networks_for_Real-Time_Visual_Tracking_CVPR_2019_paper.pdf) [[Raw Results]](https://drive.google.com/drive/folders/16uObavj1X9zqFndOxJJdxaRM43xSrHnf?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/sot/sot.md) [[Demo]]()** <br/>
SiamDW is one of the pioneering work using deep backbone networks for Siamese tracking framework. Based on sufficient analysis on network depth, output size, receptive field and padding mode, we propose guidelines to build backbone networks for Siamese tracker. Several deeper and wider networks are built following the guidelines with the proposed CIR module. 

<img src="https://github.com/JudasDie/SOTS/blob/master/demo/siamdw_overview.jpg" height="250" alt="SiamDW"/><br/>

### OceanPlus [IEEE TIP]
**[[Paper]](https://ieeexplore.ieee.org/document/9563126?source=authoralert) [[Raw Results]](https://drive.google.com/drive/folders/1doQiv82swum2rEXXo5C735WrLb_uAVbq?usp=sharing) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/OceanPlus/oceanplus.md) [[Demo]]()** <br/>
Official implementation of the OceanPlus tracker. It proposes an attention retrieval network (ARN) to perform soft spatial constraints on backbone features. Concretely, we first build a look-up-table (LUT) with the ground-truth mask in the starting frame, and then retrieve the LUT to obtain a target-aware attention map for suppressing the negative influence of background clutter. Furthermore, we introduce a multi-resolution multi-stage segmentation network (MMS) to ulteriorly weaken responses of background clutter by reusing the predicted mask to filter backbone features.

<img src="https://github.com/JudasDie/SOTS/blob/master/demo/oceanplu_overview.png"  alt="OceanPlus"/><br/>

### CSTrack [IEEE TIP]
**[[Paper]](https://arxiv.org/abs/2010.12138) [[Training and Testing Tutorial]](https://github.com/JudasDie/SOTS/tree/master/lib/tutorial/mot/cstrack.md) [[Demo]](https://motchallenge.net/method/MOT=3601&chl=10)** <br/>
CSTrack proposes a strong ReID based one-shot MOT framework. It includes a novel cross-correlation network that can effectively impel the separate branches to learn task-dependent representations, and a scale-aware attention network that learns discriminative embeddings to improve the ReID capability. This work also provides an analysis of the weak data association ability in one-shot MOT methods. Our improvements make the data association ability of our one-shot model is comparable to two-stage methods while running more faster.

<img src="https://github.com/JudasDie/SOTS/blob/master/demo/CSTrack_CCN.jpg" height="300" alt="CSTrack"/><br/>