# NeurIPS_Open_Review

This repository contains tables and figures relevant to the discussion on OpenReview.

The quantitative results of **OOD relighting on "CatSmall"** are shown as follows. The training time and inference time are calculated based on their specific hardwares.

|  | PSNR | SSIM | LPIPS | Training time | Inference Time | Hardware |
| ---------------  | --------------- | --------------- | --------------- | --------------- | --------------- |--------------- |
|NRHints    | 24.14    | 0.9101 | 0.1265 | 16 hours | 150 seconds per frame | four Nvidia V100 GPUs |
| Ours    | **25.17** | **0.9297** | **0.1135** |  40 minutes | 0.05 second per frame | a single RTX 3090 |

Visualizations of several testing illuminations are shown below. As shown in the figure, NRHints fails to infer the inherent lighting logic, such as ignoring shadows (light#1) or highlights (light#3), and tends to produce over-smoothing surfaces (light#2).

<img src="ood_result/catsmall.png" width="512px">


We will provide the results and visualizations of other scenes as soon as they are available.
