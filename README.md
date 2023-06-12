# Generative models that perform diverse style transfer for robust person re-identification
Our project is based on ICCV 2021 paper
[ICE: Inter-instance Contrastive Encoding for Unsupervised Person
Re-identification](https://arxiv.org/pdf/2103.16364.pdf).

[[Video](https://drive.google.com/file/d/1E__ru9u_oRcb44-WIH_GjBTv1-_5rcO2/view?usp=sharing)]   [[Poster](https://drive.google.com/file/d/1HEkgtUCSOixIndH1ClhRZfAQGTIFfY-n/view?usp=sharing)]

![teaser](figs/figure8.png)

## GAN

Camera style transfer

[[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8485427)]
[[Code](https://github.com/zhunzhong07/CamStyle)]

Cloth style transfer

[[Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zheng_Joint_Discriminative_and_Generative_Learning_for_Person_Re-Identification_CVPR_2019_paper.pdf)]
[[Code](https://github.com/NVlabs/DG-Net)]

Pose style transfer

[[Paper](https://openaccess.thecvf.com/content_ECCV_2018/papers/Xuelin_Qian_Pose-Normalized_Image_Generation_ECCV_2018_paper.pdf)]
[[Code](https://github.com/naiq/PN_GAN)]


## Prepare Datasets

Download the raw datasets [Market-1501](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Zheng_Scalable_Person_Re-Identification_ICCV_2015_paper.pdf)
and then unzip them under the directory like
```
ICE/examples/data
├── market1501
└── market1501_transfer
```

## Training
We used **4 GPUs** to train our model.
 
Train [Market-1501](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Zheng_Scalable_Person_Re-Identification_ICCV_2015_paper.pdf):
```
python examples/unsupervised_train.py --dataset-target market1501
```

