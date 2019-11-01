# FB-Friend-recommedation-using-Graph-mining
## Problem statement:
Given a directed social graph,we have to predict missing links to recommend friends/connections/followers(Link prediction).
## Data Overview:
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting .

Data contains two columns source and destination node in graph

Data columns (total 2 columns):
* source_node int64
* destination_node int64
## Mapping the problem into supervised learning problem:
Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.
## Business objectives and constraints:
* No low-latency requirement. 
* Probability of prediction is useful to recommend ighest probability links.

## Performance metric for supervised learning:
* Both precision and recall is important so F1 score is good choice 
* Confusion matrix.

## References:
*  https://www.cs.cornell.edu/home/kleinber/link-pred.pdf
*  https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf
*  https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf
*  https://www.youtube.com/watch?v=2M77Hgy17cg
