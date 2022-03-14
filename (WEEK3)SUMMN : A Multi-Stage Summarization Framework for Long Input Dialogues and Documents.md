**Title**:\
SUMM^N : A Multi-Stage Summarization Framework for Long Input Dialogues and Documents\
https://arxiv.org/pdf/2110.10150.pdf

**Mehtod**:
- First, segment source document into multiple subsets.
- Also segment target summary into multiple sentences.
- Then, find pairs of subsets and target sentences by greedy algorithm (don't allow duplication)
- Output multiple Coarse summary and concatenate them.
- Use the concatenated summary as an input for the next stage
- Iterate this until Language model can receive full tokens of the input.
- Then output fine-grained summary.

**Contribution**
- We propose SUMMN , a simple but effective framework for long dialogue and document summarization.
- We evaluate SUMMN on both dialogue and document domains and improve the baseline model by a large margin.
- We analyze and compare the proposed framework with baselines discuss its merits with high interpretablity.

![Screen Shot 2022-03-14 at 10 22 48](https://user-images.githubusercontent.com/50447179/158089354-891e2543-f1d9-44c5-b40d-68d7092b8ad4.png)
