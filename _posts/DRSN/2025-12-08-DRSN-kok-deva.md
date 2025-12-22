---
layout: post
title: "Deep Residual Shrinkage Network: Highly Noisy Data खातीर एक Artificial Intelligence Method"
date: 2025-12-08
tags: [Deep Learning, AI]
mathjax: true
description: "Deep Residual Shrinkage Network हें Deep Residual Network चें एक सुदारीत (improved) variant आसा. म्हळ्यारच, Deep Residual Shrinkage Network मदे Deep Residual Network, attention mechanisms, आनी soft thresholding functions हांचो आस्पाव (integration) आसा."
---

**Deep Residual Shrinkage Network हें Deep Residual Network चें एक सुदारीत (improved) variant आसा. म्हळ्यारच, Deep Residual Shrinkage Network मदे Deep Residual Network, attention mechanisms, आनी soft thresholding functions हांचो आस्पाव (integration) आसा.**

**आमी Deep Residual Shrinkage Network कशें काम करता, हें अशें समजून घेऊंक शकतात. सगळ्यांत पयलीं, हें network attention mechanisms वापरून बिन-महत्वाचे (unimportant) features identify करता. त्या उपरांत, network soft thresholding functions वापरून ह्या बिन-महत्वाच्या features-आंक zero set करता. त्याच भाशेन, हें network महत्वाचे (important) features identify करता आनी तांकां सांबाळून दवरता. हाका लागून deep neural network ची ability वाडटा. हें process network-आक noise आसलेल्या signals मधल्यान useful features extract करपाक मदत करता.**

## 1. Research Motivation (Research Motivation)

**पयलीं म्हळ्यार, जेन्ना algorithm samples classify करता, तेन्ना noise आसप हें सामकें स्वाभावीक आसा (inevitable). ह्या noise च्या उदाहरणां मदे Gaussian noise, pink noise, आनी Laplacian noise हांचो आस्पाव जाता.** चड विस्तारांन सांगपाचें जाल्यार, samples मदे जायते फावट current classification task खातीर गरजेची नाशिल्ली म्हायती (irrelevant information) आसता. आमी ह्या irrelevant information-आक noise म्हणून समजून घेऊंक शकतात. हो noise classification performance कमी करूंक शकता. (Soft thresholding हें जायत्या signal denoising algorithms मधलें एक key step आसता.)

उदाहरणा खातीर, रस्त्याच्या कडेक चलिल्ली गजाली (conversation) चिंतयात. Audio मदे गाडयांचे horns आनी चाकांचे (wheels) आवाज आसूंक शकतात. आमी ह्या signals-आंचेर speech recognition करूंक शकतात. पूण background sounds निश्चीतपणान result-आंचेर परिणाम करतात. Deep learning च्या नदरेतल्यान (perspective), deep neural network-आन horns आनी wheels खातीर आसलेले features eliminate करपाक जाय. हें elimination केल्यार हे features speech recognition च्या result-आंचेर परिणाम करचे नात.

**दुसरें म्हळ्यार, noise चें प्रमाण (amount) दर एका sample मदे वेग-वेगळें आसता. हें variation एकाच dataset मदे आसलेल्या samples मदे लेगीत दिसून येता.** (हें variation attention mechanisms सारकें आसा. एक image dataset चें उदाहरण घेऊया. वेग-वेगळ्या images मदे target object चें location वेग-वेगळें आसूंक शकता. Attention mechanisms दर एका image मदे target object च्या specific location-आचेर focus करूंक शकता.)

उदाहरणा खातीर, आमी एक cat-and-dog classifier train करतात आनी आमच्या कडेन "dog" म्हणून label केल्ल्यो पांच images आसात अशें समजूया. Image 1 मदे dog आनी mouse आसूंक शकता. Image 2 मदे dog आनी goose आसूंक शकता. Image 3 मदे dog आनी chicken आसूंक शकता. Image 4 मदे dog आनी donkey आसूंक शकता. Image 5 मदे dog आनी duck आसूंक शकता. Training च्या वेळार, irrelevant objects classifier-आक disturb करतात. ह्या objects मदे mice, geese, chickens, donkeys, आनी ducks हांचो आस्पाव जाता. ह्या interference-आक लागून classification accuracy कमी जाता. जरी आमी हे irrelevant objects identify करूंक शकले, तर आमी ह्या objects-आंक correspond करपी features eliminate करूंक शकतात. हाका लागून, आमी cat-and-dog classifier ची accuracy वाडोवंक शकतात.

## 2. Soft Thresholding (Soft Thresholding)

**जायत्या signal denoising algorithms मदे Soft thresholding हें एक core step आसा. जरी features चे absolute values एक थारावीक threshold परस कमी आसात, तर algorithm ते features eliminate करता. आनी जरी features चे absolute values त्या threshold परस चड आसात, तर algorithm त्या features-आंक zero च्या दिशेन shrink करता.** Researchers सकयल दिल्ल्या formula चो वापर करून soft thresholding implement करूंक शकतात:

$$
y = \begin{cases} 
x - \tau & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
x + \tau & x < -\tau 
\end{cases}
$$

Input च्या संदर्भान soft thresholding output चें derivative अशें आसा:

$$
\frac{\partial y}{\partial x} = \begin{cases} 
1 & x > \tau \\ 
0 & -\tau \le x \le \tau \\ 
1 & x < -\tau 
\end{cases}
$$

वयर दिल्लो formula दाखयता की soft thresholding चें derivative एक तर 1 आसा वो 0 आसा. ही property ReLU activation function च्या property सारकी same आसा. देखून, soft thresholding deep learning algorithms मदे gradient vanishing आनी gradient exploding चो risk कमी करूंक शकता.

**Soft thresholding function मदे, threshold set करतना दोन conditions satisfy करच्यो पडटात. पयलीं, threshold एक positive number आसपाक जाय. दुसरें, threshold input signal च्या maximum value परस व्हड आसूंक फावना. ना जाल्यार, output पुराय zero आसतलो.**

**ते भायर, threshold-आन तिसरी condition satisfy केली जाल्यार चड बरें. दर एका sample खातीर, त्या sample च्या noise content प्रमाण, एक स्वताचो independent threshold आसपाक जाय.**

हाचें कारण म्हळ्यार noise content दर एका sample मदे वेग-वेगळें आसता. उदाहरणा खातीर, एकाच dataset मदे Sample A मदे कमी noise आसूंक शकता, पूण Sample B मदे चड noise आसूंक शकता. हाका लागून, soft thresholding करतना Sample A खातीर ल्हान threshold वापरपाक जाय. आनी Sample B खातीर व्हड threshold वापरपाक जाय. Deep neural networks मदे, जरी ह्या features आनी thresholds हांचो explicit physical definitions नासतात, तरी पूण तांचें basic underlying logic तेंच उरता. साध्या उतरांनी सांगपाचें जाल्यार, दर एका sample खातीर एक independent threshold आसपाक जाय. Specific noise content हो threshold थारायता.

## 3. Attention Mechanism (Attention Mechanism)

Computer vision च्या क्षेत्रान attention mechanisms समजप researchers खातीर सोंपें आसा. प्राण्यांची (Animals) visual systems पुराय area fast scan करून targets distinguish करूंक शकतात. त्या उपरांत, visual systems target object-आचेर attention focus करतात. ही action systems-आंक चड details extract करपाक मदत करता. त्याच बरोबर, systems irrelevant information suppress करतात. चड म्हायती खातीर, तुमी attention mechanisms-आविशीं आसलेलें literature वाचूंक शकतात.

Squeeze-and-Excitation Network (SENet) ही attention mechanisms वापरपी एक नवी deep learning method आसा. वेग-वेगळ्या samples मदे, वेग-वेगळे feature channels classification task खातीर वेग-वेगळो contribution देतात. SENet weights चो एक set मेळोवपाक एक ल्हान sub-network वापरता. मागीर, SENet हे weights त्या त्या channels च्या features कडेन multiply करता. हें operation दर एका channel मधल्या features चें magnitude adjust करता. आमी ह्या process-आक वेग-वेगळ्या feature channels-आंचेर वेग-वेगळ्या level-आचें attention दिवप, अशें मानूंक शकतात.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_1.png" alt="Squeeze-and-Excitation Network" width="90%">
</p>

ह्या approach मदे, दर एका sample कडेन weights चो एक independent set आसता. म्हळ्यारच, खंयच्याय दोन वेग-वेगळ्या samples चे weights वेग-वेगळे आसतात. SENet मदे, weights मेळोवपाचो specific path आसा: "Global Pooling → Fully Connected Layer → ReLU Function → Fully Connected Layer → Sigmoid Function."

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/SENET_en_2.png" alt="Squeeze-and-Excitation Network" width="60%">
</p>

## 4. Deep Attention Mechanism-आ सयत Soft Thresholding (Soft Thresholding with Deep Attention Mechanism)

Deep Residual Shrinkage Network SENet sub-network चें structure वापरता. हें network deep attention mechanism च्या सकयल soft thresholding implement करपाक ह्या structure चो वापर करता. हें sub-network (जें **red box** मदे दाखयलां) **Learn a set of thresholds** करता (म्हळ्यारच thresholds चो set शिकता). उपरांत, network हे thresholds वापरून दर एका feature channel-आचेर soft thresholding apply करता.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_1.png" alt="Deep Residual Shrinkage Network" width="75%">
</p>

ह्या sub-network मदे, system पयलीं input feature map मधल्या सगळ्या features चे absolute values calculate करता. उपरांत, system global average pooling आनी averaging करून एक feature मेळयता, जाका $A$ म्हणून denote केलां. दुसऱ्या path-आन, system global average pooling जाल्या उपरांत feature map एक ल्हान fully connected network मदे input करता. हें fully connected network Sigmoid function-आक last layer कसो वापरता. हें function output-आक 0 आनी 1 च्या मदे normalize करता. ह्या process वरवीं एक coefficient मेळटा, जाका $\alpha$ म्हणून denote केलां. आमी final threshold $\alpha \times A$ असो express करूंक शकतात. म्हळ्यारच, threshold हो दोन numbers चो product (गुणाकार) आसा. एक number 0 आनी 1 च्या मदे आसा. आनी दुसरो number feature map च्या absolute values चें average आसा. **ही method ensure करता की threshold नेमान positive आसा. त्याच बरोबर ही method threshold चड व्हड आसचे ना म्हणून ensure करता.**

**आनीक म्हळ्यार, वेग-वेगळे samples वेग-वेगळे thresholds तयार करतात. देखून, आमी ह्या method-आक एक specialized attention mechanism म्हणून समजून घेऊंक शकतात. हें mechanism current task-आक irrelevant आसलेले features identify करता. हें mechanism ह्या features-आंक दोन convolutional layers वापरून zero च्या लागीं आसलेल्या values मदे transform करता. उपरांत, हें mechanism soft thresholding वापरून ह्या features-आंक zero set करता. दुसऱ्या भाशेन सांगपाचें जाल्यार, हें mechanism current task-आक relevant आसलेले features identify करता. Mechanism ह्या features-आंक दोन convolutional layers वापरून zero पयस आसलेल्या values मदे transform करता. आनी शेवटाक, हें mechanism हे features preserve करता.**

अखेरेक, आमी **Stack many basic modules** करतात (म्हळ्यारच जायते basic modules एकमेकांचेर stack करतात). आमी convolutional layers, batch normalization, activation functions, global average pooling, आनी fully connected output layers हांचोय आस्पाव करतात. हें process पुराय Deep Residual Shrinkage Network बांदता.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en_2.png" alt="Deep Residual Shrinkage Network" width="55%">
</p>

## 5. Generalization Capability (Generalization Capability)

Deep Residual Shrinkage Network ही feature learning खातीर एक general method आसा. कित्याक म्हळ्यार, जायत्या feature learning tasks मदे samples-आंत noise आसता. Samples मदे irrelevant information लेगीत आसता. हो noise आनी irrelevant information feature learning च्या performance-आचेर परिणाम करूंक शकता. उदाहरणा खातीर:

Image classification चिंतयात. एका image मदे एकाच वेळार जायत्यो हेर वस्तू (objects) आसूंक शकतात. आमी ह्या objects-आंक "noise" म्हणून समजून घेऊंक शकतात. Deep Residual Shrinkage Network attention mechanism चो वापर करपाक शकता. Network ह्या "noise"-आक notice करता. मागीर, network soft thresholding वापरून ह्या "noise"-आक correspond करपी features zero set करता. ही action image classification ची accuracy वाडोवंक शकता.

Speech recognition चिंतयात. खास करून, रस्त्याच्या कडेक वो factory workshop मदे गजाली करतना, जोय चड noise आसता. Deep Residual Shrinkage Network speech recognition ची accuracy वाडोवंक शकता. वो कमी-त-कमी, हें network एक methodology offer करता. ही methodology speech recognition accuracy वाडोवपाक सक्षम आसा.

## References

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

## Academic Impact (Academic Impact)

Google Scholar-आचेर ह्या paper-आक 1,400 परस चड citations मेळ्ळ्यात.

अपुर्ण statistics प्रमाण, researchers-आंनी Deep Residual Shrinkage Network (DRSN) चो वापर 1,000 परस चड publications/studies मदे केला. ह्या applications मदे mechanical engineering, electrical power, vision, healthcare, speech, text, radar, आनी remote sensing सारक्या वेग-वेगळ्या क्षेत्रांचो आस्पाव जाता.
