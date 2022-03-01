main content
----------
- this paper is a dateset paper, they provid the largest dataset for multidocument opinion summarization **AMASUM**
- they propose an end-to-end model selecting and summarizing reviews.  formulating  the task as jointly learning to select informative subsets of 
  reviews and summarizing the opinions expressed in these subsets.
- each product is linked to too many reviews, so, makes it virtually impossible to train a conventional encoderdecoder model using standard hardware. Moreover,
  not all reviews cover the summary content. Thus, training to predict summaries based on random review subsets results in hallucinations. this work choose to
  select relevant review subsets.
  ![2](https://user-images.githubusercontent.com/56755928/156166577-d4e3d5c5-ff8d-42eb-b718-58aadf5f6d5b.jpg)

  

