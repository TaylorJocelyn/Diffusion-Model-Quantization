# Diffusion-Model-Quantization `<img class="emoji" alt=":art:" height="30" width="30" src="https://github.githubassets.com/images/icons/emoji/unicode/1f3a8.png">`

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

<table>
<tr>
<td>Diffusion Backbone Types</td>
<td>Quantization Methods</td>
<td>Paper&Code</td>
</tr>
<tr>
<td rowspan="22" colspan="1">Unet-based Diffusion Quantization</td>
<td rowspan="2" colspan="1">Calibration Strategy Customization</td>

<td><b>[Post-training Quantization on Diffusion Models]</b>
(<a href="https://arxiv.org/abs/2211.15736" target="_blank" style="color: blue; text-decoration: underline;">Paper</a> ||
<a href="https://github.com/42shawn/ptq4dm" target="_blank" style="color: blue; text-decoration: underline;">Code:Torch-based</a>)
<i>(CVPR2023, First Diffusion Quantization Paper)<i>
</td>

</tr>
<tr>

<td><b>[EDA-DM: Enhanced Distribution Alignment for Post-Training Quantization of Diffusion Models]</b>
(<a href="https://arxiv.org/abs/2401.04585" target="_blank" style="color: blue; text-decoration: underline;">Paper</a> ||
<a href="https://github.com/BienLuky/EDA-DM" target="_blank" style="color: blue; text-decoration: underline;">Code:Torch-based</a>)
<i>(CVPR2023, First Diffusion Quantization Paper)<i>

</td>
</tr>
<tr>
<td rowspan="2" colspan="1">Bi-modal Distribution Elimination</td>
<td rowspan="2" colspan="1">[Q-Diffusion: Quantizing Diffusion Models](ICCV 2023)</td>
</tr>
<tr>
</tr>
<tr>
<td>Dynamic Quantization</td>
<td>[Temporal Dynamic Quantization for Diffusion Models] (NeurIPS 2023)</td>
</tr>
<tr>
<td rowspan="2" colspan="1">Time Information Align</td>
<td>[TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models] (CVPR 2024, Highlight)</td>
</tr>
<tr>
<td>[QVD: Post-training Quantization for Video Diffusion Models](ACM MM 2024)</td>
</tr>
<tr>
<td rowspan="5" colspan="1">Quantization Error Correction</td>
<td>[QNCD: Quantization Noise Correction for Diffusion Models](ACM MM 2024)</td>
</tr>
<tr>
<td>[PTQD: Accurate Post-Training Quantization for Diffusion Models](NeurIPS 2024)</td>
</tr>
<tr>
<td> [Softmax Bias Correction for Quantized Generative Models]  (ICCV 2023, Workshop)</td>
</tr>
<tr>
<td>[D$^2$-DPM: Dual Denoising for Quantized Diffusion Probabilistic Models](AAAI 2025)</td>
</tr>
<tr>
<td>[Timestep-Aware Correction for Quantized Diffusion Models](ECCV 2024) </td>
</tr>
<tr>
<td rowspan="3" colspan="1">Holistic QAT Optimization</td>
<td>[Q-DM: An Efficient Low-bit Quantized Diffusion Model] (NeurIPS 2023)</td>
</tr>
<tr>
<td>[QuEST: Low-bit Diffusion Model Quantization via Efficient Selective Finetuning]</td>
</tr>
<tr>
<td>[Memory-Efficient Fine-Tuning for Quantized Diffusion Model] (ECCV2024)</td>
</tr>
<tr>
<td rowspan="5" colspan="1">Ultra-Low-Bit DMs</td>
<td>[Binary Latent Diffusion]</td>
</tr>
<tr>
<td>[BiDM: Pushing the Limit of Quantization for Diffusion Models] </td>
</tr>
<tr>
<td>[Binarydm: Towards accurate binarization of diffusion model]</td>
</tr>
<tr>
<td> [BitsFusion: 1.99 bits Weight Quantization of Diffusion Model] (NeurIPS 2024)</td>
</tr>
<tr>
<td>[Binarized Diffusion Model for Image Super-Resolution] </td>
</tr>
<tr>
<td rowspan="2" colspan="1">LoRA-Based Enhancements</td>
<td>[EfficientDM: Efficient Quantization-Aware Fine-Tuning of Low-Bit Diffusion Models](ICLR 2024)</td>
</tr>
<tr>
<td>[IntLoRA: Integral Low-rank Adaptation of Quantized Diffusion Models]</td>
</tr>
<tr>
<td rowspan="6" colspan="1">Diffusion-Transformer(DiT) Quantization</td>
<td rowspan="2" colspan="1">Group-wise Quantization</td>
<td> [An Analysis on Quantizing Diffusion Transformers]   (CVPR workshop)</td>
</tr>
<tr>
<td>[Q-DIT: ACCURATE POST-TRAINING QUANTIZATION FOR DIFFUSION TRANSFORMERS](CVPR 2025)</td>
</tr>
<tr>
<td rowspan="4" colspan="1">Channel Equalization</td>
<td> [PTQ4DiT: Post-training Quantization for Diffusion Transformers] (NerIPS 2024)</td>
</tr>
<tr>
<td>[DiTAS: Quantizing Diffusion Transformers via Enhanced Activation Smoothing](WACV 2025)</td>
</tr>
<tr>
<td>[ViDiT-Q: Efficient and Accurate Quantization of Diffusion Transformers for Image and Video Generation] (ICLR 2025)</td>
</tr>
<tr>
<td>[HQ-DiT: Efficient Diffusion Transformer with FP4 Hybrid Quantization] </td>
</tr>
</table>

## A Taxonomy of Contemporary Approaches

### 1. Unet-based Diffusion Quantization

### 1.1. Calibration Strategy Customization

✅ [**Post-training Quantization on Diffusion Models**] [Paper](https://arxiv.org/abs/2211.15736) *(CVPR2023, First Diffusion Quantization Paper)*

❇️ **Code:**

* [Torch-based](https://github.com/42shawn/ptq4dm)

✅ [**EDA-DM: Enhanced Distribution Alignment for Post-Training Quantization of Diffusion Models**] [Paper](https://arxiv.org/abs/2401.04585)

❇️ **Code:**

* [Torch-based](https://github.com/BienLuky/EDA-DM)

### 1.2. Bi-modal Distribution Elimination

✅ [**Q-Diffusion: Quantizing Diffusion Models**] [Paper](https://arxiv.org/abs/2302.04304) *(ICCV 2023)*

❇️ **Code:**

* [Torch-based](https://github.com/Xiuyu-Li/q-diffusion)

### 1.3 Dynamic Quantization

✅ [**Temporal Dynamic Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2306.02316) *(NeurIPS 2023)*

### 1.4 Time Information Align

✅ [**TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2311.16503) *(CVPR 2024, Highlight)*

❇️ **Code:**

* [Torch-based](https://github.com/ModelTC/TFMQ-DM)

✅ [**QVD: Post-training Quantization for Video Diffusion Models**] [Paper](https://arxiv.org/abs/2407.11585) *(ACM MM 2024)*

### 1.5 Quantization Error Correction

✅ [**QNCD: Quantization Noise Correction for Diffusion Models**] [Paper](https://arxiv.org/abs/2403.19140) *(ACM MM 2024)*

❇️ **Code:**

* [Torch-based](https://github.com/huanpengchu/qncd)

✅ [**PTQD: Accurate Post-Training Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2305.10657) *(NeurIPS 2024)*

❇️ **Code:**

* [Torch-based](https://github.com/ziplab/ptqd)

✅ [**Softmax Bias Correction for Quantized Generative Models**] [Paper](https://arxiv.org/abs/2309.01729) *(ICCV 2023, Workshop)*

✅ [**D$^2$-DPM: Dual Denoising for Quantized Diffusion Probabilistic Models**] [Paper](https://arxiv.org/abs/2501.08180) *(AAAI 2025)*

❇️ **Code:**

* [Torch-based](https://github.com/taylorjocelyn/d2-dpm)

✅ [**Timestep-Aware Correction for Quantized Diffusion Models**] [Paper](https://arxiv.org/abs/2407.03917) *(ECCV 2024)*

### 1.6 Holistic QAT Optimization

✅ [**Q-DM: An Efficient Low-bit Quantized Diffusion Model**] [Paper](https://openreview.net/forum?id=sFGkL5BsPi) *(NeurIPS 2023)*

✅ [**QuEST: Low-bit Diffusion Model Quantization via Efficient Selective Finetuning**] [Paper](https://arxiv.org/abs/2402.03666)

❇️ **Code:**

* [Torch-based](https://github.com/hatchetProject/QuEST)

✅ [**Memory-Efficient Fine-Tuning for Quantized Diffusion Model**] [Paper](https://arxiv.org/abs/2401.04339) *(ECCV 2024)*

### 1.7 Ultra-Low-Bit DMs

✅ [**Binary Latent Diffusion**] [Paper](https://arxiv.org/abs/2304.04820)

✅ [**BiDM: Pushing the Limit of Quantization for Diffusion Models**] [Paper](https://arxiv.org/abs/2412.05926)

❇️ **Code:**

* [Torch-based](https://github.com/xingyu-zheng/bidm)

✅ [**Binarydm: Towards accurate binarization of diffusion model**] [Paper](https://arxiv.org/abs/2404.05662v1)

❇️ **Code:**

* [Torch-based](https://github.com/xingyu-zheng/binarydm)

✅ [**BitsFusion: 1.99 bits Weight Quantization of Diffusion Model**] [Paper](https://arxiv.org/abs/2406.04333) *(NeurIPS 2024)*

✅ [**Binarized Diffusion Model for Image Super-Resolution**] [Paper](https://arxiv.org/abs/2406.05723)

❇️ **Code:**

* [Torch-based](https://github.com/zhengchen1999/bi-diffsr)

### 1.8 LoRA-Based Enhancements

✅ [**EfficientDM: Efficient Quantization-Aware Fine-Tuning of Low-Bit Diffusion Models**] [Paper](https://arxiv.org/abs/2310.03270) *(ICLR 2024)*

❇️ **Code:**

* [Torch-based](https://github.com/thisisbillhe/efficientdm)

✅ [**IntLoRA: Integral Low-rank Adaptation of Quantized Diffusion Models**] [Paper](https://arxiv.org/abs/2410.21759)

❇️ **Code:**

* [Torch-based](https://github.com/csguoh/intlora)

### 2. Diffusion-Transformer(DiT) Quantization

### 2.1 Group-wise Quantization

✅ [**An Analysis on Quantizing Diffusion Transformers**] [Paper](https://arxiv.org/abs/2406.11100) *(CVPR workshop)*

✅ [**Q-DIT: ACCURATE POST-TRAINING QUANTIZATION FOR DIFFUSION TRANSFORMERS**] [Paper](https://arxiv.org/abs/2406.17343) *(CVPR 2025)*

❇️ **Code:**

* [Torch-based](https://github.com/juanerx/q-dit)

### 2.2 Channel Equalization

✅ [**PTQ4DiT: Post-training Quantization for Diffusion Transformers**] [Paper](https://arxiv.org/abs/2405.16005) *(NerIPS 2024)*

❇️ **Code:**

* [Torch-based](https://github.com/adreamwu/ptq4dit)

✅ [**DiTAS: Quantizing Diffusion Transformers via Enhanced Activation Smoothing**] [Paper](https://arxiv.org/abs/2409.07756) *(WACV 2025)*

❇️ **Code:**

* [Torch-based](https://github.com/DZY122/DiTAS)

✅ [**ViDiT-Q: Efficient and Accurate Quantization of Diffusion Transformers for Image and Video Generation**] [Paper](https://arxiv.org/abs/2406.02540) *(ICLR 2025)*

❇️ **Code:**

* [Torch-based](https://github.com/a-suozhang/vidit-q)

✅ [**HQ-DiT: Efficient Diffusion Transformer with FP4 Hybrid Quantization**] [Paper](https://arxiv.org/abs/2405.19751)

