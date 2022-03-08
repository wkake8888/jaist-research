2020\
**Title**\
Longformer: The Long-Document Transformer
https://arxiv.org/pdf/2004.05150.pdf

**Motivation**
- Transformer-based models are unable to process long sequences due to their self-attention operation, which scales quadratically with the sequence length
- Scaled Dot-Product attention directs attention from all words to all words, which led to memory consumption in 𝑛^2

Method:\
- Reduce memory consumption by directing attention only from important words to important words.
- Use sliding window attention and global attention together.

Contribution:\
- It can handle longer inputs by modifing self-attention method.
- Improve performance by pretraining and fine-tuning


![image](https://user-images.githubusercontent.com/50447179/157231971-ebb497ad-eff1-45fc-998a-34ec6f4420c7.png)
