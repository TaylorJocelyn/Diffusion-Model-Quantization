# Diffusion-Model-Quantization <img class="emoji" alt=":art:" height="30" width="30" src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a8.png">
Selected papers, corresponding codes and pre-trained models in our review paper
 <!-- **"Neural Style Transfer: A Review" [[arXiv Version]](https://arxiv.org/abs/1705.04058) [[IEEE Version]](https://ieeexplore.ieee.org/document/8732370)** -->

 *If I missed your paper in this review, please email me or just pull a request here. I am more than happy to add it. Thanks!*

<!-- 
## Citation 
If you find this repository useful for your research, please consider citing

```
@article{jing2019neural,
  title={Neural Style Transfer: A Review},
  author={Jing, Yongcheng and Yang, Yezhou and Feng, Zunlei and Ye, Jingwen and Yu, Yizhou and Song, Mingli},
  journal={IEEE Transactions on Visualization and Computer Graphics},
  year={2019}
}
```
Please also consider citing our ECCV paper and AAAI (Oral) paper:

```
@inproceedings{jing2018stroke,
  title={Stroke Controllable Fast Style Transfer with Adaptive Receptive Fields},
  author={Jing, Yongcheng and Liu, Yang and Yang, Yezhou and Feng, Zunlei and Yu, Yizhou and Tao, Dacheng and Song, Mingli},
  booktitle={ECCV},
  year={2018}
}
```
```
@inproceedings{jing2020dynamic,
  title={Dynamic Instance Normalization for Arbitrary Style Transfer},
  author={Jing, Yongcheng and Liu, Xiao and Ding, Yukang and Wang, Xinchao and Ding, Errui and Song, Mingli and Wen, Shilei},
  booktitle={AAAI},
  year={2020}
}
```

Thanks! -->


---

## *News!*

- [April, 2025] Published a review! Summarized the current mainstream quantization methods for diffusion models.

<p align='center'>
    </br>
    <img src='framework.png' width='1000'>
</p>

<!-- ## Materials corresponding to Our Paper

:white_check_mark: [**Supplementary Material (TVCG)**](https://drive.google.com/file/d/1_VTS4rUSl488wgSrz2K5BfKra33gvaHH/view?usp=sharing)

:white_check_mark: [**Pre-trained Models**](https://www.dropbox.com/s/37lje23pb75ecob/Models_neuralStyleTransferReview.zip?dl=0)

:white_check_mark: [**Images (TVCG)(.png)**](https://drive.google.com/file/d/14RN0GN09-rordzRqp4o8oU30BB7uiNcj/view?usp=sharing) -->

## A Taxonomy of Contemporary Approaches

### 1. Unet-based Diffusion Quantization
###  1.1. Calibration Strategy Customization

:white_check_mark: [**Post-training Quantization on Diffusion Models**] [Paper](https://arxiv.org/abs/2211.15736) *(CVPR2023, First Diffusion Quantization Paper)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/42shawn/ptq4dm)

:white_check_mark: [**EDA-DM: Enhanced Distribution Alignment for Post-Training Quantization of Diffusion Models**] [Paper](https://arxiv.org/abs/2401.04585) 

:sparkle: **Code:**
*   [Torch-based](https://github.com/BienLuky/EDA-DM)

### 1.2. Bi-modal Distribution Elimination

:white_check_mark: [**Q-Diffusion: Quantizing Diffusion Models**] [Paper](https://arxiv.org/abs/2302.04304) *(ICCV 2023)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/Xiuyu-Li/q-diffusion) 

### 1.3 Dynamic Quantization

:white_check_mark: [**Temporal Dynamic Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2306.02316) *(NeurIPS 2023)*

### 1.4 Time Information Align

:white_check_mark: [**TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2311.16503) *(CVPR 2024, Highlight)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/ModelTC/TFMQ-DM) 

:white_check_mark: [**QVD: Post-training Quantization for Video Diffusion Models**] [Paper](https://arxiv.org/abs/2407.11585) *(ACM MM 2024)*

### 1.5 Quantization Error Correction

:white_check_mark: [**QNCD: Quantization Noise Correction for Diffusion Models**] [Paper](https://arxiv.org/abs/2403.19140) *(ACM MM 2024)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/huanpengchu/qncd) 

:white_check_mark: [**PTQD: Accurate Post-Training Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2305.10657) *(NeurIPS 2024)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/ziplab/ptqd) 

:white_check_mark: [**Softmax Bias Correction for Quantized Generative Models**] [Paper](https://arxiv.org/abs/2309.01729) *(ICCV 2023, Workshop)*

:white_check_mark: [**D$^2$-DPM: Dual Denoising for Quantized Diffusion Probabilistic Models**] [Paper](https://arxiv.org/abs/2501.08180) *(AAAI 2025)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/taylorjocelyn/d2-dpm) 

:white_check_mark: [**Timestep-Aware Correction for Quantized Diffusion Models**] [Paper](https://arxiv.org/abs/2407.03917) *(ECCV 2024)*

### 1.6 Holistic QAT Optimization

:white_check_mark: [**Q-DM: An Efficient Low-bit Quantized Diffusion Model**] [Paper](https://openreview.net/forum?id=sFGkL5BsPi) *(NeurIPS 2023)*

:white_check_mark: [**QuEST: Low-bit Diffusion Model Quantization via Efficient Selective Finetuning**] [Paper](https://arxiv.org/abs/2402.03666)

:sparkle: **Code:**
*   [Torch-based](https://github.com/hatchetProject/QuEST) 

:white_check_mark: [**Memory-Efficient Fine-Tuning for Quantized Diffusion Model**] [Paper](https://arxiv.org/abs/2401.04339) *(ECCV 2024)*

### 1.7 Ultra-Low-Bit DMs

:white_check_mark: [**Binary Latent Diffusion**] [Paper](https://arxiv.org/abs/2304.04820)

:white_check_mark: [**BiDM: Pushing the Limit of Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2412.05926)

:sparkle: **Code:**
*   [Torch-based](https://github.com/xingyu-zheng/bidm) 

:white_check_mark: [**Binarydm: Towards accurate binarization of diffusion model**] [Paper](https://arxiv.org/abs/2404.05662v1)

:sparkle: **Code:**
*   [Torch-based](https://github.com/xingyu-zheng/binarydm) 

:white_check_mark: [**BitsFusion: 1.99 bits Weight Quantization of Diffusion Model**] [Paper](https://arxiv.org/abs/2406.04333) *(NeurIPS 2024)*


:white_check_mark: [**Binarized Diffusion Model for Image Super-Resolution**] [Paper](https://arxiv.org/abs/2406.05723)

:sparkle: **Code:**
*   [Torch-based](https://github.com/zhengchen1999/bi-diffsr)

### 1.8 LoRA-Based Enhancements

:white_check_mark: [**EfficientDM: Efficient Quantization-Aware Fine-Tuning of Low-Bit Diffusion Models**] [Paper](https://arxiv.org/abs/2310.03270) *(ICLR 2024)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/thisisbillhe/efficientdm) 

:white_check_mark: [**IntLoRA: Integral Low-rank Adaptation of Quantized Diffusion Models**] [Paper](https://arxiv.org/abs/2410.21759) 

:sparkle: **Code:**
*   [Torch-based](https://github.com/csguoh/intlora) 



### 2. Diffusion-Transformer(DiT) Quantization

### 2.1 Group-wise Quantization

:white_check_mark: [**An Analysis on Quantizing Diffusion Transformers**] [Paper](https://arxiv.org/abs/2406.11100) *(CVPR workshop)*


:white_check_mark: [**Q-DIT: ACCURATE POST-TRAINING QUANTIZATION FOR DIFFUSION TRANSFORMERS**] [Paper](https://arxiv.org/abs/2406.17343) *(CVPR 2025)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/juanerx/q-dit) 

### 2.2 Channel Equalization

:white_check_mark: [**PTQ4DiT: Post-training Quantization for Diffusion Transformers**] [Paper](https://arxiv.org/abs/2405.16005) *(NerIPS 2024)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/adreamwu/ptq4dit) 

:white_check_mark: [**DiTAS: Quantizing Diffusion Transformers via Enhanced Activation Smoothing**] [Paper](https://arxiv.org/abs/2409.07756) *(WACV 2025)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/DZY122/DiTAS) 

:white_check_mark: [**ViDiT-Q: Efficient and Accurate Quantization of Diffusion Transformers for Image and Video Generation**] [Paper](https://arxiv.org/abs/2406.02540) *(ICLR 2025)*

:sparkle: **Code:**
*   [Torch-based](https://github.com/a-suozhang/vidit-q) 

:white_check_mark: [**HQ-DiT: Efficient Diffusion Transformer with FP4 Hybrid Quantization**] [Paper](https://arxiv.org/abs/2405.19751) 


