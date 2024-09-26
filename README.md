# Channel-aware CSI Feedback: Dataset Bias Mitigated Pre-training, Online Out-of-Distribution Detection and its Domain Adaptation


## Simulation Result and Analysis
### A. Evaluation of Channel-aware CSI Feedback in the Model Training Phase
#### Experiment Setup
This subsection first verifies the bias mitigation and performance of the channel-aware CSI feedback paradigm pre-trained on mixed datasets under different setups. The efficiency of the channel-aware CSI feedback to mitigate dataset bias of the offline pre-train dataset collected from 5 multiple channel configurations is evaluated, and the downlink channels are collected in a perfect downlink channel estimation mode with the setting of the following table.
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/18aef550f9e640abab69527ad2f68d7003578957/Images/Offline%20Pre-training%20Mixed%20Dataset%20Configuration.jpg" width="450">
</p>
This study utilizes four distinct offline pre-train dataset bias settings to evaluate the channel-aware CSI feedback scheme, which is summarized in the radar chart in the following figure. 
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/18aef550f9e640abab69527ad2f68d7003578957/Images/Offline%20Pre-training%20Mixed%20Dataset%20Setups.jpg" width="500">
</p>

#### Experiment Result
This evaluation first compares the proposed channel-aware CSI feedback paradigm with baseline CsiNet and TransNet in terms of learnable parameters and Floating Point Operations per Second (FLOPs), as shown in the following table.
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/623de0036a20e32b28d5d16f09a81112e8433a49/Images/Channel-aware%20CSI%20Feedback%20Complexity.jpg" width="450">
</p>
The evaluation of mitigation bias of training with 4 mixed training dataset setups and validation of the regression error and channel-aware accuracy of the trained proposed channel-aware CSI feedback paradigm is illustrated in the bar charts of the following figures.
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/719a11dd8e6bf91a0e464520e7906b8f777f2eae/Images/Offline%20Pre-training%20Mixed%20Dataset%20Results.jpg" width="800">
</p>

### B. Evaluation of Unified Channel-aware Out-of-distribution Detection Framework in Model Monitoring
#### Experiment Setup
This subsection assesses the accuracy of the proposed unified channel-aware out-of-distribution detection framework with Softmax-score and Energy-based score functions with two online datasets setups from the IndoorHall-5GHz and the SemiUrban-300MHz, respectively, which simulate an open-world model deployment. The downlink channel is collected from the COST2100 model with channel configurations enumerated in the following table. 
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/af7fadb7b1bf7fbdcc595947b8cd0de68cdb58f6/Images/Channel-aware%20OODD%20Dataset%20Setups.jpg" width="450">
</p>

#### Experiment Result
The TPR 95% performance of the unified channel-aware out-of-distribution detection with two setups of online deployment datasets is enumerated in the following table.
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/af7fadb7b1bf7fbdcc595947b8cd0de68cdb58f6/Images/Channel-aware%20OODD%20accuracy.jpg" width="450">
</p>
The experimental results of channel-aware CSI feedback model updating utilizing returning online in-distribution subsets are presented in the following table.
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/0aba2842afea69b870d6a68fd28e8a8332d836c4/Images/Channel-aware%20OODD%20Update%20Performance.jpg" width="450">
</p>

### C. Evaluation of Unified Channel-aware Out-of-distribution Detection Framework in Model Monitoring
#### Experiment Setup
This subsection evaluates the proposed HDA scheme for online model updates. The channel-aware CSI feedback model will be updated under conditions of limited accessible training data and a restricted number of trainable iterations using an online dataset with significant data drift, which is the set of distilled ID samples from the proposed channel-aware unified out-of-distribution detection framework in the simulating online deployment dataset. The online test dataset configuration is enumerated in the following table. 
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/1d3e29e72e27d244a2ffffdd41ac4b5e2e31c6ad/Images/Channel-aware%20HDA%20Dataset%20Setups.jpg" width="550">
</p>

#### Experiment Result
The updated model with the proposed HDA is compared with conventional inductive-based online learning and the related domain adaptation approach on the channel reconstruction error and channel-aware accuracy of the prior knowledge, and the channel reconstruction error and similarity of the present knowledge. The evaluation result is presented in the following table. 
<p align="center">
  <img src = "https://github.com/TeleRagingFires/Channel-aware-Feedback/blob/1d3e29e72e27d244a2ffffdd41ac4b5e2e31c6ad/Images/Channel-aware%20HDA%20Performance.jpg" width="850">
</p>


