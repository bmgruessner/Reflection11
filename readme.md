Brian Gruessner
20190407
Biovisualization- Reflection 11

This paper from the University of Sao Paulo created CellNetVis, a visualization tool for interactions between proteins in the Cell.  While other programs can do this, none are interactive, and therefore quickly become overwhelmed by the “hairball” problem in force-directed node-link diagrams.  Additionally, this vis focused on subcellular location so that the tool could be used to infer the location of interactions.

The program uses an “iterative force-directed algorithm” to arrange the relative positions of proteins with their most-associated subcellular location.  The locations are then crosslinked.

This vis tool seems to accomplish its goals.  It is able to create complex node-link diagrams that can then be simplified to a digestible diagram.  It is visually elegant and easy to understand its function and results (Figure 1). Finally, they demonstrate that it is capable of producing results that are sensible based on what is known and to make specific inferences and hypotheses (see the MAPK section).  

However, there are some limitations to the tool.  First of all, the paper infers that the protein EGFR (involved in signaling cell growth) may interact with MAPK14 outside of the mitochondria even though MAPK14 is generally considered a mitochondrial protein.  However, this hypothesis is not backed up with experimental data.  This tool, like many developed for bioinformatics, lacks validating evidence for the hypotheses that it generates.  

The tool also tends to take six to ten minutes to generate diagrams on the scale of lower thousands of proteins, meaning that it likely cannot handle an entire proteome of an organism.  Finally, the authors admit that this program tends to initially generate hairballs that need to be pruned and manipulated to make sense.

The bulk of CellNetVis is coded in Javascript using simple circle elements to maximize performance in a web-based tool.

Source: Heberly H, et al (2017). CellNetVis: a web tool for visualization of biological networks using force-directed layout constrained by cellular components. BMC Bioinformatics, 18(Suppl10):395. 

![alt text](https://github.com/bmgruessner/Reflection11/blob/master/R11.png "Figure 1")
