# protein-interaction-network
This project aims to generate the visualization of the protein-protein directed interaction network.
1. Data sources
a.Signor3.0 https://signor.uniroma2.it/downloads.php?beta=3.0: genes directed interaction
  file all_data.tsv is directly downloaded from its website with organism filter as homo sapiens
b.Gene expression data from the TCGA (SKCM) vs. normal
  file ras_t&g.tsv is the gene expression data from the limma
2. Network element
a.Node: nodes are the significant genes based on the gene expression data with the cutoff for driven genes. The color of node represents the logFC number of the genes.
b.Edge: length and width of edges represents the confidence score of the directed interactions. The color of the edge represents the interaction mechanism of this interaction
  where red edge for activation effect while navy edge for inhibition effect.
  Default cutoff for the confidence score of interaction is 0.5.
c.Legend: logFC color legend for each node.
