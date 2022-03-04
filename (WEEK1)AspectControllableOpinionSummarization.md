**Title:**\
Aspect-Controllable Opinion Summarization\
Link: https://arxiv.org/pdf/2109.03171.pdf


Problem:\
Most of aspect specific opinion summarization is using extractive method, but it is not good.

Solution:\
- Create datasets (review, aspect label). If there is at least one seed word, the label is +1 otherwise -1.
- model Aspect controller Induction model by Using the dataset and aggregating hierarchical aspect predictions(token-level, sentence-level) and generate document-level aspect prediction.
- Create synthetic trainning datasets (review, pseudo-summary, aspects controller) 


![image](https://user-images.githubusercontent.com/50447179/156676024-47c82f75-55ab-4dd3-ac7f-b0fc2061c4fb.png)
