2020\
**Title**\
Longformer: The Long-Document Transformer
https://arxiv.org/pdf/2004.05150.pdf

**Motivation**
- Transformer-based models are unable to process long sequences due to their self-attention operation, which scales quadratically with the sequence length
- Scaled Dot-Product attention directs attention from all words to all words, which led to memory consumption in 𝑛^2

Method:
- Reduce memory consumption by directing attention only from important words to important words.
- Use mulitple attention method for multiple purpose (language modeling, pretraining, encoder-decoder model)

Contribution:
- It can handle longer inputs by modifing self-attention method.
- Improve performance by pretraining and fine-tuning

LED:
- To facilitate modeling long sequences for seq2seq learning, we propose a Longformer variant that has both the encoder and decoder Transformer stacks but instead of the full self-attention in the encoder, it uses the efficient local+global attention pattern of the Longformer. The decoder uses the full self-attention to the entire encoded tokens and to previously decoded locations
- initialize LED parameters from the BART, and follow BART’s exact architecture in terms of number of layers and hidden sizes
- The only difference is that to process longer inputs, we extend position embedding to 16K tokens (up from BART’s 1K tokens) and we initialize the new position embedding matrix by repeatedly copying BART’s 1K position embeddings 16 times
![image](https://user-images.githubusercontent.com/50447179/157231971-ebb497ad-eff1-45fc-998a-34ec6f4420c7.png)
