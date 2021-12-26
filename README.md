# Credit Risk Analysis

## Overview
The purpose of this analysis is to utilize and compare four different methods of sampling a dataset. Then the same dataset was used to train and compare the results of two different ML models.

## Results
<br>

### Random Oversampling
- <b>Accuracy Score:</b> 62.5%
<br>![image](https://user-images.githubusercontent.com/88811124/147371432-b2eca656-1b04-4ac6-abcc-51c50ae3554b.png)<br>
- While very precise with a moderate recall for low risk loans, there was almost no precision for high risk loans
<br>![image](https://user-images.githubusercontent.com/88811124/147371448-677ad195-644f-42da-adc7-01f8b7df76f9.png)<br>

### SMOTE Oversampling
- <b>Accuracy Score:</b> 65.1%
<br>![image](https://user-images.githubusercontent.com/88811124/147371491-ae8eead3-f4f5-4292-916f-596170008620.png)<br>
- Precision and recall results almost identical to Random Oversampling, with marginally better recall results for both high risk and low risk loans
<br>![image](https://user-images.githubusercontent.com/88811124/147371521-6d917053-f4ba-45ba-bd0e-942630aa9eb6.png)<br>

### Undersampling
- <b>Accuracy Score:</b> 51.6%
<br>![image](https://user-images.githubusercontent.com/88811124/147371550-1b25b4c9-e8be-4aca-a364-7ddfdb4fec55.png)<br>
- Similar Precision numbers again, but a significant drop in recall for low risk loans and a marginal drop for high risk loans
<br>![image](https://user-images.githubusercontent.com/88811124/147371627-47353462-9998-4813-bacf-9ed281537175.png)<br>

### Combination Sampling
- <b>Accuracy Score:</b> 61.6%
<br>![image](https://user-images.githubusercontent.com/88811124/147371642-6c2ca230-eb5c-4f15-8f17-662e57cca0be.png)<br>
- Better recall on the high risk loans vs the low risk loans, with similar Precision again
<br>![image](https://user-images.githubusercontent.com/88811124/147371687-5198682e-a68a-4f4b-9e97-a2626ed6977a.png)<br>

### Balanced Random Forest Classifier vs Easy Ensemble CLassifier Models
- Both have significantly higher Accuracy scores than the four sampling methods used prior
- The Easy Ensemble Classifier is clearly the better model for our current dataset, with roughly double the f score for high risk loans and a much higher f score for low risk loans, than the Random Forest Classifier model

## Summary 
- While none of these models are perfect, the Random Forest Classifier is the brightest of the bunch. However, I wouldn't recommend any of these models for any real-world application. None of the models used performed well enough when analyzing high risk loans, with the highest f score only being 14%. All of the models were very precise for low risk loans, scoring 100%, with servicable recalls as well, but none were very preice whatsoever when it came to the more important high risk loans that needed to be identified.

 
