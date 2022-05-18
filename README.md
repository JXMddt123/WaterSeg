# Collision-Free Waterway Segmentation for Inland
Unmanned Surface Vehicles (TIM2022)

Implementation for **[CPWaterSeg](https://ieeexplore.ieee.org/document/9755264)**.

![fig2](https://github.com/JXMddt123/WaterSeg/blob/master/figs/fig2.png)

![fig3](https://github.com/JXMddt123/WaterSeg/blob/master/figs/fig3.png)

## Summary

Accurate detection of passable regions in images is important for ensuring the safe navigation of unmanned surface vehicles, especially in inland waterways with irregular waterlines and various obstacles. However, the existing methods are susceptible to environmental changes and produce high false-positive rates (FPR) for confusable textures and complex edge details. We therefore propose a collision-free waterway segmentation network based on deep learning such that pixel-level classification results can be obtained. The segmentation accuracy for indistinguishable textures is improved by learning the context dependency of features through a modified context prior, and the detail refinement of waterlines and small obstacles is achieved via an asymmetric encoder–decoder structure. To learn the features of waterways as comprehensively as possible, data integration and data augmentation are performed on three public datasets. In addition, a new annotated urban waterway dataset called Dasha River Dataset is proposed and made publicly available. The proposed model is tested and cross validated using multiple inland and maritime water segmentation datasets, the results of which show that the model achieves a superior performance than the current state of art with pixel accuracy (PA) of 97.43% and FPR of 1.37%.

## Dataset

The dataset used in this project is available at:

- [Dasha River](https://ieee-dataport.org/documents/dasha-river-dataset)
- [MaSTr1325](http://box.vicos.si/borja/mastr1325_dataset/)
- [IntCatch](http://profs.scienze.univr.it/farinelli/intcatchvisiondb/intcatchvisiondb.html/)
- [Tampere-WaterSeg](https://etsin.fairdata.fi/dataset/e0c6ef65-6e1e-4739-abe3-0455697df5ab)
- [ORCA](https://www.orca-tech.cn/datasets)

## News
- A simple version of the core codes has been released. It is based on mmsegmentation. You can integrate the codes into mmseg to run the experiments.

## Citation

Please consider citing the article in your publications if it helps your research.

```
@ARTICLE{zhou2021CPWaterSeg,
  title={Collision-Free Waterway Segmentation for Inland Unmanned Surface Vehicles}, 
  author={Zhou, Rundong and Gao, Yulong and Wu, Peng and Zhao, Xiongwei and Dou, Wenhao and Sun, Chenyang and Zhong, Yu and Wang, Yang},
  journal={IEEE Transactions on Instrumentation and Measurement}, 
  year={2022},
  pages={1-1},
  doi={10.1109/TIM.2022.3165803}}
```