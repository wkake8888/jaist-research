**Title**\
Globalizing BERT-based Transformer Architectures for Long Document Summarization\
Link: https://aclanthology.org/2021.eacl-main.154.pdf

Problem:\
when associated with the current transformer-based architectures, shows several limitations when the target task requires to reason with long documents. 
Input length must be less than 512 tokens. But this is too short for long documents.

Solutions:\
 In this work, we introduce a novel hierarchical propagation layer that spreads information between multiple transformer windows. We adopt a hierarchical approach where the input is divided in multiple blocks independently processed by the scaled dot-attentions and combined between the successive layers. 
 
Reflection:
- In this experiments, summary is generated by extractive method, so we can modify this architecture for abstractive method.
- Sharing the parameters of BiGRU is no influence so we can modify this part.

![image](https://user-images.githubusercontent.com/50447179/156497800-9943c93a-7a95-4014-924a-4d5d962b786f.png)

