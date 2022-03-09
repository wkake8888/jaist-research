NAACL2021\
https://aclanthology.org/2021.naacl-main.470.pdf

Problem:\
- The length limitation of text encoder
- use a sliding window to process documents separately is not efficient because the concatenation of summaries that are independently extracted from local contexts is usually have noise (e.g. Only para 1 and 2 shoud be used for summary, but para 3, 4, 5 are also used)\
→ para 3, 4, 5 should output empty result

Method:\
propose the sliding selector network with dynamic memory for extractive summarization of long-form documents, which employs a sliding window to extract summary sentences segment by segment. \
Moreover, we adopt memory mechanism to preserve and update the history information dynamically, allowing the semantic flow across different windows.

Results:\

Contribution:
- propose a novel extractive summarization model that can summarize documents of arbitrary length without truncation loss
- the first to propose applying memory networks into extractive text summarization task
- The proposed framework (i.e., a sliding encoder combined with dynamic memory) can be easily extended to other abstractive and extractive summarization models
- Our model achieves the state-of-the-art results on two widely used datasets for long document summarization

![image](https://user-images.githubusercontent.com/50447179/157353294-64320c91-1f6e-4b36-ae07-585bee1a3da5.png)
