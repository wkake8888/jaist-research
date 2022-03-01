# TAMMIC
**Title:**\
Aspect-Controllable Opinion Summarization\
Link: https://arxiv.org/pdf/2109.03171.pdf

**Author:**\
Reinald Kim Amplayo Stefanos Angelidis Mirella Lapata

**Motivation:**
- The important information in reviews largely depends on user interst. → Needs of Aspect-specific Summarization
- There are mainly two disadvantages in Extractive method.
- 1. The summary can be incoherent and verbose containing unnecessary redundancy.
- 2. It is not clear how to control the number of aspects in the output.
- → Abstractive method is needed. 

**Method:**
- First, construct a synthetic training dataset consist of reviews, a pseudo-summary, and three types of aspect controllers which reflect different levels of granularity: aspect-related keywords, review sentences, and document-level aspect codes.
- Then fine-tune a pretrained model on summary generation using the synthethized dataset.
- 

**Insight:**
- The model achived Sota on both SPACE and OPOSUM tasks of general and aspect-specific summarization
- it can also effectively generate multi-aspect summaries based on user preferences

**Contribution summary:**\
presented an abstractive approach to aspect-controlled opinion summarization. Key to the model is the induction of aspect controllers which facilitate the creation of a synthetic training dataset and guide summary generation towards the designated aspects

# KURR
**Keyword:**\
multiple instant learning model, aspect controllers, 

**Unkown:**
- Performance of the model with more than 3 aspects.
- Performance of the model with another aspects or unkown aspects

**Reflection:**
- 

**Future Work:**
- controlling additional facets of opinion summaries such
as sentiment or length
- learn aspects from data rather than specifying
them apriori as well as dealing with unseen aspects

**Reference:**


# Notes
- Datasets = SPACE, OPOSUM
- 
