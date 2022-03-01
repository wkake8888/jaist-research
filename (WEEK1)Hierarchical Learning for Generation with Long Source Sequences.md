# TAMMIC
**Title:**\
Hierarchical Learning for Generation with Long Source Sequences\
Link: https://arxiv.org/pdf/2104.07545.pdf

**Author:**\
Tobias Rohde, Xiaoxia Wu, Yinhan Liu

**Motivation:**
- Current Seq2Seq model has difficulty on handling long sequences, such as summarization and document level translation tasks.
- RNN and Transformer-based models have limits on the input length. When input is long and it is required complehensive understanding of the entire paragraph or document, the performance is not good.
- These tasks require the model to reason at the token level as well as the sentence and paragraph level (Main idea of this paper)
- One of the main learning challenges for seq2seq models is that the decoder needs to get token level representations from the encoder to predict the next token, while at the same time it must learn from a large context.

**Method:**
- a hierarchical attention model based on the standard Transformer that produces sentence level representations, and combine them with token level representations to improve performance on long document sequence to sequence tasks
- Adding BOS to each sentences to get sentence representation, not only sequence representation.

**Insight:**
- Achieved state-of-the art ROUGE scores on four summarization tasks, including PubMed-arXiv(Scientific paper), CNN/DM,SAMSum(Multi-party conversation) and AMI(Meeting).
- Outperforms document-level machine translation baseline on the WMT20 English to German translation task

**Contribution summary:**\


# KURR
**Keyword:**\
Hierarchical Learning, Hierarchical Token, 

**Unkown:**
- when fine-tuning Encoder-only transformer hierarchical attention model on RACE, it had to be disabled dropout for the first epoch and then set it to 0.1, otherwise the model did not converge
- 

**Reflection:**\
- A hierarchical encoder-only model for classification did not get significant gain.
- However, author beleive that combination of modifying the architecture and the pre-training process might improve over current non-hierarchical models for classification tasks with long source sequences

**Reference:**\


# Notes
- 
- 
