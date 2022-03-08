NAACL2021\
**Title**\
Efficient Attentions for Long Document Summarization\
https://arxiv.org/pdf/2104.02112.pdf

**Problem**<br>
The quadratic computational and memory complexities of large Transformers have limited their scalability for long document summarization

Solution:\
HEPOS uses separate encoder-decoder heads on the same layer to cover different subsets of source tokens at fixed intervals. Each head starts at a different position, and all heads collectively attend to the full sequence


**Contribution/Result**
- we are able to process ten times more tokens than existing models that use full attentions
- we are the　first to study efficient encoder-decoder attentions
- we present a new dataset, GOVREPORT, with significantly longer documents and summaries. 
- our models produce significantly higher ROUGE scores than competitive comparisons, including new state-of-the-art results on PubMed
- propose a new evaluation metric for faithfulness, inspired by APES, a fill-in-the-blank QA metric for summary evaluation
- Show reading more input boosts informativeness
- Show reading more input boosts faithfulness


GOVREPORT:
- 19.5K US goverment report with expert-written abstractive summary
- It contains significantly longer documents (9.4k words) and summaries (553 words) than existing datasets, such as PubMed and arXiv 
- Salient content is spread throughout the documents, as opposed to cases where summary-worthy words are more heavily concentrated in specific parts of the document
- It contain labels for paragraph


![image](https://user-images.githubusercontent.com/50447179/157228546-3a3c3e94-19ae-457c-9c51-246e69bf06e4.png)
