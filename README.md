# SOT-Learning




* **综述文章**

     | **论文**              | **链接**    | **内容摘要**    |
     |:-----------           |:----------------:|:----------------|
     | ***Deep Learning for Visual Tracking: A Comprehensive Survey.*** <br /> **IEEE TITS, 2022.** Seyed Mojtaba Marvasti-Zadeh, Li Cheng, Hossein Ghanei-Yakhdan, Shohreh Kasae.     |  [[Paper](https://ieeexplore.ieee.org/document/9339950)]   |  **非常详尽的深度学习类跟踪算法综述**， 从网络结构，网络利用，网络训练，网络目标，网络输出，深度学习与相关滤波，长时跟踪，在线更新跟踪等多个维度详尽地综述了2013-2020年的深度学习类跟踪算法。  |  
     | ***Correlation Filters for Unmanned Aerial Vehicle-Based Aerial Tracking: A Review and Experimental Evaluation.*** <br />  **IEEE GRSM, 2021.** Changhong Fu, Bowen Li, Fangqiang Ding, Fuling Lin, Geng Lu.     |  [[Paper](https://dl.acm.org/doi/abs/10.1145/3309665)] <br /> [[Website](https://github.com/vision4robotics/DCFTracking4UAV)]  |  主要综述了2018年之前的相关滤波类算法和非相关滤波类算法，对2015-2018年提出的相关滤波类算法综述较为详尽。|  
     | ***Handcrafted and Deep Trackers: Recent Visual Object Tracking Approaches and Trends.*** <br />  **ACM CS, 2019.** Mustansar Fiaz, Arif Mahmood, Sajid Javed, Soon Ki Jung.     |  [[Paper](https://dl.acm.org/doi/abs/10.1145/3309665)]   |  主要综述了2018年之前的相关滤波类算法和非相关滤波类算法，对2015-2018年提出的相关滤波类算法综述较为详尽。 *深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Deep Visual Tracking: Review and Experimental Comparison.*** <br />  **PR, 2018.** Peixia Li, Dong Wang, Lijun Wang, Huchuan Lu.    |  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320317304612)]   |   主要综述了早期深度学习跟踪算法，从网络结构，网络形式，网络训练三个角度进行了细致的分析。当时，在端到端深度跟踪算法和传统跟踪算法结合深度特征还平分秋色；2019年后，端到端深度跟踪算法占据绝对统治地位。*深度学习类跟踪算法更推荐看《Deep Learning for Visual Tracking: A Comprehensive Survey》*  |  
     | ***Object Tracking Benchmark.*** <br />  **IEEE TPAMI, 2015.** Yi Wu, Jongwoo Lim, Ming-Hsuan Yang. |  [[Paper](https://ieeexplore.ieee.org/document/7001050)] <br /> [[Website](http://cvlab.hanyang.ac.kr/tracker_benchmark/)]   | **跟踪领域最经典Benchmark：OTB-100**，同样也是2013年及之前跟踪算法很好的总结，推动了跟踪算法评测的标准化，提出的**Precision和Success**指标现在仍是主流评测指标。评测了29个代表性的Trackers，但排名未进前5的CSK算法在结合了HOG特征之后，成为了2015-2019年最主要的主流算法，即相关滤波算法。| 
     | ***Understanding and Diagnosing Visual Tracking Systems.*** <br /> **ICCV, 2015.**  Naiyan Wang, Jianping Shi, Dit-Yan Yeung, Jiaya Jia.   | [[Paper](https://ieeexplore.ieee.org/document/7410712)] <br />  [[Website](http://www.winsty.net/tracker_diagnose.html)]  | 一份非常值得读的早期跟踪系统解析报告，重要结论：跟踪器性能**特征为王**，运动模型不那么重要（这个其实有数据集偏见在里面）。对现在SOT等相关领域研究也有启发意义。如果发现**所选用的特征**落后时代了，那么把外观模型（公式或结构）搞的再花哨也是意义不大的。|  
     | ***Visual Tracking: An Experimental Survey.*** <br /> **IEEE TPAMI, 2014.**  Arnold W. M. Smeulders, Dung Manh Chu, Rita Cucchiara, et al.   | [[Paper](https://ieeexplore.ieee.org/document/6671560)]    | 早期的跟踪评估综述，主要总结和评估了2012年前的知名算法。提出了有315个视频的评测数据集ALOV++，但由于在CVPR2013和TPAMI2015上发表和扩充的OTB数据库和评测标准更受研究者欢迎，ALOV++现在鲜有人用，而OTB已成为业内标准之一。   |   
     | ***Sparse Coding Based Visual Tracking: Review and Experimental Comparison.*** <br /> **PR, 2013**.  Shengping Zhang, Hongxun Yao, Xin Sun, Xiusheng Lu.   | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320312004396)]    |  稀疏表示跟踪算法的综述，稀疏表示类跟踪算法大约集中在2009-2013年，当时稀疏表示的冗余字典表示，遮挡建模，多任务建模，稀疏编码特征具有一定的优势。*但后来精度和速度均完败于**KCF**，被历史淘汰。*  |   
     | ***A Survey of Appearance Models in Visual Object Tracking.*** <br /> **ACM TIST, 2013.** Xi Li, Weiming Hu, Chunhua Shen, Zhongfei Zhang, et al.   | [[Paper](https://dl.acm.org/doi/10.1145/2508037.2508039)]   |  早期跟踪算法的综述，主要总结了2012年及之前的跟踪算法。 **当时跟踪算法主要分为：生成模型和判决模型两大流派。** **生成模型**流派主要以混合高斯，核密度估计，子空间学习，稀疏表示等为主，特点是建模目标本身，不关心背景信息；**判决模型**流派主要以各种在线分类器，判决性子空间和字典学习等为主，特点是同时建模目标和背景，强调目标和背景的区分。*后来判决模型占据主流，甚至一统SOT江湖。*  |  
     | ***Object Tracking: A Survey.*** <br /> **ACM CS, 2006.**  lper Yilmaz, Omar Javed, Mubarak Shah.   |  [[Paper](https://dl.acm.org/doi/10.1145/1177352.1177355)]   |远古时期跟踪的综述。(1) 从目标表示角度分类：中心点，多关键点，矩形框，椭圆框，多块结构，骨架，边界控制点，边界轮廓，剪影（和Mask类似）； **后来矩形框和分割Mask成为目标表示的主流** (2) 从跟踪算法的角度分类：点跟踪，核跟踪（代表性算法Meanshift, KLT, Eigentracking, SCM），剪影跟踪; **后来点跟踪更多发展为特征点跟踪，应用于SLAM等领域；核跟踪成为SOT的主流（虽然叫法不同）；剪影跟踪发展成为了基于分割的跟踪或视频分割任务。**    |

* **在线资源**

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
