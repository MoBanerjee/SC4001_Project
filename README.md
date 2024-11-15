# Flowers Recognition Task F - Group Project

## Overview

Our team focused on **Task F - Flowers Recognition**, utilizing the **Flowers102 dataset**. This dataset includes 102 distinct flower species with high visual similarity and significant variability in scale, orientation, and appearance. This complexity makes it an exceptionally challenging **fine-grained classification** problem.

Throughout this project, we experimented with a variety of state-of-the-art models, including **ResNet**, **VGG16**, and **Vision Transformers (ViT)**. We applied several advanced techniques and enhancements such as **transfer learning**, **deformable convolutions**, **triplet loss**, **MixUp**, **CutMix**, **few-shot learning**, **focal margin loss**, and **visual prompt tuning**. The objective was to explore these diverse approaches to identify the most effective model strategies for achieving high accuracy on this challenging dataset.

## Instructions for Running Notebooks

### 1. Hardware and Environment

- All experiments were executed on **T4 GPUs** via **Google Colab** or using the **CCDS GPU Cluster**.

### 2. Quick Guide to Experiments

The following experiments were conducted to evaluate various model strategies and approaches. Each experiment is linked to its corresponding notebook(s).

#### Experiment List:

| **Experiment**                                      | **Notebook**                                             |
| --------------------------------------------------- | -------------------------------------------------------- |
| **3.1 Transfer Learning on ResNet-18 and ResNet-34** | **ResNet18_ResNet34_TransferLearning_FrozenStages.ipynb** |
| **3.2 Deformable Convolutions on ResNet-18**         | **ResNet18_DeformableConvolutions.ipynb**             |
| **3.3 Using ResNet-18 with Triplet Loss**           | **ResNet_TripletLoss.ipynb**                           |
| **3.4 MixUp & CutMix**                              | **MixUpAndCutMix.ipynb**                             |
| **3.5 Few-Shot Learning using Prototypical Networks** | **PrototypicalNetworks.ipynb**                         |
| **3.6 VGG16 with Multi-Scale and Squeeze-and-Excitation Blocks** | **VGG16_MultiScaleAndSE.ipynb**, **VGG16_Frozen.ipynb**, **VGG16_FullFineTune.ipynb** |
| **3.7 Vision Transformer with Focal Margin Loss**   | **ViT_FocalMarginLoss.ipynb**, **ViT_Frozen.ipynb**, **ViT_FullFineTune.ipynb** |
| **3.8 Visual Prompt Tuning in Visual Transformer**  | **ViT_VisualPromptTuning.ipynb**, **ViT_Frozen.ipynb**, **ViT_FullFineTune.ipynb** |

**Note**: The serial numbers of the experiments correspond to the sections in the **report**.

### 3. Additional Notebooks Submitted

These are some additional notebooks submitted, although the experiments conducted in them were not covered in the final report:

1. **EfficientNetb4_ExtraConvLayer_DropoutTuning.ipynb**
2. **EfficientNetb0_FullFineTune.ipynb**
3. **EfficientNetb0_Frozen.ipynb**
4. **FewShotLearning.ipynb**

## Conclusion

Our experiments demonstrated that **Visual Prompt Tuning** and **Focal Margin Loss** in **Vision Transformers (ViT)** outperformed all other models on the Flowers102 dataset, achieving test accuracies of **95.3%** and **95.1%**, respectively. These custom adaptations proved highly effective, allowing ViT to focus on challenging samples and adapt with minimal parameter adjustments.

Additionally, **ResNet-18**, when fine-tuned with targeted **transfer learning**, performed well with a test accuracy of **88.78%**. This highlights the potential of lightweight, targeted modifications as effective alternatives to full model fine-tuning. 

In future work, further improvements could explore alternative forms of prompting—such as **language-based prompts** or **learned prompts**—to provide even greater flexibility in how the model attends to important features.

**Contributors:**

My wonderful teammates:
Leong Kit Ye \n
William Tian
and me

