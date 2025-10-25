---
title: "Your Scale Factors are My Weapon: Targeted Bit-Flip Attacks on Vision Transformers via Scale Factor Manipulation"
collection: publications
category: conferences
permalink: /publication/cvpr25-flip-s
excerpt: 'Jialai Wang, **Yuxiao Wu**, Weiye Xu, Yating Huang, Chao Zhang, Zongpeng Li, Mingwei Xu, Zhenkai Liang'
date: 2025-06-11
venue: 'Computer Vision and Pattern Recognition (CVPR’25)'
paperurl: 'https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_Your_Scale_Factors_are_My_Weapon_Targeted_Bit-Flip_Attacks_on_CVPR_2025_paper.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Abstract: 
---
Vision Transformers (ViTs) have experienced significant progress and are quantized for deployment in resource-constrained applications. Quantized models are vulnerable to targeted bit-flip attacks (BFAs). A targeted BFA prepares a trigger and a corresponding Trojan/backdoor, inserting the latter (with RowHammer bit flipping) into a victim model, to mislead its classification on samples containing the trigger. Existing targeted BFAs on quantized ViTs are limited in that: (1) they require numerous bit-flips, and (2) the separation between flipped bits is below 4 KB, making attacks infeasible with RowHammer in real-world scenarios. We propose a new and practical targeted attack Flip-S against quantized ViTs. The core insight is that in quantized models, a scale factor change ripples through a batch of model weights. Consequently, flipping bits in scale factors, rather than solely in model weights, enables more cost-effective attacks. We design a Scale-Factor-Search (SFS) algorithm to identify critical bits in scale factors for flipping, and adopt a mutual exclusion strategy to guarantee a 4 KB separation between flips. We evaluate Flip-S on CIFAR-10 and ImageNet datasets across five ViT architectures and two quantization levels. Results show that Flip-S achieves attack success rate (ASR) exceeding 90.0% on all models with 50 bits flipped, outperforming baselines with ASR typically below 80.0%. Furthermore, compared to the SOTA, Flip-S reduces the number of required bit-flips by 8×-20× while reaching equal or higher ASR. Our source code is publicly available.