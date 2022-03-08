**PDF:** https://arxiv.org/abs/2005.10043

problem
--------
Graphs that capture relations between textual units have great benefits to MDS, which can help generate more informative, concise and coherent summaries from multiple documents.Few work has studied the effectiveness of explicit graph representations on neural abstractive MDS.

Method
------
- leverage explicit graph representations of documents to more effectively process multiple input documents and distill         abstractive summaries
- incorporate explicit graph representations into the encoding process via a graphinformed attention mechanism. Under the guidance of explicit relations in graphs, our model can learn better and richer cross-document relations.
- leverage the graph structure to guide the summary decoding process, which is beneficial for long summary generation
- combine the advantages of pretrained LMs into our model![1](https://user-images.githubusercontent.com/56755928/157284981-6a6c90dd-d3ca-4d54-92ad-307770cc9c9a.jpg)
