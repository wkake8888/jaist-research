# TAMMIC
**Title:**\
Capturing Relations between Scientific Papers: An Abstractive Model for Related Work Section Generation\
Link: https://aclanthology.org/2021.acl-long.473.pdf

Problem:\
Most of existing related work section generation models follow the inflexible extractive style, which directly extract sentences from multiple original papers to form a related work discussion.

Solution:\
Propose a relation aware multi-document encoder that relates one document to another according to their content dependency in a relation graph. The relation graph and the document representation interact and are refined iteratively, complementing each other in the training process

![image](https://user-images.githubusercontent.com/50447179/156552159-a8e676ab-4ac6-48ad-86b8-70499595f52d.png)

![image](https://user-images.githubusercontent.com/50447179/156559921-c6bd8ebc-826b-449a-84b0-4f05a2d39cc7.png)
