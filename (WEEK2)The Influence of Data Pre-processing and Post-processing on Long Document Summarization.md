**Title**\
Longformer: The Long-Document Transformer
https://arxiv.org/pdf/2004.05150.pdf

**Motivation**
- Transformer-based models are unable to process long sequences due to their self-attention operation, which scales quadratically with the sequence length

Method:\
HEPOS uses separate encoder-decoder heads on the same layer to cover different subsets of source tokens at fixed intervals. Each head starts at a different position, and all heads collectively attend to the full sequence.

![image](https://user-images.githubusercontent.com/50447179/157227845-b2f8a955-61a9-44ce-84f9-7916a742e664.png)

