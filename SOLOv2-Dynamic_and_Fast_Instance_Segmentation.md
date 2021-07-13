# SOLO v2文献解读
## 基本信息

这是一篇会议论文，发表于NeurlIPS 2020。
第一作者Xinlong Wang和通讯作者Chunhua Shen来自于澳大利亚阿德莱德大学。
第二作者Rufeng Zhang来自于同济大学。第三作者Tao Kong和第四作者Lei Li来自于字节跳动。

本篇文献是SOLO[[arxiv]](https://arxiv.org/pdf/2106.15947.pdf)的姊妹篇。
SOLO发表于ECCV 2020，作者也同样是上述五位研究者。

## 主要内容
1. SOLO创新点
   1. 与Mask RCNN这种“detect-then-segment”模型,或者针对图片的每一个像素先做嵌入，再做聚类的方法都不同, 提出了一种新的名为SOLO的实例分割框架，见于下图：
   ![SOLO Framework](https://github.com/algo-exchange/interpretations/raw/5812bc04b01979bc54296a50882b72095a0b723f/images/solo_framework.png)
   2. 除了提出这一框架之外，基于SOLO，作者还派生出Vanilla SOLO、Decoupled SOLO、和Dynamic SOLO。
   3. 不仅在实例分割上得到应用，还能够用于目标监测、全景分割和抠图。

2. SOLOv2创新点

## 参考的工作
1. SOLO
   1. 在两步分割模型（作者分类为自顶向下的实例分割）类型中，主要参考了FCIS、Mask R-CNN、PANet、Mask Scoring R-CNN、HTC、TensorMask。
   2. 在先嵌入再聚合的分割模型（作者分类为自底向上的实例分割）类型中，则主要参考了SGN、SSAP。
   3. 直接分割模型中，作者引用了AdaptIS和PoloarMask。