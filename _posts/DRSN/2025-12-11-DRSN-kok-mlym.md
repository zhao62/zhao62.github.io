---
layout: post
title: "Deep Residual Shrinkage Network: Highly Noisy Data-അന്തു Use കൊർചെ ഏക Artificial Intelligence Method"
subtitle: "An Artificial Intelligence Method for Highly Noisy Data"
date: 2025-12-11
tags: [Deep Learning, AI]
mathjax: true
---

**Deep Residual Shrinkage Network മ്ഹള്യരി Deep Residual Network-ചെ ഏക improved variant (മെച്ചപ്പെടുത്തിയ രൂപം) ആസ. അസൽ മ്ഹള്യരി, Deep Residual Shrinkage Network ഹെ Deep Residual Network, attention mechanisms, അനി soft thresholding functions ഹക്ക integrate കർത്താ.**

**Deep Residual Shrinkage Network കശ്ശി work കർത്താ മ്ഹണു അമി അശ്ശി മനസ്സിലാക്കി ഘെവിയാ. ഫസ്റ്റ്, unimportant features കൊണ-തെ ഒളഖുചാക് ഹെ network attention mechanisms use കർത്താ. നന്തര, ഹെ unimportant features-അക്ക zero (0) കൊർചാക് soft thresholding functions use കർത്താ. തിത്ലെ ൻഹയി, important features-അക്ക ഹെ network ഒളഖുനു അസ്സശ്ശി ദവർത്താ. ഹെ process deep neural network-ചെ കഴിവ് ജാസ്തി കർത്താ. Noise അസ്സചെ signals-അന്തു ദൊണു useful features കാടുങ്ക ഹെ process സഹായി കർത്താ.**

## 1. Research Motivation

**ഫസ്റ്റ് സാംഗുക അസ്സരി, algorithm samples-അക്ക classify കൊർതനാ noise മ്ഹള്യരി സഹജ് ജാവ്നു അസ്സചെ ജാവുനു ആസ. Gaussian noise, pink noise, അനി Laplacian noise ഹജ്ജെ ഉദാഹരണങ്ങളു.** അജ്ജി സാംഗുക അസ്സരി, **samples**-അന്തു ചഡാവു വഖത് **current classification task**-അക്ക വേണ്ടാത്ത ഇൻഫർമേഷൻ അസ്സു യെത്ത. ഹെ വേണ്ടാത്ത ഇൻഫർമേഷൻ അമി **noise** മ്ഹണു ധൊരയ. ഹെ **noise** നിമിത്തം **classification performance** കമ്മി ജാവു യെത്ത. (**Soft thresholding** മ്ഹള്യരി മസ്ത് **signal denoising algorithms**-അന്തു ഏക **key step** ആസ.)

ഉദാഹരണാക്, എക റോഡാ സൈഡരി ഉലയ്ത അസ്സ മ്ഹണു വിചാർ കൊരയ. ആ **audio**-ന്തു വണ്ടിയാ ഹോൺ അനി ടയറാ ശബ്ദ അസ്സു യെത്ത. അമി ഹജ്ജെരി **speech recognition** കൊർത്ത അസ്സരി, ഹെ ബാക്ഗ്രൗണ്ട് ശബ്ദ ഫലത്ത അഫക്ട് കർത്താ. **Deep learning perspective**-അന്തു ദൊണു പോളയ്തന, **deep neural network** ആ ഹോൺ അനി ടയറാ ശബ്ദ അക്ക **eliminate** (ഒഴിവാക്ക്) കൊർക്ക. അശ്ശി കെല്യരി മാത്ര, **features** പോവ്നു **speech recognition results**-അക്ക അഫക്ട് കൊർനശ്ശി അസ്സത്ത.

**സെക്കൻഡ് മ്ഹള്യരി, ഓരോ samples-അന്തു അസ്സചെ noise amount വിത്യാസ് അസ്സു യെത്ത. ഒരേ dataset-അന്തു അസ്സചെ samples-അന്തു സയ്ത് ഹെ വിത്യാസ് അസ്സു യെത്ത.** (ഹെ വിത്യാസ് അനി **attention mechanisms** തമ്മിൽ സാമ്യം ആസ. ഏക **image dataset** ഉദാഹരണാക് ഘെവിയാ. ഓരോ ഫോട്ടോന്തു **target object** അസ്സചെ സ്ഥാന് വിത്യാസ് അസ്സു യെത്ത. **Attention mechanisms**-അക്ക ആ **specific location**-അന്തു ശ്രദ്ധ കൊർചാക് സാധിക്കിത്ത.)

ഉദാഹരണാക്, 5 "നായ" ഫോട്ടോ വെച്ചുനു ഏക **cat-and-dog classifier** ട്രെയിൻ കർത്താ മ്ഹണു വിചാർ കൊരയ. **Image 1**-അന്തു നായ അനി എലി അസ്സു യെത്ത. **Image 2**-അന്തു നായ അനി വാത്ത്, **Image 3**-അന്തു നായ അനി കോഴി, **Image 4**-അന്തു നായ അനി കഴുത, **Image 5**-അന്തു നായ അനി താറാവ് അശ്ശി അസ്സു യെത്ത. **Training** സമയത്തു, ഹെ വേണ്ടാത്ത സാധനങ്ങളു **classifier**-അക്ക **interfere** കർത്താ. ഹജ്ജെ കൂട്ടത്തിൽ എലി, വാത്ത്, കോഴി, കഴുത, അനി താറാവ് ഒക്കെ പെടത്ത. ഹെ **interference** നിമിത്തം **classification accuracy** കമ്മി ജാത്താ. അമി ഹെ വേണ്ടാത്ത സാധനങ്ങളു ഒളഖുനു, ഹജ്ജെ **features**-അക്ക **eliminate** കെല്യരി, അമ്ഗെലെ **cat-and-dog classifier**-ചെ **accuracy** കൂട്ടാക് സാധിക്കിത്ത.

## 2. Soft Thresholding

**മസ്ത് signal denoising algorithms-ചെ ഏക core step ആസ Soft thresholding. Features-ചെ absolute values ഏക പ്രത്യേക threshold-നേക്കാൾ കമ്മി ആസ ജല്യരി, algorithm ആ features-അക്ക eliminate കർത്താ. ഇനി, absolute values ആ threshold-നേക്കാൾ ജാസ്തി ആസ ജല്യരി, algorithm ആ features-അക്ക zero-ചെ അടുത്തേക്ക് shrink കർത്താ.** Researchers ഹെ താഴെ ദില്ലെ ഫോർമുല വെച്ചുനു **soft thresholding** implement കർത്താച്ചി:

$$
y = \begin{cases} 
x - \tau & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
x + \tau & x < -\tau 
\end{cases}
$$

**Input**-അക്ക സംബന്ധിച് **soft thresholding output**-ചെ **derivative** അശ്ശി ആസ:

$$
\frac{\partial y}{\partial x} = \begin{cases} 
1 & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
1 & x < -\tau 
\end{cases}
$$

മേലെ ദില്ലെ ഫോർമുല പ്രകാരം, **soft thresholding**-ചെ **derivative** ഒന്നുക്കിൽ 1, അല്ലെങ്കിൽ 0 ജാത്താ. ഹെ ഗുൺ **ReLU activation function**-ചെ വരി ആസ. തക്കെലാഗി, **deep learning algorithms**-അന്തു **gradient vanishing** അനി **gradient exploding**-ചെ റിസ്ക് കമ്മി കൊർചാക് **soft thresholding** സഹായി കർത്താ.

**Soft thresholding function-അന്തു threshold set കൊർതനാ ദൊന്ന് കാര്യങ്ങളു ശ്രദ്ധിക്ക. ഫസ്റ്റ്, threshold positive ജാവുക്ക. സെക്കൻഡ്, threshold എന്നത് input signal-ചെ maximum value-നേക്കാൾ ജാസ്തി ജാവുനായ. അശ്ശി ജല്യരി output ഫുൾ zero ജാത്താ.**

**ഇതിലെ കൂടെ, threshold മൂന്നാമത്തെ ഏക കാര്യം കൂടി പാലിക്കില്യരി ചാംഗ. ഓരോ samples-അക്ക, ഹജ്ജന്തു അസ്സചെ noise content അനുസരിച് ഹജ്ജെതയ ജാലെ independent threshold അസ്സുക്ക.**

കാരണം, ഓരോ **samples**-അന്തു അസ്സചെ **noise content** വിത്യാസ് അസ്സു യെത്ത. ഉദാഹരണാക്, ഒരേ **dataset**-അന്തു **Sample A**-ന്തു **noise** കമ്മി അസ്സു യെത്ത, പക്ഷെ **Sample B**-ന്തു **noise** ജാസ്തി അസ്സു യെത്ത. അശ്ശി അസ്സതന, **soft thresholding** കൊർതന **Sample A**-ന്തു ചെറിയ **threshold** അനി **Sample B**-ന്തു വലിയ **threshold use** കൊർക്ക. **Deep neural networks**-അന്തു ഹെ **features** അനി **thresholds**-അക്ക കൃത്യമായ **physical definitions** (ഫിസിക്കൽ അർത്ഥം) ഇല്ല ജല്യരി സയ്ത്, ഹജ്ജെ അടിസ്ഥാന് **logic** സെയിം ആസ. മ്ഹള്യരി, ഓരോ **sample**-അക്ക എക **independent threshold** അസ്സുക്ക. അവിടുത്തെ **noise content** ഹെ **threshold** തീരുമാനി കർത്താ.

## 3. Attention Mechanism

**Computer vision** ഫീൽഡാന്തു **attention mechanisms** മനസ്സിലാക്കുചാക് മസ്ത് എളുപ്പ ആസ. മൃഗങ്ങളേ കണ്ണി, എല്ലാ ഏരിയയും വേഗത്തിൽ സ്കാൻ കൊർനു കാര്യങ്ങളു ഒളഖുനു ഘെത്ത. നന്തര, കണ്ണു **target object**-ചെ മേലെ ശ്രദ്ധ (**attention**) കേന്ദ്രീകരി കർത്താ. ഹെ നിമിത്തം കൂടുതൽ **details** കിട്ടുചാക് സഹായി കർത്താ. ഒപ്പം, വേണ്ടാത്ത ഇൻഫർമേഷൻ ഒഴിവാക്കുവുചാക് സഹായി കർത്താ. കൂടുതൽ വിവരങ്ങൾക്ക **attention mechanisms**-പറ്റി അസ്സചെ പുസ്തകങ്ങളു **refer** കൊരയ.

**Squeeze-and-Excitation Network (SENet)** എന്നത് **attention mechanisms use** കൊർചെ ഏക പുതിയ **deep learning method** ആസ. വിത്യാസ് **samples**-അന്തു, വിത്യാസ് **feature channels** **classification task**-അന്തു വേറെ വേറെ രീതിയിങ്കു സഹായി കർത്താ. **SENet** എക ചെറിയ **sub-network use** കൊർനു എക set **weights** കണ്ടുപിടി കർത്താ. നന്തര, **SENet** ഹെ **weights** വെച്ചുനു അതാത് **channels**-ചെ **features**-അക്ക ഗുണി കർത്താ. ഹെ operation ഓരോ **channel**-ചെ **features**-ചെ വലുപ്പം (magnitude) adjust കർത്താ. വിത്യാസ് **feature channels**-അക്ക വിത്യാസ് അളവുചെ **attention** കൊടുക്കില വരി അമി ഹക്ക കാണയ.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_1.png" alt="Squeeze-and-Excitation Network" width="90%">
</p>

ഹെ രീതിയിങ്കു, ഓരോ **sample**-അക്ക ഹജ്ജെതയ ജാലെ **independent set of weights** അസ്സു യെത്ത. മ്ഹള്യരി, ഏത് ദൊന്ന് **samples** ഘെത്ല്യരി സയ്ത് ഹജ്ജെ **weights** വിത്യാസ് ജാവുനു അസ്സത്ത. **SENet**-അന്തു **weights** കിട്ടുചെ path അശ്ശി ആസ: "**Global Pooling → Fully Connected Layer → ReLU Function → Fully Connected Layer → Sigmoid Function**".

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_2.png" alt="Squeeze-and-Excitation Network" width="60%">
</p>

## 4. Soft Thresholding with Deep Attention Mechanism

**Deep Residual Shrinkage Network**, **SENet sub-network**-ചെ structure **use** കർത്താ. **Deep attention mechanism** വെച്ചുനു **soft thresholding** implement കൊർചാക് ഹെ structure സഹായി കർത്താ. **Sub-network** (ചുവന്ന ബോക്സാന്തു അസ്സചെ) **learn a set of thresholds** (ഏക സെറ്റ് thresholds പഠി കർത്താ). നന്തര, **network** ഹെ **thresholds use** കൊർനു ഓരോ **feature channel**-അന്തു **soft thresholding** apply കർത്താ.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_1.png" alt="Deep Residual Shrinkage Network" width="75%">
</p>

ഹെ **sub-network**-അന്തു, സിസ്റ്റം ഫസ്റ്റ് **input feature map**-ചെ എല്ലാ **features**-ചെയും absolute values കാഡുനു ഘെത്ത. നന്തര, **global average pooling** അനി **averaging** കൊർനു *A* എന്ന് വിളിക്കുചെ എക **feature** റെഡി കർത്താ. വേറെ എക path-ഇങ്കു, **global average pooling** കഴിഞ്ഞ് **feature map**-അക്ക എക ചെറിയ **fully connected network**-അന്തു കൊടുക്ക. ഹെ **fully connected network** ലാസ്റ്റ് ലെയർ ജാവുനു **Sigmoid function use** കർത്താ. ഹെ **function output**-അക്ക 0 അനി 1-ചെ ഇടയ്ക്ക് **normalize** കർത്താ. ഹെ process *α* മ്ഹള്യ എക coefficient തരുത്ത. ഫൈനൽ **threshold**-അക്ക അമി *α × A* മ്ഹണു കണക്കാക്ക. അതായത്, **threshold** മ്ഹള്യരി ദൊന്ന് നമ്പേഴ്സ് ഗുണിചെ ഫലം ആസ. എക നമ്പർ 0 അനി 1-ചെ ഇടയ്ക്ക് ആസ. മറ്റേ നമ്പർ **feature map absolute values**-ചെ average ആസ. **ഹെ method threshold positive ആസ മ്ഹണു ഉറപ്പു വരുത്ത. തിത്ലെ ൻഹയി, threshold ഒത്തിരി വലുത് ജാവുനായ മ്ഹണു ഹെ ഉറപ്പു വരുത്ത.**

**കൂടാതെ, വിത്യാസ് samples-അക്ക വിത്യാസ് thresholds കിട്ടാ. അതുകൊണ്ടു, അമി ഹക്ക എക പ്രത്യേക attention mechanism മ്ഹണു വിചാർ കൊരയ. ഹെ mechanism നിലവിലെ task-അക്ക വേണ്ടാത്ത features-അക്ക ഒളഖുനു ഘെത്ത. നന്തര ദൊന്ന് convolutional layers വഴി ഹെ features-അക്ക 0-ചെ അടുത്തേക്ക് കൊണ്ടു യെത്ത. പിന്നെ, soft thresholding വഴി ഹെ features-അക്ക ഫുൾ 'സീറോ' (zero) ആക്കി മാറ്റാ. നേരെ മറിച്, task-അക്ക ആവശ്യമുള്ള features-അക്ക ഹെ mechanism ഒളഖുനു ഘെത്ത. ദൊന്ന് convolutional layers വഴി ഹെ features-അക്ക 0-യിൽ നിന്നു ദൂരേക്ക് കൊണ്ടു വത്ത. ഫൈനലി, ഹെ mechanism ആ features-അക്ക അസ്സശ്ശി preserve കർത്താ.**

അവസാനം, അമി കുറച്ച് **basic modules** ഒന്നിന് മേലെ ഒന്നായി **stack** കർത്താ (**Stack many basic modules**). ഹജ്ജെ ഒപ്പം **convolutional layers**, **batch normalization**, **activation functions**, **global average pooling**, അനി **fully connected output layers** അമി ചേർക്ക. അശ്ശി അമി ഫുൾ **Deep Residual Shrinkage Network** ഉണ്ടാക്കി ഘെത്ത.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_2.png" alt="Deep Residual Shrinkage Network" width="55%">
</p>

## 5. Generalization Capability

**Deep Residual Shrinkage Network** എന്നത് **feature learning**-നു വേണ്ടി അസ്സചെ എക **general method** ആസ. കാരണം, മസ്ത് **feature learning tasks**-അന്തു **samples**-അന്തു **noise** അസ്സു യെത്ത. **Samples**-അന്തു വേണ്ടാത്ത ഇൻഫർമേഷൻ അസ്സു യെത്ത. ഹെ **noise** അനി വേണ്ടാത്ത കാര്യങ്ങളു **feature learning**-ചെ ഗുണത്തെ ബാധി കർത്താ. ഉദാഹരണാക്:

**Image classification** വിചാർ കൊരയ. എക ഫോട്ടോന്തു ഒരേ സമയം മസ്ത് വേറെ സാധനങ്ങളു അസ്സു യെത്ത. ഹെ സാധനങ്ങളെ അമി "**noise**" മ്ഹണു വിചാർ കൊരയ. **Deep Residual Shrinkage Network**-അക്ക **attention mechanism use** കൊർചാക് സാധിക്കിത്ത. **Network** ഹെ "**noise**"-അക്ക ശ്രദ്ധിക്ക. നന്തര, **soft thresholding use** കൊർനു ഹെ "**noise**"-ചെ **features**-അക്ക സീറോ (zero) ആക്കി മാറ്റാ. ഹെ പരിപാടി **image classification accuracy** കൂട്ടാക് സഹായി കർത്താ.

**Speech recognition** വിചാർ കൊരയ. പ്രത്യേകിച്ചു റോഡാ സൈഡരി അല്ലെങ്കിൽ ഫാക്ടറി ഉള്ളിൽ ഒക്കെ ഉലയ്തന **noise** ജാസ്തി അസ്സത്ത ൻഹ്യവേ? **Deep Residual Shrinkage Network** അവിടുത്തെ **speech recognition accuracy** കൂട്ടാക് സഹായി ജാത്താ. അല്ലെങ്കിൽ കുറഞ്ഞത്, **network** എക മെത്തേഡ് (methodology) തരുത്ത. ആ മെത്തേഡ് **speech recognition accuracy** കൂട്ടാക് സഹായി കർത്താ.

## Reference

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

## Academic Impact

ഹെ പേപ്പർ **Google Scholar**-അന്തു 1400-ൽ അധികം **citations** കിട്ടി അസ.

ലഭ്യമായ കണക്കു പ്രകാരം, researchers 1000-ൽ അധികം പഠനങ്ങളിൽ **Deep Residual Shrinkage Network (DRSN)** **apply** കൊർനു ആസ. **Mechanical engineering**, **electrical power**, **vision**, **healthcare**, **speech**, **text**, **radar**, അനി **remote sensing** തുടങ്ങി മസ്ത് ഫീൽഡുകളിൽ ഹജ്ജെ ഉപയോഗ് നടന്നു ആസ.
