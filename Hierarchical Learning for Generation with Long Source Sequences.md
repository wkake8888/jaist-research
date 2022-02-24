# TAMMIC
**Title:**\
Hierarchical Learning for Generation with Long Source Sequences\
Link: https://arxiv.org/pdf/2104.07545.pdf

**Author:**\
Tobias Rohde, Xiaoxia Wu, Yinhan Liu

**Motivation:**
- Current Seq2Seq model has difficulty on handling long sequences, such as summarization and document level translation tasks.
- RNN and Transformer-based models have limits on the input length. When input is long and it is required complehensive understanding of the entire paragraph or document.
- These tasks require the model to reason at the token level as well as the sentence and paragraph level
- One of the main learning challenges for seq2seq models is that the decoder needs to get token level representations from the encoder to predict the next token, while at the same time it must learn from a large context.

**Method:**
- a new Hierarchical Attention Transformer-based architecture (HAT) 
- a hierarchical attention model based on the standard Transformer that produces sentence level representations, and combine them with token level representations to improve performance on long document sequence to sequence tasks

**Insight:**
- Achieved state-of-the art ROUGE scores on four summarization tasks, including PubMed-arXiv(Scientific paper), CNN/DM,SAMSum(Multi-party conversation) and AMI(Meeting).
- Outperforms document-level machine translation baseline on the WMT20 English to German translation task

**Contribution summary:**\
Ilya Sutskever, Oriol Vinyals, Quoc V. Le

# KURR
**Keyword:**\
LSTM, beam-search, SMT, RNN, 

**Unkown:**
- Perfect explanaiton about why reversing the order of sentences improved performance.
- Sensitive to word order.

**Reflection:**\
- It can handle seq to seq problem, so this model can be used widely.

**Reference:**\
Ilya Sutskever, Oriol Vinyals, Quoc V. Le

# Notes
- DNNs have to know the dimentionality of the input and the ouput. But many problems are best expressed with sequence of unknown length.
- Useful property of LSTM is that it can map input sequences to fixed dimentional vector representation.
