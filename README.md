# SOT-Learning

## 内容

## 资源

* **代码框架**
     | **框架**              | **链接**    | **简介**    |
     |:-----------           |:----------------|:----------------|
     | **pysot**             | https://github.com/STVIR/pysot             | STVIR组提供的跟踪框架，主要包括SiamFC，SiamRPN，DaSiamRPN，SiamRPN++，SiamMask等算法。|     
     | **pytracking**        | https://github.com/visionml/pytracking     | visionml组提供的跟踪框架，主要包括pyECO, ATOM, Dimp, PrDimp, KeepTrack等算法。|     
     | **TracKit**           | https://github.com/researchmm/TracKit      | MSRA-MM组提供的跟踪框架，主要包括SiamDW，Ocean跟踪算法。|
     | **mmtracking**        | https://github.com/open-mmlab/mmtracking   | Open-mmlab Tracking相关库，包括视频目标检测，单目标跟踪，多目标跟踪，视频实例分割。其中单目标跟踪算法支持SiameseRPN++(CVPR2019)，STARK(ICCV2021)，PrDiMP(CVPR2020)等算法。和Open-mmlab一脉相承，未来有很大潜力。 |
     | **got-10k-toolkit**   | https://github.com/got-10k/toolkit   | Got-10k数据集网站提供的评估工具，方便大量跟踪数据库上的实验测评，如OTB(2013/2015), VOT(2013~2018), DTB70, TColor128, NfS(30/240 fps), UAV(123/20L), LaSOT, TrackingNet等。 |

* **综述文章**

     | **论文**              | **链接**    | **内容摘要**    |
     |:-----------           |:----------------:|:----------------|
     | ***Visual Object Tracking with Discriminative Filters and Siamese Networks: A Survey and Outlook.*** <br /> **Arxiv, 2021.** Sajid Javed, Martin Danelljan, Fahad Shahbaz Khan, et al. | [[Paper](https://arxiv.org/abs/2112.02838)]   |  **:star2:非常详尽的判决性滤波和深度孪生网络方面的综述**，大量的实验评估。SiamR-CNN基本上算是深度孪生卷积网络类跟踪算法的精度巅峰，但于2021年被简单的Transformer跟踪算法超越。*2021年开始，SOT全面进入Transformer时代。* | 
     | ***Deep Learning for Visual Tracking: A Comprehensive Survey.*** <br /> **IEEE TITS, 2022.** Seyed Mojtaba Marvasti-Zadeh, Li Cheng, Hossein Ghanei-Yakhdan, Shohreh Kasae.     |  [[Paper](https://ieeexplore.ieee.org/document/9339950)]   |  **:star2:非常详尽的深度学习类跟踪算法综述**， 从网络结构，网络利用，网络训练，网络目标，网络输出，深度学习与相关滤波，长时跟踪，在线更新跟踪等多个维度详尽地综述了2013-2020年的深度学习类跟踪算法。<br /> *2019-2020时的深度学习类跟踪相关已显著超越相关滤波结合深度特征类算法，SOT已彻底全面步入深度学习时代。* |   
     | ***Handcrafted and Deep Trackers: Recent Visual Object Tracking Approaches and Trends.*** <br />  **ACM CS, 2019.** Mustansar Fiaz, Arif Mahmood, Sajid Javed, Soon Ki Jung.     |  [[Paper](https://dl.acm.org/doi/abs/10.1145/3309665)]   |  主要综述了2018年之前的相关滤波类算法和非相关滤波类算法，对2015-2018年提出的相关滤波类算法综述较为详尽。<br />  *深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Deep Visual Tracking: Review and Experimental Comparison.*** <br />  **PR, 2018.** Peixia Li, Dong Wang, Lijun Wang, Huchuan Lu.    |  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320317304612)]   |   主要综述了早期深度学习跟踪算法，从网络结构，网络形式，网络训练三个角度进行了细致的分析。当时，在端到端深度跟踪算法和传统跟踪算法结合深度特征还平分秋色；2019年后，端到端深度跟踪算法占据绝对统治地位。<br /> *深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Object Tracking Benchmark.*** <br />  **IEEE TPAMI, 2015.** Yi Wu, Jongwoo Lim, Ming-Hsuan Yang. |  [[Paper](https://ieeexplore.ieee.org/document/7001050)] <br /> [[Website](http://cvlab.hanyang.ac.kr/tracker_benchmark/)]   | **跟踪领域最经典Benchmark：OTB-100**，同样也是2013年及之前跟踪算法很好的总结，推动了跟踪算法评测的标准化，提出的**Precision和Success**指标现在仍是主流评测指标。评测了29个代表性的Trackers，但排名未进前5的CSK算法在结合了HOG特征之后，成为了2015-2019年最主要的主流算法，即相关滤波算法。| 
     | ***Understanding and Diagnosing Visual Tracking Systems.*** <br /> **ICCV, 2015.**  Naiyan Wang, Jianping Shi, Dit-Yan Yeung, Jiaya Jia.   | [[Paper](https://ieeexplore.ieee.org/document/7410712)] <br />  [[Website](http://www.winsty.net/tracker_diagnose.html)]  | 一份非常值得读的早期跟踪系统解析报告，重要结论：跟踪器性能**特征为王**，运动模型不那么重要（这个其实有数据集偏见在里面）。对现在SOT等相关领域研究也有启发意义。如果发现**所选用的特征**落后时代了，那么把外观模型（公式或结构）搞的再花哨也是意义不大的。|  
     | ***Visual Tracking: An Experimental Survey.*** <br /> **IEEE TPAMI, 2014.**  Arnold W. M. Smeulders, Dung Manh Chu, Rita Cucchiara, et al.   | [[Paper](https://ieeexplore.ieee.org/document/6671560)]    | 早期的跟踪评估综述，主要总结和评估了2012年前的知名算法。提出了有315个视频的评测数据集ALOV++，但由于在CVPR2013和TPAMI2015上发表和扩充的OTB数据库和评测标准更受研究者欢迎，ALOV++现在鲜有人用，而OTB已成为业内标准之一。   |   
     | ***Sparse Coding Based Visual Tracking: Review and Experimental Comparison.*** <br /> **PR, 2013**.  Shengping Zhang, Hongxun Yao, Xin Sun, Xiusheng Lu.   | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320312004396)]    |  稀疏表示跟踪算法的综述，稀疏表示类跟踪算法大约集中在2009-2013年，当时稀疏表示的冗余字典表示，遮挡建模，多任务建模，稀疏编码特征具有一定的优势。*但后来精度和速度均完败于**KCF**，被历史淘汰。*  |   
     | ***A Survey of Appearance Models in Visual Object Tracking.*** <br /> **ACM TIST, 2013.** Xi Li, Weiming Hu, Chunhua Shen, Zhongfei Zhang, et al.   | [[Paper](https://dl.acm.org/doi/10.1145/2508037.2508039)]   |  早期跟踪算法的综述，主要总结了2012年及之前的跟踪算法。 **当时跟踪算法主要分为：生成模型和判决模型两大流派。** **生成模型**流派主要以混合高斯，核密度估计，子空间学习，稀疏表示等为主，特点是建模目标本身，不关心背景信息；**判决模型**流派主要以各种在线分类器，判决性子空间和字典学习等为主，特点是同时建模目标和背景，强调目标和背景的区分。*后来判决模型占据主流，甚至一统SOT江湖。*  |  
     | ***Object Tracking: A Survey.*** <br /> **ACM CS, 2006.**  lper Yilmaz, Omar Javed, Mubarak Shah.   |  [[Paper](https://dl.acm.org/doi/10.1145/1177352.1177355)]   |远古时期跟踪的综述。(1) 从目标表示角度分类：中心点，多关键点，矩形框，椭圆框，多块结构，骨架，边界控制点，边界轮廓，剪影（和Mask类似）； **后来矩形框和分割Mask成为目标表示的主流** (2) 从跟踪算法的角度分类：点跟踪，核跟踪（代表性算法Meanshift, KLT, Eigentracking, SCM），剪影跟踪; **后来点跟踪更多发展为特征点跟踪，应用于SLAM等领域；核跟踪成为SOT的主流（虽然叫法不同）；剪影跟踪发展成为了基于分割的跟踪或视频分割任务。**    |

* **历年[VOT](https://www.votchallenge.net/)冠军算法**

     | **年份**              | **赛道**    | **冠军简介**    |
     |:-----------           |:----------------|:----------------|    
     | [**VOT2021**](https://www.votchallenge.net/vot2021/)  | RGBD | |  
     | [**VOT2021**](https://www.votchallenge.net/vot2021/)  | LT | |     
     | [**VOT2021**](https://www.votchallenge.net/vot2021/)  | RT | |     
     | [**VOT2021**](https://www.votchallenge.net/vot2021/)  | ST | |     
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | RGBD | |
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | RGBT | |
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | LT | |
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | RT | |
     | [**VOT2020**](https://www.votchallenge.net/vot2020/)  | ST | |
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | RGBD | --From [《VOT2019 Report》](https://prints.vicos.si/publications/375)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。**|
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | RGBT | --From [《VOT2019 Report》](https://prints.vicos.si/publications/375)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。**|
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | LT |--From [《VOT2019 Report》](https://prints.vicos.si/publications/375)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。** |
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | RT | --From [《VOT2019 Report》](https://prints.vicos.si/publications/375)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。**|
     | [**VOT2019**](https://www.votchallenge.net/vot2019/)  | ST | --From [《VOT2019 Report》](https://prints.vicos.si/publications/375)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。**|
     | [**VOT2018**](https://www.votchallenge.net/vot2018/)  | LT | **MBMD**( MobileNet based tracking by detection algorithm)：The proposed tracker consists of a bounding box regression network and a verifier network. The regression network regresses the target object’s bounding box in a search region given the target in the first frame. Its outputs are several candidate boxes and each box’s reliability is evaluated by the verifier todetermine the predicted target box. If the predicted scores of both networks are below the thresholds, the tracker searches the target in the whole image. The regression network uses SSD-MobileNet architecture [[35](https://arxiv.org/abs/1704.04861),[52](https://link.springer.com/chapter/10.1007/978-3-319-46448-0_2)] and its parameters are fixed during online tracking. The verifier is similar to MDNet [[64](https://openaccess.thecvf.com/content_cvpr_2016/html/Nam_Learning_Multi-Domain_Convolutional_CVPR_2016_paper.html)] and is implemented by VGGM pretrained on ImageNet classification dataset. The last three layers’ parameters of the verifier are updated online to filter the distractors for the tracker. --From [《VOT2018 Report》](https://prints.vicos.si/publications/365)<br />**核心：[MBMD算法](https://arxiv.org/abs/1809.04320)，滑动窗搜索+类SiamRPN回归+MDNet验证，但速度慢。改进算法[SPLT](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)精度类似，速度可达到实时，发表于[ICCV2019](https://openaccess.thecvf.com/content_ICCV_2019/html/Yan_Skimming-Perusal_Tracking_A_Framework_for_Real-Time_and_Robust_Long-Term_Tracking_ICCV_2019_paper.html)。** |
     | [**VOT2018**](https://www.votchallenge.net/vot2018/)  | RT | **SiamRPN**(High Performance Visual Tracking with Siamese Region Proposal Network)：The tracker SiamRPN consists of a Siamese sub-network for feature extraction and a region proposal sub-network including the classification branch and regression branch. In the inference phase, the proposed framework is formulated as a local one-shot detection task. The template branch of the Siamese subnetwork is pre-computed while correlation layers are formulated as convolution layers to perform online tracking [[48](https://ieeexplore.ieee.org/document/8579033)]. What is more, SiamRPN introduces an effective sampling strategy to control the imbalanced sample distribution and make the model focus on the semantic distractors [[102](https://link.springer.com/chapter/10.1007/978-3-030-01240-3_7)]. --From [《VOT2018 Report》](https://prints.vicos.si/publications/365)<br />**核心：[SiamRPN跟踪框架](https://ieeexplore.ieee.org/document/8579033)，Siamese网络特征提取，互相关融合模板与搜索区域，RPN生成候选，分类回归头输出目标位置，发表于[CVPR2018](https://ieeexplore.ieee.org/document/8579033)。** |     
     | [**VOT2018**](https://www.votchallenge.net/vot2018/)  | ST | **MFT**(Multi-solution Fusion for Visual Tracking)：MFT tracker is based on correlation filtering algorithm. Firstly, different multi-resolution features with continuous convolution operator [[15](https://ieeexplore.ieee.org/document/8100216)] are combined. Secondly, in order to improve the robustness a multi-solution using different features is trained and multi-solutions are optimally fused to predict the target location. Lastly, different combinations of Res50, SE-Res50, Hog, and CN features are applied to the different tracking situations. --From [《VOT2018 Report》](https://prints.vicos.si/publications/365)<br />**核心：相关滤波结合多种深浅层特征。** |
     | [**VOT2017**](https://www.votchallenge.net/vot2017/)  | TIR | **DSLT**(Dense Structural Learning based Tracker)：DSLT extends Struck with the ability to learn from dense samples and high dimensional features. DSLT runs in a simple tracking by detection mode, with no scale adaptation and occlusion handling. Compared to our initial work [[79](https://www.sciencedirect.com/science/article/abs/pii/S0167865517301654)], the feature representation in DSLT consists of 28D HOG features computed without block normalization as well as a 1D motion feature which is simply the absolute difference between consecutive frames. The search range is also set larger to account for faster motion and to get more training samples. --From [《VOT2017 Report》](https://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w28/Kristan_The_Visual_Object_ICCV_2017_paper.pdf)<br />**核心：[DSLT算法](https://www.sciencedirect.com/science/article/abs/pii/S0167865517301654)，密集采样，Structured SVM和相关滤波相结合，发表于[PRL2018](https://www.sciencedirect.com/science/article/abs/pii/S0167865517301654)。** | 
     | [**VOT2017**](https://www.votchallenge.net/vot2017/)  | RT | **SiamFC**(Fully-Convolutional Siamese Network)：SiamFC [[5](https://link.springer.com/chapter/10.1007/978-3-319-48881-3_56)] applies a fully-convolutional Siamese network trained to locate an exemplar image within a larger search image. The network is fully convolutional with respect to the search image: dense and efficient slidingwindow evaluation is achieved with a bilinear layer that computes the cross-correlation of two inputs. The deep conv-net is trained offline on the ILSVRC VID dataset [[56](https://link.springer.com/article/10.1007/s11263-015-0816-y)] to address a general similarity learning problem. This similarity function is then used within a simplistic tracking algorithm. The architecture of the conv-net resembles ‘AlexNet’ [[34](https://papers.nips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html)]. This version of SiamFC incorporates some minor improvements and is available as the baseline model of the CFNet paper [[64](https://openaccess.thecvf.com/content_cvpr_2017/html/Valmadre_End-To-End_Representation_Learning_CVPR_2017_paper.html)]. --From [《VOT2017 Report》](https://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w28/Kristan_The_Visual_Object_ICCV_2017_paper.pdf)<br />**核心：[SiamFC算法](https://link.springer.com/chapter/10.1007/978-3-319-48881-3_56)，Siamese Tracking鼻祖，发表于[ECCVW2016](https://link.springer.com/chapter/10.1007/978-3-319-48881-3_56)。** |   
     | [**VOT2017**](https://www.votchallenge.net/vot2017/)  | ST | **CFCF**(Convolutional Features for Correlation Filters)：The tracker ‘CFCF’ is based on the feature learning study in [[23](https://ieeexplore.ieee.org/abstract/document/8291524)] and the correlation filter based tracker in [[17](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_29)]. The proposed tracker employs a fully convolutional neural network (CNN) model trained on ILSVRC15 [[56](https://link.springer.com/article/10.1007/s11263-015-0816-y)] video dataset by the introduced learning framework in [[23](https://ieeexplore.ieee.org/abstract/document/8291524)]. This framework is designed for correlation filter formulation in [[13](http://www.bmva.org/bmvc/2014/papers/paper038/index.html)]. To learn features, convolutional layers of VGGM-2048 network [[10](http://www.bmva.org/bmvc/2014/papers/paper054/index.html)], which is trained on [18], with an extra convolutional layer is fine-tuned on ILSVRC15 dataset. The first, fifth and sixth convolutional layers of the learned network, HOG [[47](https://ieeexplore.ieee.org/document/1467360)] and Colour Names (CN) [[65](https://ieeexplore.ieee.org/document/4982667)] are integrated to the tracker of [[17](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_29)]. The reader is referred to [[23](https://ieeexplore.ieee.org/abstract/document/8291524)] for details. --From [《VOT2017 Report》](https://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w28/Kristan_The_Visual_Object_ICCV_2017_paper.pdf)<br />**核心：相关滤波结合浅深层特征。** |   
     | [**VOT2016**](https://www.votchallenge.net/vot2016/)  | TIR | **EBT**(Edge Box Tracker)：EBT tracker is not limited to a local search window and has ability to probe efficiently the entire frame. It generates a small number of ‘high-quality’ proposals by a novel instance-specific objectness measure and evaluates them against the object model that can be adopted from an existing tracking-by-detection approach as a core tracker. During the tracking process, it updates the object model concentrating on hard false-positives supplied by the proposals, which help suppressing distractors caused by difficult background clutters, and learns how to re-rank proposals according to the object model. Since the number of hypotheses the core tracker evaluates is reduced significantly, richer object descriptors and stronger detectors can be used. More details can be found in [[25](https://ieeexplore.ieee.org/document/7780477)]. --From [《VOT-TIR2016 Report》](https://data.votchallenge.net/vot2016/presentations/vot_tir_2016_paper.pdf)<br />**核心：[EBT算法](https://ieeexplore.ieee.org/document/7780477)，Edge Box提取全局Proposal，在线更新Structured SVM分类，发表于[CVPR2016](https://ieeexplore.ieee.org/document/7780477)。**  |  
     | [**VOT2016**](https://www.votchallenge.net/vot2016/)  | ST | **TCNN**(Tree-structured Convolutional Neural Network Tracker)：TCNN [[96](https://arxiv.org/abs/1608.07242)] maintains multiple target appearance models based on CNNs in a tree structure to preserve model consistency and handle appearance multi-modality effectively. TCNN tracker consists of two main components, state estimation and model update. When a new frame is given, candidate samples around the target state estimated in the previous frame are drawn, and the likelihood of each sample based on the weighted average of the scores from multiple CNNs is computed. The weight of each CNN is determined by the reliability of the path along which the CNN has been updated in the tree structure. The target state in the current frame is estimated by finding the candidate with the maximum likelihood. After tracking a predefined number of frames, a new CNN is derived from an existing one, which has the highest weight among the contributing CNNs to target state estimation.-From [《VOT2016 Report》](https://data.votchallenge.net/vot2016/presentations/vot_2016_paper.pdf)<br />**核心：[TCNN算法](https://arxiv.org/abs/1608.07242)，稀疏候选采样，树结构集成CNN分类及在线更新。**  | 
     | [**VOT2015**](https://www.votchallenge.net/vot2015/)  | TIR | **sPST**(simplified Proposal Selection Tracker)：The simplified Proposal Selection Tracker (sPST) is based on our ICCV2015 paper [[21](https://ieeexplore.ieee.org/document/7410711)]. sPST operates in two phases. Firstly, we propose a set of candidate object locations computed by tracking-by-detection framework [[35](https://ieeexplore.ieee.org/document/6619152/)], where we use the frame as is and rotate them according to the ground truth annotation in the initial frame if applicable. Secondly, we determine the best candidate as the tracking result by two cues: detection confidence score and an objectness measure computed with edges [[48](https://link.springer.com/chapter/10.1007/978-3-319-10602-1_26)]. Note that the full version of our tracker uses additional proposals and motion boundaries calculated with optical flow. But it is not included in this submission due to the computational cost of the optical flow method. The reader is referred to [[21](https://ieeexplore.ieee.org/document/7410711)] for details.--From [《VOT-TIR2015 Report》](https://data.votchallenge.net/vot2015/presentations/vot_tir_2015_paper.pdf)<br />**核心：[PST算法](https://ieeexplore.ieee.org/document/7410711)，先生成Proposal再利用SVM检测置信值+Objectness来选择，发表于[ICCV2015](https://ieeexplore.ieee.org/document/7410711)。**|
     | [**VOT2015**](https://www.votchallenge.net/vot2015/)  | ST | **MDNet**(Multi-Domain Convolutional Neural Network Tracker)：MDNet tracker represents the target object using a Convolutional Neural Network (CNN). MDNet pre-trains the CNN using a set of videos with tracking ground-truth annotations to obtain a generic representation for an arbitrary new sequence. The network is composed of two partsshared layers and domain specific layers, where domains correspond to individual tracking sequences and each domain has a separate branch for binary classification. After training, a generic representation in the shared layers across all domains is obtained. The tracking is performed by sampling target candidates around the previous target state, evaluating them on the CNN, and identifying the sample with the maximum score. For more details, the interested reader is referred to [[52](https://arxiv.org/pdf/1510.07945.pdf)].--From [《VOT2015 Report》](https://data.votchallenge.net/vot2015/presentations/vot_2015_paper.pdf)<br />**核心：[MDNet算法](https://openaccess.thecvf.com/content_cvpr_2016/html/Nam_Learning_Multi-Domain_Convolutional_CVPR_2016_paper.html)，早期经典深度学习跟踪算法，利用稀疏采样+深度分类，发表于[CVPR2016](https://openaccess.thecvf.com/content_cvpr_2016/html/Nam_Learning_Multi-Domain_Convolutional_CVPR_2016_paper.html)。**|
     | [**VOT2014**](https://www.votchallenge.net/vot2014/)  | ST | **DSST**(Discriminative Scale Space Tracker)：The Discriminative Scale Space Tracker (DSST) [[14](http://www.bmva.org/bmvc/2014/papers/paper038/index.html)]  extends the Minimum Output Sum of Squared Errors (MOSSE) tracker [[5](https://ieeexplore.ieee.org/document/5539960/)] with robust scale estimation. The MOSSE tracker works by training a discriminative correlation filter on a set of observed sample grey scale patches. This correlation filter is then applied to estimate the target translation in the next frame. The DSST additionally learns a one-dimensional discriminative scale filter, that is used to estimate the target size. For the translation filter, the intensity features employed in the MOSSE tracker is combined with a pixel-dense representation of HOG-features.  --From [《VOT2014 Report》](https://www.votchallenge.net/vot2014/download/vot_2014_paper.pdf)<br /> **核心：相关滤波算法[DSST](http://www.bmva.org/bmvc/2014/papers/paper038/index.html)，发表于[BMVC2014](http://www.bmva.org/bmvc/2014/papers/paper038/index.html)。**|
     | [**VOT2013**](https://www.votchallenge.net/vot2013/)  | ST | **PLT**(Single scale pixel based LUT tracker)：PLT runs a classifier at a fixed single scale for each test image, to determine the top scoring bounding box which is then the result of object detection. The classifier uses a binary feature vector constructed from color, grayscale and gradient information. To select a small set of discriminative features, an online sparse structural SVM [[20](https://ieeexplore.ieee.org/document/6126251)] is used. Since the object can be non-rigid and the bounding box may be noisy, not all pixels in the bounding box belong to the object. Hence, a probabilistic object-background segmentation mask from color histograms is created and used to weight the features during SVM training. The resulting weighted and convex problem can be solved in three steps: (i) compute the probability that a pixel belongs to the objectby using its color. (ii) solve the original non-sparse structural SVM and (iii) shrink the solution [[21](https://ieeexplore.ieee.org/document/6248061)], i.e. features with smallest values are discarded. Since the feature vector is binary, the linear classifier can be implemented as a lookup table for fast speed.  --From [《VOT2013 Report》](https://www.votchallenge.net/vot2013/Download/vot_2013_paper.pdf) <br /> **核心：在线结构SVM分类器，[Struck](https://ieeexplore.ieee.org/document/6126251)跟踪算法，发表于[CVPR2011](https://ieeexplore.ieee.org/document/6126251)。**|

* **在线学习/报告资源**

     | **视频/博客**              | 内容摘要    |
     |:-----------               |:----------------:|
     |**[叫我林林就行](https://space.bilibili.com/209664735/)：[Github](https://github.com/HonglinChu), [B站视频](https://space.bilibili.com/209664735/)** |CF和Siamese系列工作介绍复现；轻量级跟踪器NanoTrack|
     |**[东大阿德](https://space.bilibili.com/6794832/)：[单目标跟踪零基础代码入门-B站视频](https://space.bilibili.com/6794832/channel/collectiondetail?sid=400776)** |SiamFC, SiamRPN, pytracking系列代码讲解；RGBT跟踪介绍|
     |**[深度大脑](https://space.bilibili.com/9456738)：[从零开始的单目标跟踪算法世界-B站视频](https://www.bilibili.com/video/BV1WK4y1C7JG)** |pytracking系列代码讲解|
     |**[VALSE_Webinar](https://space.bilibili.com/562085182/)(跟踪问题)：[B站视频](https://space.bilibili.com/562085182/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |基础知识，前沿报告，论文速览；公众号：VALSE |
     |**[极市平台](https://space.bilibili.com/85300886/)(跟踪问题)：[B站视频](https://space.bilibili.com/85300886/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |部分原作者论文报告；公众号：极市平台|
     |**[AITracker](https://space.bilibili.com/8948069)：[B站视频](https://space.bilibili.com/8948069)** |系列讲座，经验分享；公众号：目标跟踪与检测基础前沿|
     |**[人工智能前沿讲习](https://bbs.sffai.com/)(跟踪问题)：[B站视频](https://space.bilibili.com/388690539/search/video?keyword=%E8%B7%9F%E8%B8%AA)** |系列讲座，经验分享；公众号：人工智能前沿讲习|
     |**[YaqiLYU(知乎)](https://www.zhihu.com/people/YaqiLYU)：[深度学习和目标跟踪(知乎专栏)](https://www.zhihu.com/column/DCF-tracking)** |算法总结感悟，移动端跟踪|
     |**[NTRのSAO年(B站)](https://space.bilibili.com/5567932)：[B站专栏](https://space.bilibili.com/5567932/article)** |部分论文速览|
