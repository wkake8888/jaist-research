# TAMMIC
**Title:**\
EmailSum: Abstractive Email Thread Summarization

**Author:**\
Shiyue Zhang

**Motivation:**
- Encoder-Decoder Model has diffiuclty on dealing with long senteces.

**Method:**
- General end-to-end approach to sequence learing that makes minimal assumption on the sequence structure.
- Use mulitlayered LSTM to map input sequence to a vector
- Then decode the target sequence from the vector by another deep LSTM.

**Insight:**\
- Main result is that on an English to French translation task using WMT'14 dataset, achived BREU score of 34.8
- LSTM did not have difficulty on long sentences.
- LSTM learned sensible phrase and sentence representations that are sensitive to word order and are relatively invariant to the active and passive voices.
- Improved LSTM's performance by reversing the order of the words in the all source sentences.

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
