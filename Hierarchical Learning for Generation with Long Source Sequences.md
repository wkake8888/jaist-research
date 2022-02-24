# TAMMIC
**Title:**\
Hierarchical Learning for Generation with Long Source Sequences\
Link: https://arxiv.org/pdf/2104.07545.pdf

**Author:**\
Tobias Rohde, Xiaoxia Wu, Yinhan Liu

**Motivation:**
- Current Seq2Seq model has difficulty on handling long sequences, such as summarization and document level translation tasks.
- These tasks require the model to reason at the token level as well as the sentence and paragraph level

**Method:**
- a new Hierarchical Attention Transformer-based architecture (HAT) 
- 

**Insight:**
- Achieved state-of-the art ROUGE scores on four summarization tasks, including PubMed-arXiv(Scientific paper), CNN/DM,SAMSum(Multi-party conversation) \and AMI(Meeting).
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
