---
layout: post
title: "Deep Residual Shrinkage Network: High Noise Data ಖಾತಿರ್ ಏಕ್ Artificial Intelligence Method"
subtitle: "An Artificial Intelligence Method for Highly Noisy Data"
date: 2025-12-11
tags: [Deep Learning, AI]
mathjax: true
---

**Deep Residual Shrinkage Network ಹೆ Deep Residual Network-ಚೆ ಏಕ್ improved variant ಜಾವ್ನ್ ಆಸಾ. ಮುಖ್ಯ ಜಾವ್ನ್, Deep Residual Shrinkage Network-ಅಂತು Deep Residual Network, Attention mechanisms, ಮತ್ತು Soft thresholding functions ಒಟ್ಟು integrate ಕೆಲ್ಲೆ ಆಸಾ.**

**Deep Residual Shrinkage Network ಕಶಿ ವರ್ಕ್ ಜಾತ್ತಾ ಮ್ಹಣು ಅಮಿ ಹಿ ರಿತಿನ್ ಅರ್ಥ್ ಕರ್ನು ಘೆವ್ಯೆತ್. ಸುರ್ವಾತೆಕ್, network-ಅಂತು unimportant features identify ಕರ್ಚೆ ಖಾತಿರ್ attention mechanisms use ಕರ್ತಾತ್. ನಂತರ, ಹ್ಯಾ unimportant features-ಅಂಕ್ zero ಸೆಟ್ ಕರ್ಚೆ ಖಾತಿರ್ network *Soft thresholding functions* use ಕರ್ತಾ. ತಶಿಚಿ, network important features identify ಕರ್ತಾ ಅನಿ ಹ್ಯಾ important features-ಅಂಕ್ retain ಕರ್ತಾ. ಹಿ process deep neural network-ಚಿ ability improve ಕರ್ತಾ. Noise ಆಶ್ಶಿಲ signals-ಇಂದ useful features extract ಕರ್ಚೆ ಖಾತಿರ್ ಹಿ process network-ಅಕ್ help ಕರ್ತಾ.**

## 1. **Research Motivation (Research Motivation)**

**ಸುರ್ವಾತೆಕ್, algorithm samples classify ಕರ್ತಾನಾ, Noise inevitable ಆಸಾ. ಹ್ಯಾ noise-ಅಕ್ examples ಮ್ಹಳ್ಯಾರ್ Gaussian noise, pink noise, ಅನಿ Laplacian noise.** ಇನ್ನು broad ಜಾವ್ನ್ ಸಾಂಗ್ಚೆ ತರ್, current classification task-ಅಕ್ ಸಂಬಂಧ್ ನಾಶ್ಶಿಲಿ information samples-ಅಂತು ಆಸ್ತಾ. ಹ್ಯಾ irrelevant information-ಅಕ್ ಅಮಿ Noise ಮ್ಹಣು ಅರ್ಥ್ ಕರ್ನು ಘೆವ್ಯೆತ್. ಹೆ Noise classification performance ಕಡಿಮೆ ಕರ್ತಾ. (*Soft thresholding* ಹೆ signal denoising algorithms-ಅಂತು ಏಕ್ key step ಜಾವ್ನ್ ಆಸಾ.)

ಉದಾಹರಣಕ್, ರಸ್ತೆ ಬದಿ ಆಶ್ಶಿಲಿ ಏಕ್ conversation ಪೊಳೆಯಾ. Audio-ಂತು car horns ಅನಿ wheels-ಚೆ sound ಆಸು ಯೆತಾ. ಅಮಿ ಹ್ಯಾ signals-ಚೆ speech recognition ಕರ್ಯೆತ್. Background sounds results-ಅಕ್ affect ಕರ್ತಾತ್. Deep learning perspective-ಇಂದ ಪಳೆಲ್ಯಾರ್, deep neural network-ಆನ್ horns ಅನಿ wheels-ಅಕ್ correspond ಜಾಂವ್ಚೆ features eliminate ಕರ್ಕಾ. ಅಶಿ eliminate ಕೆಲರಿ features speech recognition results-ಅಕ್ affect ಕರ್ಚೆ ನಾ.

**ದುಸ್ರೆ ಮ್ಹಳ್ಯಾರ್, samples-ಅಂತು noise amount vary ಜಾಂವ್ಚೆ common ಆಸಾ. Same dataset-ಅಂತು ಕೂಡ ಅಶಿ vary ಜಾತ್ತಾ.** (ಹೆ variation attention mechanisms ವರಿ same ಆಸಾ. ಏಕ್ image dataset-ಚೆ example ಘೆವ್ಯಾ. Target object-ಚೆ location image-ಇಂದ image-ಅಕ್ different ಆಸು ಯೆತಾ. Attention mechanisms ಪ್ರತಿ image-ಅಂತು target object-ಚೆ specific location-ಅಕ್ focus ಕರ್ತಾ.)

ಉದಾಹರಣಕ್, "dog" label ಆಶ್ಶಿಲ 5 images ದವರ್ನು cat-and-dog classifier train ಕರ್ಚೆ ಪೊಳೆಯಾ. Image 1-ಅಂತು dog ಅನಿ mouse ಆಸು ಯೆತಾ. Image 2-ಅಂತು dog ಅನಿ goose ಆಸು ಯೆತಾ. Image 3-ಅಂತು dog ಅನಿ chicken ಆಸು ಯೆತಾ. Image 4-ಅಂತು dog ಅನಿ donkey ಆಸು ಯೆತಾ. Image 5-ಅಂತು dog ಅನಿ duck ಆಸು ಯೆತಾ. Training time-ಅರ್, irrelevant objects classifier-ಅಕ್ interfere ಕರ್ತಾತ್. ಹ್ಯಾ objects ಮ್ಹಳ್ಯಾರ್ mice, geese, chickens, donkeys, ಅನಿ ducks. ಹ್ಯಾ interference ಕಾರಣ classification accuracy ಕಡಿಮೆ ಜಾತ್ತಾ. ಸಪೋಸ್ ಅಮಿ ಹ್ಯಾ irrelevant objects identify ಕರ್ಯೆತ್ ತರ್, ಅಮಿ ಹ್ಯಾ objects-ಅಕ್ correspond ಜಾಂವ್ಚೆ features eliminate ಕರ್ಯೆತ್. ಹ್ಯಾ ರೀತಿನ್, ಅಮಿ cat-and-dog classifier-ಚಿ accuracy improve ಕರ್ಯೆತ್.

## 2. **Soft Thresholding (Soft Thresholding)**

**Soft thresholding ಮ್ಹಳ್ಯಾರ್ signal denoising algorithms-ಅಂತು ಏಕ್ core step. Features-ಚೆ absolute values ಏಕ್ certain threshold-ಕಿಂತ ಕಡಿಮೆ ಆಸ್ಸ ತರ್, algorithm ಹ್ಯಾ features eliminate ಕರ್ತಾ. Features-ಚೆ absolute values threshold-ಕಿಂತ ಜಾಸ್ತಿ ಆಸ್ಸ ತರ್, algorithm ಹ್ಯಾ features-ಅಂಕ್ zero ಕಡೆ shrink ಕರ್ತಾ.** Researchers ಸಕಲ್ ದಿಲ್ಲಿ formula use ಕರ್ನು Soft thresholding implement ಕರ್ತಾತ್:

$$
y = \begin{cases} 
x - \tau & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
x + \tau & x < -\tau 
\end{cases}
$$

Input-ಅಕ್ respect ಜಾವ್ನ್ soft thresholding output-ಚೆ derivative ಅಶಿ ಆಸಾ:

$$
\frac{\partial y}{\partial x} = \begin{cases} 
1 & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
1 & x < -\tau 
\end{cases}
$$

ವಯ್ರ್ ದಿಲ್ಲಿ formula ಪಳೆಲ್ಯಾರ್ soft thresholding-ಚೆ derivative ಒಂದ್ ತರ್ 1 ಅಥವಾ 0 ಜಾವ್ನ್ ಆಸಾ. ಹಿ property ReLU activation function-ಚೆ property ವರಿ same ಆಸಾ. ದೆಕುನ್, deep learning algorithms-ಅಂತು gradient vanishing ಅನಿ gradient exploding risk ಕಡಿಮೆ ಕರ್ಚೆ ಖಾತಿರ್ soft thresholding help ಕರ್ತಾ.

**Soft thresholding function-ಅಂತು, threshold set ಕರ್ತಾನಾ ದೋನ್ conditions satisfy ಜಾಯ್ಜೆ. First, threshold positive number ಜಾವ್ನ್ ಆಸ್ಕಾ. Second, input signal-ಚೆ maximum value-ಕಿಂತ threshold ಜಾಸ್ತಿ ಆಸು ನಜ. ಹಾಂಕಿಂತ ಜಾಸ್ತಿ ಆಸ್ಸ ತರ್, output full zero ಜಾತ್ತಾ.**

**ಅದು ಮಾತ್ರ್ ನ್ಹಯ್, threshold third condition ಕೂಡ satisfy ಕೆಲ್ಯಾರ್ ಚಾಂಗ್. Sample-ಅಂತು ಆಶ್ಶಿಲ noise content ಪ್ರಕಾರ ಪ್ರತಿ sample-ಅಕ್ ತಜ್ಜೆ ಸ್ವಂತ independent threshold ಆಸ್ಕಾ.**

ಕಾರಣ ಮ್ಹಳ್ಯಾರ್, samples ಮದ್ಯೆ noise content ಯಾವಾಗು vary ಜಾತ್ತಾ. ಉದಾಹರಣಕ್, same dataset-ಅಂತು Sample A-ಂತು less noise ಆಸು ಯೆತಾ ಅನಿ Sample B-ಂತು more noise ಆಸು ಯೆತಾ. ಅಸ್ಸ ಆಸ್ತಾನಾ, soft thresholding ಕರ್ತಾನಾ Sample A-ನ್ smaller threshold use ಕರ್ಕಾ. Sample B-ನ್ larger threshold use ಕರ್ಕಾ. Deep neural networks-ಅಂತು ಹ್ಯಾ features ಅನಿ thresholds-ಅಕ್ explicit physical definitions ನಾಸ್ಲೆರಿ, basic logic same ಆಸಾ. ಮ್ಹಳ್ಯಾರ್, ಪ್ರತಿ sample-ಅಕ್ independent threshold ಆಸ್ಕಾ. Specific noise content ಹೆ threshold determine ಕರ್ತಾ.

## 3. **Attention Mechanism (Attention Mechanism)**

Computer vision field-ಅಂತು attention mechanisms ಕಶಿ ವರ್ಕ್ ಜಾತ್ತಾ ಮ್ಹಣು researchers-ಅಂಕ್ sulabh ಜಾವ್ನ್ ಅರ್ಥ್ ಜಾತ್ತಾ. Animals-ಚೆ visual systems full area rapid scan ಕರ್ನು targets distinguish ಕರ್ತಾತ್. ನಂತರ, visual systems target object-ಚೆರ್ attention focus ಕರ್ತಾತ್. ಅಶಿ ಕೆಲ್ಯಾರ್ systems-ಅಕ್ more details extract ಕರುಂಕ್ ಮೆಳ್ತಾ. ಅದೆ ಸಮಯಾರ್, systems irrelevant information suppress ಕರ್ತಾ. Specifics ಖಾತಿರ್, attention mechanisms-ಚೆ literature refer ಕರಾ.

Squeeze-and-Excitation Network (SENet) ಮ್ಹಳ್ಯಾರ್ attention mechanisms use ಕರ್ಚೆ ಏಕ್ relatively new deep learning method. Different samples-ಅಂತು, classification task-ಅಕ್ different feature channels different level-ಅರ್ contribute ಕರ್ತಾತ್. SENet ಏಕ್ small sub-network use ಕರ್ನು **Learn a set of weights** (weights-ಚಿ ಏಕ್ set) ghetà. ನಂತರ, SENet ಹ್ಯಾ weights-ಅಂಕ್ respective channels-ಚೆ features ಒಟ್ಟು multiply ಕರ್ತಾ. ಹೆ operation ಪ್ರತಿ channel-ಚೆ features-ಚೆ magnitude adjust ಕರ್ತಾ. ಹ್ಯಾ process-ಅಕ್ ಅಮಿ different feature channels-ಅಕ್ different levels of attention apply ಕರ್ಚೆ ಮ್ಹಣು ಪಳೆಯೆತ್ (**Apply weighting to each feature channel**).

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_1.png" alt="Squeeze-and-Excitation Network" width="90%">
</p>

ಹ್ಯಾ approach-ಅಂತು, ಪ್ರತಿ sample-ಅಕ್ independent set of weights ಆಸ್ತಾ. ಮ್ಹಳ್ಯಾರ್, arbitrary two samples-ಚೆ weights different ಆಸ್ತಾ. SENet-ಅಂತು, weights ghevche specific path ಅಶಿ ಆಸಾ: "Global Pooling → Fully Connected Layer → ReLU Function → Fully Connected Layer → Sigmoid Function."

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_2.png" alt="Squeeze-and-Excitation Network" width="60%">
</p>

## 4. **Deep Attention Mechanism ಒಟ್ಟು Soft Thresholding (Soft Thresholding with Deep Attention Mechanism)**

Deep Residual Shrinkage Network ಹೆ SENet sub-network-ಚೆ structure use ಕರ್ತಾ. Deep attention mechanism under soft thresholding implement ಕರ್ಚೆ ಖಾತಿರ್ network ಹಿ structure use ಕರ್ತಾ. Sub-network (image-ಅಂತು red box-ಅಂತು indicate ಕೆಲ್ಲೆ) **Learn a set of thresholds** (thresholds-ಚಿ ಏಕ್ set learn ಕರ್ತಾ). ನಂತರ, ಹ್ಯಾ thresholds use ಕರ್ನು network ಪ್ರತಿ feature channel-ಅಕ್ **Soft thresholding** apply ಕರ್ತಾ.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_1.png" alt="Deep Residual Shrinkage Network" width="75%">
</p>

ಹ್ಯಾ sub-network-ಅಂತು, system ಸುರ್ವಾತೆಕ್ input feature map-ಚೆ all features-ಚೆ absolute values calculate ಕರ್ತಾ. ನಂತರ, system global average pooling ಅನಿ averaging ಕರ್ನು *A* ಮ್ಹಣು denote ಕೆಲ್ಲೆ feature ghetà. ದುಸ್ರಿ path-ಅಂತು (**Identity path** ಸೊಡ್ನು), global average pooling ನಂತರ system feature map-ಅಂಕ್ ಏಕ್ small fully connected network-ಅಂತು input ಕರ್ತಾ. ಹ್ಯಾ fully connected network Sigmoid function-ಅಂಕ್ final layer ಜಾವ್ನ್ use ಕರ್ತಾ. ಹೆ function output-ಅಂಕ್ 0 ಅನಿ 1 ಮದ್ಯೆ normalize ಕರ್ತಾ. ಹ್ಯಾ process-ಇಂದ *α* ಮ್ಹಣು denote ಕೆಲ್ಲೆ coefficient ಮೆಳ್ತಾ. Final threshold-ಅಂಕ್ ಅಮಿ *α × A* ಮ್ಹಣು express ಕರ್ಯೆತ್. ದೆಕುನ್, threshold ಮ್ಹಳ್ಯಾರ್ ದೋನ್ numbers-ಚೆ product. ಏಕ್ number 0 ಅನಿ 1 ಮದ್ಯೆ ಆಸಾ. ದುಸ್ರೆ number feature map-ಚೆ absolute values-ಚೆ average. **ಹಿ method threshold positive ಆಸಾ ಮ್ಹಣು ensure ಕರ್ತಾ. ತಶಿಚಿ ಹಿ method threshold excessively large ನಾ ಮ್ಹಣು ensure ಕರ್ತಾ.**

**ಮುಕಾರ ವಚ್ಚುನ್, different samples different thresholds result ಕರ್ತಾತ್. Consequently, ಅಮಿ ಹ್ಯಾ method-ಅಕ್ specialized attention mechanism ಮ್ಹಣು interpret ಕರ್ಯೆತ್. Current task-ಅಕ್ irrelevant ಆಶ್ಶಿಲೆ features-ಅಂಕ್ ಹಿ mechanism identify ಕರ್ತಾ. ಹಿ mechanism ದೋನ್ convolutional layers use ಕರ್ನು ಹ್ಯಾ features-ಅಂಕ್ 0-ಚೆ close ಆಶ್ಶಿಲೆ values-ಅಕ್ transform ಕರ್ತಾ. ನಂತರ, soft thresholding use ಕರ್ನು mechanism ಹ್ಯಾ features-ಅಂಕ್ zero set ಕರ್ತಾ. ಅಥವಾ, current task-ಅಕ್ relevant ಆಶ್ಶಿಲೆ features-ಅಂಕ್ mechanism identify ಕರ್ತಾ. ಹಿ mechanism ದೋನ್ convolutional layers use ಕರ್ನು ಹ್ಯಾ features-ಅಂಕ್ 0-ಇಂದ far ಆಶ್ಶಿಲೆ values-ಅಕ್ transform ಕರ್ತಾ. Finally, mechanism ಹ್ಯಾ features-ಅಂಕ್ preserve ಕರ್ತಾ.**

Last-ಅಕ್, ಅಮಿ certain number of basic modules stack ಕರ್ತಾತ್ (**Stack many basic modules**). ಅಮಿ convolutional layers, batch normalization, activation functions, global average pooling, ಅನಿ fully connected output layers ಕೂಡ include ಕರ್ತಾತ್. ಹೆ process complete Deep Residual Shrinkage Network construct ಕರ್ತಾ.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_2.png" alt="Deep Residual Shrinkage Network" width="55%">
</p>

## 5. **Generalization Capability (Generalization Capability)**

Deep Residual Shrinkage Network feature learning-ಅಕ್ ಏಕ್ general method ಜಾವ್ನ್ ಆಸಾ. ಕಾರಣ ಮ್ಹಳ್ಯಾರ್, features learning tasks-ಅಂತು samples-ಅಂತು noise ಆಸ್ಚೆ common. Samples-ಅಂತು irrelevant information ಕೂಡ ಆಸ್ತಾ. ಹೆ noise ಅನಿ irrelevant information feature learning-ಚೆ performance affect ಕರ್ಯೆತ್. ಉದಾಹರಣಕ್:

Image classification ಪೊಳೆಯಾ. ಏಕ್ image-ಅಂತು simultaneously khub other objects ಆಸು ಯೆತಾ. ಹ್ಯಾ objects-ಅಂಕ್ ಅಮಿ "noise" ಮ್ಹಣು understand ಕರ್ಯೆತ್. Deep Residual Shrinkage Network attention mechanism use ಕರುಂಕ್ ಸಾಧ್ಯ್ ಆಸಾ. Network ಹ್ಯಾ "noise"-ಅಕ್ notice ಕರ್ತಾ. ನಂತರ, network **Soft thresholding** use ಕರ್ನು ಹ್ಯಾ "noise"-ಅಕ್ correspond ಜಾಂವ್ಚೆ features zero set ಕರ್ತಾ. ಹೆ action image classification accuracy improve ಕರ್ಯೆತ್.

Speech recognition ಪೊಳೆಯಾ. Specifically, ರಸ್ತೆ ಬದಿ ಅಥವಾ factory workshop-ಅಂತು ಆಸ್ಚೆ relatively noisy environments ಪೊಳೆಯಾ. Deep Residual Shrinkage Network speech recognition accuracy improve ಕರ್ಯೆತ್. At least, network ಏಕ್ methodology offer ಕರ್ತಾ. ಹಿ methodology speech recognition accuracy improve ಕರ್ಚೆ capability ದವರ್ತಾ.

## **Reference**

Minghang Zhao, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht, Deep residual shrinkage networks for fault diagnosis, IEEE Transactions on Industrial Informatics, 2020, 16(7): 4681-4690.

[https://ieeexplore.ieee.org/document/8850096](https://ieeexplore.ieee.org/document/8850096)

## BibTeX
```bibtex
@article{Zhao2020,
  author    = {Minghang Zhao and Shisheng Zhong and Xuyun Fu and Baoping Tang and Michael Pecht},
  title     = {Deep Residual Shrinkage Networks for Fault Diagnosis},
  journal   = {IEEE Transactions on Industrial Informatics},
  year      = {2020},
  volume    = {16},
  number    = {7},
  pages     = {4681-4690},
  doi       = {10.1109/TII.2019.2943898}
}
```

## **Academic Impact (Academic Impact)**

Google Scholar-ಅರ್ ಹ್ಯಾ paper-ಅಕ್ 1400-ಕಿಂತ ಜಾಸ್ತಿ citations ಮೆಳ್ಳಾ.

Incomplete statistics ಪ್ರಕಾರ, researchers Deep Residual Shrinkage Network (DRSN)-ಅಂಕ್ 1000-ಕಿಂತ ಜಾಸ್ತಿ publications/studies-ಅಂತು apply ಕೆಲಾಂತ್. ಹ್ಯಾ applications wide range of fields cover ಕರ್ತಾತ್. ಹ್ಯಾ fields-ಅಂತು mechanical engineering, electrical power, vision, healthcare, speech, text, radar, ಅನಿ remote sensing include ಆಸಾತ್.
