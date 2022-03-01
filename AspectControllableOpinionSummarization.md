# TAMMIC
**Title:**\
Aspect-Controllable Opinion Summarization\
Link: https://arxiv.org/pdf/2109.03171.pdf

**Author:**\
Reinald Kim Amplayo Stefanos Angelidis Mirella Lapata

**Motivation:**
- The notion of salience in reviews largely depends on user interst. → Needs of Aspect-specific Summarization
- There are mainly two disadvantages in Extractive method.
- 1. The summary can be incoherent and verbose containing unnecessary redundancy.
- 2. It is not clear how to control the number of aspects in the output.
- → Abstractive method is needed. 

**Method:**
- First, construct a synthetic training dataset consist of reviews, a pseudo-summary, and three types of aspect controllers which reflect different levels of granularity: aspect-related keywords, review sentences, and document-level aspect codes.
- Then fine-tune a pretrained model on summary generation using the synthethized dataset.
- 

**Insight:**
- The model outperforms previous approaches on both SPACE and OPOSUM tasks of general and aspect-specific summarization
- it can effectively generate multi-aspect summaries based on user preferences

**Contribution summary:**\


# KURR
**Keyword:**\
multiple instant learning model, aspect controllers, 

**Unkown:**
- 

**Reflection:**\
- 

**Reference:**\


# Notes
- Datasets = SPACE, OPOSUM
- 
