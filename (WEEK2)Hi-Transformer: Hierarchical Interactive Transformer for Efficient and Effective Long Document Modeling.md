ACL2021\
https://aclanthology.org/2021.acl-short.107.pdf

**Problem**\
Whole documents can not be inputted to Transformer\
→ Solve this problem by hierarchical way.\
→ Prepare a token for sentence representaion (CLS) and input it to Document Transformer. The number of input is number of sentences, so usually it works.

**Method**
1. first learns sentence representations
2. then learns document representations
3. Next, we use another sentence Transformer to enhance sentence modeling using the global document context
4. Finally, we use hierarchical pooling method to obtain document embedding

**Evaluation**\
Datasets: Amazon Electronics, IMDB, MIND\
(Evaluated by classification task)

**Note**
- Document Transformer is important because the performance consistently declines when the global document contexts are not encoded into sentence representations\
  → This is because the local contexts within a single sentence may be insufficient for accurate sentence modeling, and global contexts in the entire document can provide rich complementary information for sentence understanding\
  → propagating the document contexts to enhance sentence modeling can improve long document modeling.
  
![image](https://user-images.githubusercontent.com/50447179/156952523-94c1d16d-c3b4-4045-afe6-6fd1768d0ddd.png)
