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
