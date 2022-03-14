**Title**:\
DYLE: Dynamic Latent Extraction for Abstractive Long-Input Summarization\
https://arxiv.org/pdf/2110.08168.pdf

There 4 ways to tackle long-input summarization:
1. Sparse Attention
2. Hierarchical Modeling
3. Segmentation of source text
4. extract-then-generate method

→ Extract-then-generate method is very similar to the way a person acctualy would summarize long input text.\
→ This would be the best method. (Actually this method is proposed in human summarization task)\
<img width="230" alt="image" src="https://user-images.githubusercontent.com/50447179/157569774-d441995d-0307-4419-9770-140796c011a3.png">

**Contribution**
- We introduce dynamic latent extraction for the abstractive long-input summarization task, a new approach that better captures information in the long input, allows interpretable dynamic weights, and reduces computational complexity
- We propose multiple auxiliary optimizations: extractive oracle as a learning signal for the extractor, consistency loss that bridges extraction and generation, hybrid training methods that furthers generalizability of the extractor.
- Experimental results show that our approach achieves state-of-the-art results on two long input summarization datasets in documents and dialogues. We also conducted detailed analysis on the interpretability of our model.

