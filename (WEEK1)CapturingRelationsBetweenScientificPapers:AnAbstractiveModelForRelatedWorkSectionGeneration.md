# TAMMIC
**Title:**\
Capturing Relations between Scientific Papers: An Abstractive Model for Related Work Section Generation\
Link: https://aclanthology.org/2021.acl-long.473.pdf

**Author:**\
Xiuying Chen, Hind Alamro

**Motivation:**
- Most of existing related work section generation models follow the inflexible extractive style.
- However, they are not good at paraphrasing and generalization, and often lead to a related work section with poor coherence and readability
- →Abstractive method
- But there are two main challenges,
- 1. the related work should summarize the contribution of each paper
- 2. explain the relationship between different papers such as parallel, turning, and progressive relation, so as to introduce them in a logical order.
- → Relation aware Related work Generator (RRG)

**Method:**
- encode the multiple input articles in a hierarchical manner, obtaining the overall representation for each document
- Apply a relationaware multi-document encoder that relates multiple input documents in a relation graph
- In the training process, the relation graph and the document representation interact and are refined iteratively, complementing each other
- Finally, in the decoder part, we utilize the relation graph information to assist the decoding process, where the model learns to decide whether to pay attention to the input documents or the relationship between them

**Insight:**
- 

**Contribution summary:**\
This paper proposes a Relation aware Related work Generator (RRG), which generates an abstractive related work section from multiple scientific papers in the same research area. \
Main contributions are,
- We address an abstractive related work generation task, which aims to generate an abstractive related work with novel words and phrases.
- We propose a relation-aware multi-document encoder that relates one of the multiple input documents to another, and establishes a relation graph storing the dependency between documents.
- We contribute two public large-scale related work generation datasets that are beneficial for the community

# KURR
**Keyword:**\
related work section generation, Hierarchical Encoder, graph-based relationship modeling (RM)

**Unkown:**
- 

**Reflection:**\
- 

**Reference:**\


# Notes
- 
- 
