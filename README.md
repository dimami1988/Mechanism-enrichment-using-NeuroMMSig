# Mechanism-enrichment-using-NeuroMMSig
Seminar

Steps:
1) Find a proper research in database regarding desease of interest (preferably with at least 2 clear groups - cancer/healthy cells
2) Run analysis at service and download the resulting table
3) Load results into pandas dataframe
4) Filter out most up and downregulated genes (check FClog value in research). The amount of genes should be around 50-100
5) Pick up one or more genes and find a proper pathway where edges have at least 2 clear groups that can be classified as up and down: -1 or +1
6) 
7)
8)
9)
10)


Algorithm:
0) Assign all nodes with 0
1) Find genes (nodes) in pathway netwrokx structure that also presented in db from research 
2) Assign 1 or -1 according to FClog value from db

3) Split graph into subgraphs (based on strategy - for each node we take all neighbors). This node becomes a root node of subgraph.
4) For this node we calculate the charge
For child in children:
  charge + = NodeWeight * EdgeWeight 
  
5) Go one layer upper and calculate the same
6) Go until root node of pathway
7)   
